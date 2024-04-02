# Comparing `tmp/gcs-torch-dataflux-0.1.0.tar.gz` & `tmp/gcs-torch-dataflux-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcs-torch-dataflux-0.1.0.tar", last modified: Fri Mar 15 00:24:48 2024, max compression
+gzip compressed data, was "gcs-torch-dataflux-1.0.0.tar", last modified: Tue Apr  2 21:38:54 2024, max compression
```

## Comparing `gcs-torch-dataflux-0.1.0.tar` & `gcs-torch-dataflux-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-x---   0 bernardhan (1020501) primarygroup (89939)        0 2024-03-15 00:24:48.744047 gcs-torch-dataflux-0.1.0/
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)    11357 2024-02-13 19:40:08.000000 gcs-torch-dataflux-0.1.0/LICENSE
--rw-r--r--   0 bernardhan (1020501) primarygroup (89939)    10880 2024-03-15 00:24:48.744047 gcs-torch-dataflux-0.1.0/PKG-INFO
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)     9776 2024-03-15 00:23:05.000000 gcs-torch-dataflux-0.1.0/README.md
-drwxr-x---   0 bernardhan (1020501) primarygroup (89939)        0 2024-03-15 00:24:48.736047 gcs-torch-dataflux-0.1.0/dataflux_client_python/
-drwxr-x---   0 bernardhan (1020501) primarygroup (89939)        0 2024-03-15 00:24:48.740047 gcs-torch-dataflux-0.1.0/dataflux_client_python/dataflux_core/
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)      606 2024-02-13 19:40:08.000000 gcs-torch-dataflux-0.1.0/dataflux_client_python/dataflux_core/__init__.py
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)    19861 2024-03-14 20:37:10.000000 gcs-torch-dataflux-0.1.0/dataflux_client_python/dataflux_core/download.py
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)    23107 2024-03-07 22:03:08.000000 gcs-torch-dataflux-0.1.0/dataflux_client_python/dataflux_core/fast_list.py
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)     8825 2024-02-13 19:40:08.000000 gcs-torch-dataflux-0.1.0/dataflux_client_python/dataflux_core/range_splitter.py
-drwxr-x---   0 bernardhan (1020501) primarygroup (89939)        0 2024-03-15 00:24:48.740047 gcs-torch-dataflux-0.1.0/dataflux_pytorch/
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)      613 2024-02-13 19:40:08.000000 gcs-torch-dataflux-0.1.0/dataflux_pytorch/__init__.py
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)     2400 2024-03-07 22:03:08.000000 gcs-torch-dataflux-0.1.0/dataflux_pytorch/dataflux_checkpoint.py
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)     6969 2024-03-14 20:37:10.000000 gcs-torch-dataflux-0.1.0/dataflux_pytorch/dataflux_iterable_dataset.py
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)     6250 2024-03-14 20:37:10.000000 gcs-torch-dataflux-0.1.0/dataflux_pytorch/dataflux_mapstyle_dataset.py
-drwxr-x---   0 bernardhan (1020501) primarygroup (89939)        0 2024-03-15 00:24:48.744047 gcs-torch-dataflux-0.1.0/gcs_torch_dataflux.egg-info/
--rw-r--r--   0 bernardhan (1020501) primarygroup (89939)    10880 2024-03-15 00:24:48.000000 gcs-torch-dataflux-0.1.0/gcs_torch_dataflux.egg-info/PKG-INFO
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)      614 2024-03-15 00:24:48.000000 gcs-torch-dataflux-0.1.0/gcs_torch_dataflux.egg-info/SOURCES.txt
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)        1 2024-03-15 00:24:48.000000 gcs-torch-dataflux-0.1.0/gcs_torch_dataflux.egg-info/dependency_links.txt
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)       63 2024-03-15 00:24:48.000000 gcs-torch-dataflux-0.1.0/gcs_torch_dataflux.egg-info/requires.txt
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)       31 2024-03-15 00:24:48.000000 gcs-torch-dataflux-0.1.0/gcs_torch_dataflux.egg-info/top_level.txt
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)     1101 2024-03-15 00:23:39.000000 gcs-torch-dataflux-0.1.0/pyproject.toml
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)       38 2024-03-15 00:24:48.744047 gcs-torch-dataflux-0.1.0/setup.cfg
--rw-r-----   0 bernardhan (1020501) primarygroup (89939)      332 2024-02-13 19:40:08.000000 gcs-torch-dataflux-0.1.0/setup.py
+drwxr-x---   0 bernardhan (1020501) primarygroup (89939)        0 2024-04-02 21:38:54.798883 gcs-torch-dataflux-1.0.0/
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)    11357 2024-02-13 19:40:08.000000 gcs-torch-dataflux-1.0.0/LICENSE
+-rw-r--r--   0 bernardhan (1020501) primarygroup (89939)    14317 2024-04-02 21:38:54.798883 gcs-torch-dataflux-1.0.0/PKG-INFO
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)    13200 2024-04-02 20:58:59.000000 gcs-torch-dataflux-1.0.0/README.md
+drwxr-x---   0 bernardhan (1020501) primarygroup (89939)        0 2024-04-02 21:38:54.794882 gcs-torch-dataflux-1.0.0/dataflux_client_python/
+drwxr-x---   0 bernardhan (1020501) primarygroup (89939)        0 2024-04-02 21:38:54.794882 gcs-torch-dataflux-1.0.0/dataflux_client_python/dataflux_core/
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)      606 2024-02-13 19:40:08.000000 gcs-torch-dataflux-1.0.0/dataflux_client_python/dataflux_core/__init__.py
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)    19911 2024-04-02 21:36:46.000000 gcs-torch-dataflux-1.0.0/dataflux_client_python/dataflux_core/download.py
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)    23957 2024-04-02 21:36:46.000000 gcs-torch-dataflux-1.0.0/dataflux_client_python/dataflux_core/fast_list.py
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)     8825 2024-02-13 19:40:08.000000 gcs-torch-dataflux-1.0.0/dataflux_client_python/dataflux_core/range_splitter.py
+drwxr-x---   0 bernardhan (1020501) primarygroup (89939)        0 2024-04-02 21:38:54.798883 gcs-torch-dataflux-1.0.0/dataflux_pytorch/
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)      613 2024-02-13 19:40:08.000000 gcs-torch-dataflux-1.0.0/dataflux_pytorch/__init__.py
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)     2400 2024-03-07 22:03:08.000000 gcs-torch-dataflux-1.0.0/dataflux_pytorch/dataflux_checkpoint.py
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)     6969 2024-04-01 17:57:59.000000 gcs-torch-dataflux-1.0.0/dataflux_pytorch/dataflux_iterable_dataset.py
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)     6250 2024-03-27 20:08:16.000000 gcs-torch-dataflux-1.0.0/dataflux_pytorch/dataflux_mapstyle_dataset.py
+drwxr-x---   0 bernardhan (1020501) primarygroup (89939)        0 2024-04-02 21:38:54.798883 gcs-torch-dataflux-1.0.0/gcs_torch_dataflux.egg-info/
+-rw-r--r--   0 bernardhan (1020501) primarygroup (89939)    14317 2024-04-02 21:38:54.000000 gcs-torch-dataflux-1.0.0/gcs_torch_dataflux.egg-info/PKG-INFO
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)      614 2024-04-02 21:38:54.000000 gcs-torch-dataflux-1.0.0/gcs_torch_dataflux.egg-info/SOURCES.txt
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)        1 2024-04-02 21:38:54.000000 gcs-torch-dataflux-1.0.0/gcs_torch_dataflux.egg-info/dependency_links.txt
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)       63 2024-04-02 21:38:54.000000 gcs-torch-dataflux-1.0.0/gcs_torch_dataflux.egg-info/requires.txt
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)       31 2024-04-02 21:38:54.000000 gcs-torch-dataflux-1.0.0/gcs_torch_dataflux.egg-info/top_level.txt
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)     1114 2024-04-02 21:36:45.000000 gcs-torch-dataflux-1.0.0/pyproject.toml
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)       38 2024-04-02 21:38:54.798883 gcs-torch-dataflux-1.0.0/setup.cfg
+-rw-r-----   0 bernardhan (1020501) primarygroup (89939)      332 2024-02-13 19:40:08.000000 gcs-torch-dataflux-1.0.0/setup.py
```

### Comparing `gcs-torch-dataflux-0.1.0/LICENSE` & `gcs-torch-dataflux-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcs-torch-dataflux-0.1.0/PKG-INFO` & `gcs-torch-dataflux-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gcs-torch-dataflux
-Version: 0.1.0
+Version: 1.0.0
 Summary: A GCS data loading integration for PyTorch
 Maintainer-email: Google Dataflux Dev Team <dataflux-customer-support@google.com>
 Project-URL: Homepage, https://github.com/GoogleCloudPlatform/dataflux-pytorch
 Project-URL: Issues, https://github.com/GoogleCloudPlatform/dataflux-pytorch/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,15 +25,15 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # Dataflux Dataset for PyTorch with Google Cloud Storage
 
 The Dataflux Dataset for PyTorch lets you connect directly to a GCS bucket as a PyTorch dataset, without pre-loading the data to local disk, and with optimizations to make training up to **3X faster** when the dataset consists of many small files (e.g., 100 - 500 KB).
 
