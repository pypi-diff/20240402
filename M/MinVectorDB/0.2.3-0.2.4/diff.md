# Comparing `tmp/MinVectorDB-0.2.3.tar.gz` & `tmp/MinVectorDB-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MinVectorDB-0.2.3.tar", last modified: Thu Mar  7 03:06:27 2024, max compression
+gzip compressed data, was "MinVectorDB-0.2.4.tar", last modified: Tue Apr  2 10:44:44 2024, max compression
```

## Comparing `MinVectorDB-0.2.3.tar` & `MinVectorDB-0.2.4.tar`

### file list

```diff
@@ -1,32 +1,45 @@
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-03-07 03:06:27.071564 MinVectorDB-0.2.3/
--rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 MinVectorDB-0.2.3/LICENSE
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-03-07 03:06:27.071142 MinVectorDB-0.2.3/MinVectorDB.egg-info/
--rw-r--r--   0 guobingming   (501) staff       (20)    22214 2024-03-07 03:06:27.000000 MinVectorDB-0.2.3/MinVectorDB.egg-info/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)      564 2024-03-07 03:06:27.000000 MinVectorDB-0.2.3/MinVectorDB.egg-info/SOURCES.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 MinVectorDB-0.2.3/MinVectorDB.egg-info/dependency_links.txt
--rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 MinVectorDB-0.2.3/MinVectorDB.egg-info/not-zip-safe
--rw-r--r--   0 guobingming   (501) staff       (20)      145 2024-03-07 03:06:27.000000 MinVectorDB-0.2.3/MinVectorDB.egg-info/requires.txt
--rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-03-07 03:06:27.000000 MinVectorDB-0.2.3/MinVectorDB.egg-info/top_level.txt
--rw-r--r--   0 guobingming   (501) staff       (20)    22214 2024-03-07 03:06:27.071352 MinVectorDB-0.2.3/PKG-INFO
--rw-r--r--   0 guobingming   (501) staff       (20)    21007 2024-03-07 03:03:44.000000 MinVectorDB-0.2.3/README.md
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-03-07 03:06:27.070410 MinVectorDB-0.2.3/min_vec/
--rw-r--r--   0 guobingming   (501) staff       (20)       70 2024-02-27 06:10:26.000000 MinVectorDB-0.2.3/min_vec/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    10049 2024-03-07 02:06:51.000000 MinVectorDB-0.2.3/min_vec/api.py
--rw-r--r--   0 guobingming   (501) staff       (20)      517 2024-02-28 05:58:00.000000 MinVectorDB-0.2.3/min_vec/authorize.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2232 2024-02-28 02:53:23.000000 MinVectorDB-0.2.3/min_vec/config.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1622 2024-02-29 06:40:54.000000 MinVectorDB-0.2.3/min_vec/engines.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2316 2024-03-07 02:06:51.000000 MinVectorDB-0.2.3/min_vec/fields_mapper.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1036 2024-03-06 14:55:44.000000 MinVectorDB-0.2.3/min_vec/filter.py
--rw-r--r--   0 guobingming   (501) staff       (20)     7512 2024-02-23 09:32:28.000000 MinVectorDB-0.2.3/min_vec/ivf_index.py
--rw-r--r--   0 guobingming   (501) staff       (20)     1600 2024-02-26 06:57:51.000000 MinVectorDB-0.2.3/min_vec/kmeans.py
--rw-r--r--   0 guobingming   (501) staff       (20)    28902 2024-03-07 02:03:15.000000 MinVectorDB-0.2.3/min_vec/matrix_serializer.py
--rw-r--r--   0 guobingming   (501) staff       (20)     9042 2024-03-07 02:07:46.000000 MinVectorDB-0.2.3/min_vec/query.py
--rw-r--r--   0 guobingming   (501) staff       (20)     2790 2024-03-07 02:58:49.000000 MinVectorDB-0.2.3/min_vec/scaler.py
--rw-r--r--   0 guobingming   (501) staff       (20)      362 2024-02-26 09:43:31.000000 MinVectorDB-0.2.3/min_vec/session.py
--rw-r--r--   0 guobingming   (501) staff       (20)    10735 2024-03-06 14:35:21.000000 MinVectorDB-0.2.3/min_vec/storage.py
--rw-r--r--   0 guobingming   (501) staff       (20)     4500 2024-02-26 09:43:31.000000 MinVectorDB-0.2.3/min_vec/utils.py
--rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-03-07 03:06:27.071599 MinVectorDB-0.2.3/setup.cfg
--rw-r--r--   0 guobingming   (501) staff       (20)     1594 2024-02-29 03:40:51.000000 MinVectorDB-0.2.3/setup.py
-drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-03-07 03:06:27.070879 MinVectorDB-0.2.3/test/
--rw-r--r--   0 guobingming   (501) staff       (20)       31 2024-01-31 10:38:44.000000 MinVectorDB-0.2.3/test/__init__.py
--rw-r--r--   0 guobingming   (501) staff       (20)    12645 2024-03-07 02:27:36.000000 MinVectorDB-0.2.3/test/test_model.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.925522 MinVectorDB-0.2.4/
+-rw-r--r--   0 guobingming   (501) staff       (20)    11357 2023-09-19 11:00:45.000000 MinVectorDB-0.2.4/LICENSE
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.924993 MinVectorDB-0.2.4/MinVectorDB.egg-info/
+-rw-r--r--   0 guobingming   (501) staff       (20)    18634 2024-04-02 10:44:44.000000 MinVectorDB-0.2.4/MinVectorDB.egg-info/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)      950 2024-04-02 10:44:44.000000 MinVectorDB-0.2.4/MinVectorDB.egg-info/SOURCES.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-04-02 10:44:44.000000 MinVectorDB-0.2.4/MinVectorDB.egg-info/dependency_links.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)        1 2024-03-07 03:06:27.000000 MinVectorDB-0.2.4/MinVectorDB.egg-info/not-zip-safe
+-rw-r--r--   0 guobingming   (501) staff       (20)      145 2024-04-02 10:44:44.000000 MinVectorDB-0.2.4/MinVectorDB.egg-info/requires.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)       13 2024-04-02 10:44:44.000000 MinVectorDB-0.2.4/MinVectorDB.egg-info/top_level.txt
+-rw-r--r--   0 guobingming   (501) staff       (20)    18634 2024-04-02 10:44:44.925266 MinVectorDB-0.2.4/PKG-INFO
+-rw-r--r--   0 guobingming   (501) staff       (20)    17426 2024-04-02 10:37:16.000000 MinVectorDB-0.2.4/README.md
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.920038 MinVectorDB-0.2.4/min_vec/
+-rw-r--r--   0 guobingming   (501) staff       (20)       81 2024-04-02 09:07:59.000000 MinVectorDB-0.2.4/min_vec/__init__.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.920376 MinVectorDB-0.2.4/min_vec/api/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:42.000000 MinVectorDB-0.2.4/min_vec/api/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    10441 2024-04-02 10:16:24.000000 MinVectorDB-0.2.4/min_vec/api/api.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.920725 MinVectorDB-0.2.4/min_vec/computational_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:06:12.000000 MinVectorDB-0.2.4/min_vec/computational_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2245 2024-04-02 08:22:33.000000 MinVectorDB-0.2.4/min_vec/computational_layer/engines.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.921071 MinVectorDB-0.2.4/min_vec/configs/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:24.000000 MinVectorDB-0.2.4/min_vec/configs/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2184 2024-04-02 10:16:24.000000 MinVectorDB-0.2.4/min_vec/configs/config.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.922296 MinVectorDB-0.2.4/min_vec/data_structures/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:07:22.000000 MinVectorDB-0.2.4/min_vec/data_structures/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     2316 2024-03-07 02:06:51.000000 MinVectorDB-0.2.4/min_vec/data_structures/fields_mapper.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1036 2024-03-06 14:55:44.000000 MinVectorDB-0.2.4/min_vec/data_structures/filter.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     1578 2024-03-28 05:59:46.000000 MinVectorDB-0.2.4/min_vec/data_structures/kmeans.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      687 2024-04-02 10:06:58.000000 MinVectorDB-0.2.4/min_vec/data_structures/limited_dict.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     3405 2024-04-02 09:57:20.000000 MinVectorDB-0.2.4/min_vec/data_structures/scaler.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.923297 MinVectorDB-0.2.4/min_vec/execution_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:09:45.000000 MinVectorDB-0.2.4/min_vec/execution_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    29345 2024-04-02 09:51:33.000000 MinVectorDB-0.2.4/min_vec/execution_layer/matrix_serializer.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     9163 2024-04-02 08:40:53.000000 MinVectorDB-0.2.4/min_vec/execution_layer/query.py
+-rw-r--r--   0 guobingming   (501) staff       (20)      362 2024-02-26 09:43:31.000000 MinVectorDB-0.2.4/min_vec/execution_layer/session.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.923640 MinVectorDB-0.2.4/min_vec/storage_layer/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:04:15.000000 MinVectorDB-0.2.4/min_vec/storage_layer/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    21534 2024-04-02 10:06:58.000000 MinVectorDB-0.2.4/min_vec/storage_layer/storage.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.924132 MinVectorDB-0.2.4/min_vec/utils/
+-rw-r--r--   0 guobingming   (501) staff       (20)        0 2024-03-22 08:10:09.000000 MinVectorDB-0.2.4/min_vec/utils/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)     4533 2024-04-01 09:19:24.000000 MinVectorDB-0.2.4/min_vec/utils/utils.py
+-rw-r--r--   0 guobingming   (501) staff       (20)       38 2024-04-02 10:44:44.925562 MinVectorDB-0.2.4/setup.cfg
+-rw-r--r--   0 guobingming   (501) staff       (20)     1422 2024-04-02 09:07:59.000000 MinVectorDB-0.2.4/setup.py
+drwxr-xr-x   0 guobingming   (501) staff       (20)        0 2024-04-02 10:44:44.924637 MinVectorDB-0.2.4/test/
+-rw-r--r--   0 guobingming   (501) staff       (20)       31 2024-01-31 10:38:44.000000 MinVectorDB-0.2.4/test/__init__.py
+-rw-r--r--   0 guobingming   (501) staff       (20)    12645 2024-03-07 02:27:36.000000 MinVectorDB-0.2.4/test/test_model.py
```

### Comparing `MinVectorDB-0.2.3/LICENSE` & `MinVectorDB-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `MinVectorDB-0.2.3/MinVectorDB.egg-info/PKG-INFO` & `MinVectorDB-0.2.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,36 @@
-Metadata-Version: 2.1
-Name: MinVectorDB
-Version: 0.2.3
-Summary: MinVectorDB is a pure Python-implemented, lightweight, stateless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
-Home-page: https://github.com/BirchKwok/MinVectorDB
-Author: Birch Kwok
-Author-email: birchkwok@gmail.com
-Keywords: vector database
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy>=1.17.0
-Requires-Dist: spinesUtils>=0.3.13
-Requires-Dist: torch>=2.0.0
-Requires-Dist: msgpack>=1.0.2
-Requires-Dist: h5py>=3.4.0
-Requires-Dist: scikit-learn>=1.0.0
-Requires-Dist: cloudpickle>=2.0.0
-Requires-Dist: numexpr>=2.7.3
-Requires-Dist: pyroaring>=0.4.5
-
 <div align="center">
-  <h1>MinVectorDB</h1>
+  <h1><a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB"></a></h1>
   <h3>A pure Python-implemented, lightweight, stateless, locally deployed vector database.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/dm/MinVectorDB" alt="PyPI - Downloads"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/implementation/MinVectorDB" alt="PyPI - Implementation"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/wheel/MinVectorDB" alt="PyPI - Wheel"></a>
+    <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
   </p>
 </div>
 
-
+<div align="center">
+  <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/terminal-demo-show.gif" alt="Demo"></a>
+</div>
 > **WARNING**: MinVectorDB is actively being updated, and API backward compatibility is not guaranteed. You should use version numbers as a strong constraint during deployment to avoid unnecessary feature conflicts and errors.
 > **Although our goal is to enable brute force search or inverted indexing on billion-scale vectors, we currently still recommend using it on a scale of millions of vectors or less for the best experience.**
 
 *MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, stateless, and easy to deploy locally. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
 
 - **Optimizing Global Search Performance**: We are focusing on algorithm and data structure enhancements to speed up searches across the database, enabling faster retrieval of vector data.
 - **Enhancing Cluster Search with Inverted Indexes**: Utilizing inverted index technology, we aim to refine the cluster search process for better search efficiency and precision.
 - **Refining Clustering Algorithms**: By improving our clustering algorithms, we intend to offer more precise and efficient data clustering to support complex queries.
 - **Facilitating Vector Modifications and Deletions**: We will introduce features to modify and delete vectors, allowing for more flexible data management.
 - **Implementing Rollback Strategies**: To increase database robustness and data security, rollback strategies will be added, helping users recover from incorrect operations or system failures easily.
 
-Additionally, we are introducing a query caching feature, with a default cache for the most recent 10,000 query results. In cases where a query does not hit the cache, the system will calculate the cosine similarity between the given vector and cached vectors. If the similarity is greater than 0.8, it will return the result of the closest cached vector directly.
+Additionally, we are introducing a query caching feature, with a default cache for the most recent 10,000 query results. In cases where a query does not hit the cache, the system will calculate the cosine similarity between the given vector and cached vectors. If the similarity is greater than 0.85, it will return the result of the closest cached vector directly.
 
 MinVectorDB focuses on achieving a 100% recall rate, prioritizing recall accuracy over high-speed search performance. This approach ensures that users can reliably retrieve all relevant vector data, making MinVectorDB particularly suitable for applications requiring responses within 100 milliseconds.
 
 While the project has not yet been benchmarked against other systems, we believe these planned features will significantly enhance MinVectorDB's capabilities in managing and retrieving vector data, addressing a wide range of user needs.
 
 ## Install
 
@@ -86,548 +59,404 @@
 # whether to add time to log
 os.environ['MVDB_LOG_WITH_TIME'] = 'False'  # default: False
 
 # clustering settings
 # kmeans epochs
 os.environ['MVDB_KMEANS_EPOCHS'] = '500'  # default: 100
 
-# bulk add batch size
-os.environ['MVDB_BULK_ADD_BATCH_SIZE'] = '100000'  # default: 100000
-
-# cache size
-os.environ['MVDB_CACHE_SIZE'] = '10000'  # default: 10000
+# query cache size
+os.environ['MVDB_QUERY_CACHE_SIZE'] = '10000'  # default: 10000
 
 # cosine similarity threshold for cache result matching 
-os.environ['MVDB_COSINE_SIMILARITY_THRESHOLD'] = '0.9'  # 'None' for disable this feature, default to 0.8
+os.environ['MVDB_COSINE_SIMILARITY_THRESHOLD'] = '0.9'  # 'None' for disable this feature, default to 0.85
 
 # computing platform, can be set to platforms supported by torch.device 
-os.environ['MVDB_COMPUTE_DEVICE'] = 'cpu' # default to 'cpu', torch.device
+os.environ['MVDB_COMPUTE_DEVICE'] = 'mps' # default to 'cpu', torch.device
+
+# specify the number of chunks in the memory cache
+os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20'  # default to '20', must be integer-like string
 ```
 
 
 ```python
 import min_vec
 print("MinVectorDB version is: ", min_vec.__version__)
 print("MinVectorDB all configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in min_vec.get_all_configs().items()]))
 ```
 
