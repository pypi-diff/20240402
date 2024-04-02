# Comparing `tmp/epochalyst-0.1.7.tar.gz` & `tmp/epochalyst-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epochalyst-0.1.7.tar", last modified: Fri Mar 22 09:50:46 2024, max compression
+gzip compressed data, was "epochalyst-0.2.tar", last modified: Tue Apr  2 11:55:01 2024, max compression
```

## Comparing `epochalyst-0.1.7.tar` & `epochalyst-0.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:50:46.668656 epochalyst-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-03-22 09:50:42.000000 epochalyst-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-03-22 09:50:46.668656 epochalyst-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-22 09:50:42.000000 epochalyst-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:50:46.664656 epochalyst-0.1.7/epochalyst/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:50:46.664656 epochalyst-0.1.7/epochalyst/_core/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:50:46.664656 epochalyst-0.1.7/epochalyst/_core/_caching/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/_core/_caching/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13453 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/_core/_caching/_cacher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:50:46.664656 epochalyst-0.1.7/epochalyst/_core/_logging/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/_core/_logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/_core/_logging/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:50:46.664656 epochalyst-0.1.7/epochalyst/_core/_pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/_core/_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/_core/_pipeline/_custom_data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:50:46.668656 epochalyst-0.1.7/epochalyst/logging/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/logging/section_separator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:50:46.668656 epochalyst-0.1.7/epochalyst/pipeline/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/pipeline/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:50:46.668656 epochalyst-0.1.7/epochalyst/pipeline/model/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/pipeline/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/pipeline/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:50:46.668656 epochalyst-0.1.7/epochalyst/pipeline/model/training/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/pipeline/model/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/pipeline/model/training/pretrain_block.py
--rw-r--r--   0 runner    (1001) docker     (127)    23439 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/pipeline/model/training/torch_trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/pipeline/model/training/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4568 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/pipeline/model/training/training_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:50:46.668656 epochalyst-0.1.7/epochalyst/pipeline/model/transformation/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/pipeline/model/transformation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/pipeline/model/transformation/transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-03-22 09:50:42.000000 epochalyst-0.1.7/epochalyst/pipeline/model/transformation/transformation_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 09:50:46.668656 epochalyst-0.1.7/epochalyst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-03-22 09:50:46.000000 epochalyst-0.1.7/epochalyst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-22 09:50:46.000000 epochalyst-0.1.7/epochalyst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 09:50:46.000000 epochalyst-0.1.7/epochalyst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-22 09:50:46.000000 epochalyst-0.1.7/epochalyst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 09:50:46.000000 epochalyst-0.1.7/epochalyst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-22 09:50:42.000000 epochalyst-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 09:50:46.668656 epochalyst-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.669842 epochalyst-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-02 11:54:53.000000 epochalyst-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-02 11:55:01.669842 epochalyst-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-02 11:54:53.000000 epochalyst-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.661842 epochalyst-0.2/epochalyst/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/_core/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/_core/_caching/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/_caching/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14747 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/_caching/_cacher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/_core/_logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/_logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/_logging/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/_core/_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/_core/_pipeline/_custom_data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/logging/section_separator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/pipeline/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/pipeline/model/training/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/training/pretrain_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23839 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/training/torch_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/training/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/training/training_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.665842 epochalyst-0.2/epochalyst/pipeline/model/transformation/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/transformation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/transformation/transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-02 11:54:53.000000 epochalyst-0.2/epochalyst/pipeline/model/transformation/transformation_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 11:55:01.669842 epochalyst-0.2/epochalyst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-02 11:55:01.000000 epochalyst-0.2/epochalyst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-02 11:55:01.000000 epochalyst-0.2/epochalyst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 11:55:01.000000 epochalyst-0.2/epochalyst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-02 11:55:01.000000 epochalyst-0.2/epochalyst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 11:55:01.000000 epochalyst-0.2/epochalyst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-02 11:54:53.000000 epochalyst-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 11:55:01.669842 epochalyst-0.2/setup.cfg
```

### Comparing `epochalyst-0.1.7/LICENSE` & `epochalyst-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `epochalyst-0.1.7/PKG-INFO` & `epochalyst-0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: epochalyst
-Version: 0.1.7
+Version: 0.2
 Summary: This package contains the code for team Epoch's pipeline
 Author-email: Jasper van Selm <jmvanselm@gmail.com>, Ariel Ebersberger <arielebersberger@gmail.com>, Tolga Kopar <cahittolgakopar@gmail.com>, Jeffrey Lim <jeffrey-lim@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22.4
-Requires-Dist: dask>=2023.12.0
-Requires-Dist: pandas>=1.3.0
-Requires-Dist: pyarrow>=6.0.0
 Requires-Dist: torch>=2.1.0
-Requires-Dist: agogos>=0.2.1
+Requires-Dist: agogos==0.3.4
 
 ![image](./docs/_static/images/logo/Epochalyst_Logo_Dark.png#gh-light-mode-only)
 ![image](./docs/_static/images/logo/Epochalyst_Logo_Light.png#gh-dark-mode-only)
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/epochalyst.svg)](https://pypi.org/project/epochalyst/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/epochalyst.svg?label=PyPI%20downloads)](https://pypi.org/project/epochalyst/)
 
@@ -43,17 +40,28 @@
 ```
 
 ## Pytest coverage report
 
 To generate pytest coverage report run
 
 ```python
-python -m pytest --cov=epochalyst --cov-report=html:coverage_re
+python -m pytest --cov=epochalyst --cov-branch --cov-report=html:coverage_re
 ```
 
