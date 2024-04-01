# Comparing `tmp/xibabel-0.0.1a1.tar.gz` & `tmp/xibabel-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xibabel-0.0.1a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xibabel-0.0.1a2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xibabel-0.0.1a1.tar` & `xibabel-0.0.1a2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2951 2024-04-01 22:53:59.280176 xibabel-0.0.1a1/README.md
--rw-r--r--   0        0        0     1176 2024-04-01 23:00:24.571221 xibabel-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0      104 2024-04-01 22:57:23.006276 xibabel-0.0.1a1/src/xibabel/__init__.py
--rw-r--r--   0        0        0      571 2024-04-01 20:13:24.938488 xibabel-0.0.1a1/src/xibabel/bench/bench_nib_xib_load.py
--rw-r--r--   0        0        0    18610 2024-04-01 22:51:03.504803 xibabel-0.0.1a1/src/xibabel/loaders.py
--rw-r--r--   0        0        0       20 2024-04-01 20:13:24.938858 xibabel-0.0.1a1/src/xibabel/testing/.gitignore
--rw-r--r--   0        0        0      921 2024-04-01 20:13:24.939016 xibabel-0.0.1a1/src/xibabel/testing/__init__.py
--rw-r--r--   0        0        0      627 2024-04-01 20:13:24.939155 xibabel-0.0.1a1/src/xibabel/testing/__main__.py
--rw-r--r--   0        0        0     5075 2024-04-01 20:13:24.939378 xibabel-0.0.1a1/src/xibabel/testing/fetcher.py
--rw-r--r--   0        0        0      463 2024-04-01 20:13:24.939585 xibabel-0.0.1a1/src/xibabel/testing/test_files.yml
--rw-r--r--   0        0        0      396 2024-04-01 20:13:24.939726 xibabel-0.0.1a1/src/xibabel/testing/test_sets.yml
--rw-r--r--   0        0        0        0 2024-04-01 20:13:24.939864 xibabel-0.0.1a1/src/xibabel/tests/__init__.py
--rw-r--r--   0        0        0     2512 2024-04-01 20:13:24.940151 xibabel-0.0.1a1/src/xibabel/tests/conftest.py
--rw-r--r--   0        0        0     1306 2024-04-01 20:13:24.940358 xibabel-0.0.1a1/src/xibabel/tests/run_server.py
--rw-r--r--   0        0        0    14228 2024-04-01 22:51:03.505743 xibabel-0.0.1a1/src/xibabel/tests/test_loaders.py
--rw-r--r--   0        0        0     1205 2024-04-01 20:13:24.940719 xibabel-0.0.1a1/src/xibabel/tests/test_merge.py
--rw-r--r--   0        0        0     2792 2024-04-01 20:13:24.940931 xibabel-0.0.1a1/src/xibabel/tests/test_scripting.py
--rw-r--r--   0        0        0      794 2024-04-01 20:13:24.941154 xibabel-0.0.1a1/src/xibabel/xutils.py
--rw-r--r--   0        0        0     4500 1970-01-01 00:00:00.000000 xibabel-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     2939 2024-04-01 23:04:39.559789 xibabel-0.0.1a2/README.md
+-rw-r--r--   0        0        0     1176 2024-04-01 23:00:24.571221 xibabel-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0      104 2024-04-01 23:05:58.039253 xibabel-0.0.1a2/src/xibabel/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-01 20:13:24.938488 xibabel-0.0.1a2/src/xibabel/bench/bench_nib_xib_load.py
+-rw-r--r--   0        0        0    18610 2024-04-01 22:51:03.504803 xibabel-0.0.1a2/src/xibabel/loaders.py
+-rw-r--r--   0        0        0       20 2024-04-01 20:13:24.938858 xibabel-0.0.1a2/src/xibabel/testing/.gitignore
+-rw-r--r--   0        0        0      921 2024-04-01 20:13:24.939016 xibabel-0.0.1a2/src/xibabel/testing/__init__.py
+-rw-r--r--   0        0        0      627 2024-04-01 20:13:24.939155 xibabel-0.0.1a2/src/xibabel/testing/__main__.py
+-rw-r--r--   0        0        0     5075 2024-04-01 20:13:24.939378 xibabel-0.0.1a2/src/xibabel/testing/fetcher.py
+-rw-r--r--   0        0        0      463 2024-04-01 20:13:24.939585 xibabel-0.0.1a2/src/xibabel/testing/test_files.yml
+-rw-r--r--   0        0        0      396 2024-04-01 20:13:24.939726 xibabel-0.0.1a2/src/xibabel/testing/test_sets.yml
+-rw-r--r--   0        0        0        0 2024-04-01 20:13:24.939864 xibabel-0.0.1a2/src/xibabel/tests/__init__.py
+-rw-r--r--   0        0        0     2512 2024-04-01 20:13:24.940151 xibabel-0.0.1a2/src/xibabel/tests/conftest.py
+-rw-r--r--   0        0        0     1306 2024-04-01 20:13:24.940358 xibabel-0.0.1a2/src/xibabel/tests/run_server.py
+-rw-r--r--   0        0        0    14228 2024-04-01 22:51:03.505743 xibabel-0.0.1a2/src/xibabel/tests/test_loaders.py
+-rw-r--r--   0        0        0     1205 2024-04-01 20:13:24.940719 xibabel-0.0.1a2/src/xibabel/tests/test_merge.py
+-rw-r--r--   0        0        0     2792 2024-04-01 20:13:24.940931 xibabel-0.0.1a2/src/xibabel/tests/test_scripting.py
+-rw-r--r--   0        0        0      794 2024-04-01 20:13:24.941154 xibabel-0.0.1a2/src/xibabel/xutils.py
+-rw-r--r--   0        0        0     4488 1970-01-01 00:00:00.000000 xibabel-0.0.1a2/PKG-INFO
```

### Comparing `xibabel-0.0.1a1/README.md` & `xibabel-0.0.1a2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 It builds on the standard Nibabel package, but adds the extensions listed below.
 
 The extensions allow code like this:
 
 ## Quickstart
 