-    MinVectorDB version is:  0.2.2
+    MinVectorDB version is:  0.2.3
     MinVectorDB all configs:  
      - MVDB_LOG_LEVEL: INFO
      - MVDB_LOG_PATH: ./min_vec_db.log
      - MVDB_TRUNCATE_LOG: True
      - MVDB_LOG_WITH_TIME: False
      - MVDB_KMEANS_EPOCHS: 500
-     - MVDB_BULK_ADD_BATCH_SIZE: 100000
-     - MVDB_CACHE_SIZE: 10000
+     - MVDB_QUERY_CACHE_SIZE: 10000
      - MVDB_COSINE_SIMILARITY_THRESHOLD: 0.9
      - MVDB_COMPUTE_DEVICE: cpu
+     - MVDB_USER_MESSAGE_PATH: None
+     - MVDB_DATALOADER_BUFFER_SIZE: 20
 
 
-
-```python
-# define the display function, this is optional in actual use.
-try:
-    from IPython.display import display_markdown
-except ImportError:
-    def display_markdown(text, raw=True):
-        print(text)
-```
-
 ### Sequentially add vectors.
 
 
 ```python
 import numpy as np
 from tqdm import tqdm
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-vectors = 10_0000
-
-display_markdown("*Demo 1* -- **Sequentially add vectors**", raw=True)
-
-# distance can be 'L2' or 'cosine'
-# index_mode can be 'FLAT' or 'IVF-FLAT', default is 'IVF-FLAT'
-db = MinVectorDB(dim=1024, database_path='/Volumes/西数SSD/test_min_vec.mvdb', distance='cosine', index_mode='FLAT', chunk_size=100000, use_cache=True)
 
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
-timer.start()
+# distance can be 'L2' or 'cosine'
+# index_mode can be 'FLAT' or 'IVF-FLAT', default is 'IVF-FLAT'
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', distance='cosine',
+                 index_mode='FLAT', chunk_size=100000, use_cache=False, scaler_bits=8)
+
 # ========== Use automatic commit statements. Recommended. =============
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():
     # Define the initial ID.
     id = 0
-    for t in tqdm(get_test_vectors((vectors, 1024)), total=vectors, unit="vector"):
+    for t in tqdm(get_test_vectors((1000000, 1024)), total=1000000, unit="vector"):
+        if id == 0:
+            query = t / np.linalg.norm(t)
+            query_id = 0
+            query_field = None
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
-        # Here, normalization can be directly specified, achieving the same effect as the previous sentence.
         db.add_item(t, index=id, normalize=True, save_immediately=False)
 
-        # ID increments by 1 with each loop iteration.
         id += 1
 
-# ============== Or use manual commit statements. =================
-# id = 0
-# for t in get_test_vectors((vectors, 1024)):
-#     # Vectors need to be normalized before writing to the database.
-#     # t = t / np.linalg.norm(t) 
-#     # Here, normalization can be directly specified, achieving the same effect as the previous sentence.
-#     db.add_item(t, index=id, normalize=True)
-    
-#     # ID increments by 1 with each loop iteration.
-#     id += 1
-# db.commit()
-
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
-
-query = db.head()[0]
-query_id = db.head(returns='indices')[0]
-query_field = db.head(returns='fields')[0]
-
 res = db.query(query, k=10)
 
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 1* -- **Sequentially add vectors**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
-    //    dim=1024, database_path='/Volumes/西数SSD/test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=100000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    dim=1024, database_path='test_min_vec.mvdb', 
+    //    n_cluster=16, chunk_size=100000,
+    //    distance='cosine', index_mode='FLAT', 
+    //    dtypes='float32', use_cache=False, 
+    //    reindex_if_conflict=False, scaler_bits=8
     
-    100%|██████████| 100000/100000 [00:02<00:00, 42802.86vector/s]
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
+    100%|██████████| 1000000/1000000 [00:15<00:00, 65961.24vector/s]
 
 
-    
-    * [Insert data] Time cost 2.4119 s.
       - Query sample id:  0
-      - Query sample field:  
+      - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.14636 s
-    | - Query vector: [0.02898663 0.05306277 0.04289231 ... 0.0143056  0.01658326 0.04808333]
+    | - Database shape: (1000000, 1024)
+    | - Query time: 0.34045 s
     | - Query K: 10
-    | - Query fields: None
     | - Query normalize: False
-    | - Query subset_indices: None
-    | - Top 10 results index: [    0 67927 53447 47665 64134 13859 41949  5788 38082 18507]
-    | - Top 10 results similarity: [1.0000002  0.78101647 0.77775997 0.7771763  0.77591014 0.77581763
-     0.77578723 0.77570754 0.77500904 0.77420104]
+    | - Top 10 results index: [     0 126163 934623 376250 136782  67927 927723 454821 909201 283657]
+    | - Top 10 results similarity: [1.         0.7866893  0.7823357  0.78192943 0.78141373 0.78101647
+     0.78069043 0.7806051  0.78056455 0.78041667]
     * - END OF REPORT -
     
 
 
 ### Bulk add vectors
 
 
 ```python
 import numpy as np
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-display_markdown("*Demo 2* -- **Bulk add vectors**", raw=True)
-
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, n_cluster=8, index_mode='FLAT')
-
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
-
-timer.start()
+        
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='FLAT')
 
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():  
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
         vectors.append((t, id))
-        # ID increments by 1 with each loop iteration.
         id += 1
         
     # Here, normalization can be directly specified, achieving the same effect as `t = t / np.linalg.norm(t) `.
     db.bulk_add_items(vectors, normalize=True, save_immediately=False)
 
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
 
-query = db.head(10)[2]
-query_id = db.head(10, returns='indices')[2]
-query_field = db.head(10, returns='fields')[2]
+query = db.head(10)[0]
+query_id = db.head(10, returns='indices')[0]
+query_field = db.head(10, returns='fields')[0]
 
 res = db.query(query, k=10)
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
-
-timer.end()
-
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 2* -- **Bulk add vectors**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=10000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    n_cluster=16, chunk_size=10000,
+    //    distance='cosine', index_mode='FLAT', 
+    //    dtypes='float32', use_cache=True, 
+    //    reindex_if_conflict=False, scaler_bits=None
     
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-    
-    * [Insert data] Time cost 4.1953 s.
-      - Query sample id:  2
+      - Query sample id:  0
       - Query sample field:  
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.15137 s
-    | - Query vector: [0.04493065 0.00245387 0.03883836 ... 0.02070636 0.05214242 0.03655052]
+    | - Query time: 0.03720 s
     | - Query K: 10
-    | - Query fields: None
     | - Query normalize: False