+## Imports
+
+### Caching
+
+For caching some imports are only required, these have to be manually installed when needed
+- dask >= 2023.12.0 & dask-expr
+- pandas >= 1.3.0
+- polars
+- pyarrow >= 6.0.0 (Read parquet files)
+- annotated-types >= 0.6.0
+
 ## Documentation
 
 Documentation is generated using [Sphinx](https://www.sphinx-doc.org/en/master/).
 
 To make the documentation, run `make html` with `docs` as the working directory. The documentation can then be found in `docs/_build/html/index.html`.
 
 Here's a short command to make the documentation and open it in the browser:
```

### Comparing `epochalyst-0.1.7/README.md` & `epochalyst-0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -25,17 +25,28 @@
 ```
 
 ## Pytest coverage report
 
 To generate pytest coverage report run
 
 ```python
-python -m pytest --cov=epochalyst --cov-report=html:coverage_re
+python -m pytest --cov=epochalyst --cov-branch --cov-report=html:coverage_re
 ```
 
+## Imports
+
+### Caching
+
+For caching some imports are only required, these have to be manually installed when needed
+- dask >= 2023.12.0 & dask-expr
+- pandas >= 1.3.0
+- polars
+- pyarrow >= 6.0.0 (Read parquet files)
+- annotated-types >= 0.6.0
+
 ## Documentation
 
 Documentation is generated using [Sphinx](https://www.sphinx-doc.org/en/master/).
 
 To make the documentation, run `make html` with `docs` as the working directory. The documentation can then be found in `docs/_build/html/index.html`.
 
 Here's a short command to make the documentation and open it in the browser:
```

### Comparing `epochalyst-0.1.7/epochalyst/_core/_caching/_cacher.py` & `epochalyst-0.2/epochalyst/_core/_caching/_cacher.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,73 @@
 import glob
+import os
 import pickle
-from epochalyst._core._logging._logger import _Logger
-from typing import Any
+from typing import Any, TypedDict, Literal
+
 import dask.array as da
 import dask.dataframe as dd
 import numpy as np
-import os
 import pandas as pd
+import polars as pl
 
+from epochalyst._core._logging._logger import _Logger
 
-class _Cacher(_Logger):
-    """The cacher is a flexible class that allows for caching of any data.
 
-    The cacher uses cache_args to determine if the data is already cached and if so, return the cached data.
-    cache_args is a dictionary that contains the arguments to determine if the data is already cached. Currently listed cache_args are
-    supported if more are required create a new issue on the github repository.
+class _CacheArgs(TypedDict):
+    """The cache arguments.
+
+    Currently listed cache_args are supported. If more are required, create a new GitHub issue.
 
-    cache_args supports the following keys:
+    The following keys are supported:
         - output_data_type: The type of the output data.
-            - "dask_array": The output data is a dask array.
-            - "numpy_array": The output data is a numpy array.
-            - "pandas_dataframe": The output data is a pandas dataframe.
-            - "dask_dataframe": The output data is a dask dataframe.
+            - "dask_array": The output data is a Dask array.
+            - "numpy_array": The output data is a NumPy array.
+            - "pandas_dataframe": The output data is a Pandas dataframe.
+            - "dask_dataframe": The output data is a Dask dataframe.
+            - "polars_dataframe": The output data is a Polars dataframe.
         - storage_type: The type of the storage.
-            - ".npy": The storage type is a numpy file.
-            - ".parquet": The storage type is a parquet file.
-            - ".csv": The storage type is a csv file.
-            - ".npy_stack": The storage type is a numpy stack.
+            - ".npy": The storage type is a NumPy file.
+            - ".parquet": The storage type is a Parquet file.
+            - ".csv": The storage type is a CSV file.
+            - ".npy_stack": The storage type is a NumPy stack.
             - ".pkl": The storage type is a pickle file
         - storage_path: The path to the storage.
 
-    ### Methods:
-    ```python
-    def _cache_exists(name: str, cache_args: dict[str, Any] = {}) -> bool: # Check if the cache exists
+    :param output_data_type: The type of the output data.
+    :param storage_type: The type of the storage.
+    :param storage_path: The path to the storage.
+    """
+
+    output_data_type: Literal[
+        "dask_array",
+        "numpy_array",
+        "pandas_dataframe",
+        "dask_dataframe",
+        "polars_dataframe",
+    ]
+    storage_type: Literal[".npy", ".parquet", ".csv", ".npy_stack", ".pkl"]
+    storage_path: str  # TODO(Jeffrey) Allow str | bytes | os.PathLike[str] | os.PathLike[bytes] instead of just str
+
+
+class _Cacher(_Logger):
+    """The cacher is a flexible class that allows for caching of any data.
+
+    The cacher uses cache_args to determine if the data is already cached and if so, return the cached data.
+    cache_args is a dictionary that contains the arguments to determine if the data is already cached.
+
+    Methods:
+    .. code-block:: python
+        def _cache_exists(name: str, cache_args: _CacheArgs | None = None) -> bool: # Check if the cache exists
 
-    def _get_cache(name: str, cache_args: dict[str, Any] = {}) -> Any: # Load the cache
+        def _get_cache(name: str, cache_args: _CacheArgs | None = None) -> Any: # Load the cache
 
-    def _store_cache(name: str, data: Any, cache_args: dict[str, Any] = {}) -> None: # Store data
-    ```
+        def _store_cache(name: str, data: Any, cache_args: _CacheArgs | None = None) -> None: # Store data
     """
 
-    def _cache_exists(self, name: str, cache_args: dict[str, Any] = {}) -> bool:
+    def _cache_exists(self, name: str, cache_args: _CacheArgs | None = None) -> bool:
         """Check if the cache exists.
 
         :param cache_args: The cache arguments.
         :return: True if the cache exists, False otherwise.
         """
         if not cache_args:
             return False
@@ -84,15 +107,15 @@
 
         self.log_to_debug(
             f"Cache exists is {path_exists} for type: {storage_type} and path: {storage_path}"
         )
 
         return path_exists
 
-    def _get_cache(self, name: str, cache_args: dict[str, Any] = {}) -> Any:
+    def _get_cache(self, name: str, cache_args: _CacheArgs | None = None) -> Any:
         """Load the cache.
 
         :param name: The name of the cache.
         :param cache_args: The cache arguments.
         :return: The cached data.
         """
 
@@ -140,34 +163,38 @@
                 return pd.read_parquet(storage_path + name + ".parquet")
             elif output_data_type == "dask_dataframe":
                 return dd.read_parquet(storage_path + name + ".parquet")
             elif output_data_type == "numpy_array":
                 return pd.read_parquet(storage_path + name + ".parquet").to_numpy()
             elif output_data_type == "dask_array":
                 return dd.read_parquet(storage_path + name + ".parquet").to_dask_array()
+            elif output_data_type == "polars_dataframe":
+                return pl.read_parquet(storage_path + name + ".parquet")
             else:
                 self.log_to_debug(
                     f"Invalid output data type: {output_data_type}, for loading .parquet file."
                 )
                 raise ValueError(
-                    "output_data_type must be pandas_dataframe, dask_dataframe, numpy_array or dask_array, other types not supported yet"
+                    "output_data_type must be pandas_dataframe, dask_dataframe, numpy_array, dask_array, or polars_dataframe, other types not supported yet"
                 )
         elif storage_type == ".csv":
             # Check if output_data_type is supported and load cache to output_data_type
             self.log_to_debug(f"Loading .csv file from {storage_path + name}")
             if output_data_type == "pandas_dataframe":
                 return pd.read_csv(storage_path + name + ".csv")
             elif output_data_type == "dask_dataframe":
                 return dd.read_csv(storage_path + name + "/*.part")
+            elif output_data_type == "polars_dataframe":
+                return pl.read_csv(storage_path + name + ".csv")
             else:
                 self.log_to_debug(
                     f"Invalid output data type: {output_data_type}, for loading .csv file."
                 )
                 raise ValueError(
-                    "output_data_type must be pandas_dataframe or dask_dataframe, other types not supported yet"
+                    "output_data_type must be pandas_dataframe, dask_dataframe, or polars_dataframe, other types not supported yet"
                 )
         elif storage_type == ".npy_stack":
             # Check if output_data_type is supported and load cache to output_data_type
             self.log_to_debug(f"Loading .npy_stack file from {storage_path + name}")
             if output_data_type == "dask_array":
                 return da.from_npy_stack(storage_path + name)
             else:
@@ -182,19 +209,19 @@
             self.log_to_debug(
                 f"Loading pickle file from {storage_path + name + '.pkl'}"
             )
             return pickle.load(open(storage_path + name + ".pkl", "rb"))
         else:
             self.log_to_debug(f"Invalid storage type: {storage_type}")
             raise ValueError(
-                "storage_type must be .npy, .parquet, .csv or .npy_stack, other types not supported yet"
+                "storage_type must be .npy, .parquet, .csv, or .npy_stack, other types not supported yet"
             )
 
     def _store_cache(
-        self, name: str, data: Any, cache_args: dict[str, Any] = {}
+        self, name: str, data: Any, cache_args: _CacheArgs | None = None
     ) -> None:
         """Store one set of data.
 
         :param name: The name of the cache.
         :param data: The data to store.
         :param cache_args: The cache arguments.
         """
@@ -247,34 +274,38 @@
                 pd.DataFrame(data).to_parquet(storage_path + name + ".parquet")
             elif output_data_type == "dask_array":
                 new_dd = dd.from_dask_array(data)
                 new_dd = new_dd.rename(
                     columns={col: str(col) for col in new_dd.columns}
                 )
                 new_dd.to_parquet(storage_path + name + ".parquet")
+            elif output_data_type == "polars_dataframe":
+                data.write_parquet(storage_path + name + ".parquet")
             else:
                 self.log_to_debug(
                     f"Invalid output data type: {output_data_type}, for storing .parquet file."
                 )
                 raise ValueError(
-                    "output_data_type must be pandas_dataframe, dask_dataframe, numpy_array or dask_array, other types not supported yet"
+                    "output_data_type must be pandas_dataframe, dask_dataframe, numpy_array, dask_array, or polars_dataframe, other types not supported yet"
                 )
         elif storage_type == ".csv":
             # Check if output_data_type is supported and store cache to output_data_type
             self.log_to_debug(f"Storing .csv file to {storage_path + name}")
             if output_data_type == "pandas_dataframe":
                 data.to_csv(storage_path + name + ".csv", index=False)
             elif output_data_type == "dask_dataframe":
                 data.to_csv(storage_path + name, index=False)
+            elif output_data_type == "polars_dataframe":
+                data.write_csv(storage_path + name + ".csv")
             else:
                 self.log_to_debug(
                     f"Invalid output data type: {output_data_type}, for storing .csv file."
                 )
                 raise ValueError(
-                    "output_data_type must be pandas_dataframe or dask_dataframe, other types not supported yet"
+                    "output_data_type must be pandas_dataframe, dask_dataframe, or polars_dataframe, other types not supported yet"
                 )
         elif storage_type == ".npy_stack":
             # Check if output_data_type is supported and store cache to output_data_type
             self.log_to_debug(f"Storing .npy_stack file to {storage_path + name}")
             if output_data_type == "dask_array":
                 da.to_npy_stack(storage_path + name, data)
             else:
```

### Comparing `epochalyst-0.1.7/epochalyst/_core/_logging/_logger.py` & `epochalyst-0.2/epochalyst/_core/_logging/_logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,33 +2,33 @@
 from typing import Any
 from epochalyst.logging.section_separator import print_section_separator
 
 
 class _Logger:
     """Logger abstract class for logging methods.
 
-    ### Methods:
-    ```python
-    @abstractmethod
-    def log_to_terminal(self, message: str) -> None: # Logs to terminal if implemented
+    Methods:
+    .. code-block:: python
+        @abstractmethod
+        def log_to_terminal(self, message: str) -> None: # Logs to terminal if implemented
 
-    @abstractmethod
-    def log_to_debug(self, message: str) -> None: # Logs to debugger if implemented
+        @abstractmethod
+        def log_to_debug(self, message: str) -> None: # Logs to debugger if implemented
 
-    @abstractmethod
-    def log_to_warning(self, message: str) -> None: # Logs to warning if implemented
+        @abstractmethod
+        def log_to_warning(self, message: str) -> None: # Logs to warning if implemented
 
-    @abstractmethod
-    def log_to_external(self, message: dict[str, Any], **kwargs: Any) -> None: # Logs to external site
+        @abstractmethod
+        def log_to_external(self, message: dict[str, Any], **kwargs: Any) -> None: # Logs to external site
 
-    @abstractmethod
-    def external_define_metric(self, metric: str, metric_type: str) -> None: # Defines an external metric
+        @abstractmethod
+        def external_define_metric(self, metric: str, metric_type: str) -> None: # Defines an external metric
 
-    @abstractmethod
-    def log_section_separator(self, message: str) -> None: # Logs a section separator
+        @abstractmethod
+        def log_section_separator(self, message: str) -> None: # Logs a section separator
     """
 
     @abstractmethod
     def log_to_terminal(self, message: str) -> None:
         """Log terminal method, if no logging override with empty.
 
         :param message: The message to log."""
```

### Comparing `epochalyst-0.1.7/epochalyst/logging/section_separator.py` & `epochalyst-0.2/epochalyst/logging/section_separator.py`

 * *Files identical despite different names*

### Comparing `epochalyst-0.1.7/epochalyst/pipeline/model/training/pretrain_block.py` & `epochalyst-0.2/epochalyst/pipeline/model/training/pretrain_block.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,48 +8,46 @@
 from epochalyst.pipeline.model.training.training_block import TrainingBlock
 
 
 @dataclass
 class PretrainBlock(TrainingBlock):
     """Pretrain block class
 
-    ### Parameters
+    Parameters:
     - test_size : float
 
-    ### Methods
-    ```python
-    @abstractmethod
-    def pretrain_train(self, x: Any, y: Any, train_indices: list[int], *, save_pretrain: bool = True, save_pretrain_with_split: bool = False) -> tuple[Any, Any]:
+    Methods:
+    .. code-block:: python
+        @abstractmethod
+        def pretrain_train(self, x: Any, y: Any, train_indices: list[int], *, save_pretrain: bool = True, save_pretrain_with_split: bool = False) -> tuple[Any, Any]:
 
-    @abstractmethod
-    def custom_predict(self, x: Any, **pred_args: Any) -> Any: # Predict pretrain block method.
+        @abstractmethod
+        def custom_predict(self, x: Any, **pred_args: Any) -> Any: # Predict pretrain block method.
 
-    def train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]: # Train pretrain block method.
+        def train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]: # Train pretrain block method.
 
-    def predict(self, x: Any, **pred_args: Any) -> Any: # Predict pretrain block method.
+        def predict(self, x: Any, **pred_args: Any) -> Any: # Predict pretrain block method.
 
-    def train_split_hash(self, train_indices: list[int]) -> str: # Split the hash on train split
-    ```
+        def train_split_hash(self, train_indices: list[int]) -> str: # Split the hash on train split
 
-    ### Usage:
-    ```python
-    from epochalyst.pipeline.model.training.pretrain_block import PretrainBlock
+    Usage:
+    .. code-block:: python
+        from epochalyst.pipeline.model.training.pretrain_block import PretrainBlock
 
-    class CustomPretrainBlock(PretrainBlock):
-        def pretrain_train(self, x: Any, y: Any, train_indices: list[int], *, save_pretrain: bool = True, save_pretrain_with_split: bool = False) -> tuple[Any, Any]:
-            return x, y
+        class CustomPretrainBlock(PretrainBlock):
+            def pretrain_train(self, x: Any, y: Any, train_indices: list[int], *, save_pretrain: bool = True, save_pretrain_with_split: bool = False) -> tuple[Any, Any]:
+                return x, y
 
-        def custom_predict(self, x: Any, **pred_args: Any) -> Any:
-            return x
+            def custom_predict(self, x: Any, **pred_args: Any) -> Any:
+                return x
 
-    custom_pretrain_block = CustomPretrainBlock()
+        custom_pretrain_block = CustomPretrainBlock()
 
-    x, y = custom_pretrain_block.train(x, y)
-    x = custom_pretrain_block.predict(x)
-    ```
+        x, y = custom_pretrain_block.train(x, y)
+        x = custom_pretrain_block.predict(x)
     """
 
     test_size: float = 0.2
 
     @abstractmethod
     def pretrain_train(
         self,
```

### Comparing `epochalyst-0.1.7/epochalyst/pipeline/model/training/torch_trainer.py` & `epochalyst-0.2/epochalyst/pipeline/model/training/torch_trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,102 +23,100 @@
 T_co = TypeVar("T_co", covariant=True)
 
 
 @dataclass
 class TorchTrainer(TrainingBlock):
     """Abstract class for torch trainers, override necessary functions for custom implementation.
 
-    ### Parameters:
+    Parameters:
     - `model` (nn.Module): The model to train.
     - `optimizer` (functools.partial[Optimizer]): Optimizer to use for training.
     - `criterion` (nn.Module): Criterion to use for training.
     - `scheduler` (Callable[[Optimizer], LRScheduler] | None): Scheduler to use for training.
     - `epochs` (int): Number of epochs
     - `batch_size` (int): Batch size
     - `patience` (int): Patience for early stopping
     - `test_size` (float): Relative size of the test set
 
-    ### Methods:
-    ```python
-    @abstractmethod
-    def log_to_terminal(self, message: str) -> None:
-        # Logs to terminal if implemented
+    Methods:
+    .. code-block:: python
+        @abstractmethod
+        def log_to_terminal(self, message: str) -> None:
+            # Logs to terminal if implemented
 
-    @abstractmethod
-    def log_to_debug(self, message: str) -> None:
-        # Logs to debugger if implemented
+        @abstractmethod
+        def log_to_debug(self, message: str) -> None:
+            # Logs to debugger if implemented
 
-    @abstractmethod
-    def log_to_warning(self, message: str) -> None:
-        # Logs to warning if implemented
+        @abstractmethod
+        def log_to_warning(self, message: str) -> None:
+            # Logs to warning if implemented
 
-    @abstractmethod
-    def log_to_external(self, message: dict[str, Any], **kwargs: Any) -> None:
-        # Logs to external site
+        @abstractmethod
+        def log_to_external(self, message: dict[str, Any], **kwargs: Any) -> None:
+            # Logs to external site
 
-    @abstractmethod
-    def external_define_metric(self, metric: str, metric_type: str) -> None:
-        # Defines an external metric
+        @abstractmethod
+        def external_define_metric(self, metric: str, metric_type: str) -> None:
+            # Defines an external metric
 
-    def train(self, x: Any, y: Any, cache_args: dict[str, Any] = {}, **train_args: Any) -> tuple[Any, Any]:
-        # Applies caching and calls custom_train, overridding removes caching
+        def train(self, x: Any, y: Any, cache_args: dict[str, Any] = {}, **train_args: Any) -> tuple[Any, Any]:
+            # Applies caching and calls custom_train, overridding removes caching
 
-    def predict(self, x: Any, cache_args: dict[str, Any] = {}, **pred_args: Any) -> Any:
-        # Applies caching and calls custom_predict, overridding removes caching
+        def predict(self, x: Any, cache_args: dict[str, Any] = {}, **pred_args: Any) -> Any:
+            # Applies caching and calls custom_predict, overridding removes caching
 
-    def custom_train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:
-        # Implements torch training. If you are going to override this method and not use any other functionality, inherit from TrainingBlock.
+        def custom_train(self, x: Any, y: Any, **train_args: Any) -> tuple[Any, Any]:
+            # Implements torch training. If you are going to override this method and not use any other functionality, inherit from TrainingBlock.
 
-    def custom_predict(self, x: Any, **pred_args: Any) -> Any:
-        # Implements torch prediction. If you are going to override this method and not use any other functionality, inherit from TrainingBlock.
+        def custom_predict(self, x: Any, **pred_args: Any) -> Any:
+            # Implements torch prediction. If you are going to override this method and not use any other functionality, inherit from TrainingBlock.
 
-    def predict_on_loader(loader: DataLoader[tuple[Tensor, ...]]) -> npt.NDArray[np.float32]:
-        # Predict using a dataloader.
+        def predict_on_loader(loader: DataLoader[tuple[Tensor, ...]]) -> npt.NDArray[np.float32]:
+            # Predict using a dataloader.
 
-    def create_datasets(x: npt.NDArray[np.float32], y: npt.NDArray[np.float32], train_indices: list[int], test_indices: list[int], cache_size: int = -1) -> tuple[Dataset[tuple[Tensor, ...]], Dataset[tuple[Tensor, ...]]]:
-        # Create the datasets for training and validation.
+        def create_datasets(x: npt.NDArray[np.float32], y: npt.NDArray[np.float32], train_indices: list[int], test_indices: list[int], cache_size: int = -1) -> tuple[Dataset[tuple[Tensor, ...]], Dataset[tuple[Tensor, ...]]]:
+            # Create the datasets for training and validation.
 
-    def create_prediction_dataset(x: npt.NDArray[np.float32]) -> Dataset[tuple[Tensor, ...]]:
-        # Create the prediction dataset.
+        def create_prediction_dataset(x: npt.NDArray[np.float32]) -> Dataset[tuple[Tensor, ...]]:
+            # Create the prediction dataset.
 
-    def create_dataloaders(train_dataset: Dataset[tuple[Tensor, ...]], test_dataset: Dataset[tuple[Tensor, ...]]) -> tuple[DataLoader[tuple[Tensor, ...]], DataLoader[tuple[Tensor, ...]]]:
-        # Create the dataloaders for training and validation.
+        def create_dataloaders(train_dataset: Dataset[tuple[Tensor, ...]], test_dataset: Dataset[tuple[Tensor, ...]]) -> tuple[DataLoader[tuple[Tensor, ...]], DataLoader[tuple[Tensor, ...]]]:
+            # Create the dataloaders for training and validation.
 
-    def update_model_directory(model_directory: str) -> None:
-        # Update the model directory for caching (default: tm).
-    ```
+        def update_model_directory(model_directory: str) -> None:
+            # Update the model directory for caching (default: tm).
 
-    ### Usage:
-    ```python
-    from epochalyst.pipeline.model.training.torch_trainer import TorchTrainer
-    from torch import nn
-    from torch.optim import Adam
-    from torch.optim.lr_scheduler import StepLR
-    from torch.nn import MSELoss
+    Usage:
+    .. code-block:: python
+        from epochalyst.pipeline.model.training.torch_trainer import TorchTrainer
+        from torch import nn
+        from torch.optim import Adam
+        from torch.optim.lr_scheduler import StepLR
+        from torch.nn import MSELoss
 
-    class MyTorchTrainer(TorchTrainer):
+        class MyTorchTrainer(TorchTrainer):
 
-        def log_to_terminal(self, message: str) -> None:
+            def log_to_terminal(self, message: str) -> None:
+
+            ....
 
-        ....
+        model = nn.Sequential(nn.Linear(1, 1))
+        optimizer = functools.partial(Adam, lr=0.01)
+        criterion = MSELoss()
+        scheduler = functools.partial(StepLR, step_size=1, gamma=0.1)
+        epochs = 10
+        batch_size = 32
+        patience = 5
+        test_size = 0.2
 
-    model = nn.Sequential(nn.Linear(1, 1))
-    optimizer = functools.partial(Adam, lr=0.01)
-    criterion = MSELoss()
-    scheduler = functools.partial(StepLR, step_size=1, gamma=0.1)
-    epochs = 10
-    batch_size = 32
-    patience = 5
-    test_size = 0.2
-
-    trainer = MyTorchTrainer(model=model, optimizer=optimizer, criterion=criterion, scheduler=scheduler, epochs=epochs, batch_size=batch_size, patience=patience, test_size=test_size)
-
-    x, y = trainer.train(x, y)
-    x = trainer.predict(x)
-    ```
+        trainer = MyTorchTrainer(model=model, optimizer=optimizer, criterion=criterion, scheduler=scheduler, epochs=epochs, batch_size=batch_size, patience=patience, test_size=test_size)
+
+        x, y = trainer.train(x, y)
+        x = trainer.predict(x)
     """
 
     model: nn.Module
     optimizer: functools.partial[Optimizer]
     criterion: nn.Module
     scheduler: Callable[[Optimizer], LRScheduler] | None = None
     epochs: Annotated[int, Gt(0)] = 10
@@ -256,18 +254,21 @@
         :return: The output of the system.
         """
         self._load_model()
 
         print_section_separator(f"Predicting model: {self.model.__class__.__name__}")
         self.log_to_debug(f"Predicting model: {self.model.__class__.__name__}")
 
+        # Parse pred_args
+        curr_batch_size = pred_args.get("batch_size", self.batch_size)
+
         # Create dataset
         pred_dataset = self.create_prediction_dataset(x)
         pred_dataloader = DataLoader(
-            pred_dataset, batch_size=self.batch_size, shuffle=False
+            pred_dataset, batch_size=curr_batch_size, shuffle=False
         )
 
         # Predict
         return self.predict_on_loader(pred_dataloader)
 
     def predict_on_loader(
         self, loader: DataLoader[tuple[Tensor, ...]]
@@ -589,20 +590,22 @@
 
         return TrainTestDataset(
             train_dataset, test_dataset, train_indices, test_indices
         )
 
 
 class TrainTestDataset(Dataset[T_co]):
-    r"""Dataset as a concatenation of multiple datasets.
+    """Dataset as a concatenation of multiple datasets.
 
     This class is useful to assemble different existing datasets.
 
-    Args:
-        datasets (sequence): List of datasets to be concatenated
+    :param train_dataset: The train dataset
+    :param test_dataset: The test dataset
+    :param train_indices: The train indices
+    :param test_indices: The test indices
     """
 
     train_dataset: Dataset[T_co]
     test_dataset: Dataset[T_co]
     train_indices: List[int]
     test_indices: List[int]
```

### Comparing `epochalyst-0.1.7/epochalyst/pipeline/model/training/training_block.py` & `epochalyst-0.2/epochalyst/pipeline/model/training/training_block.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,66 +1,65 @@
 from agogos.training import Trainer
 from typing import Any
 from epochalyst._core._logging._logger import _Logger
 from abc import abstractmethod
-from epochalyst._core._caching._cacher import _Cacher
+from epochalyst._core._caching._cacher import _Cacher, _CacheArgs
 
 
 class TrainingBlock(Trainer, _Cacher, _Logger):
     """The training block is a flexible block that allows for training of any model.
 
-    ### Methods:
-    ```python
-    @abstractmethod
-    def custom_train(self, x: Any, y: Any, **train_args) -> tuple[Any, Any]: # Custom training implementation
+    Methods:
+    .. code-block:: python
+        @abstractmethod
+        def custom_train(self, x: Any, y: Any, **train_args) -> tuple[Any, Any]: # Custom training implementation
 
-    @abstractmethod
-    def custom_predict(self, x: Any, y: Any, **pred_args) -> tuple[Any, Any]: # Custom prediction implementation
+        @abstractmethod
+        def custom_predict(self, x: Any, y: Any, **pred_args) -> tuple[Any, Any]: # Custom prediction implementation
 
-    @abstractmethod
-    def log_to_terminal(self, message: str) -> None: # Logs to terminal if implemented
+        @abstractmethod
+        def log_to_terminal(self, message: str) -> None: # Logs to terminal if implemented
 
-    @abstractmethod
-    def log_to_debug(self, message: str) -> None: # Logs to debugger if implemented
+        @abstractmethod
+        def log_to_debug(self, message: str) -> None: # Logs to debugger if implemented
 
-    @abstractmethod
-    def log_to_warning(self, message: str) -> None: # Logs to warning if implemented
+        @abstractmethod
+        def log_to_warning(self, message: str) -> None: # Logs to warning if implemented
 
-    @abstractmethod
-    def log_to_external(self, message: dict[str, Any], **kwargs: Any) -> None: # Logs to external site
+        @abstractmethod
+        def log_to_external(self, message: dict[str, Any], **kwargs: Any) -> None: # Logs to external site
 
-    @abstractmethod
-    def external_define_metric(self, metric: str, metric_type: str) -> None: # Defines an external metric
+        @abstractmethod
+        def external_define_metric(self, metric: str, metric_type: str) -> None: # Defines an external metric
 
-    def train(self, x: Any, y: Any, cache_args: dict[str, Any] = {}, **train_args: Any) -> tuple[Any, Any]: # Applies caching and calls custom_train
+        def train(self, x: Any, y: Any, cache_args: dict[str, Any] = {}, **train_args: Any) -> tuple[Any, Any]: # Applies caching and calls custom_train
 
-    def predict(self, x: Any, cache_args: dict[str, Any] = {}, **pred_args: Any) -> Any: # Applies caching and calls custom_predict
+        def predict(self, x: Any, cache_args: dict[str, Any] = {}, **pred_args: Any) -> Any: # Applies caching and calls custom_predict
 
-    ### Usage:
-    ```python
-    from epochalyst.pipeline.model.training.training_block import TrainingBlock
+    Usage:
+    .. code-block:: python
+        from epochalyst.pipeline.model.training.training_block import TrainingBlock
 
-    class CustomTrainingBlock(TrainingBlock):
-        def custom_train(self, x: Any, y: Any) -> tuple[Any, Any]:
-            return x, y
+        class CustomTrainingBlock(TrainingBlock):
+            def custom_train(self, x: Any, y: Any) -> tuple[Any, Any]:
+                return x, y
 
-        def custom_predict(self, x: Any) -> Any:
-            return x
+            def custom_predict(self, x: Any) -> Any:
+                return x
 
-        ....
+            ....
 
-    custom_training_block = CustomTrainingBlock()
+        custom_training_block = CustomTrainingBlock()
 
-    x, y = custom_training_block.train(x, y)
-    x = custom_training_block.predict(x)
-    ```
+        x, y = custom_training_block.train(x, y)
+        x = custom_training_block.predict(x)
     """
 
     def train(
-        self, x: Any, y: Any, cache_args: dict[str, Any] = {}, **train_args: Any
+        self, x: Any, y: Any, cache_args: _CacheArgs | None = None, **train_args: Any
     ) -> tuple[Any, Any]:
         """Train the model.
 
         :param x: The input data.
         :param y: The target data.
         :param cache_args: The cache arguments.
         :return: The predicted data and the labels
@@ -96,15 +95,17 @@
         :param y: The target data.
         :return: The predicted data and the labels
         """
         raise NotImplementedError(
             f"Custom transform method not implemented for {self.__class__}"
         )
 
-    def predict(self, x: Any, cache_args: dict[str, Any] = {}, **pred_args: Any) -> Any:
+    def predict(
+        self, x: Any, cache_args: _CacheArgs | None = None, **pred_args: Any
+    ) -> Any:
         """Predict using the model.
 
         :param x: The input data.
         :param cache_args: The cache arguments.
         :return: The predicted data.
         """
         if cache_args and self._cache_exists(
```

### Comparing `epochalyst-0.1.7/epochalyst.egg-info/PKG-INFO` & `epochalyst-0.2/epochalyst.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: epochalyst
-Version: 0.1.7
+Version: 0.2
 Summary: This package contains the code for team Epoch's pipeline
 Author-email: Jasper van Selm <jmvanselm@gmail.com>, Ariel Ebersberger <arielebersberger@gmail.com>, Tolga Kopar <cahittolgakopar@gmail.com>, Jeffrey Lim <jeffrey-lim@outlook.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.22.4
-Requires-Dist: dask>=2023.12.0
-Requires-Dist: pandas>=1.3.0
-Requires-Dist: pyarrow>=6.0.0
 Requires-Dist: torch>=2.1.0
-Requires-Dist: agogos>=0.2.1
+Requires-Dist: agogos==0.3.4
 
 ![image](./docs/_static/images/logo/Epochalyst_Logo_Dark.png#gh-light-mode-only)
 ![image](./docs/_static/images/logo/Epochalyst_Logo_Light.png#gh-dark-mode-only)
 
 [![PyPI Latest Release](https://img.shields.io/pypi/v/epochalyst.svg)](https://pypi.org/project/epochalyst/)
 [![PyPI Downloads](https://img.shields.io/pypi/dm/epochalyst.svg?label=PyPI%20downloads)](https://pypi.org/project/epochalyst/)
 
@@ -43,17 +40,28 @@
 ```
 
 ## Pytest coverage report
 
 To generate pytest coverage report run
 
 ```python
-python -m pytest --cov=epochalyst --cov-report=html:coverage_re
+python -m pytest --cov=epochalyst --cov-branch --cov-report=html:coverage_re
 ```
 
+## Imports
+
+### Caching
+
+For caching some imports are only required, these have to be manually installed when needed
+- dask >= 2023.12.0 & dask-expr
+- pandas >= 1.3.0
+- polars
+- pyarrow >= 6.0.0 (Read parquet files)
+- annotated-types >= 0.6.0
+
 ## Documentation
 
 Documentation is generated using [Sphinx](https://www.sphinx-doc.org/en/master/).
 
 To make the documentation, run `make html` with `docs` as the working directory. The documentation can then be found in `docs/_build/html/index.html`.
 
 Here's a short command to make the documentation and open it in the browser:
```

### Comparing `epochalyst-0.1.7/epochalyst.egg-info/SOURCES.txt` & `epochalyst-0.2/epochalyst.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 epochalyst/_core/_logging/__init__.py
 epochalyst/_core/_logging/_logger.py
 epochalyst/_core/_pipeline/__init__.py
 epochalyst/_core/_pipeline/_custom_data_parallel.py
 epochalyst/logging/__init__.py
 epochalyst/logging/section_separator.py
 epochalyst/pipeline/__init__.py
+epochalyst/pipeline/ensemble.py
 epochalyst/pipeline/model/__init__.py
 epochalyst/pipeline/model/model.py
 epochalyst/pipeline/model/training/__init__.py
 epochalyst/pipeline/model/training/pretrain_block.py
 epochalyst/pipeline/model/training/torch_trainer.py
 epochalyst/pipeline/model/training/training.py
 epochalyst/pipeline/model/training/training_block.py
```

### Comparing `epochalyst-0.1.7/pyproject.toml` & `epochalyst-0.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "epochalyst"
-version = "0.1.7"
+version = "0.2"
 authors = [
     { name = "Jasper van Selm", email = "jmvanselm@gmail.com" },
     { name = "Ariel Ebersberger", email = "arielebersberger@gmail.com" },
     { name = "Tolga Kopar", email = "cahittolgakopar@gmail.com" },
     { name = "Jeffrey Lim", email = "jeffrey-lim@outlook.com" },
 ]
 description = "This package contains the code for team Epoch's pipeline"
@@ -16,21 +16,22 @@
     "Operating System :: OS Independent",
 ]
 dependencies= [
     # Machine Learning Libraries
     "numpy>=1.22.4",
 
     # Parallel Processing Libraries
-    "dask>=2023.12.0",
+    # "dask>=2023.12.0",
 
     # Data Processing Libraries
-    "pandas>=1.3.0",
+    # "pandas>=1.3.0",
+    # "polars",
 
     # Parquet
-    "pyarrow>=6.0.0",
+    # "pyarrow>=6.0.0",
 
     # PyTorch
     "torch>=2.1.0",
 
     # Agogos
-    "agogos>=0.2.1",
+    "agogos==0.3.4",
 ]
```