-The Dataflux Dataset for PyTorch implements PyTorch’s [dataset primitive](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html) that can be used to efficiently load training data from GCS. The library currently supports [map-style datasets](https://pytorch.org/docs/stable/data.html#map-style-datasets) for random data access patterns.
+The Dataflux Dataset for PyTorch implements PyTorch’s [dataset primitive](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html) that can be used to efficiently load training data from GCS. The library currently supports [map-style datasets](https://pytorch.org/docs/stable/data.html#map-style-datasets) for random data access patterns and [iterable-style datasets](https://pytorch.org/docs/stable/data.html#iterable-style-datasets) for streaming data access patterns.
 
 Furthermore, the Dataflux Dataset for PyTorch provides a checkpointing interface to conveniently save and load checkpoints directly to and from a Google Cloud Storage (GCS) bucket.
 
 Note that the Dataflux Dataset for PyTorch library is in an early preview stage and the team is consistently working on improvements and support for new features.
 
 ## Getting started
 
@@ -57,38 +57,54 @@
 ### Examples
 Please checkout the `demo` directory for a complete set of examples, which includes a [simple starter Jupyter Notebook (hosted by Google Colab)](demo/simple-walkthrough/Getting%20Started%20with%20Dataflux%20Dataset%20for%20PyTorch%20with%20Google%20Cloud%20Storage.ipynb) and an [end-to-end image segmentation training workload walkthrough](demo/image-segmentation/README.md). Those examples will help you understand how the Dataflux Dataset for PyTorch works and how you can integrate it into your own workload. 
 
 #### Sample Examples
 Before getting started, please make sure you have installed the library and configured authentication following the instructions above.
 
 ##### Data Loading
-Dataflux Dataset for PyTorch can be constructed by specifying the project name, bucket name and an optional prefix.
+Both Dataflux map-style and iterable-style datasets for PyTorch can be constructed by specifying the project name, bucket name and an optional prefix.
 ```python
 from dataflux_pytorch import dataflux_mapstyle_dataset
 
 # Please update these fields.
 PROJECT_NAME = "<PROJECT_NAME>"
 BUCKET_NAME = "<BUCKET_NAME>"
 PREFIX = "<PREFIX>"
 
-dataset = dataflux_mapstyle_dataset.DataFluxMapStyleDataset(
+# Map-style dataset.
+map_dataset = dataflux_mapstyle_dataset.DataFluxMapStyleDataset(
   project_name=PROJECT_NAME,
   bucket_name=BUCKET_NAME,
   config=dataflux_mapstyle_dataset.Config(prefix=PREFIX),
 )
 
 # Random access to an object.
-sample_object = dataset.objects[0]
+sample_object = map_dataset.objects[0]
 
 # Learn about the name and the size (in bytes) of the object.
 name = sample_object[0]
 size = sample_object[1]
 
 # Iterate over the datasets.
-for each_object in dataset:
+for each_object in map_dataset:
+  # Raw bytes of the object.
+  print(each_object)
+```
+Similarly, for `DataFluxIterableDataset`:
+```python
+from dataflux_pytorch import dataflux_iterable_dataset
+
+# Iterable-style dataset.
+iterable_dataset = dataflux_iterable_dataset.DataFluxIterableDataset(
+  project_name=PROJECT_ID,
+  bucket_name=BUCKET_NAME,
+  config=dataflux_iterable_dataset.Config(prefix=PREFIX),
+)
+
+for each_object in iterable_dataset:
   # Raw bytes of the object.
   print(each_object)
 ```
 
 Dataflux Dataset for PyTorch offers the flexibility to transform the downloaded raw bytes of data into any format of choice. This is particularly useful since the `PyTorch DataLoader` works well with Numpy arrays or PyTorch tensors.
 
 ```python
@@ -96,21 +112,34 @@
 # to load them into Numpy arrays for training.
 import io
 import numpy
 from PIL import Image
 
 transform = lambda img_in_bytes : numpy.asarray(Image.open(io.BytesIO(img_in_bytes)))
 
-dataset = dataflux_mapstyle_dataset.DataFluxMapStyleDataset(
+map_dataset = dataflux_mapstyle_dataset.DataFluxMapStyleDataset(
   project_name=PROJECT_NAME,
   bucket_name=BUCKET_NAME,
   config=dataflux_mapstyle_dataset.Config(prefix=PREFIX),
   data_format_fn=transform,
 )
 
+for each_object in map_dataset:
+  # each_object is now a Numpy array.
+  print(each_object)
+```
+
+Similarly, for `DataFluxIterableDataset`:
+```python
+iterable_dataset = dataflux_iterable_dataset.DataFluxIterableDataset(
+  project_name=PROJECT_ID,
+  bucket_name=BUCKET_NAME,
+  config=dataflux_mapstyle_dataset.Config(prefix=PREFIX),
+  data_format_fn=transform,
+)
 for each_object in dataset:
   # each_object is now a Numpy array.
   print(each_object)
 ```
 
 ##### Checkpointing
 
@@ -135,15 +164,87 @@
 with ckpt.reader(CKPT_PATH) as reader:
   read_state_dict = torch.load(reader)
 
 model.load_state_dict(read_state_dict)
 ```
 
 ## Performance
-We tested Dataflux's early performance using [DLIO benchmark](https://github.com/argonne-lcf/dlio_benchmark) simulations with standard mean file-sizes and dataset sizes. A total of 5 training epochs were simulated. For small files (100KB, 500KB), Dataflux can be **2-3x** faster than using GCS native APIs.
+
+### Dataflux Map-style Dataset
+We tested Dataflux Map-style Dataset's early performance using [DLIO benchmark](https://github.com/argonne-lcf/dlio_benchmark) simulations with standard mean file-sizes and dataset sizes. A total of 5 training epochs were simulated. For small files (100KB, 500KB), Dataflux can be **2-3x** faster than using GCS native APIs.
+
+<table>
+  <tr>
+   <td style="background-color: #d9d2e9"><strong>File size / count</strong>
+   </td>
+   <td style="background-color: #d9d2e9"><strong>Tool</strong>
+   </td>
+   <td style="background-color: #d9d2e9"><strong>Training time (s)</strong>
+   </td>
+  </tr>
+  <tr>
+   <td rowspan="2" style="background-color: #d9d9d9"><em>100 KiB / 500000 files</em>
+   </td>
+   <td style="background-color: #d9d9d9">Direct GCS API calls
+   </td>
+   <td style="background-color: #d9d9d9">1,299
+   </td>
+  </tr>
+  <tr>
+   <td style="background-color: #d9d9d9"><strong>Dataflux Map-style Dataset</strong>
+   </td>
+   <td style="background-color: #d9d9d9"><strong>515</strong>
+   </td>
+  </tr>
+  <tr>
+   <td rowspan="2" style="background-color: #f3f3f3"><em>500 KiB / 2.2m files</em>
+   </td>
+   <td style="background-color: #f3f3f3">Direct GCS API calls
+   </td>
+   <td style="background-color: #f3f3f3">6,499
+   </td>
+  </tr>
+  <tr>
+   <td style="background-color: #f3f3f3"><strong>Dataflux Map-style Dataset</strong>
+   </td>
+   <td style="background-color: #f3f3f3"><strong>2,058</strong>
+   </td>
+  </tr>
+  <tr>
+   <td rowspan="2" style="background-color: #d9d9d9"><em>3 MiB / 50000 files</em>
+   </td>
+   <td style="background-color: #d9d9d9">Direct GCS API calls
+   </td>
+   <td style="background-color: #d9d9d9">399
+   </td>
+  </tr>
+  <tr>
+   <td style="background-color: #d9d9d9"><strong>Dataflux Map-style Dataset</strong>
+   </td>
+   <td style="background-color: #d9d9d9"><strong>277</strong>
+   </td>
+  </tr>
+  <tr>
+   <td rowspan="2" style="background-color: #f3f3f3"><em>150 MiB / 5000 files</em>
+   </td>
+   <td style="background-color: #f3f3f3">Direct GCS API calls
+   </td>
+   <td style="background-color: #f3f3f3">1,396
+   </td>
+  </tr>
+  <tr>
+   <td style="background-color: #f3f3f3"><strong>Dataflux Map-style Dataset</strong>
+   </td>
+   <td style="background-color: #f3f3f3"><strong>1,173</strong>
+   </td>
+  </tr>
+</table>
+
+### Dataflux Iterable-style Dataset
+Since the [DLIO benchmark](https://github.com/argonne-lcf/dlio_benchmark) doesn’t easily support an implementation of a PyTorch iterable dataset, we implemented a [simple training loop](demo/simple_iterable_dataset.py) that has similar IO behaviors as the DLIO benchmark and used that loop to benchmark the Dataflux Iterable Datasets.
 
 <table>
   <tr>
    <td style="background-color: #d9d2e9"><strong>File size / count</strong>
    </td>
    <td style="background-color: #d9d2e9"><strong>Tool</strong>
    </td>
@@ -151,63 +252,63 @@
    </td>
   </tr>
   <tr>
    <td rowspan="2" style="background-color: #d9d9d9"><em>100 KiB / 500000 files</em>
    </td>
    <td style="background-color: #d9d9d9">Direct GCS API calls
    </td>
-   <td style="background-color: #d9d9d9">2,459
+   <td style="background-color: #d9d9d9">1,145
    </td>
   </tr>
   <tr>
-   <td style="background-color: #d9d9d9"><strong>Dataflux</strong>
+   <td style="background-color: #d9d9d9"><strong>Dataflux Iterable-style Dataset</strong>
    </td>
-   <td style="background-color: #d9d9d9"><strong>757</strong>
+   <td style="background-color: #d9d9d9"><strong>611</strong>
    </td>
   </tr>
   <tr>
    <td rowspan="2" style="background-color: #f3f3f3"><em>500 KiB / 2.2m files</em>
    </td>
    <td style="background-color: #f3f3f3">Direct GCS API calls
    </td>
-   <td style="background-color: #f3f3f3">7,472
+   <td style="background-color: #f3f3f3">5,174
    </td>
   </tr>
   <tr>
-   <td style="background-color: #f3f3f3"><strong>Dataflux</strong>
+   <td style="background-color: #f3f3f3"><strong>Dataflux Iterable-style Dataset</strong>
    </td>
-   <td style="background-color: #f3f3f3"><strong>2,696</strong>
+   <td style="background-color: #f3f3f3"><strong>2,503</strong>
    </td>
   </tr>
   <tr>
    <td rowspan="2" style="background-color: #d9d9d9"><em>3 MiB / 50000 files</em>
    </td>
    <td style="background-color: #d9d9d9">Direct GCS API calls
    </td>
-   <td style="background-color: #d9d9d9">463
+   <td style="background-color: #d9d9d9">413
    </td>
   </tr>
   <tr>
-   <td style="background-color: #d9d9d9"><strong>Dataflux</strong>
+   <td style="background-color: #d9d9d9"><strong>Dataflux Iterable-style Dataset</strong>
    </td>
-   <td style="background-color: #d9d9d9"><strong>318</strong>
+   <td style="background-color: #d9d9d9"><strong>384</strong>
    </td>
   </tr>
   <tr>
    <td rowspan="2" style="background-color: #f3f3f3"><em>150 MiB / 5000 files</em>
    </td>
    <td style="background-color: #f3f3f3">Direct GCS API calls
    </td>
-   <td style="background-color: #f3f3f3">1,228
+   <td style="background-color: #f3f3f3">1,225
    </td>
   </tr>
   <tr>
-   <td style="background-color: #f3f3f3"><strong>Dataflux</strong>
+   <td style="background-color: #f3f3f3"><strong>Dataflux Iterable-style Dataset</strong>
    </td>
-   <td style="background-color: #f3f3f3"><strong>1,288</strong>
+   <td style="background-color: #f3f3f3"><strong>1,143</strong>
    </td>
   </tr>
 </table>
 
 *Note: Within each experiment, all training parameters such as batch size and parallelism are consistent. The team is working on publishing a detailed analysis soon.*
 
 ## Limitations
```

### Comparing `gcs-torch-dataflux-0.1.0/dataflux_client_python/dataflux_core/__init__.py` & `gcs-torch-dataflux-1.0.0/dataflux_client_python/dataflux_core/__init__.py`

 * *Files identical despite different names*

### Comparing `gcs-torch-dataflux-0.1.0/dataflux_client_python/dataflux_core/download.py` & `gcs-torch-dataflux-1.0.0/dataflux_client_python/dataflux_core/download.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,35 +228,36 @@
     """
     chunk_size = math.ceil(len(objects) / threads)
     chunks = []
     for i in range(threads):
         chunk = objects[i * chunk_size : (i + 1) * chunk_size]
         if chunk:
             chunks.append(chunk)
-    results_queue = queue.Queue()
+    results_queues = [queue.Queue() for _ in chunks]
     thread_list = []
-    for chunk in chunks:
+    for i, chunk in enumerate(chunks):
         thread = threading.Thread(
             target=df_download_thread,
             args=(
-                results_queue,
+                results_queues[i],
                 project_name,
                 bucket_name,
                 chunk,
                 storage_client,
                 dataflux_download_optimization_params,
             ),
         )
         thread_list.append(thread)
         thread.start()
     for thread in thread_list:
         thread.join()
     results = []
-    while not results_queue.empty():
-        results.extend(results_queue.get())
+    for q in results_queues:
+        while not q.empty():
+            results.extend(q.get())
     return results
 
 
 def dataflux_download_parallel(
     project_name: str,
     bucket_name: str,
     objects: list[tuple[str, int]],
```

### Comparing `gcs-torch-dataflux-0.1.0/dataflux_client_python/dataflux_core/fast_list.py` & `gcs-torch-dataflux-1.0.0/dataflux_client_python/dataflux_core/fast_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,30 @@
 
 from google.cloud import storage
 from google.api_core.client_info import ClientInfo
 
 DEFAULT_ALLOWED_CLASS = ["STANDARD"]
 
 
+def remove_prefix(text: str, prefix: str):
+    """Helper function that removes prefix from a string.
+
+    Args:
+        text: String of text to trim a prefix from.
+        prefix: String of text that will be trimmed from text.
+
+    Returns:
+        Text value with the specified prefix removed.
+    """
+    # Note that as of python 3.9 removeprefix is built into string.
+    if text.startswith(prefix):
+        return text[len(prefix) :]
+    return text
+
+
 class ListWorker(object):
     """Worker that lists a range of objects from a GCS bucket.
 
     Attributes:
         name: String name of the worker.
         gcs_project: The string name of the google cloud storage project to list from.
         bucket: The string name of the storage bucket to list from.from . import fast_list, download
@@ -71,15 +87,15 @@
         results_queue: "multiprocessing.Queue[set[tuple[str, int]]]",
         metadata_queue: "multiprocessing.Queue[tuple[str, int]]",
         start_range: str,
         end_range: str,
         client: storage.Client = None,
         skip_compose: bool = True,
         list_directory_objects: bool = False,
-        prefix: str = None,
+        prefix: str = "",
         allowed_storage_classes: list[str] = DEFAULT_ALLOWED_CLASS,
         max_retries: int = 5,
     ):
         self.name = name
         self.gcs_project = gcs_project
         self.bucket = bucket
         self.send_work_stealing_needed_queue = send_work_stealing_needed_queue
@@ -94,15 +110,15 @@
         self.results: set[tuple[str, int]] = set()
         self.client = client
         self.max_results = 5000
         self.splitter = None
         self.default_alph = "a"
         self.skip_compose = skip_compose
         self.list_directory_objects = list_directory_objects
-        self.prefix = prefix
+        self.prefix = prefix if prefix else ""
         self.allowed_storage_classes = allowed_storage_classes
         self.api_call_count = 0
         self.max_retries = max_retries
 
     def wait_for_work(self) -> bool:
         """Indefinitely waits for available work and consumes it once available.
 
@@ -159,16 +175,18 @@
                 return
         retries_remaining = self.max_retries
         while True:
             has_results = False
             try:
                 list_blob_args = {
                     "max_results": self.max_results,
-                    "start_offset": self.start_range,
-                    "end_offset": self.end_range,
+                    "start_offset": self.prefix + self.start_range,
+                    "end_offset": (
+                        "" if not self.end_range else self.prefix + self.end_range
+                    ),
                 }
                 if self.prefix:
                     list_blob_args["prefix"] = self.prefix
                 blobs = self.client.bucket(self.bucket).list_blobs(**list_blob_args)
                 self.api_call_count += 1
                 retries_remaining = self.max_retries
                 i = 0
@@ -180,15 +198,18 @@
                             not self.skip_compose
                             or not blob.name.startswith(COMPOSED_PREFIX)
                         )
                         and (self.list_directory_objects or blob.name[-1] != "/")
                         and blob.storage_class in self.allowed_storage_classes
                     ):
                         self.results.add((blob.name, blob.size))
-                    self.start_range = blob.name
+                    # Remove the prefix from the name so that range calculations remain prefix-agnostic.
+                    # This is necessary due to the unbounded end-range when splitting string namespaces
+                    # of unknown size.
+                    self.start_range = remove_prefix(blob.name, self.prefix)
                     if i == self.max_results:
                         # Only allow work stealing when paging.
                         has_results = True
                         break
             except Exception as e:
                 retries_remaining -= 1
                 logging.error(
@@ -233,15 +254,15 @@
     unidle_queue: "multiprocessing.Queue[str]",
     results_queue: "multiprocessing.Queue[set[tuple[str, int]]]",
     metadata_queue: "multiprocessing.Queue[tuple[str, int]]",
     start_range: str,
     end_range: str,
     client: storage.Client = None,
     skip_compose: bool = True,
-    prefix: str = None,
+    prefix: str = "",
     allowed_storage_classes: list[str] = DEFAULT_ALLOWED_CLASS,
 ) -> None:
     """Helper function to execute a ListWorker.
 
     Args:
       name: String name of the list worker.
       gcs_project: String name of the google cloud project in use.
@@ -249,15 +270,15 @@
       send_work_stealing_needed_queue: Multiprocessing queue pushed to when a worker needs more work.
       heartbeat_queue: Multiprocessing queue pushed to while a worker is running nominally.
       direct_work_available_queue: Multiprocessing queue to push availble work stealing ranges to.
       idle_queue: Multiprocessing queue pushed to when worker is waiting for new work to steal.
       unidle_queue: Multiprocessing queue pushed to when the worker has successfully stolen work.
       results_queue: Multiprocessing queue on which the worker pushes its listing results onto.
       metadata_queue: Multiprocessing queue on which the worker pushes tracking metadata.
-      start_range: Stirng start range worker will begin listing from.
+      start_range: String start range worker will begin listing from.
       end_range: String end range worker will list until.
       client: The GCS storage client. When not provided, will be derived from background auth.
       skip_compose: When true, skip listing files with the composed object prefix.
       prefix: When provided, only list objects under this prefix.
       allowed_storage_classes: The set of GCS Storage Class types fast list will include.
     """
     ListWorker(
@@ -299,15 +320,15 @@
     def __init__(
         self,
         max_parallelism: int,
         project: str,
         bucket: str,
         sort_results: bool = False,
         skip_compose: bool = True,
-        prefix: str = None,
+        prefix: str = "",
         allowed_storage_classes: list[str] = DEFAULT_ALLOWED_CLASS,
     ):
         # The maximum number of threads utilized in the fast list operation.
         self.max_parallelism = max_parallelism
         self.gcs_project = project
         self.bucket = bucket
         self.inited = set()
```

### Comparing `gcs-torch-dataflux-0.1.0/dataflux_client_python/dataflux_core/range_splitter.py` & `gcs-torch-dataflux-1.0.0/dataflux_client_python/dataflux_core/range_splitter.py`

 * *Files identical despite different names*

### Comparing `gcs-torch-dataflux-0.1.0/dataflux_pytorch/__init__.py` & `gcs-torch-dataflux-1.0.0/dataflux_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `gcs-torch-dataflux-0.1.0/dataflux_pytorch/dataflux_checkpoint.py` & `gcs-torch-dataflux-1.0.0/dataflux_pytorch/dataflux_checkpoint.py`

 * *Files identical despite different names*

### Comparing `gcs-torch-dataflux-0.1.0/dataflux_pytorch/dataflux_iterable_dataset.py` & `gcs-torch-dataflux-1.0.0/dataflux_pytorch/dataflux_iterable_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,43 +107,43 @@
 
         self.objects = self._list_GCS_blobs_with_retry()
 
     def __iter__(self):
         worker_info = data.get_worker_info()
         if worker_info is None:
             # Single-process data loading.
-            yield from [
+            yield from (
                 self.data_format_fn(bytes_content)
                 for bytes_content in dataflux_core.download.dataflux_download_lazy(
                     project_name=self.project_name,
                     bucket_name=self.bucket_name,
                     objects=self.objects,
                     storage_client=self.storage_client,
                     dataflux_download_optimization_params=self.dataflux_download_optimization_params,
                 )
-            ]
+            )
         else:
             # Multi-process data loading. Split the workload among workers.
             # Ref: https://pytorch.org/docs/stable/data.html#torch.utils.data.IterableDataset.
             per_worker = int(
                 math.ceil(len(self.objects) / float(worker_info.num_workers))
             )
             worker_id = worker_info.id
             start = worker_id * per_worker
             end = min(start + per_worker, len(self.objects))
-            yield from [
+            yield from (
                 self.data_format_fn(bytes_content)
                 for bytes_content in dataflux_core.download.dataflux_download_lazy(
                     project_name=self.project_name,
                     bucket_name=self.bucket_name,
                     objects=self.objects[start:end],
                     storage_client=self.storage_client,
                     dataflux_download_optimization_params=self.dataflux_download_optimization_params,
                 )
-            ]
+            )
 
     def _list_GCS_blobs_with_retry(self):
         """Retries Dataflux Listing upon exceptions, up to the retries defined in self.config."""
         error = None
         listed_objects = []
         for _ in range(self.config.max_listing_retries):
             try:
```

### Comparing `gcs-torch-dataflux-0.1.0/dataflux_pytorch/dataflux_mapstyle_dataset.py` & `gcs-torch-dataflux-1.0.0/dataflux_pytorch/dataflux_mapstyle_dataset.py`

 * *Files identical despite different names*

### Comparing `gcs-torch-dataflux-0.1.0/gcs_torch_dataflux.egg-info/PKG-INFO` & `gcs-torch-dataflux-1.0.0/gcs_torch_dataflux.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: gcs-torch-dataflux
-Version: 0.1.0
+Version: 1.0.0
 Summary: A GCS data loading integration for PyTorch
 Maintainer-email: Google Dataflux Dev Team <dataflux-customer-support@google.com>
 Project-URL: Homepage, https://github.com/GoogleCloudPlatform/dataflux-pytorch
 Project-URL: Issues, https://github.com/GoogleCloudPlatform/dataflux-pytorch/issues
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: Apache Software License
@@ -25,15 +25,15 @@
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 
 # Dataflux Dataset for PyTorch with Google Cloud Storage
 
 The Dataflux Dataset for PyTorch lets you connect directly to a GCS bucket as a PyTorch dataset, without pre-loading the data to local disk, and with optimizations to make training up to **3X faster** when the dataset consists of many small files (e.g., 100 - 500 KB).
 
-The Dataflux Dataset for PyTorch implements PyTorch’s [dataset primitive](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html) that can be used to efficiently load training data from GCS. The library currently supports [map-style datasets](https://pytorch.org/docs/stable/data.html#map-style-datasets) for random data access patterns.
+The Dataflux Dataset for PyTorch implements PyTorch’s [dataset primitive](https://pytorch.org/tutorials/beginner/basics/data_tutorial.html) that can be used to efficiently load training data from GCS. The library currently supports [map-style datasets](https://pytorch.org/docs/stable/data.html#map-style-datasets) for random data access patterns and [iterable-style datasets](https://pytorch.org/docs/stable/data.html#iterable-style-datasets) for streaming data access patterns.
 
 Furthermore, the Dataflux Dataset for PyTorch provides a checkpointing interface to conveniently save and load checkpoints directly to and from a Google Cloud Storage (GCS) bucket.
 
 Note that the Dataflux Dataset for PyTorch library is in an early preview stage and the team is consistently working on improvements and support for new features.
 
 ## Getting started
 
@@ -57,38 +57,54 @@
 ### Examples
 Please checkout the `demo` directory for a complete set of examples, which includes a [simple starter Jupyter Notebook (hosted by Google Colab)](demo/simple-walkthrough/Getting%20Started%20with%20Dataflux%20Dataset%20for%20PyTorch%20with%20Google%20Cloud%20Storage.ipynb) and an [end-to-end image segmentation training workload walkthrough](demo/image-segmentation/README.md). Those examples will help you understand how the Dataflux Dataset for PyTorch works and how you can integrate it into your own workload. 
 
 #### Sample Examples
 Before getting started, please make sure you have installed the library and configured authentication following the instructions above.
 
 ##### Data Loading
-Dataflux Dataset for PyTorch can be constructed by specifying the project name, bucket name and an optional prefix.
+Both Dataflux map-style and iterable-style datasets for PyTorch can be constructed by specifying the project name, bucket name and an optional prefix.
 ```python
 from dataflux_pytorch import dataflux_mapstyle_dataset
 
 # Please update these fields.
 PROJECT_NAME = "<PROJECT_NAME>"
 BUCKET_NAME = "<BUCKET_NAME>"
 PREFIX = "<PREFIX>"
 
-dataset = dataflux_mapstyle_dataset.DataFluxMapStyleDataset(
+# Map-style dataset.
+map_dataset = dataflux_mapstyle_dataset.DataFluxMapStyleDataset(
   project_name=PROJECT_NAME,
   bucket_name=BUCKET_NAME,
   config=dataflux_mapstyle_dataset.Config(prefix=PREFIX),
 )
 
 # Random access to an object.
-sample_object = dataset.objects[0]
+sample_object = map_dataset.objects[0]
 
 # Learn about the name and the size (in bytes) of the object.
 name = sample_object[0]
 size = sample_object[1]
 
 # Iterate over the datasets.
-for each_object in dataset:
+for each_object in map_dataset:
+  # Raw bytes of the object.
+  print(each_object)
+```
+Similarly, for `DataFluxIterableDataset`:
+```python
+from dataflux_pytorch import dataflux_iterable_dataset
+
+# Iterable-style dataset.
+iterable_dataset = dataflux_iterable_dataset.DataFluxIterableDataset(
+  project_name=PROJECT_ID,
+  bucket_name=BUCKET_NAME,
+  config=dataflux_iterable_dataset.Config(prefix=PREFIX),
+)
+
+for each_object in iterable_dataset:
   # Raw bytes of the object.
   print(each_object)
 ```
 
 Dataflux Dataset for PyTorch offers the flexibility to transform the downloaded raw bytes of data into any format of choice. This is particularly useful since the `PyTorch DataLoader` works well with Numpy arrays or PyTorch tensors.
 
 ```python
@@ -96,21 +112,34 @@
 # to load them into Numpy arrays for training.
 import io
 import numpy
 from PIL import Image
 
 transform = lambda img_in_bytes : numpy.asarray(Image.open(io.BytesIO(img_in_bytes)))
 
-dataset = dataflux_mapstyle_dataset.DataFluxMapStyleDataset(
+map_dataset = dataflux_mapstyle_dataset.DataFluxMapStyleDataset(
   project_name=PROJECT_NAME,
   bucket_name=BUCKET_NAME,
   config=dataflux_mapstyle_dataset.Config(prefix=PREFIX),
   data_format_fn=transform,
 )
 
+for each_object in map_dataset:
+  # each_object is now a Numpy array.
+  print(each_object)
+```
+
+Similarly, for `DataFluxIterableDataset`:
+```python
+iterable_dataset = dataflux_iterable_dataset.DataFluxIterableDataset(
+  project_name=PROJECT_ID,
+  bucket_name=BUCKET_NAME,
+  config=dataflux_mapstyle_dataset.Config(prefix=PREFIX),
+  data_format_fn=transform,
+)
 for each_object in dataset:
   # each_object is now a Numpy array.
   print(each_object)
 ```
 
 ##### Checkpointing
 
@@ -135,15 +164,87 @@
 with ckpt.reader(CKPT_PATH) as reader:
   read_state_dict = torch.load(reader)
 
 model.load_state_dict(read_state_dict)
 ```
 
 ## Performance
-We tested Dataflux's early performance using [DLIO benchmark](https://github.com/argonne-lcf/dlio_benchmark) simulations with standard mean file-sizes and dataset sizes. A total of 5 training epochs were simulated. For small files (100KB, 500KB), Dataflux can be **2-3x** faster than using GCS native APIs.
+
+### Dataflux Map-style Dataset
+We tested Dataflux Map-style Dataset's early performance using [DLIO benchmark](https://github.com/argonne-lcf/dlio_benchmark) simulations with standard mean file-sizes and dataset sizes. A total of 5 training epochs were simulated. For small files (100KB, 500KB), Dataflux can be **2-3x** faster than using GCS native APIs.
+
+<table>
+  <tr>
+   <td style="background-color: #d9d2e9"><strong>File size / count</strong>
+   </td>
+   <td style="background-color: #d9d2e9"><strong>Tool</strong>
+   </td>
+   <td style="background-color: #d9d2e9"><strong>Training time (s)</strong>
+   </td>
+  </tr>
+  <tr>
+   <td rowspan="2" style="background-color: #d9d9d9"><em>100 KiB / 500000 files</em>
+   </td>
+   <td style="background-color: #d9d9d9">Direct GCS API calls
+   </td>
+   <td style="background-color: #d9d9d9">1,299
+   </td>
+  </tr>
+  <tr>
+   <td style="background-color: #d9d9d9"><strong>Dataflux Map-style Dataset</strong>
+   </td>
+   <td style="background-color: #d9d9d9"><strong>515</strong>
+   </td>
+  </tr>
+  <tr>
+   <td rowspan="2" style="background-color: #f3f3f3"><em>500 KiB / 2.2m files</em>
+   </td>
+   <td style="background-color: #f3f3f3">Direct GCS API calls
+   </td>
+   <td style="background-color: #f3f3f3">6,499
+   </td>
+  </tr>
+  <tr>
+   <td style="background-color: #f3f3f3"><strong>Dataflux Map-style Dataset</strong>
+   </td>
+   <td style="background-color: #f3f3f3"><strong>2,058</strong>
+   </td>
+  </tr>
+  <tr>
+   <td rowspan="2" style="background-color: #d9d9d9"><em>3 MiB / 50000 files</em>
+   </td>
+   <td style="background-color: #d9d9d9">Direct GCS API calls
+   </td>
+   <td style="background-color: #d9d9d9">399
+   </td>
+  </tr>
+  <tr>
+   <td style="background-color: #d9d9d9"><strong>Dataflux Map-style Dataset</strong>
+   </td>
+   <td style="background-color: #d9d9d9"><strong>277</strong>
+   </td>
+  </tr>
+  <tr>
+   <td rowspan="2" style="background-color: #f3f3f3"><em>150 MiB / 5000 files</em>
+   </td>
+   <td style="background-color: #f3f3f3">Direct GCS API calls
+   </td>
+   <td style="background-color: #f3f3f3">1,396
+   </td>
+  </tr>
+  <tr>
+   <td style="background-color: #f3f3f3"><strong>Dataflux Map-style Dataset</strong>
+   </td>
+   <td style="background-color: #f3f3f3"><strong>1,173</strong>
+   </td>
+  </tr>
+</table>
+
+### Dataflux Iterable-style Dataset
+Since the [DLIO benchmark](https://github.com/argonne-lcf/dlio_benchmark) doesn’t easily support an implementation of a PyTorch iterable dataset, we implemented a [simple training loop](demo/simple_iterable_dataset.py) that has similar IO behaviors as the DLIO benchmark and used that loop to benchmark the Dataflux Iterable Datasets.
 
 <table>
   <tr>
    <td style="background-color: #d9d2e9"><strong>File size / count</strong>
    </td>
    <td style="background-color: #d9d2e9"><strong>Tool</strong>
    </td>
@@ -151,63 +252,63 @@
    </td>
   </tr>
   <tr>
    <td rowspan="2" style="background-color: #d9d9d9"><em>100 KiB / 500000 files</em>
    </td>
    <td style="background-color: #d9d9d9">Direct GCS API calls
    </td>
-   <td style="background-color: #d9d9d9">2,459
+   <td style="background-color: #d9d9d9">1,145
    </td>
   </tr>
   <tr>
-   <td style="background-color: #d9d9d9"><strong>Dataflux</strong>
+   <td style="background-color: #d9d9d9"><strong>Dataflux Iterable-style Dataset</strong>
    </td>
-   <td style="background-color: #d9d9d9"><strong>757</strong>
+   <td style="background-color: #d9d9d9"><strong>611</strong>
    </td>
   </tr>
   <tr>
    <td rowspan="2" style="background-color: #f3f3f3"><em>500 KiB / 2.2m files</em>
    </td>
    <td style="background-color: #f3f3f3">Direct GCS API calls
    </td>
-   <td style="background-color: #f3f3f3">7,472
+   <td style="background-color: #f3f3f3">5,174
    </td>
   </tr>
   <tr>
-   <td style="background-color: #f3f3f3"><strong>Dataflux</strong>
+   <td style="background-color: #f3f3f3"><strong>Dataflux Iterable-style Dataset</strong>
    </td>
-   <td style="background-color: #f3f3f3"><strong>2,696</strong>
+   <td style="background-color: #f3f3f3"><strong>2,503</strong>
    </td>
   </tr>
   <tr>
    <td rowspan="2" style="background-color: #d9d9d9"><em>3 MiB / 50000 files</em>
    </td>
    <td style="background-color: #d9d9d9">Direct GCS API calls
    </td>
-   <td style="background-color: #d9d9d9">463
+   <td style="background-color: #d9d9d9">413
    </td>
   </tr>
   <tr>
-   <td style="background-color: #d9d9d9"><strong>Dataflux</strong>
+   <td style="background-color: #d9d9d9"><strong>Dataflux Iterable-style Dataset</strong>
    </td>
-   <td style="background-color: #d9d9d9"><strong>318</strong>
+   <td style="background-color: #d9d9d9"><strong>384</strong>
    </td>
   </tr>
   <tr>
    <td rowspan="2" style="background-color: #f3f3f3"><em>150 MiB / 5000 files</em>
    </td>
    <td style="background-color: #f3f3f3">Direct GCS API calls
    </td>
-   <td style="background-color: #f3f3f3">1,228
+   <td style="background-color: #f3f3f3">1,225
    </td>
   </tr>
   <tr>
-   <td style="background-color: #f3f3f3"><strong>Dataflux</strong>
+   <td style="background-color: #f3f3f3"><strong>Dataflux Iterable-style Dataset</strong>
    </td>
-   <td style="background-color: #f3f3f3"><strong>1,288</strong>
+   <td style="background-color: #f3f3f3"><strong>1,143</strong>
    </td>
   </tr>
 </table>
 
 *Note: Within each experiment, all training parameters such as batch size and parallelism are consistent. The team is working on publishing a detailed analysis soon.*
 
 ## Limitations
```

### Comparing `gcs-torch-dataflux-0.1.0/gcs_torch_dataflux.egg-info/SOURCES.txt` & `gcs-torch-dataflux-1.0.0/gcs_torch_dataflux.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcs-torch-dataflux-0.1.0/pyproject.toml` & `gcs-torch-dataflux-1.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gcs-torch-dataflux"
-version = "0.1.0"
+version = "1.0.0"
 description = "A GCS data loading integration for PyTorch"
 requires-python = ">=3.8,<3.13"
 readme = "README.md"
 maintainers = [
     { name = "Google Dataflux Dev Team", email = "dataflux-customer-support@google.com" },
 ]
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: Apache Software License",
```