-    | - Query subset_indices: None
-    | - Top 10 results index: [    2 91745 34952 73172 16234 21556 56017  3534   440 36253]
-    | - Top 10 results similarity: [0.99999994 0.7895216  0.78557634 0.7839494  0.78385794 0.78378147
-     0.78375924 0.78356993 0.7831306  0.78296286]
+    | - Top 10 results index: [    0 67927 53447 47665 64134 13859 41949  5788 38082 18507]
+    | - Top 10 results similarity: [1.0000002  0.78101647 0.77775997 0.7771763  0.77591014 0.77581763
+     0.77578723 0.77570754 0.77500904 0.77420104]
     * - END OF REPORT -
     
 
 
 ### Use field to improve Searching Recall
 
 
 ```python
 import numpy as np
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-display_markdown("*Demo 3* -- **Use field to improve Searching Recall**", raw=True)
-
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000)
 
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
-timer.start()
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000)
+
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
         vectors.append((t, id, 'test_'+str(id // 100)))
-        # ID increments by 1 with each loop iteration.
         id += 1
         
     db.bulk_add_items(vectors, normalize=True)
 
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
-
 query = db.head(10)[0]
 query_id = db.head(10, returns='indices')[0]
 query_field = db.head(10, returns='fields')[0]
 
 res = db.query(query, k=10, fields=[query_field])
 
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
-timer.end()
-
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 3* -- **Use field to improve Searching Recall**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=10000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='IVF-FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    n_cluster=16, chunk_size=10000,
+    //    distance='cosine', index_mode='IVF-FLAT', 
+    //    dtypes='float32', use_cache=True, 
+    //    reindex_if_conflict=False, scaler_bits=None
     
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
-    MinVectorDB - INFO - Building index...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-    
-    * [Insert data] Time cost 6.3419 s.
-      - Query sample id:  150
-      - Query sample field:  test_1
+      - Query sample id:  11
+      - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.12271 s
-    | - Query vector: [0.03762956 0.05180147 0.04209524 ... 0.04615058 0.05285349 0.05330994]
+    | - Query time: 0.01311 s
     | - Query K: 10
-    | - Query fields: ['test_1']
     | - Query normalize: False
-    | - Query subset_indices: None
-    | - Top 10 results index: [150 122 118 199 177 130 175 194 126 168]
-    | - Top 10 results similarity: [1.         0.7638782  0.76372206 0.7636392  0.7589303  0.75863093
-     0.7581293  0.7578685  0.75781167 0.75737965]
+    | - Top 10 results index: [11 11  2 58 71 71 88 88 81 81]
+    | - Top 10 results similarity: [1.         1.         0.7702445  0.76463264 0.764104   0.764104
+     0.7637025  0.7637025  0.7620634  0.7620634 ]
     * - END OF REPORT -
     
 
 
-    MinVectorDB - INFO - Saving ann model...
-    MinVectorDB - INFO - Saving ivf index...
-
-
 ### Use subset_indices to narrow down the search range
 
 
 ```python
 import numpy as np
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-display_markdown("*Demo 4* -- **Use subset_indices to narrow down the search range**", raw=True)
-
-timer.start()
-
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
 
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
+
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
         vectors.append((t, id, 'test_'+str(id // 100)))
-        # ID increments by 1 with each loop iteration.
         id += 1
         
     db.bulk_add_items(vectors, normalize=True)
 
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
-
 query = db.head(10)[0]
 query_id = db.head(10, returns='indices')[0]
 query_field = db.head(10, returns='fields')[0]
 
 # You may define both 'subset_indices' and 'fields'
 res = db.query(query, k=10, subset_indices=list(range(query_id - 20, query_id + 20)))
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
-timer.end()
-
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 4* -- **Use subset_indices to narrow down the search range**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=10000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='IVF-FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    n_cluster=16, chunk_size=10000,
+    //    distance='cosine', index_mode='IVF-FLAT', 
+    //    dtypes='float32', use_cache=True, 
+    //    reindex_if_conflict=False, scaler_bits=None
     
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
-    MinVectorDB - INFO - Building index...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-    
-    * [Insert data] Time cost 6.2138 s.
-      - Query sample id:  150
-      - Query sample field:  test_1
+      - Query sample id:  11
+      - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.10610 s
-    | - Query vector: [0.03762956 0.05180147 0.04209524 ... 0.04615058 0.05285349 0.05330994]
+    | - Query time: 0.01752 s
     | - Query K: 10
-    | - Query fields: None
     | - Query normalize: False
-    | - Query subset_indices: [130, 131, 132, 133, 134, 135, 136, 137, 138, 139, 140, 141, 142, 143, 144, 145, 146, 147, 148, 149, 150, 151, 152, 153, 154, 155, 156, 157, 158, 159, 160, 161, 162, 163, 164, 165, 166, 167, 168, 169]
-    | - Top 10 results index: [150 130 168 167 141 144 161 166 162 157]
-    | - Top 10 results similarity: [1.         0.75863093 0.75737965 0.75729394 0.75688565 0.7568122
-     0.75455916 0.7535342  0.7531498  0.7517347 ]
+    | - Top 10 results index: [11 11  2 25  4 19 21 29 30 13]
+    | - Top 10 results similarity: [1.         1.         0.7702445  0.7628149  0.7586509  0.75613594
+     0.7559968  0.7528333  0.74891967 0.7427169 ]
     * - END OF REPORT -
     
 
 
-    MinVectorDB - INFO - Saving ann model...
-    MinVectorDB - INFO - Saving ivf index...
-
-
 ### Conduct searches by specifying both subset_indices and fields simultaneously.
 
 
 ```python
 import numpy as np
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-display_markdown("*Demo 5* -- **Conduct searches by specifying both subset_indices and fields simultaneously**", raw=True)
-
-timer.start()
-
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000)
-
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, distance='L2')
+
+
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
+    last_field = None
     for t in get_test_vectors((100000, 1024)):
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
         vectors.append((t, id, 'test_'+str(id // 100)))
-        # ID increments by 1 with each loop iteration.
         id += 1
         
     db.bulk_add_items(vectors, normalize=True)
 
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
-
 query = db.head(10)[0]
 query_id = db.head(10, returns='indices')[0]
 query_field = db.head(10, returns='fields')[0]
 
 # You may define both 'subset_indices' and 'fields'
 # If there is no intersection between subset_indices and fields, there will be no result. 
 # If there is an intersection, the query results within the intersection will be returned.
-res = db.query(query, k=10, subset_indices=list(range(query_id-20, query_id + 20)), fields=['test_0', 'test_2'])
+res = db.query(query, k=10, subset_indices=list(range(query_id-20, query_id + 20)), fields=[query_field])
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 5* -- **Conduct searches by specifying both subset_indices and fields simultaneously**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=10000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='IVF-FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    n_cluster=16, chunk_size=10000,
+    //    distance='L2', index_mode='IVF-FLAT', 
+    //    dtypes='float32', use_cache=True, 
+    //    reindex_if_conflict=False, scaler_bits=None
     
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
-    MinVectorDB - INFO - Building index...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-    
-    * [Insert data] Time cost 6.1384 s.
-      - Query sample id:  150
-      - Query sample field:  test_1
+      - Query sample id:  11
+      - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.11414 s
-    | - Query vector: [0.03762956 0.05180147 0.04209524 ... 0.04615058 0.05285349 0.05330994]
+    | - Query time: 0.02081 s
     | - Query K: 10
-    | - Query fields: ['test_0', 'test_2']
     | - Query normalize: False
-    | - Query subset_indices: [130, 131, 132, 133, 134, 135, 136, 137, 138, 139, 140, 141, 142, 143, 144, 145, 146, 147, 148, 149, 150, 151, 152, 153, 154, 155, 156, 157, 158, 159, 160, 161, 162, 163, 164, 165, 166, 167, 168, 169]
-    | - Top 10 results index: []
-    | - Top 10 results similarity: []
+    | - Top 10 results index: [11 11  2 25  4 19 21 29 30  1]
+    | - Top 10 results similarity: [0.         0.         0.6778725  0.68874544 0.69476485 0.6983754
+     0.69857436 0.7030885  0.70863307 0.70987064]
     * - END OF REPORT -
     
 
-
-    MinVectorDB - INFO - Saving ann model...
-    MinVectorDB - INFO - Saving ivf index...
-
```

### Comparing `MinVectorDB-0.2.3/PKG-INFO` & `MinVectorDB-0.2.4/MinVectorDB.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,63 +1,66 @@
 Metadata-Version: 2.1
 Name: MinVectorDB
-Version: 0.2.3
+Version: 0.2.4
 Summary: MinVectorDB is a pure Python-implemented, lightweight, stateless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
 Home-page: https://github.com/BirchKwok/MinVectorDB
 Author: Birch Kwok
 Author-email: birchkwok@gmail.com
 Keywords: vector database
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.17.0
 Requires-Dist: spinesUtils>=0.3.13
 Requires-Dist: torch>=2.0.0
 Requires-Dist: msgpack>=1.0.2
 Requires-Dist: h5py>=3.4.0
 Requires-Dist: scikit-learn>=1.0.0
 Requires-Dist: cloudpickle>=2.0.0
 Requires-Dist: numexpr>=2.7.3
 Requires-Dist: pyroaring>=0.4.5
 
 <div align="center">
-  <h1>MinVectorDB</h1>
+  <h1><a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB"></a></h1>
   <h3>A pure Python-implemented, lightweight, stateless, locally deployed vector database.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/dm/MinVectorDB" alt="PyPI - Downloads"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/implementation/MinVectorDB" alt="PyPI - Implementation"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/wheel/MinVectorDB" alt="PyPI - Wheel"></a>
+    <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
   </p>
 </div>
 
-
+<div align="center">
+  <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/terminal-demo-show.gif" alt="Demo"></a>
+</div>
 > **WARNING**: MinVectorDB is actively being updated, and API backward compatibility is not guaranteed. You should use version numbers as a strong constraint during deployment to avoid unnecessary feature conflicts and errors.
 > **Although our goal is to enable brute force search or inverted indexing on billion-scale vectors, we currently still recommend using it on a scale of millions of vectors or less for the best experience.**
 
 *MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, stateless, and easy to deploy locally. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
 
 - **Optimizing Global Search Performance**: We are focusing on algorithm and data structure enhancements to speed up searches across the database, enabling faster retrieval of vector data.
 - **Enhancing Cluster Search with Inverted Indexes**: Utilizing inverted index technology, we aim to refine the cluster search process for better search efficiency and precision.
 - **Refining Clustering Algorithms**: By improving our clustering algorithms, we intend to offer more precise and efficient data clustering to support complex queries.
 - **Facilitating Vector Modifications and Deletions**: We will introduce features to modify and delete vectors, allowing for more flexible data management.
 - **Implementing Rollback Strategies**: To increase database robustness and data security, rollback strategies will be added, helping users recover from incorrect operations or system failures easily.
 
-Additionally, we are introducing a query caching feature, with a default cache for the most recent 10,000 query results. In cases where a query does not hit the cache, the system will calculate the cosine similarity between the given vector and cached vectors. If the similarity is greater than 0.8, it will return the result of the closest cached vector directly.
+Additionally, we are introducing a query caching feature, with a default cache for the most recent 10,000 query results. In cases where a query does not hit the cache, the system will calculate the cosine similarity between the given vector and cached vectors. If the similarity is greater than 0.85, it will return the result of the closest cached vector directly.
 
 MinVectorDB focuses on achieving a 100% recall rate, prioritizing recall accuracy over high-speed search performance. This approach ensures that users can reliably retrieve all relevant vector data, making MinVectorDB particularly suitable for applications requiring responses within 100 milliseconds.
 
 While the project has not yet been benchmarked against other systems, we believe these planned features will significantly enhance MinVectorDB's capabilities in managing and retrieving vector data, addressing a wide range of user needs.
 
 ## Install
 
@@ -86,548 +89,404 @@
 # whether to add time to log
 os.environ['MVDB_LOG_WITH_TIME'] = 'False'  # default: False
 
 # clustering settings
 # kmeans epochs
 os.environ['MVDB_KMEANS_EPOCHS'] = '500'  # default: 100
 
-# bulk add batch size
-os.environ['MVDB_BULK_ADD_BATCH_SIZE'] = '100000'  # default: 100000
-
-# cache size
-os.environ['MVDB_CACHE_SIZE'] = '10000'  # default: 10000
+# query cache size
+os.environ['MVDB_QUERY_CACHE_SIZE'] = '10000'  # default: 10000
 
 # cosine similarity threshold for cache result matching 
-os.environ['MVDB_COSINE_SIMILARITY_THRESHOLD'] = '0.9'  # 'None' for disable this feature, default to 0.8
+os.environ['MVDB_COSINE_SIMILARITY_THRESHOLD'] = '0.9'  # 'None' for disable this feature, default to 0.85
 
 # computing platform, can be set to platforms supported by torch.device 
-os.environ['MVDB_COMPUTE_DEVICE'] = 'cpu' # default to 'cpu', torch.device
+os.environ['MVDB_COMPUTE_DEVICE'] = 'mps' # default to 'cpu', torch.device
+
+# specify the number of chunks in the memory cache
+os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20'  # default to '20', must be integer-like string
 ```
 
 
 ```python
 import min_vec
 print("MinVectorDB version is: ", min_vec.__version__)
 print("MinVectorDB all configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in min_vec.get_all_configs().items()]))
 ```
 
-    MinVectorDB version is:  0.2.2
+    MinVectorDB version is:  0.2.3
     MinVectorDB all configs:  
      - MVDB_LOG_LEVEL: INFO
      - MVDB_LOG_PATH: ./min_vec_db.log
      - MVDB_TRUNCATE_LOG: True
      - MVDB_LOG_WITH_TIME: False
      - MVDB_KMEANS_EPOCHS: 500
-     - MVDB_BULK_ADD_BATCH_SIZE: 100000
-     - MVDB_CACHE_SIZE: 10000
+     - MVDB_QUERY_CACHE_SIZE: 10000
      - MVDB_COSINE_SIMILARITY_THRESHOLD: 0.9
      - MVDB_COMPUTE_DEVICE: cpu
+     - MVDB_USER_MESSAGE_PATH: None
+     - MVDB_DATALOADER_BUFFER_SIZE: 20
 
 
-
-```python
-# define the display function, this is optional in actual use.
-try:
-    from IPython.display import display_markdown
-except ImportError:
-    def display_markdown(text, raw=True):
-        print(text)
-```
-
 ### Sequentially add vectors.
 
 
 ```python
 import numpy as np
 from tqdm import tqdm
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-vectors = 10_0000
-
-display_markdown("*Demo 1* -- **Sequentially add vectors**", raw=True)
-
-# distance can be 'L2' or 'cosine'
-# index_mode can be 'FLAT' or 'IVF-FLAT', default is 'IVF-FLAT'
-db = MinVectorDB(dim=1024, database_path='/Volumes/西数SSD/test_min_vec.mvdb', distance='cosine', index_mode='FLAT', chunk_size=100000, use_cache=True)
 
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
-timer.start()
+# distance can be 'L2' or 'cosine'
+# index_mode can be 'FLAT' or 'IVF-FLAT', default is 'IVF-FLAT'
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', distance='cosine',
+                 index_mode='FLAT', chunk_size=100000, use_cache=False, scaler_bits=8)
+
 # ========== Use automatic commit statements. Recommended. =============
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():
     # Define the initial ID.
     id = 0
-    for t in tqdm(get_test_vectors((vectors, 1024)), total=vectors, unit="vector"):
+    for t in tqdm(get_test_vectors((1000000, 1024)), total=1000000, unit="vector"):
+        if id == 0:
+            query = t / np.linalg.norm(t)
+            query_id = 0
+            query_field = None
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
-        # Here, normalization can be directly specified, achieving the same effect as the previous sentence.
         db.add_item(t, index=id, normalize=True, save_immediately=False)
 
-        # ID increments by 1 with each loop iteration.
         id += 1
 
-# ============== Or use manual commit statements. =================
-# id = 0
-# for t in get_test_vectors((vectors, 1024)):
-#     # Vectors need to be normalized before writing to the database.
-#     # t = t / np.linalg.norm(t) 
-#     # Here, normalization can be directly specified, achieving the same effect as the previous sentence.
-#     db.add_item(t, index=id, normalize=True)
-    
-#     # ID increments by 1 with each loop iteration.
-#     id += 1
-# db.commit()
-
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
-
-query = db.head()[0]
-query_id = db.head(returns='indices')[0]
-query_field = db.head(returns='fields')[0]
-
 res = db.query(query, k=10)
 
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 1* -- **Sequentially add vectors**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
-    //    dim=1024, database_path='/Volumes/西数SSD/test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=100000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    dim=1024, database_path='test_min_vec.mvdb', 
+    //    n_cluster=16, chunk_size=100000,
+    //    distance='cosine', index_mode='FLAT', 
+    //    dtypes='float32', use_cache=False, 
+    //    reindex_if_conflict=False, scaler_bits=8
     
-    100%|██████████| 100000/100000 [00:02<00:00, 42802.86vector/s]
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
+    100%|██████████| 1000000/1000000 [00:15<00:00, 65961.24vector/s]
 
 
-    
-    * [Insert data] Time cost 2.4119 s.
       - Query sample id:  0
-      - Query sample field:  
+      - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.14636 s
-    | - Query vector: [0.02898663 0.05306277 0.04289231 ... 0.0143056  0.01658326 0.04808333]
+    | - Database shape: (1000000, 1024)
+    | - Query time: 0.34045 s
     | - Query K: 10
-    | - Query fields: None
     | - Query normalize: False
-    | - Query subset_indices: None
-    | - Top 10 results index: [    0 67927 53447 47665 64134 13859 41949  5788 38082 18507]
-    | - Top 10 results similarity: [1.0000002  0.78101647 0.77775997 0.7771763  0.77591014 0.77581763
-     0.77578723 0.77570754 0.77500904 0.77420104]
+    | - Top 10 results index: [     0 126163 934623 376250 136782  67927 927723 454821 909201 283657]
+    | - Top 10 results similarity: [1.         0.7866893  0.7823357  0.78192943 0.78141373 0.78101647
+     0.78069043 0.7806051  0.78056455 0.78041667]
     * - END OF REPORT -
     
 
 
 ### Bulk add vectors
 
 
 ```python
 import numpy as np
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-display_markdown("*Demo 2* -- **Bulk add vectors**", raw=True)
-
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, n_cluster=8, index_mode='FLAT')
-
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
-
-timer.start()
+        
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='FLAT')
 
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():  
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
         vectors.append((t, id))
-        # ID increments by 1 with each loop iteration.
         id += 1
         
     # Here, normalization can be directly specified, achieving the same effect as `t = t / np.linalg.norm(t) `.
     db.bulk_add_items(vectors, normalize=True, save_immediately=False)
 
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
 
-query = db.head(10)[2]
-query_id = db.head(10, returns='indices')[2]
-query_field = db.head(10, returns='fields')[2]
+query = db.head(10)[0]
+query_id = db.head(10, returns='indices')[0]
+query_field = db.head(10, returns='fields')[0]
 
 res = db.query(query, k=10)
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
-
-timer.end()
-
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 2* -- **Bulk add vectors**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=10000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    n_cluster=16, chunk_size=10000,
+    //    distance='cosine', index_mode='FLAT', 
+    //    dtypes='float32', use_cache=True, 
+    //    reindex_if_conflict=False, scaler_bits=None
     
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-    
-    * [Insert data] Time cost 4.1953 s.
-      - Query sample id:  2
+      - Query sample id:  0
       - Query sample field:  
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.15137 s
-    | - Query vector: [0.04493065 0.00245387 0.03883836 ... 0.02070636 0.05214242 0.03655052]
+    | - Query time: 0.03720 s
     | - Query K: 10
-    | - Query fields: None
     | - Query normalize: False
-    | - Query subset_indices: None
-    | - Top 10 results index: [    2 91745 34952 73172 16234 21556 56017  3534   440 36253]
-    | - Top 10 results similarity: [0.99999994 0.7895216  0.78557634 0.7839494  0.78385794 0.78378147
-     0.78375924 0.78356993 0.7831306  0.78296286]
+    | - Top 10 results index: [    0 67927 53447 47665 64134 13859 41949  5788 38082 18507]
+    | - Top 10 results similarity: [1.0000002  0.78101647 0.77775997 0.7771763  0.77591014 0.77581763
+     0.77578723 0.77570754 0.77500904 0.77420104]
     * - END OF REPORT -
     
 
 
 ### Use field to improve Searching Recall
 
 
 ```python
 import numpy as np
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-display_markdown("*Demo 3* -- **Use field to improve Searching Recall**", raw=True)
-
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000)
 
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
-timer.start()
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000)
+
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
         vectors.append((t, id, 'test_'+str(id // 100)))
-        # ID increments by 1 with each loop iteration.
         id += 1
         
     db.bulk_add_items(vectors, normalize=True)
 
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
-
 query = db.head(10)[0]
 query_id = db.head(10, returns='indices')[0]
 query_field = db.head(10, returns='fields')[0]
 
 res = db.query(query, k=10, fields=[query_field])
 
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
-timer.end()
-
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 3* -- **Use field to improve Searching Recall**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=10000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='IVF-FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    n_cluster=16, chunk_size=10000,
+    //    distance='cosine', index_mode='IVF-FLAT', 
+    //    dtypes='float32', use_cache=True, 
+    //    reindex_if_conflict=False, scaler_bits=None
     
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
-    MinVectorDB - INFO - Building index...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-    
-    * [Insert data] Time cost 6.3419 s.
-      - Query sample id:  150
-      - Query sample field:  test_1
+      - Query sample id:  11
+      - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.12271 s
-    | - Query vector: [0.03762956 0.05180147 0.04209524 ... 0.04615058 0.05285349 0.05330994]
+    | - Query time: 0.01311 s
     | - Query K: 10
-    | - Query fields: ['test_1']
     | - Query normalize: False
-    | - Query subset_indices: None
-    | - Top 10 results index: [150 122 118 199 177 130 175 194 126 168]
-    | - Top 10 results similarity: [1.         0.7638782  0.76372206 0.7636392  0.7589303  0.75863093
-     0.7581293  0.7578685  0.75781167 0.75737965]
+    | - Top 10 results index: [11 11  2 58 71 71 88 88 81 81]
+    | - Top 10 results similarity: [1.         1.         0.7702445  0.76463264 0.764104   0.764104
+     0.7637025  0.7637025  0.7620634  0.7620634 ]
     * - END OF REPORT -
     
 
 
-    MinVectorDB - INFO - Saving ann model...
-    MinVectorDB - INFO - Saving ivf index...
-
-
 ### Use subset_indices to narrow down the search range
 
 
 ```python
 import numpy as np
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-display_markdown("*Demo 4* -- **Use subset_indices to narrow down the search range**", raw=True)
-
-timer.start()
-
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
 
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
+
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
         vectors.append((t, id, 'test_'+str(id // 100)))
-        # ID increments by 1 with each loop iteration.
         id += 1
         
     db.bulk_add_items(vectors, normalize=True)
 
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
-
 query = db.head(10)[0]
 query_id = db.head(10, returns='indices')[0]
 query_field = db.head(10, returns='fields')[0]
 
 # You may define both 'subset_indices' and 'fields'
 res = db.query(query, k=10, subset_indices=list(range(query_id - 20, query_id + 20)))
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
-timer.end()
-
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 4* -- **Use subset_indices to narrow down the search range**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=10000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='IVF-FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    n_cluster=16, chunk_size=10000,
+    //    distance='cosine', index_mode='IVF-FLAT', 
+    //    dtypes='float32', use_cache=True, 
+    //    reindex_if_conflict=False, scaler_bits=None
     
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
-    MinVectorDB - INFO - Building index...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-    
-    * [Insert data] Time cost 6.2138 s.
-      - Query sample id:  150
-      - Query sample field:  test_1
+      - Query sample id:  11
+      - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.10610 s
-    | - Query vector: [0.03762956 0.05180147 0.04209524 ... 0.04615058 0.05285349 0.05330994]
+    | - Query time: 0.01752 s
     | - Query K: 10
-    | - Query fields: None
     | - Query normalize: False
-    | - Query subset_indices: [130, 131, 132, 133, 134, 135, 136, 137, 138, 139, 140, 141, 142, 143, 144, 145, 146, 147, 148, 149, 150, 151, 152, 153, 154, 155, 156, 157, 158, 159, 160, 161, 162, 163, 164, 165, 166, 167, 168, 169]
-    | - Top 10 results index: [150 130 168 167 141 144 161 166 162 157]
-    | - Top 10 results similarity: [1.         0.75863093 0.75737965 0.75729394 0.75688565 0.7568122
-     0.75455916 0.7535342  0.7531498  0.7517347 ]
+    | - Top 10 results index: [11 11  2 25  4 19 21 29 30 13]
+    | - Top 10 results similarity: [1.         1.         0.7702445  0.7628149  0.7586509  0.75613594
+     0.7559968  0.7528333  0.74891967 0.7427169 ]
     * - END OF REPORT -
     
 
 
-    MinVectorDB - INFO - Saving ann model...
-    MinVectorDB - INFO - Saving ivf index...
-
-
 ### Conduct searches by specifying both subset_indices and fields simultaneously.
 
 
 ```python
 import numpy as np
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-display_markdown("*Demo 5* -- **Conduct searches by specifying both subset_indices and fields simultaneously**", raw=True)
-
-timer.start()
-
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000)
-
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, distance='L2')
+
+
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
+    last_field = None
     for t in get_test_vectors((100000, 1024)):
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
         vectors.append((t, id, 'test_'+str(id // 100)))
-        # ID increments by 1 with each loop iteration.
         id += 1
         
     db.bulk_add_items(vectors, normalize=True)
 
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
-
 query = db.head(10)[0]
 query_id = db.head(10, returns='indices')[0]
 query_field = db.head(10, returns='fields')[0]
 
 # You may define both 'subset_indices' and 'fields'
 # If there is no intersection between subset_indices and fields, there will be no result. 
 # If there is an intersection, the query results within the intersection will be returned.
-res = db.query(query, k=10, subset_indices=list(range(query_id-20, query_id + 20)), fields=['test_0', 'test_2'])
+res = db.query(query, k=10, subset_indices=list(range(query_id-20, query_id + 20)), fields=[query_field])
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 5* -- **Conduct searches by specifying both subset_indices and fields simultaneously**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=10000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='IVF-FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    n_cluster=16, chunk_size=10000,
+    //    distance='L2', index_mode='IVF-FLAT', 
+    //    dtypes='float32', use_cache=True, 
+    //    reindex_if_conflict=False, scaler_bits=None
     
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
-    MinVectorDB - INFO - Building index...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-    
-    * [Insert data] Time cost 6.1384 s.
-      - Query sample id:  150
-      - Query sample field:  test_1
+      - Query sample id:  11
+      - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.11414 s
-    | - Query vector: [0.03762956 0.05180147 0.04209524 ... 0.04615058 0.05285349 0.05330994]
+    | - Query time: 0.02081 s
     | - Query K: 10
-    | - Query fields: ['test_0', 'test_2']
     | - Query normalize: False
-    | - Query subset_indices: [130, 131, 132, 133, 134, 135, 136, 137, 138, 139, 140, 141, 142, 143, 144, 145, 146, 147, 148, 149, 150, 151, 152, 153, 154, 155, 156, 157, 158, 159, 160, 161, 162, 163, 164, 165, 166, 167, 168, 169]
-    | - Top 10 results index: []
-    | - Top 10 results similarity: []
+    | - Top 10 results index: [11 11  2 25  4 19 21 29 30  1]
+    | - Top 10 results similarity: [0.         0.         0.6778725  0.68874544 0.69476485 0.6983754
+     0.69857436 0.7030885  0.70863307 0.70987064]
     * - END OF REPORT -
     
 
-
-    MinVectorDB - INFO - Saving ann model...
-    MinVectorDB - INFO - Saving ivf index...
-
```

### Comparing `MinVectorDB-0.2.3/README.md` & `MinVectorDB-0.2.4/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,66 @@
+Metadata-Version: 2.1
+Name: MinVectorDB
+Version: 0.2.4
+Summary: MinVectorDB is a pure Python-implemented, lightweight, stateless vector, locally deployed databasethat offers clear and concise Python APIs, aimed at lowering the barrier to the use of vector databases.
+Home-page: https://github.com/BirchKwok/MinVectorDB
+Author: Birch Kwok
+Author-email: birchkwok@gmail.com
+Keywords: vector database
+Classifier: Intended Audience :: Science/Research
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy>=1.17.0
+Requires-Dist: spinesUtils>=0.3.13
+Requires-Dist: torch>=2.0.0
+Requires-Dist: msgpack>=1.0.2
+Requires-Dist: h5py>=3.4.0
+Requires-Dist: scikit-learn>=1.0.0
+Requires-Dist: cloudpickle>=2.0.0
+Requires-Dist: numexpr>=2.7.3
+Requires-Dist: pyroaring>=0.4.5
+
 <div align="center">
-  <h1>MinVectorDB</h1>
+  <h1><a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/logo.png" alt="MinVectorDB"></a></h1>
   <h3>A pure Python-implemented, lightweight, stateless, locally deployed vector database.</h3>
   <p>
     <a href="https://badge.fury.io/py/MinVectorDB"><img src="https://badge.fury.io/py/MinVectorDB.svg" alt="PyPI version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/pyversions/MinVectorDB" alt="PyPI - Python Version"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/l/MinVectorDB" alt="PyPI - License"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/dm/MinVectorDB" alt="PyPI - Downloads"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/implementation/MinVectorDB" alt="PyPI - Implementation"></a>
     <a href="https://pypi.org/project/MinVectorDB/"><img src="https://img.shields.io/pypi/wheel/MinVectorDB" alt="PyPI - Wheel"></a>
+    <a href="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml"><img src="https://github.com/BirchKwok/MinVectorDB/actions/workflows/python-package.yml/badge.svg" alt="Python package"></a>
   </p>
 </div>
 
-
+<div align="center">
+  <a href="https://github.com/BirchKwok/MinVectorDB"><img src="https://github.com/BirchKwok/MinVectorDB/blob/main/pic/terminal-demo-show.gif" alt="Demo"></a>
+</div>
 > **WARNING**: MinVectorDB is actively being updated, and API backward compatibility is not guaranteed. You should use version numbers as a strong constraint during deployment to avoid unnecessary feature conflicts and errors.
 > **Although our goal is to enable brute force search or inverted indexing on billion-scale vectors, we currently still recommend using it on a scale of millions of vectors or less for the best experience.**
 
 *MinVectorDB* is a vector database implemented purely in Python, designed to be lightweight, stateless, and easy to deploy locally. It offers straightforward and clear Python APIs, aiming to lower the entry barrier for using vector databases. In response to user needs and to enhance its practicality, we are planning to introduce new features, including but not limited to:
 
 - **Optimizing Global Search Performance**: We are focusing on algorithm and data structure enhancements to speed up searches across the database, enabling faster retrieval of vector data.
 - **Enhancing Cluster Search with Inverted Indexes**: Utilizing inverted index technology, we aim to refine the cluster search process for better search efficiency and precision.
 - **Refining Clustering Algorithms**: By improving our clustering algorithms, we intend to offer more precise and efficient data clustering to support complex queries.
 - **Facilitating Vector Modifications and Deletions**: We will introduce features to modify and delete vectors, allowing for more flexible data management.
 - **Implementing Rollback Strategies**: To increase database robustness and data security, rollback strategies will be added, helping users recover from incorrect operations or system failures easily.
 
-Additionally, we are introducing a query caching feature, with a default cache for the most recent 10,000 query results. In cases where a query does not hit the cache, the system will calculate the cosine similarity between the given vector and cached vectors. If the similarity is greater than 0.8, it will return the result of the closest cached vector directly.
+Additionally, we are introducing a query caching feature, with a default cache for the most recent 10,000 query results. In cases where a query does not hit the cache, the system will calculate the cosine similarity between the given vector and cached vectors. If the similarity is greater than 0.85, it will return the result of the closest cached vector directly.
 
 MinVectorDB focuses on achieving a 100% recall rate, prioritizing recall accuracy over high-speed search performance. This approach ensures that users can reliably retrieve all relevant vector data, making MinVectorDB particularly suitable for applications requiring responses within 100 milliseconds.
 
 While the project has not yet been benchmarked against other systems, we believe these planned features will significantly enhance MinVectorDB's capabilities in managing and retrieving vector data, addressing a wide range of user needs.
 
 ## Install
 
@@ -56,548 +89,404 @@
 # whether to add time to log
 os.environ['MVDB_LOG_WITH_TIME'] = 'False'  # default: False
 
 # clustering settings
 # kmeans epochs
 os.environ['MVDB_KMEANS_EPOCHS'] = '500'  # default: 100
 
-# bulk add batch size
-os.environ['MVDB_BULK_ADD_BATCH_SIZE'] = '100000'  # default: 100000
-
-# cache size
-os.environ['MVDB_CACHE_SIZE'] = '10000'  # default: 10000
+# query cache size
+os.environ['MVDB_QUERY_CACHE_SIZE'] = '10000'  # default: 10000
 
 # cosine similarity threshold for cache result matching 
-os.environ['MVDB_COSINE_SIMILARITY_THRESHOLD'] = '0.9'  # 'None' for disable this feature, default to 0.8
+os.environ['MVDB_COSINE_SIMILARITY_THRESHOLD'] = '0.9'  # 'None' for disable this feature, default to 0.85
 
 # computing platform, can be set to platforms supported by torch.device 
-os.environ['MVDB_COMPUTE_DEVICE'] = 'cpu' # default to 'cpu', torch.device
+os.environ['MVDB_COMPUTE_DEVICE'] = 'mps' # default to 'cpu', torch.device
+
+# specify the number of chunks in the memory cache
+os.environ['MVDB_DATALOADER_BUFFER_SIZE'] = '20'  # default to '20', must be integer-like string
 ```
 
 
 ```python
 import min_vec
 print("MinVectorDB version is: ", min_vec.__version__)
 print("MinVectorDB all configs: ", '\n - ' + '\n - '.join([f'{k}: {v}' for k, v in min_vec.get_all_configs().items()]))
 ```
 
-    MinVectorDB version is:  0.2.2
+    MinVectorDB version is:  0.2.3
     MinVectorDB all configs:  
      - MVDB_LOG_LEVEL: INFO
      - MVDB_LOG_PATH: ./min_vec_db.log
      - MVDB_TRUNCATE_LOG: True
      - MVDB_LOG_WITH_TIME: False
      - MVDB_KMEANS_EPOCHS: 500
-     - MVDB_BULK_ADD_BATCH_SIZE: 100000
-     - MVDB_CACHE_SIZE: 10000
+     - MVDB_QUERY_CACHE_SIZE: 10000
      - MVDB_COSINE_SIMILARITY_THRESHOLD: 0.9
      - MVDB_COMPUTE_DEVICE: cpu
+     - MVDB_USER_MESSAGE_PATH: None
+     - MVDB_DATALOADER_BUFFER_SIZE: 20
 
 
-
-```python
-# define the display function, this is optional in actual use.
-try:
-    from IPython.display import display_markdown
-except ImportError:
-    def display_markdown(text, raw=True):
-        print(text)
-```
-
 ### Sequentially add vectors.
 
 
 ```python
 import numpy as np
 from tqdm import tqdm
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-vectors = 10_0000
-
-display_markdown("*Demo 1* -- **Sequentially add vectors**", raw=True)
-
-# distance can be 'L2' or 'cosine'
-# index_mode can be 'FLAT' or 'IVF-FLAT', default is 'IVF-FLAT'
-db = MinVectorDB(dim=1024, database_path='/Volumes/西数SSD/test_min_vec.mvdb', distance='cosine', index_mode='FLAT', chunk_size=100000, use_cache=True)
 
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
-timer.start()
+# distance can be 'L2' or 'cosine'
+# index_mode can be 'FLAT' or 'IVF-FLAT', default is 'IVF-FLAT'
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', distance='cosine',
+                 index_mode='FLAT', chunk_size=100000, use_cache=False, scaler_bits=8)
+
 # ========== Use automatic commit statements. Recommended. =============
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():
     # Define the initial ID.
     id = 0
-    for t in tqdm(get_test_vectors((vectors, 1024)), total=vectors, unit="vector"):
+    for t in tqdm(get_test_vectors((1000000, 1024)), total=1000000, unit="vector"):
+        if id == 0:
+            query = t / np.linalg.norm(t)
+            query_id = 0
+            query_field = None
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
-        # Here, normalization can be directly specified, achieving the same effect as the previous sentence.
         db.add_item(t, index=id, normalize=True, save_immediately=False)
 
-        # ID increments by 1 with each loop iteration.
         id += 1
 
-# ============== Or use manual commit statements. =================
-# id = 0
-# for t in get_test_vectors((vectors, 1024)):
-#     # Vectors need to be normalized before writing to the database.
-#     # t = t / np.linalg.norm(t) 
-#     # Here, normalization can be directly specified, achieving the same effect as the previous sentence.
-#     db.add_item(t, index=id, normalize=True)
-    
-#     # ID increments by 1 with each loop iteration.
-#     id += 1
-# db.commit()
-
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
-
-query = db.head()[0]
-query_id = db.head(returns='indices')[0]
-query_field = db.head(returns='fields')[0]
-
 res = db.query(query, k=10)
 
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 1* -- **Sequentially add vectors**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
-    //    dim=1024, database_path='/Volumes/西数SSD/test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=100000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    dim=1024, database_path='test_min_vec.mvdb', 
+    //    n_cluster=16, chunk_size=100000,
+    //    distance='cosine', index_mode='FLAT', 
+    //    dtypes='float32', use_cache=False, 
+    //    reindex_if_conflict=False, scaler_bits=8
     
-    100%|██████████| 100000/100000 [00:02<00:00, 42802.86vector/s]
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
+    100%|██████████| 1000000/1000000 [00:15<00:00, 65961.24vector/s]
 
 
-    
-    * [Insert data] Time cost 2.4119 s.
       - Query sample id:  0
-      - Query sample field:  
+      - Query sample field:  None
     
     * - MOST RECENT QUERY REPORT -
-    | - Database shape: (100000, 1024)
-    | - Query time: 0.14636 s
-    | - Query vector: [0.02898663 0.05306277 0.04289231 ... 0.0143056  0.01658326 0.04808333]
+    | - Database shape: (1000000, 1024)
+    | - Query time: 0.34045 s
     | - Query K: 10
-    | - Query fields: None
     | - Query normalize: False
-    | - Query subset_indices: None
-    | - Top 10 results index: [    0 67927 53447 47665 64134 13859 41949  5788 38082 18507]
-    | - Top 10 results similarity: [1.0000002  0.78101647 0.77775997 0.7771763  0.77591014 0.77581763
-     0.77578723 0.77570754 0.77500904 0.77420104]
+    | - Top 10 results index: [     0 126163 934623 376250 136782  67927 927723 454821 909201 283657]
+    | - Top 10 results similarity: [1.         0.7866893  0.7823357  0.78192943 0.78141373 0.78101647
+     0.78069043 0.7806051  0.78056455 0.78041667]
     * - END OF REPORT -
     
 
 
 ### Bulk add vectors
 
 
 ```python
 import numpy as np
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-display_markdown("*Demo 2* -- **Bulk add vectors**", raw=True)
-
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, n_cluster=8, index_mode='FLAT')
-
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
-
-timer.start()
+        
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='FLAT')
 
 # You can perform this operation multiple times, and the data will be appended to the database.
 with db.insert_session():  
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
         vectors.append((t, id))
-        # ID increments by 1 with each loop iteration.
         id += 1
         
     # Here, normalization can be directly specified, achieving the same effect as `t = t / np.linalg.norm(t) `.
     db.bulk_add_items(vectors, normalize=True, save_immediately=False)
 
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
 
-query = db.head(10)[2]
-query_id = db.head(10, returns='indices')[2]
-query_field = db.head(10, returns='fields')[2]
+query = db.head(10)[0]
+query_id = db.head(10, returns='indices')[0]
+query_field = db.head(10, returns='fields')[0]
 
 res = db.query(query, k=10)
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
-
-timer.end()
-
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 2* -- **Bulk add vectors**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=10000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    n_cluster=16, chunk_size=10000,
+    //    distance='cosine', index_mode='FLAT', 
+    //    dtypes='float32', use_cache=True, 
+    //    reindex_if_conflict=False, scaler_bits=None
     
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-    
-    * [Insert data] Time cost 4.1953 s.
-      - Query sample id:  2
+      - Query sample id:  0
       - Query sample field:  
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.15137 s
-    | - Query vector: [0.04493065 0.00245387 0.03883836 ... 0.02070636 0.05214242 0.03655052]
+    | - Query time: 0.03720 s
     | - Query K: 10
-    | - Query fields: None
     | - Query normalize: False
-    | - Query subset_indices: None
-    | - Top 10 results index: [    2 91745 34952 73172 16234 21556 56017  3534   440 36253]
-    | - Top 10 results similarity: [0.99999994 0.7895216  0.78557634 0.7839494  0.78385794 0.78378147
-     0.78375924 0.78356993 0.7831306  0.78296286]
+    | - Top 10 results index: [    0 67927 53447 47665 64134 13859 41949  5788 38082 18507]
+    | - Top 10 results similarity: [1.0000002  0.78101647 0.77775997 0.7771763  0.77591014 0.77581763
+     0.77578723 0.77570754 0.77500904 0.77420104]
     * - END OF REPORT -
     
 
 
 ### Use field to improve Searching Recall
 
 
 ```python
 import numpy as np
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-display_markdown("*Demo 3* -- **Use field to improve Searching Recall**", raw=True)
-
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000)
 
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
-timer.start()
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000)
+
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
         vectors.append((t, id, 'test_'+str(id // 100)))
-        # ID increments by 1 with each loop iteration.
         id += 1
         
     db.bulk_add_items(vectors, normalize=True)
 
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
-
 query = db.head(10)[0]
 query_id = db.head(10, returns='indices')[0]
 query_field = db.head(10, returns='fields')[0]
 
 res = db.query(query, k=10, fields=[query_field])
 
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
-timer.end()
-
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 3* -- **Use field to improve Searching Recall**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=10000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='IVF-FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    n_cluster=16, chunk_size=10000,
+    //    distance='cosine', index_mode='IVF-FLAT', 
+    //    dtypes='float32', use_cache=True, 
+    //    reindex_if_conflict=False, scaler_bits=None
     
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
-    MinVectorDB - INFO - Building index...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-    
-    * [Insert data] Time cost 6.3419 s.
-      - Query sample id:  150
-      - Query sample field:  test_1
+      - Query sample id:  11
+      - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.12271 s
-    | - Query vector: [0.03762956 0.05180147 0.04209524 ... 0.04615058 0.05285349 0.05330994]
+    | - Query time: 0.01311 s
     | - Query K: 10
-    | - Query fields: ['test_1']
     | - Query normalize: False
-    | - Query subset_indices: None
-    | - Top 10 results index: [150 122 118 199 177 130 175 194 126 168]
-    | - Top 10 results similarity: [1.         0.7638782  0.76372206 0.7636392  0.7589303  0.75863093
-     0.7581293  0.7578685  0.75781167 0.75737965]
+    | - Top 10 results index: [11 11  2 58 71 71 88 88 81 81]
+    | - Top 10 results similarity: [1.         1.         0.7702445  0.76463264 0.764104   0.764104
+     0.7637025  0.7637025  0.7620634  0.7620634 ]
     * - END OF REPORT -
     
 
 
-    MinVectorDB - INFO - Saving ann model...
-    MinVectorDB - INFO - Saving ivf index...
-
-
 ### Use subset_indices to narrow down the search range
 
 
 ```python
 import numpy as np
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-display_markdown("*Demo 4* -- **Use subset_indices to narrow down the search range**", raw=True)
-
-timer.start()
-
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
 
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, index_mode='IVF-FLAT')
+
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
     for t in get_test_vectors((100000, 1024)):
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
         vectors.append((t, id, 'test_'+str(id // 100)))
-        # ID increments by 1 with each loop iteration.
         id += 1
         
     db.bulk_add_items(vectors, normalize=True)
 
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
-
 query = db.head(10)[0]
 query_id = db.head(10, returns='indices')[0]
 query_field = db.head(10, returns='fields')[0]
 
 # You may define both 'subset_indices' and 'fields'
 res = db.query(query, k=10, subset_indices=list(range(query_id - 20, query_id + 20)))
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
-timer.end()
-
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 4* -- **Use subset_indices to narrow down the search range**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=10000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='IVF-FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    n_cluster=16, chunk_size=10000,
+    //    distance='cosine', index_mode='IVF-FLAT', 
+    //    dtypes='float32', use_cache=True, 
+    //    reindex_if_conflict=False, scaler_bits=None
     
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
-    MinVectorDB - INFO - Building index...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-    
-    * [Insert data] Time cost 6.2138 s.
-      - Query sample id:  150
-      - Query sample field:  test_1
+      - Query sample id:  11
+      - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.10610 s
-    | - Query vector: [0.03762956 0.05180147 0.04209524 ... 0.04615058 0.05285349 0.05330994]
+    | - Query time: 0.01752 s
     | - Query K: 10
-    | - Query fields: None
     | - Query normalize: False
-    | - Query subset_indices: [130, 131, 132, 133, 134, 135, 136, 137, 138, 139, 140, 141, 142, 143, 144, 145, 146, 147, 148, 149, 150, 151, 152, 153, 154, 155, 156, 157, 158, 159, 160, 161, 162, 163, 164, 165, 166, 167, 168, 169]
-    | - Top 10 results index: [150 130 168 167 141 144 161 166 162 157]
-    | - Top 10 results similarity: [1.         0.75863093 0.75737965 0.75729394 0.75688565 0.7568122
-     0.75455916 0.7535342  0.7531498  0.7517347 ]
+    | - Top 10 results index: [11 11  2 25  4 19 21 29 30 13]
+    | - Top 10 results similarity: [1.         1.         0.7702445  0.7628149  0.7586509  0.75613594
+     0.7559968  0.7528333  0.74891967 0.7427169 ]
     * - END OF REPORT -
     
 
 
-    MinVectorDB - INFO - Saving ann model...
-    MinVectorDB - INFO - Saving ivf index...
-
-
 ### Conduct searches by specifying both subset_indices and fields simultaneously.
 
 
 ```python
 import numpy as np
 
-from spinesUtils.timer import Timer
 from min_vec import MinVectorDB
 
-timer = Timer()
-
-display_markdown("*Demo 5* -- **Conduct searches by specifying both subset_indices and fields simultaneously**", raw=True)
-
-timer.start()
-
-db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000)
-
+# Generate vectors that need to be saved, this code is only for this demo
 np.random.seed(23)
-
-
 def get_test_vectors(shape):
     for i in range(shape[0]):
         yield np.random.random(shape[1])
 
+db = MinVectorDB(dim=1024, database_path='test_min_vec.mvdb', chunk_size=10000, distance='L2')
+
+
 with db.insert_session():     
     # Define the initial ID.
     id = 0
     vectors = []
+    last_field = None
     for t in get_test_vectors((100000, 1024)):
         # Vectors need to be normalized before writing to the database.
-        # t = t / np.linalg.norm(t) 
         vectors.append((t, id, 'test_'+str(id // 100)))
-        # ID increments by 1 with each loop iteration.
         id += 1
         
     db.bulk_add_items(vectors, normalize=True)
 
-print(f"\n* [Insert data] Time cost {timer.last_timestamp_diff():>.4f} s.")
-
 query = db.head(10)[0]
 query_id = db.head(10, returns='indices')[0]
 query_field = db.head(10, returns='fields')[0]
 
 # You may define both 'subset_indices' and 'fields'
 # If there is no intersection between subset_indices and fields, there will be no result. 
 # If there is an intersection, the query results within the intersection will be returned.
-res = db.query(query, k=10, subset_indices=list(range(query_id-20, query_id + 20)), fields=['test_0', 'test_2'])
+res = db.query(query, k=10, subset_indices=list(range(query_id-20, query_id + 20)), fields=[query_field])
 print("  - Query sample id: ", query_id)
 print("  - Query sample field: ", query_field)
 
 # Query report
 print(db.query_report_)
 
 # This sentence is for demo demonstration purposes, 
 # to clear the currently created .mvdb files from the database, 
 # but this is optional in actual use.
 db.delete()
 ```
 
-
-*Demo 5* -- **Conduct searches by specifying both subset_indices and fields simultaneously**
-
-
     MinVectorDB - INFO - Initializing MinVectorDB with: 
     //    dim=1024, database_path='test_min_vec.mvdb', 
-    //    n_cluster=8, chunk_size=10000,
-    //    distance='cosine', bloom_filter_size=100000000, 
-    //    index_mode='IVF-FLAT', dtypes='float32',
-    //    use_cache=True, reindex_if_conflict=False
+    //    n_cluster=16, chunk_size=10000,
+    //    distance='L2', index_mode='IVF-FLAT', 
+    //    dtypes='float32', use_cache=True, 
+    //    reindex_if_conflict=False, scaler_bits=None
     
-    MinVectorDB - INFO - Saving chunk immediately...
-    MinVectorDB - INFO - Saving id filter...
-    MinVectorDB - INFO - Building index...
+    MinVectorDB - INFO - Initializing database folder path: 'test_min_vec/'
 
 
-    
-    * [Insert data] Time cost 6.1384 s.
-      - Query sample id:  150
-      - Query sample field:  test_1
+      - Query sample id:  11
+      - Query sample field:  test_0
     
     * - MOST RECENT QUERY REPORT -
     | - Database shape: (100000, 1024)
-    | - Query time: 0.11414 s
-    | - Query vector: [0.03762956 0.05180147 0.04209524 ... 0.04615058 0.05285349 0.05330994]
+    | - Query time: 0.02081 s
     | - Query K: 10
-    | - Query fields: ['test_0', 'test_2']
     | - Query normalize: False
-    | - Query subset_indices: [130, 131, 132, 133, 134, 135, 136, 137, 138, 139, 140, 141, 142, 143, 144, 145, 146, 147, 148, 149, 150, 151, 152, 153, 154, 155, 156, 157, 158, 159, 160, 161, 162, 163, 164, 165, 166, 167, 168, 169]
-    | - Top 10 results index: []
-    | - Top 10 results similarity: []
+    | - Top 10 results index: [11 11  2 25  4 19 21 29 30  1]
+    | - Top 10 results similarity: [0.         0.         0.6778725  0.68874544 0.69476485 0.6983754
+     0.69857436 0.7030885  0.70863307 0.70987064]
     * - END OF REPORT -
     
 
-
-    MinVectorDB - INFO - Saving ann model...
-    MinVectorDB - INFO - Saving ivf index...
-
```

### Comparing `MinVectorDB-0.2.3/min_vec/api.py` & `MinVectorDB-0.2.4/min_vec/api/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """api.py - The MinVectorDB API."""
+import gc
 
-from min_vec.config import *
+from min_vec.configs.config import *
 
 
 class MinVectorDB:
     """
     A class for managing a vector database stored in .mvdb files and computing vectors similarity.
     """
 
     from spinesUtils.asserts import ParameterValuesAssert, ParameterTypeAssert
 
     @ParameterTypeAssert({
         'use_cache': bool, 'reindex_if_conflict': bool
     }, func_name='MinVectorDB')
     def __init__(
-            self, dim, database_path, n_cluster=8, chunk_size=100_000, distance='cosine',
-            index_mode='IVF-FLAT', dtypes='float64',
-            use_cache=True, reindex_if_conflict=False, scaler_bits=8
+            self, dim, database_path, n_cluster=16, chunk_size=100_000, distance='cosine',
+            index_mode='IVF-FLAT', dtypes='float32',
+            use_cache=True, reindex_if_conflict=False, scaler_bits=None, n_threads=None
     ) -> None:
         """
         Initialize the vector database.
 
         Parameters:
             dim (int): Dimension of the vectors.
             database_path (str): Path to the database file.
@@ -30,26 +31,28 @@
                 Options are 'cosine' or 'L2' for Euclidean distance. Default is 'cosine'.
             index_mode (str): The storage mode of the database.
                 Options are 'FLAT' or 'IVF-FLAT'. Default is 'IVF-FLAT'.
             dtypes (str): The data type of the vectors. Default is 'float32'.
                 Options are 'float16', 'float32' or 'float64'.
             use_cache (bool): Whether to use cache for query. Default is True.
             reindex_if_conflict (bool): Whether to reindex if there is a conflict. Default is False.
-            scaler_bits (int): The number of bits for scalar quantization. Default is 8.
+            scaler_bits (int): The number of bits for scalar quantization.
                 Options are 8, 16, or 32. The default is None, which means no scalar quantization.
                 The 8 for 8-bit, 16 for 16-bit, and 32 for 32-bit.
+            n_threads (int): The number of threads to use for parallel processing. Default is None,
+                which means the number of CPUs.
 
         Raises:
             ValueError: If `chunk_size` is less than or equal to 1.
         """
         from spinesUtils.logging import Logger
         from spinesUtils.timer import Timer
 
-        from min_vec.query import DatabaseQuery
-        from min_vec.matrix_serializer import MatrixSerializer
+        from min_vec.execution_layer.query import DatabaseQuery
+        from min_vec.execution_layer.matrix_serializer import MatrixSerializer
 
         logger = Logger(
             fp=MVDB_LOG_PATH,
             name='MinVectorDB',
             truncate_file=MVDB_TRUNCATE_LOG,
             with_time=MVDB_LOG_WITH_TIME,
             level=MVDB_LOG_LEVEL
@@ -71,20 +74,20 @@
             n_clusters=n_cluster,
             chunk_size=chunk_size,
             distance=distance,
             index_mode=index_mode,
             logger=logger,
             dtypes=dtypes,
             reindex_if_conflict=reindex_if_conflict,
-            scaler_bits=scaler_bits
+            scaler_bits=scaler_bits,
+            n_threads=n_threads
         )
         # matrix_serializer functions
         self.add_item = self._matrix_serializer.add_item
         self.bulk_add_items = self._matrix_serializer.bulk_add_items
-        self.delete = self._matrix_serializer.delete
         self._data_loader = self._matrix_serializer.iterable_dataloader
         self.check_commit = self._matrix_serializer.check_commit
         self._id_filter = self._matrix_serializer.id_filter
         self.commit = self._matrix_serializer.commit
 
         self._timer = Timer()
         self.use_cache = use_cache
@@ -112,19 +115,16 @@
             res = self._matrix_query.query(vector=vector, k=k, fields=fields, normalize=normalize,
                                            subset_indices=subset_indices, index_mode=self._matrix_serializer.index_mode,
                                            now_time=datetime.datetime.now().timestamp(), distance=self.distance)
 
         time_cost = self._timer.last_timestamp_diff()
         self._most_recent_query_report['Database shape'] = self.shape
         self._most_recent_query_report['Query time'] = f"{time_cost :>.5f} s"
-        self._most_recent_query_report['Query vector'] = vector
         self._most_recent_query_report['Query K'] = k
-        self._most_recent_query_report['Query fields'] = fields
         self._most_recent_query_report['Query normalize'] = normalize
-        self._most_recent_query_report['Query subset_indices'] = subset_indices
         self._most_recent_query_report[f'Top {k} results index'] = res[0]
         self._most_recent_query_report[f'Top {k} results similarity'] = res[1]
 
         return res
 
     @property
     def shape(self):
@@ -139,15 +139,16 @@
     def _get_n_elements(self, returns, n, from_tail=False):
         """get the first/last n vectors/indices/fields in the database."""
         import numpy as np
 
         _database = None
         _indices = []
         _fields = []
-        for database, indices, fields in self._data_loader(read_chunk_only=False, from_tail=from_tail):
+        for database, indices, fields in self._data_loader(read_chunk_only=False, from_tail=from_tail,
+                                                           order_read=True):
             if _database is None:
                 _database = database
             else:
                 _database = np.vstack((_database, database))
 
             _indices.extend(indices)
             _fields.extend(fields)
@@ -203,18 +204,27 @@
 
         return self._get_n_elements(returns, n, from_tail=True)
 
     def insert_session(self):
         """
         Create a session to insert data, which will automatically commit the data when the session ends.
         """
-        from min_vec.session import DatabaseSession
+        from min_vec.execution_layer.session import DatabaseSession
 
         return DatabaseSession(self)
 
+    def delete(self):
+        """
+        Delete the database.
+        """
+        self._matrix_serializer.delete()
+        self._matrix_query.query.clear_cache()
+
+        gc.collect()
+
     @property
     def query_report_(self):
         """
         Return the most recent query report.
         """
         # print as a pretty string
         # title use bold font
@@ -241,16 +251,22 @@
             'Database reindex_if_conflict': self._matrix_serializer.reindex_if_conflict,
             'Database status': 'DELETED' if self._matrix_serializer.IS_DELETED else 'ACTIVE'
         }}
 
         return db_report
 
     def __repr__(self):
-        title = "MinVectorDB object with status: \n"
+        title = "Deleted MinVectorDB object with status: \n"
         report = '\n* - DATABASE STATUS REPORT -\n'
         for key, value in self.status_report_['DATABASE STATUS REPORT'].items():
             report += f'| - {key}: {value}\n'
 
         return title + report
 
     def __str__(self):
         return self.__repr__()
+
+    def __len__(self):
+        return self.shape[0]
+
+    def is_deleted(self):
+        return self._matrix_serializer.IS_DELETED
```

### Comparing `MinVectorDB-0.2.3/min_vec/config.py` & `MinVectorDB-0.2.4/min_vec/configs/config.py`

 * *Files 19% similar despite different names*

```diff
@@ -29,34 +29,31 @@
 
 
 MVDB_LOG_LEVEL = get_env_variable('MVDB_LOG_LEVEL', 'INFO', str)
 MVDB_LOG_PATH = get_env_variable('MVDB_LOG_PATH', None, str)
 MVDB_TRUNCATE_LOG = get_env_variable('MVDB_TRUNCATE_LOG', True, bool)
 MVDB_LOG_WITH_TIME = get_env_variable('MVDB_LOG_WITH_TIME', False, bool)
 MVDB_KMEANS_EPOCHS = get_env_variable('MVDB_KMEANS_EPOCHS', 100, int)
-MVDB_BULK_ADD_BATCH_SIZE = get_env_variable('MVDB_BULK_ADD_BATCH_SIZE', 100000, int)
-MVDB_CACHE_SIZE = get_env_variable('MVDB_CACHE_SIZE', 10000, int)
+MVDB_QUERY_CACHE_SIZE = get_env_variable('MVDB_QUERY_CACHE_SIZE', 10000, int)
+MVDB_DATALOADER_BUFFER_SIZE = get_env_variable('MVDB_DATALOADER_BUFFER_SIZE', 20, int)
 
-MVDB_COSINE_SIMILARITY_THRESHOLD = os.environ.get('MVDB_COSINE_SIMILARITY_THRESHOLD', 0.8)
+MVDB_COSINE_SIMILARITY_THRESHOLD = os.environ.get('MVDB_COSINE_SIMILARITY_THRESHOLD', 0.85)
 if MVDB_COSINE_SIMILARITY_THRESHOLD == 'None':
     MVDB_COSINE_SIMILARITY_THRESHOLD = None
 else:
     MVDB_COSINE_SIMILARITY_THRESHOLD = float(MVDB_COSINE_SIMILARITY_THRESHOLD)
 
 MVDB_COMPUTE_DEVICE = get_env_variable('MVDB_COMPUTE_DEVICE', 'cuda' if torch.cuda.is_available() else 'cpu', str)
 
-MVDB_USER_MESSAGE_PATH = get_env_variable('MVDB_USER_MESSAGE_PATH', None, str)
-
 
 def get_all_configs():
     return {
         'MVDB_LOG_LEVEL': MVDB_LOG_LEVEL,
         'MVDB_LOG_PATH': MVDB_LOG_PATH,
         'MVDB_TRUNCATE_LOG': MVDB_TRUNCATE_LOG,
         'MVDB_LOG_WITH_TIME': MVDB_LOG_WITH_TIME,
         'MVDB_KMEANS_EPOCHS': MVDB_KMEANS_EPOCHS,
-        'MVDB_BULK_ADD_BATCH_SIZE': MVDB_BULK_ADD_BATCH_SIZE,
-        'MVDB_CACHE_SIZE': MVDB_CACHE_SIZE,
+        'MVDB_QUERY_CACHE_SIZE': MVDB_QUERY_CACHE_SIZE,
         'MVDB_COSINE_SIMILARITY_THRESHOLD': MVDB_COSINE_SIMILARITY_THRESHOLD,
-        'MVDB_COMPUTE_DEVICE': MVDB_COMPUTE_DEVICE
+        'MVDB_COMPUTE_DEVICE': MVDB_COMPUTE_DEVICE,
+        'MVDB_DATALOADER_BUFFER_SIZE': MVDB_DATALOADER_BUFFER_SIZE
     }
-
```

### Comparing `MinVectorDB-0.2.3/min_vec/fields_mapper.py` & `MinVectorDB-0.2.4/min_vec/data_structures/fields_mapper.py`

 * *Files identical despite different names*

### Comparing `MinVectorDB-0.2.3/min_vec/filter.py` & `MinVectorDB-0.2.4/min_vec/data_structures/filter.py`

 * *Files identical despite different names*

### Comparing `MinVectorDB-0.2.3/min_vec/kmeans.py` & `MinVectorDB-0.2.4/min_vec/data_structures/kmeans.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from sklearn.cluster import MiniBatchKMeans
 
 
 class BatchKMeans:
     def __init__(self, n_clusters, random_state=42, epochs=100, batch_size=1024, distance='euclidean'):
         self.model = MiniBatchKMeans(n_clusters=n_clusters, random_state=random_state, max_iter=epochs,
-                                     batch_size=batch_size, n_init='auto', reassignment_ratio=0)
+                                     batch_size=batch_size, n_init='auto')
 
         self.n_clusters = n_clusters
         self.distance = distance
         self.epochs = epochs
         self.batch_size = batch_size
 
         self.fitted = False
```

### Comparing `MinVectorDB-0.2.3/min_vec/matrix_serializer.py` & `MinVectorDB-0.2.4/min_vec/execution_layer/matrix_serializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-import os.path
 from datetime import datetime
-from functools import lru_cache
 from pathlib import Path
 import shutil
 
 import numpy as np
 from spinesUtils.asserts import raise_if
 
-from min_vec.engines import to_normalize
-from min_vec.filter import IDFilter
-from min_vec.utils import io_checker
-from min_vec.config import *
-from min_vec.kmeans import BatchKMeans
-from min_vec.scaler import ScalarQuantization
-from min_vec.fields_mapper import FieldsMapper
-from min_vec.storage import StorageWorker
+from min_vec.computational_layer.engines import to_normalize
+from min_vec.data_structures.filter import IDFilter
+from min_vec.utils.utils import io_checker
+from min_vec.configs.config import *
+from min_vec.data_structures.kmeans import BatchKMeans
+from min_vec.data_structures.scaler import ScalarQuantization
+from min_vec.data_structures.fields_mapper import FieldsMapper
+from min_vec.storage_layer.storage import StorageWorker
 
 
 class MatrixSerializer:
     def __init__(
             self, dim, database_path, distance, logger, n_clusters=16, chunk_size=1_000_000,
-            index_mode='IVF-FLAT', dtypes='float64',
-            reindex_if_conflict=False, scaler_bits=8
+            index_mode='IVF-FLAT', dtypes='float32',
+            reindex_if_conflict=False, scaler_bits=None, n_threads=10
     ) -> None:
         """
         Initialize the vector database.
 
         Parameters:
             dim (int): Dimension of the vectors.
             database_path (str): Path to the database file.
@@ -36,17 +34,18 @@
             chunk_size (int): The size of each data chunk. Default is 1_000_000.
             index_mode (str): The index mode of the database.
                 Options are 'FLAT' or 'IVF-FLAT'. Default is 'IVF-FLAT'.
             dtypes (str): The data type of the vectors. Default is 'float32'.
                 Options are 'float16', 'float32' or 'float64'.
             reindex_if_conflict (bool): Whether to reindex the database if there is an index mode conflict.
                 Default is False.
-            scaler_bits (int): The number of bits for scalar quantization. Default is 8.
+            scaler_bits (int): The number of bits for scalar quantization. Default is None.
                 Options are 8, 16, 32. If None, scalar quantization will not be used.
                 The 8 bits for uint8, 16 bits for uint16, 32 bits for uint32.
+            n_threads (int): The number of threads to use for reading and writing the database. Default is 10.
 
         Raises:
             ValueError: If `chunk_size` is less than or equal to 1.
         """
         raise_if(ValueError, not isinstance(dim, int), 'dim must be int')
         raise_if(ValueError, not str(database_path).endswith('mvdb'), 'database_path must end with .mvdb')
         raise_if(ValueError, not isinstance(chunk_size, int) or chunk_size <= 1,
@@ -63,15 +62,15 @@
         self.last_commit_time = None
         self.reindex_if_conflict = reindex_if_conflict
         # set commit flag, if the flag is True, the database will not be saved
         self.COMMIT_FLAG = True
         # set flag for scalar quantization, if the flag is True, the database will be rescanned for scalar quantization
         self.RESCAN_FOR_SQ_FLAG = False
 
-        self.IS_DELETED = None
+        self.IS_DELETED = False
 
         self.logger = logger
 
         # set parent path
         self._initialize_parent_path(database_path)
 
         self._dtypes_map = {'float16': np.float16, 'float32': np.float32, 'float64': np.float64}
@@ -92,22 +91,22 @@
         self._filter_path = self.database_path_parent / 'id_filter.mvdb'
         # set device
         self.device = torch.device(MVDB_COMPUTE_DEVICE)
         # set scalar quantization bits
         self.scaler_bits = scaler_bits if scaler_bits is not None else None
 
         # set database path
-        self.database_path = self.database_path_parent / Path(database_path).name
+        self.database_path = self.database_path_parent / Path(database_path).name.split('.mvdb')[0]
 
         # initialize the storage worker
-        self.storage_worker = StorageWorker(self.database_path, self.dim, self.chunk_size)
+        self.storage_worker = StorageWorker(self.database_path_parent, self.dim, self.chunk_size, n_threads=n_threads)
 
-        self.logger.info(f"Initializing database folder path: '{'.mvdb'.join(database_path.split('.mvdb')[:-1])}/',"
-                         " database file path: "
-                         f"'{'.mvdb'.join(database_path.split('.mvdb')[:-1]) + '/' + database_path}'")
+        self.logger.info(f"Initializing database folder path: '{'.mvdb'.join(database_path.split('.mvdb')[:-1])}/'")
+        if MVDB_COMPUTE_DEVICE != 'cpu':
+            self.logger.info(f"Using device: {MVDB_COMPUTE_DEVICE}")
 
         # ============== Loading or create one empty database ==============
         # first of all, initialize a database
         self.database = []
         self.indices = []
         self.fields = []
 
@@ -278,15 +277,15 @@
     def reset_database(self):
         """Reset the database to its initial state with zeros."""
         self.database = []
         self.indices = []
         self.fields = []
 
     @io_checker
-    def iterable_dataloader(self, read_chunk_only=False, from_tail=False, mode='eager'):
+    def iterable_dataloader(self, read_chunk_only=False, from_tail=False, mode='eager', order_read=False):
         """
         Generator for loading the database and index.
 
         Parameters:
             read_chunk_only (bool): Whether to read only the chunk.
             from_tail (bool): Whether to read from the end of the file.
             mode (str): The mode of the generator. Options are 'eager' or 'lazy'. Default is 'eager'.
@@ -297,25 +296,30 @@
         Raises:
             FileNotFoundError: If the file does not exist.
             IOError: If the file cannot be read.
             PermissionError: If the file cannot be read due to permission issues.
             UnKnownError: If an unknown error occurs.
         """
         if self.scaler_bits is not None:
-            decoder = self.scaler.decode
-        else:
-            decoder = lambda x: x
+            # decoder = self.scaler.decode
+            self.storage_worker.update_scaler(self.scaler)
+        # else:
+        #     decoder = lambda x: x
 
         read_type = 'all' if not read_chunk_only else 'chunk'
 
-        for data, indices, fields in self.storage_worker.read(read_type=read_type, reverse=from_tail):
+        for data, indices, fields in self.storage_worker.read(read_type=read_type, reverse=from_tail,
+                                                              order_read=order_read):
+            if data is None:
+                continue
+
             if mode == 'lazy':
-                yield decoder(data), indices, fields
+                yield data, indices, fields
             else:
-                yield decoder(data), indices, self.fields_mapper.decode(fields)
+                yield data, indices, self.fields_mapper.decode(fields)
 
     def cluster_dataloader(self, cluster_id, mode='eager'):
         """
         Generator for loading the database and index. Only used for querying when index_mode is IVF-FLAT.
 
         Parameters:
             cluster_id (int): The cluster id.
@@ -328,23 +332,24 @@
             FileNotFoundError: If the file does not exist.
             IOError: If the file cannot be read.
             PermissionError: If the file cannot be read due to permission issues.
             UnKnownError: If an unknown error occurs.
         """
         if self.scaler_bits is not None:
             raise_if(ValueError, not self.scaler.fitted, 'The model must be fitted before decoding.')
-            decoder = self.scaler.decode
-        else:
-            decoder = lambda x: x
+            # decoder = self.scaler.decode
+            self.storage_worker.update_scaler(self.scaler)
+        # else:
+        #     decoder = lambda x: x
 
         for data, indices, fields in self.storage_worker.read(read_type='cluster', cluster_id=str(cluster_id)):
             if mode == 'lazy':
-                yield decoder(data), indices, fields
+                yield data, indices, fields
             else:
-                yield decoder(data), indices, self.fields_mapper.decode(fields)
+                yield data, indices, self.fields_mapper.decode(fields)
 
     def _is_database_reset(self):
         """
         Check if the database is in its reset state (empty list).
 
         Returns:
             bool: True if the database is reset, False otherwise.
@@ -366,30 +371,25 @@
         """
         Reset the chunk partition.
         """
         self.storage_worker.delete_chunk()
 
     def save_data(self, data, indices, fields, to_chunk=True, cluster_id=None):
         """Optimized method to save data to chunk or cluster group with reusable logic."""
-        data_type = self.dtypes
-
         if self.scaler_bits is not None:
-            self.scaler.partial_fit(data)
-            data = self.scaler.encode(data)
-            data_type = self.scaler.bits
+            self.storage_worker.update_scaler(self.scaler)
 
         if isinstance(fields, str) or all(isinstance(i, str) for i in fields):
             fields_indices = self.fields_mapper.encode(fields)
         else:
             fields_indices = fields
 
         self.storage_worker.write(data, indices, fields_indices,
                                   write_type='chunk' if to_chunk else 'cluster',
-                                  cluster_id=str(cluster_id) if cluster_id is not None else cluster_id,
-                                  data_dtype=data_type)
+                                  cluster_id=str(cluster_id) if cluster_id is not None else cluster_id)
 
     @io_checker
     def save_chunk_immediately(self):
         """
         Save the current state of the database to a .mvdb file.
 
         Returns:
@@ -425,38 +425,38 @@
 
     def commit(self):
         """
         Save the database, ensuring that all data is written to disk.
         This method is required to be called after saving vectors to query them.
         """
         if not self.COMMIT_FLAG:
-            self.logger.info('Saving chunk immediately...')
+            self.logger.debug('Saving chunk immediately...')
             self.save_chunk_immediately()
 
-            self.logger.info('Saving id filter...')
+            self.logger.debug('Saving id filter...')
             # save filter
             self.id_filter.to_file(self._filter_path)
 
             # save scalar quantization model
             if self.scaler_bits is not None:
-                self.logger.info('Saving scalar quantization model...')
+                self.logger.debug('Saving scalar quantization model...')
                 self.scaler.save(self.database_path_parent / 'sq_model.mvdb')
 
             # save fields mapper
-            self.logger.info('Saving fields mapper...')
+            self.logger.debug('Saving fields mapper...')
             self.fields_mapper.save(self.database_path_parent / 'fields_mapper.mvdb')
 
             chunk_partition_size = self.storage_worker.get_shape(read_type='chunk')[0]
             if chunk_partition_size >= 100000 and self.index_mode != 'FLAT':
-                self.logger.info('Building index...')
+                self.logger.debug('Building index...')
                 # build index
                 self.build_index()
 
                 # save ivf index and k-means model
-                self.logger.info('Saving ann model...')
+                self.logger.debug('Saving ann model...')
                 self.ann_model.save(self.database_path_parent / 'ann_model.mvdb')
 
             self.reset_database()
 
             # save params
             self.storage_worker.write_file_attributes({'index_mode': self.index_mode})
 
@@ -478,62 +478,62 @@
     def _process_vector_item(self, vector, index, field, normalize):
         if index in self.id_filter:
             raise ValueError(f'id {index} already exists')
 
         if len(vector) != self.dim:
             raise ValueError(f'vector dim error, expect {self.dim}, got {len(vector)}')
 
-        vector = vector.astype(self.dtypes)
+        if vector.dtype != self.dtypes:
+            vector = vector.astype(self.dtypes)
 
         if vector.ndim == 1:
             vector = vector.reshape(1, -1)
 
         if normalize:
             vector = to_normalize(vector)
 
         return vector, index, field if field is not None else ''
 
-    def bulk_add_items(self, vectors, normalize: bool = False, save_immediately=False):
+    def bulk_add_items(self, vectors, *, normalize: bool = False, save_immediately=False):
         """
         Bulk add vectors to the database in batches.
 
         Parameters: vectors (list or tuple): A list or tuple of vectors to be saved. Each vector can be a tuple of (
             vector, id, field).
-        normalize (bool): Whether to normalize the input vector.
-        save_immediately (bool): Whether to save the database immediately.
+        normalize (bool, optional, keyword-only): Whether to normalize the input vectors. Default is False.
+        save_immediately (bool, optional, keyword-only): Whether to save the database immediately. Default is False.
 
         Returns:
             list: A list of indices where the vectors are stored.
         """
         raise_if(ValueError, not isinstance(vectors, (tuple, list)),
                  f'vectors must be tuple or list, got {type(vectors)}')
         raise_if(ValueError, not isinstance(normalize, bool),
                  f'normalize must be bool, got {type(normalize)}')
         raise_if(ValueError, not isinstance(save_immediately, bool),
                  f'save_immediately must be bool, got {type(save_immediately)}')
-        raise_if(ValueError, not all(1 <= len(i) <= 3 and isinstance(i, tuple) for i in vectors),
-                 f'vectors must be tuple of (vector, id, field), got {vectors}')
-
-        batch_size = MVDB_BULK_ADD_BATCH_SIZE
+        raise_if(ValueError, not all(isinstance(i, tuple) for i in vectors),
+                 f'vectors must be tuple of (vector, id[optional], field[optional]).')
 
         new_ids = []
 
-        for i in range(0, len(vectors), batch_size):
-            batch = vectors[i:i + batch_size]
-            # temp_vectors, temp_indices, temp_fields = [], [], []
+        for i in range(0, len(vectors), self.chunk_size):
+            batch = vectors[i:i + self.chunk_size]
 
             for sample in batch:
                 if len(sample) == 1:
                     vector = sample[0]
                     index = None
                     field = ''
                 elif len(sample) == 2:
                     vector, index = sample
                     field = ''
                 else:
+                    raise_if(ValueError, len(sample) != 3,
+                             f'vectors must be tuple of (vector, id[optional], field[optional]).')
                     vector, index, field = sample
 
                 index = self._generate_new_id() if index is None else index
 
                 raise_if(ValueError, index < 0, f'id must be greater than 0, got {index}')
 
                 field = '' if field is None else field
@@ -549,25 +549,26 @@
             self.save_chunk_immediately() if save_immediately else self.auto_save_chunk()
 
         if self.COMMIT_FLAG:
             self.COMMIT_FLAG = False
 
         return new_ids
 
-    def add_item(self, vector, index: int = None, field: str = None, normalize: bool = False,
+    def add_item(self, vector, *, index: int = None, field: str = None, normalize: bool = False,
                  save_immediately=False) -> int:
         """
         Add a single vector to the database.
 
         Parameters:
             vector (np.ndarray): The vector to be added.
-            index (int, optional): Optional ID for the vector.
-            field (str, optional): Optional field for the vector.
-            normalize (bool): Whether to normalize the input vector.
-            save_immediately (bool): Whether to save the database immediately.
+            index (int, optional, keyword-only): The ID of the vector. If None, a new ID will be generated.
+            field (str, optional, keyword-only): The field of the vector. Default is None. If None, the field will be
+                set to an empty string.
+            normalize (bool, optional, keyword-only): Whether to normalize the input vector. Default is False.
+            save_immediately (bool, optional, keyword-only): Whether to save the database immediately. Default is False.
         Returns:
             int: The ID of the added vector.
 
         Raises:
             ValueError: If the vector dimensions don't match or the ID already exists.
         """
         raise_if(ValueError, len(vector) != self.dim,
@@ -607,28 +608,32 @@
     def delete(self):
         """Delete database."""
         if not self.database_path_parent.exists():
             return None
 
         try:
             shutil.rmtree(self.database_path_parent)
-            self.IS_DELETED = True
         except FileNotFoundError:
             pass
 
+        self.IS_DELETED = True
         self.reset_database()
 
         # reinitialize
         if self.scaler_bits is not None:
             self._initialize_scalar_quantization()
 
         self._initialize_fields_mapper()
         self._initialize_ann_model()
         self._initialize_id_filter()
 
+        # clear cache
+        self.storage_worker.clear_cache()
+
+
     def _kmeans_clustering(self, data):
         """kmeans clustering"""
         self.ann_model = self.ann_model.partial_fit(data)
 
         return self.ann_model.cluster_centers_, self.ann_model.labels_
 
     def _clustering_for_ivf(self, data, indices, fields):
@@ -681,21 +686,11 @@
 
             if len(all_vectors) == 0:
                 continue
 
             self.save_data(all_vectors, all_indices, all_fields, to_chunk=False,
                            cluster_id=cluster_id)
 
-    @lru_cache(maxsize=1)
-    def _get_shape(self, mtime):
-        """
-        Return the shape of the entire database.
-
-        Returns:
-            tuple: The number of vectors and the dimension of each vector in the database.
-        """
-        return self.storage_worker.get_shape(read_type='all')
-
     @property
     def shape(self):
         self.check_commit()
-        return self._get_shape(int(os.path.getmtime(self.database_path) * 1000))
+        return tuple(self.storage_worker.get_shape(read_type='all'))
```

### Comparing `MinVectorDB-0.2.3/min_vec/query.py` & `MinVectorDB-0.2.4/min_vec/execution_layer/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 """query.py: this file is used to query the database for the vectors most similar to the given vector."""
-from spinesUtils.asserts import raise_if_not
+import os
+from concurrent.futures import ThreadPoolExecutor
 
-from min_vec.config import *
+from pyroaring import BitMap
+
+from min_vec.configs.config import *
+from min_vec.computational_layer.engines import argsort_topk
 
 
 class DatabaseQuery:
-    from min_vec.utils import VectorCache
+    from min_vec.utils.utils import QueryVectorCache
 
     def __init__(self, matrix_serializer) -> None:
         """
         Query the database for the vectors most similar to the given vector.
 
         Parameters:
             matrix_serializer (MatrixSerializer): The database to be queried.
         """
-        from min_vec.engines import cosine_distance, euclidean_distance
+        from min_vec.computational_layer.engines import cosine_distance, euclidean_distance
 
         self.matrix_serializer = matrix_serializer
 
         self.logger = self.matrix_serializer.logger
         # attributes
         self.dtypes = self.matrix_serializer.dtypes
         self.distance = self.matrix_serializer.distance
@@ -64,38 +68,38 @@
         if subset_indices is not None:
             subset_indices = sorted(list(set(subset_indices)))
             si_condition = np.isin(index_chunk, subset_indices)
 
         if field_condition is not None and si_condition is not None:
             condition = np.logical_and(field_condition, si_condition)
             database_chunk = database_chunk[condition]
-            index_chunk = np.array(index_chunk)[condition]
+            index_chunk = index_chunk[condition]
         elif field_condition is not None:
             condition = field_condition
             database_chunk = database_chunk[condition]
-            index_chunk = np.array(index_chunk)[condition]
+            index_chunk = index_chunk[condition]
         elif si_condition is not None:
             condition = si_condition
             database_chunk = database_chunk[condition]
-            index_chunk = np.array(index_chunk)[condition]
+            index_chunk = index_chunk[condition]
 
         if len(index_chunk) == 0:
             return [], []
 
         # Distance calculation core code
-        scores = self.distance_func(database_chunk, vector, device=self.device)
+        scores = self.distance_func(vector, database_chunk, device=self.device)
 
         if scores.ndim == 0:
             scores = [scores]
         elif scores.ndim == 2:
             scores = scores.squeeze()
 
         return index_chunk, scores
 
-    @VectorCache(MVDB_CACHE_SIZE)
+    @QueryVectorCache(MVDB_QUERY_CACHE_SIZE)
     def query(self, vector, k: int | str = 12,
               fields: list = None, normalize: bool = False, subset_indices=None, **kwargs):
         """
         Query the database for the vectors most similar to the given vector in batches.
 
         Parameters:
             vector (np.ndarray): The query vector.
@@ -110,15 +114,15 @@
         Raises:
             ValueError: If the database is empty.
         """
 
         import numpy as np
         from spinesUtils.asserts import raise_if
 
-        from min_vec.engines import to_normalize
+        from min_vec.computational_layer.engines import to_normalize
 
         self.logger.debug(f'Query vector: {vector.tolist()}')
         self.logger.debug(f'Query k: {k}')
         self.logger.debug(f'Query fields: {fields}')
         self.logger.debug(f'Query normalize: {normalize}')
         self.logger.debug(f'Query subset_indices: {subset_indices}')
 
@@ -147,74 +151,69 @@
 
         vector = to_normalize(vector) if normalize else vector
 
         vector = vector.reshape(1, -1) if vector.ndim == 1 else vector
 
         all_scores = []
         all_index = []
-        unique_indices = set()
+        unique_indices = BitMap()
 
         def sort_results(all_s, all_i):
             all_scores_i = np.array(all_s)
             all_index_i = np.array(all_i)
-            top_k_indices = np.argsort(self.is_reversed * all_scores_i)[:k]
+
+            top_k_indices = argsort_topk(self.is_reversed * all_scores_i, k)
 
             return all_index_i[top_k_indices], all_scores_i[top_k_indices]
 
-        def batch_query(vector, fields=None, subset_indices=None, is_ivf=True, cluster_id=None):
+        def batch_query(vector, fields=None, subset_indices=None, is_ivf=True, cluster_id=None, sort=True):
             nonlocal all_scores, all_index
 
             dataloader = self.matrix_serializer.cluster_dataloader(cluster_id, mode='lazy') \
                 if is_ivf and self.matrix_serializer.ann_model \
                 else self.matrix_serializer.iterable_dataloader(mode='lazy')
 
-            # for i in dataloader:
-            #     print(i)
-
-            futures = list(filter(lambda x: len(x[0]) != 0, map(
-                lambda x: self._query_chunk(x[0], x[1], x[2], vector, fields, subset_indices),
-                dataloader
-            )))
+            with ThreadPoolExecutor(max_workers=os.cpu_count()) as executor:
+                futures = [i for i in executor.map(
+                    lambda x: self._query_chunk(x[0], x[1], x[2], vector, fields, subset_indices), dataloader)
+                    if len(i[0]) != 0]
 
-            if len(futures) == 0:
+            if not futures:
                 return [], []
 
             index, scores = zip(*futures)
+
             # if index[0] is iterable, then index is a tuple of numpy ndarray, so we need to flatten it
             if len(index[0].shape) > 0:
                 index = [item for sublist in index for item in sublist]
                 scores = [item for sublist in scores for item in sublist]
 
             index = np.array(index)
             scores = np.array(scores)
 
             if len(index) != 0:
-                new_index = index[~np.isin(index, list(unique_indices))]
-                new_scores = scores[~np.isin(index, list(unique_indices))]
+                new_index = index[~np.isin(index, unique_indices.to_array())]
+                new_scores = scores[~np.isin(index, unique_indices.to_array())]
                 all_scores.extend(new_scores)
                 all_index.extend(new_index)
                 unique_indices.update(new_index)
 
-            del futures
-
-            all_scores_inside = np.array(all_scores)
-            all_index_inside = np.array(all_index)
-
-            return sort_results(all_scores_inside, all_index_inside)
+            return sort_results(all_scores, all_index) if sort else None
 
         # if the index mode is FLAT, use FLAT
         if not (self.matrix_serializer.ann_model is not None and self.matrix_serializer.ann_model.fitted):
             return batch_query(vector, fields, subset_indices, False)
 
         # otherwise, use IVF-FLAT
-        cluster_distances = self.distance_func(vector, self.matrix_serializer.ann_model.cluster_centers_.T,
+        cluster_distances = self.distance_func(vector, self.matrix_serializer.ann_model.cluster_centers_,
                                                device=self.device).squeeze()
 
-        cluster_id_sorted = np.argsort(cluster_distances)[::-1]
+        cluster_id_sorted = np.argsort(cluster_distances)[::-1] if self.distance == 'cosine' else np.argsort(
+            cluster_distances)
 
         for cluster_id in cluster_id_sorted:
-            batch_query(vector, fields, subset_indices, cluster_id=str(cluster_id))
+            batch_query(vector, fields, subset_indices, cluster_id=str(cluster_id), sort=False)
 
             if len(all_index) >= k:
                 break
 
-        return sort_results(np.array(all_scores), np.array(all_index))
+        return sort_results(all_scores, all_index)
```

### Comparing `MinVectorDB-0.2.3/min_vec/utils.py` & `MinVectorDB-0.2.4/min_vec/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """utils.py: this file contains some useful functions and decorators."""
 
 from functools import wraps
 
-from min_vec.config import MVDB_COSINE_SIMILARITY_THRESHOLD
+from min_vec.configs.config import MVDB_COSINE_SIMILARITY_THRESHOLD
 
 
 class UnKnownError(Exception):
     pass
 
 
 def io_checker(func):
@@ -31,22 +31,22 @@
         except Exception:
             raise_if(UnKnownError, True, f"Encounter Unknown Error "
                                          f"when read or write the file.")
 
     return wrapper
 
 
-class VectorCache:
+class QueryVectorCache:
     """A decorator that caches the results of a function call with the same arguments.
         Only use for DatabaseQuery.query function.
     """
 
     def __init__(self, max_size=1000):
         from collections import OrderedDict
-        from min_vec.engines import cosine_distance
+        from min_vec.computational_layer.engines import cosine_distance
 
         self.cache = OrderedDict()
         self.max_size = max_size
         self._cosine_similarity = cosine_distance
 
     def clear_cache(self):
         self.cache.clear()
```

### Comparing `MinVectorDB-0.2.3/setup.py` & `MinVectorDB-0.2.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 from setuptools import find_packages, setup
 
 
 def read_requirements(path):
     return list(Path(path).read_text().splitlines())
 
 
+reqs = read_requirements(Path('.').parent.joinpath("requirements.txt"))
+
+
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='MinVectorDB',
-    version="0.2.3",
+    version="0.2.4",
     description='MinVectorDB is a pure Python-implemented, lightweight, stateless vector, locally deployed database' \
                 'that offers clear and concise Python APIs, aimed at lowering the barrier to ' \
                 'the use of vector databases.',
     keywords='vector database',
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -27,24 +30,14 @@
         'Topic :: Scientific/Engineering',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
-    python_requires=">=3.9",
+    python_requires=">=3.10",
     url='https://github.com/BirchKwok/MinVectorDB',
     author='Birch Kwok',
     author_email='birchkwok@gmail.com',
-    install_requires=[
-        'numpy>=1.17.0',
-        'spinesUtils>=0.3.13',
-        'torch>=2.0.0',
-        'msgpack>=1.0.2',
-        'h5py>=3.4.0',
-        'scikit-learn>=1.0.0',
-        'cloudpickle>=2.0.0',
-        'numexpr>=2.7.3',
-        'pyroaring>=0.4.5',
-    ],
+    install_requires=reqs,
     zip_safe=False,
 )
```

### Comparing `MinVectorDB-0.2.3/test/test_model.py` & `MinVectorDB-0.2.4/test/test_model.py`

 * *Files identical despite different names*