-Here is a basic read and slice operation with Xibabel.  Compare to the more manual labor that you would have to do with Nibabel.
+Here is a basic read and slice operation with Xibabel. Compare to the more manual labor that you would have to do with Nibabel.
 
 ```python
 # Basic read and slice with Xibabel
 import xibabel as xib
 
 import matplotlib.pyplot as plt
 plt.rc('image', cmap='gray')
@@ -29,41 +29,41 @@
 plt.imshow(mean_img.sel(k=32))
 ```
 
 See the example notebooks in the `experiments` directory for more.
 
 ## Features
 
-* Xibabel images are [Xarrays](https://docs.xarray.dev).  They have labeled
+- Xibabel images are [Xarrays](https://docs.xarray.dev). They have labeled
   axes, with default labels for spatial axes of `i`, `j` and `k`; time is
-  `time`.  The labels allow slicing operations such as selecting slices over
+  `time`. The labels allow slicing operations such as selecting slices over
   time.
-* The labels allow concise and readable operations on named axes.  See the
+- The labels allow concise and readable operations on named axes. See the
   `glm_in_xibabel` notebook in the `experiments` directory.
-* Xarrays have attributes that can be attached to the image or the axes of the
-  image.  We can load these attributes from
-  [BIDS](https://bids.neuroimaging.io/) format JSON files.  This allows better
+- Xarrays have attributes that can be attached to the image or the axes of the
+  image. We can load these attributes from
+  [BIDS](https://bids.neuroimaging.io/) format JSON files. This allows better
   transmission of metadata.
-* The Xarrays have a Dask backend, to computations can be deferred and run at
+- The Xarrays have a Dask backend, to computations can be deferred and run at
   the point at which you need the data in memory.
-* Xarrays and Dask allow new storage formats, including storage in
+- Xarrays and Dask allow new storage formats, including storage in
   [Zarr](https://zarr.readthedocs.io) and
   HDF5 / [netCDF](https://en.wikipedia.org/wiki/NetCDF).
-* You can optimize the on-disk format for memory and CPU by adjusting
-  *chunking*.  We are working on performance metrics for different processing
+- You can optimize the on-disk format for memory and CPU by adjusting
+  _chunking_. We are working on performance metrics for different processing
   steps.
-* Xibabel uses [fsspec](https://filesystem-spec.readthedocs.io) for reading
+- Xibabel uses [fsspec](https://filesystem-spec.readthedocs.io) for reading
   NIfTI and other files, allowing you to use many filesystems as the source for
-  your data, including HTTP, Amazon, Google Cloud and others.  See the FSSpec
+  your data, including HTTP, Amazon, Google Cloud and others. See the FSSpec
   documentation for details, and the code above for an example using HTTP as
   a backing store.
 
 ## Status
 
-Xibabel is in development mode at the moment.  We are still experimenting with the API.  We'd love to hear from you if you are interested to help.   Please do not rely on any particular features in this alpha version, including compatibility of file formats; prefer
+Xibabel is in development mode at the moment. We are still experimenting with the API. We'd love to hear from you if you are interested to help. Please do not rely on any particular features in this alpha version, including compatibility of file formats; prefer
 
 ## Install
 
 From Pip — the current pre-release:
 
 ```bash
 pip install --pre xarray
```

### Comparing `xibabel-0.0.1a1/pyproject.toml` & `xibabel-0.0.1a2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a1/src/xibabel/bench/bench_nib_xib_load.py` & `xibabel-0.0.1a2/src/xibabel/bench/bench_nib_xib_load.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a1/src/xibabel/loaders.py` & `xibabel-0.0.1a2/src/xibabel/loaders.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a1/src/xibabel/testing/__init__.py` & `xibabel-0.0.1a2/src/xibabel/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a1/src/xibabel/testing/__main__.py` & `xibabel-0.0.1a2/src/xibabel/testing/__main__.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a1/src/xibabel/testing/fetcher.py` & `xibabel-0.0.1a2/src/xibabel/testing/fetcher.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a1/src/xibabel/tests/conftest.py` & `xibabel-0.0.1a2/src/xibabel/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a1/src/xibabel/tests/run_server.py` & `xibabel-0.0.1a2/src/xibabel/tests/run_server.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a1/src/xibabel/tests/test_loaders.py` & `xibabel-0.0.1a2/src/xibabel/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a1/src/xibabel/tests/test_merge.py` & `xibabel-0.0.1a2/src/xibabel/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a1/src/xibabel/tests/test_scripting.py` & `xibabel-0.0.1a2/src/xibabel/tests/test_scripting.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a1/src/xibabel/xutils.py` & `xibabel-0.0.1a2/src/xibabel/xutils.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a1/PKG-INFO` & `xibabel-0.0.1a2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xibabel
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Init for Xibabel package
 Author-email: Matthew Brett <matthew.brett@gmail.com>, Paul Ivanov <pi@berkeley.edu>, "Christopher J. Markiewicz" <markiewicz@stanford.edu>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Dist: xarray
@@ -44,15 +44,15 @@
 
 It builds on the standard Nibabel package, but adds the extensions listed below.
 
 The extensions allow code like this:
 
 ## Quickstart
 
-Here is a basic read and slice operation with Xibabel.  Compare to the more manual labor that you would have to do with Nibabel.
+Here is a basic read and slice operation with Xibabel. Compare to the more manual labor that you would have to do with Nibabel.
 
 ```python
 # Basic read and slice with Xibabel
 import xibabel as xib
 
 import matplotlib.pyplot as plt
 plt.rc('image', cmap='gray')
@@ -69,41 +69,41 @@
 plt.imshow(mean_img.sel(k=32))
 ```
 
 See the example notebooks in the `experiments` directory for more.
 
 ## Features
 
-* Xibabel images are [Xarrays](https://docs.xarray.dev).  They have labeled
+- Xibabel images are [Xarrays](https://docs.xarray.dev). They have labeled
   axes, with default labels for spatial axes of `i`, `j` and `k`; time is
-  `time`.  The labels allow slicing operations such as selecting slices over
+  `time`. The labels allow slicing operations such as selecting slices over
   time.
-* The labels allow concise and readable operations on named axes.  See the
+- The labels allow concise and readable operations on named axes. See the
   `glm_in_xibabel` notebook in the `experiments` directory.
-* Xarrays have attributes that can be attached to the image or the axes of the
-  image.  We can load these attributes from
-  [BIDS](https://bids.neuroimaging.io/) format JSON files.  This allows better
+- Xarrays have attributes that can be attached to the image or the axes of the
+  image. We can load these attributes from
+  [BIDS](https://bids.neuroimaging.io/) format JSON files. This allows better
   transmission of metadata.
-* The Xarrays have a Dask backend, to computations can be deferred and run at
+- The Xarrays have a Dask backend, to computations can be deferred and run at
   the point at which you need the data in memory.
-* Xarrays and Dask allow new storage formats, including storage in
+- Xarrays and Dask allow new storage formats, including storage in
   [Zarr](https://zarr.readthedocs.io) and
   HDF5 / [netCDF](https://en.wikipedia.org/wiki/NetCDF).
-* You can optimize the on-disk format for memory and CPU by adjusting
-  *chunking*.  We are working on performance metrics for different processing
+- You can optimize the on-disk format for memory and CPU by adjusting
+  _chunking_. We are working on performance metrics for different processing
   steps.
-* Xibabel uses [fsspec](https://filesystem-spec.readthedocs.io) for reading
+- Xibabel uses [fsspec](https://filesystem-spec.readthedocs.io) for reading
   NIfTI and other files, allowing you to use many filesystems as the source for
-  your data, including HTTP, Amazon, Google Cloud and others.  See the FSSpec
+  your data, including HTTP, Amazon, Google Cloud and others. See the FSSpec
   documentation for details, and the code above for an example using HTTP as
   a backing store.
 
 ## Status
 
-Xibabel is in development mode at the moment.  We are still experimenting with the API.  We'd love to hear from you if you are interested to help.   Please do not rely on any particular features in this alpha version, including compatibility of file formats; prefer
+Xibabel is in development mode at the moment. We are still experimenting with the API. We'd love to hear from you if you are interested to help. Please do not rely on any particular features in this alpha version, including compatibility of file formats; prefer
 
 ## Install
 
 From Pip — the current pre-release:
 
 ```bash
 pip install --pre xarray
```

