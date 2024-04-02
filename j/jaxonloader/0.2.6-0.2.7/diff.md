# Comparing `tmp/jaxonloader-0.2.6.tar.gz` & `tmp/jaxonloader-0.2.7.tar.gz`

## Comparing `jaxonloader-0.2.6.tar` & `jaxonloader-0.2.7.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/.pre-commit-config.yaml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/mkdocs.yml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/noxfile.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/.github/workflows/nox.yaml
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/.github/workflows/pre_commit.yaml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/docs/api.md
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/docs/future.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/docs/getting-started.md
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/docs/index.md
--rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/docs/images/performance.png
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/jaxonloader/__init__.py
--rw-r--r--   0        0        0     6114 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/jaxonloader/_datasets.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/jaxonloader/dataloader.py
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/jaxonloader/dataset.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/jaxonloader/utils.py
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/tests/test_mnist.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/tests/test_tinyshakespeare.py
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/LICENSE
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/README.md
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 jaxonloader-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/mkdocs.yml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/noxfile.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/.github/workflows/nox.yaml
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/.github/workflows/pre_commit.yaml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/docs/api.md
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/docs/future.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/docs/getting-started.md
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/docs/index.md
+-rw-r--r--   0        0        0   126325 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/docs/images/performance.png
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/jaxonloader/__init__.py
+-rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/jaxonloader/dataloader.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/jaxonloader/dataset.py
+-rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/jaxonloader/datasets.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/jaxonloader/utils.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/tests/test_mnist.py
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/tests/test_tinyshakespeare.py
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/README.md
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3491 2020-02-02 00:00:00.000000 jaxonloader-0.2.7/PKG-INFO
```

### Comparing `jaxonloader-0.2.6/.github/workflows/nox.yaml` & `jaxonloader-0.2.7/.github/workflows/nox.yaml`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.6/docs/getting-started.md` & `jaxonloader-0.2.7/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.6/docs/index.md` & `jaxonloader-0.2.7/docs/index.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.6/docs/images/performance.png` & `jaxonloader-0.2.7/docs/images/performance.png`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.6/jaxonloader/_datasets.py` & `jaxonloader-0.2.7/jaxonloader/datasets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,82 +1,122 @@
 import os
 import pathlib
-import urllib.request
-import zipfile
+import pickle
 from collections.abc import Callable
 
 import numpy as np
 import pandas as pd
 import polars as pl
 from loguru import logger
-from numpy.typing import NDArray as Array
+from numpy import ndarray as NDArray
 
-from jaxonloader.dataset import JaxonDataset, SingleArrayDataset
-from jaxonloader.utils import jaxonloader_cache, JAXONLOADER_PATH
+from jaxonloader.dataset import DataTargetDataset, JaxonDataset, SingleArrayDataset
+from jaxonloader.utils import (
+    download_and_extract_zip,
+    jaxonloader_cache,
+    JAXONLOADER_PATH,
+)
 
 
 @jaxonloader_cache(dataset_name="mnist")
 def get_mnist() -> tuple[JaxonDataset, JaxonDataset]:
-    MNIST_TRAIN_URL = (
-        "https://omnisium.eu-central-1.linodeobjects.com/mnist/mnist_train.csv.zip"
-    )
-    MNIST_TEST_URL = (
-        "https://omnisium.eu-central-1.linodeobjects.com/mnist/mnist_test.csv.zip"
-    )
-
+    data_url = "https://omnisium.eu-central-1.linodeobjects.com/mnist/mnist.zip"
     data_path = pathlib.Path(JAXONLOADER_PATH) / "mnist"
-    if not os.path.exists(data_path / "mnist_train.csv"):
-        logger.info(f"Downloading the dataset from {MNIST_TRAIN_URL}")
-        urllib.request.urlretrieve(MNIST_TRAIN_URL, data_path / "mnist_train.csv.zip")
-        with zipfile.ZipFile(data_path / "mnist_train.csv.zip", "r") as zip_ref:
-            logger.info(f"Extracting the dataset to {data_path}")
-            zip_ref.extractall(data_path)
-
-    if not os.path.exists(data_path / "mnist_test.csv"):
-        logger.info(f"Downloading the dataset from {MNIST_TEST_URL}")
-        urllib.request.urlretrieve(MNIST_TEST_URL, data_path / "mnist_test.csv.zip")
-        with zipfile.ZipFile(data_path / "mnist_test.csv.zip", "r") as zip_ref:
-            logger.info(f"Extracting the dataset to {data_path}")
-            zip_ref.extractall(data_path)
-
-    assert os.path.exists(
-        data_path / "mnist_train.csv"
-    ), "Failed to download the dataset"
-    assert os.path.exists(
-        data_path / "mnist_test.csv"
-    ), "Failed to download the dataset"
+    download_and_extract_zip(data_url, data_path)
 
     train_df = pl.read_csv(data_path / "mnist_train.csv")
     test_df = pl.read_csv(data_path / "mnist_test.csv")
 
     x_train = train_df.to_numpy()
     x_test = test_df.to_numpy()
 
     train_dataset = SingleArrayDataset(x_train)
     test_dataset = SingleArrayDataset(x_test)
     return train_dataset, test_dataset
 
 
-def get_cifar10():
-    raise NotImplementedError("get_cifar10 is not implemented yet.")
+@jaxonloader_cache(dataset_name="cifar10")
+def get_cifar10() -> tuple[JaxonDataset, JaxonDataset]:
+    data_url = "https://omnisium.eu-central-1.linodeobjects.com/cifar10/cifar-10-batches-py.zip"
+    data_path = pathlib.Path(JAXONLOADER_PATH) / "cifar10"
+    download_and_extract_zip(data_url, data_path)
+    n_batches = 5
+    train_data = []
+    train_labels = []
+    for i in range(1, n_batches + 1):
+        with open(data_path / f"cifar-10-batches-py/data_batch_{i}", "rb") as f:
+            data = pickle.load(f, encoding="bytes")
+            train_data.append(data[b"data"])
+            train_labels.append(data[b"labels"])
+    train_data = np.concatenate(train_data)
+    train_labels = np.concatenate(train_labels)
+
+    with open(data_path / "cifar-10-batches-py/test_batch", "rb") as f:
+        data = pickle.load(f, encoding="bytes")
+        test_data = data[b"data"]
+        test_labels = data[b"labels"]
+
+    train_dataset = DataTargetDataset(train_data, train_labels)
+    test_dataset = DataTargetDataset(test_data, test_labels)
+
+    return train_dataset, test_dataset
+
+
+@jaxonloader_cache(dataset_name="cifar100")
+def get_cifar100() -> tuple[JaxonDataset, JaxonDataset]:
+    dataset_url = (
+        "https://omnisium.eu-central-1.linodeobjects.com/cifar100/cifar-100-python.zip"
+    )
+    data_path = pathlib.Path(JAXONLOADER_PATH) / "cifar100"
+    download_and_extract_zip(dataset_url, data_path)
+
+    if os.path.exists(data_path) and not os.path.exists(data_path / "cifar-100-python"):
+        raise FileNotFoundError(
+            f"The data folder {data_path} exists but the dataset is missing. "
+            + "If this error persists, please delete the data folder and try again."
+        )
+
+    with open(data_path / "cifar-100-python/train", "rb") as f:
+        train_data = pickle.load(f, encoding="bytes")
+    with open(data_path / "cifar-100-python/test", "rb") as f:
+        test_data = pickle.load(f, encoding="bytes")
+
+    class CiFar100Dataset(JaxonDataset):
+        def __init__(
+            self, data: NDArray, fine_labels: list[int], coarse_labels: list[int]
+        ):
+            self.data = data
+            self.fine_labels = np.array(fine_labels)
+            self.coarse_labels = np.array(coarse_labels)
+
+        def __len__(self) -> int:
+            return len(self.data)
+
+        def __getitem__(self, idx: NDArray) -> tuple[NDArray, NDArray, NDArray]:
+            return self.data[idx], self.fine_labels[idx], self.coarse_labels[idx]
 
+    train_dataset = CiFar100Dataset(
+        train_data[b"data"], train_data[b"fine_labels"], train_data[b"coarse_labels"]
+    )
+    test_dataset = CiFar100Dataset(
+        test_data[b"data"], test_data[b"fine_labels"], test_data[b"coarse_labels"]
+    )
 
-def get_cifar100():
-    raise NotImplementedError("get_cifar100 is not implemented yet.")
+    return train_dataset, test_dataset
 
 
 def get_fashion_mnist():
     raise NotImplementedError("get_fashion_mnist is not implemented yet.")
 
 
 @jaxonloader_cache(dataset_name="tinyshakespeare")
 def get_tiny_shakespeare(
     block_size: int = 8, train_ratio: float = 0.8
 ) -> tuple[
-    JaxonDataset, JaxonDataset, int, Callable[[str], Array], Callable[[Array], str]
+    JaxonDataset, JaxonDataset, int, Callable[[str], NDArray], Callable[[NDArray], str]
 ]:
     """
     Get the tiny shakespeare dataset from Andrej Karpathy's char-rnn repository.
 
     Args:
         block_size: The number of tokens in a block in a sequence.
         train_ratio: The ratio of the dataset to be used for training.
@@ -113,18 +153,18 @@
     text = get_text()
     chars = sorted(list(set(text)))
     vocab_size = len(chars)
 
     char_to_idx = {ch: i for i, ch in enumerate(chars)}
     idx_to_char = {i: ch for i, ch in enumerate(chars)}
 
-    def encode(string: str) -> Array:
+    def encode(string: str) -> NDArray:
         return np.array([char_to_idx[ch] for ch in string])
 
-    def decode(latent: Array) -> str:
+    def decode(latent: NDArray) -> str:
         return "".join([idx_to_char[idx] for idx in latent])
 
     encoder = encode
     decoder = decode
     data = np.array(encode(text))
     n = int(train_ratio * len(data))
 
@@ -151,15 +191,14 @@
 
     Args:
     dataframe: A polars.DataFrame (or pandas.DataFrame).
 
     Returns:
     A JaxonDataset.
     """
-
     df: pl.DataFrame = (
         pl.from_pandas(dataframe) if isinstance(dataframe, pd.DataFrame) else dataframe
     )
     data = df.to_numpy()
     return SingleArrayDataset(data)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `jaxonloader-0.2.6/jaxonloader/dataloader.py` & `jaxonloader-0.2.7/jaxonloader/dataloader.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,18 +28,18 @@
             self.indices = np.array(list(range(len(dataset))))
         rng = get_rng(key)
 
         if self.shuffle:
             self.indices = rng.permutation(self.indices)
         self.index = 0
 
-    def __iter__(self):
+    def __iter__(self) -> "JaxonDataLoader":
         return self
 
-    def __next__(self) -> npt.NDArray:
+    def __next__(self) -> npt.NDArray | tuple[npt.NDArray, ...]:
         if self.index < len(self.indices):
             batch_indices = self.indices[self.index : self.index + self.batch_size]
             self.index += self.batch_size
             return self.dataset[batch_indices]
         else:
             self.index = 0
             raise StopIteration
```

### Comparing `jaxonloader-0.2.6/.gitignore` & `jaxonloader-0.2.7/.gitignore`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.6/LICENSE` & `jaxonloader-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.6/README.md` & `jaxonloader-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `jaxonloader-0.2.6/pyproject.toml` & `jaxonloader-0.2.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 [project]
 name = "jaxonloader"
-version = "0.2.6"
+version = "0.2.7"
 description = "A dataloader, but for JAX"
 readme = "README.md"
 requires-python ="~=3.10"
 license = {file = "LICENSE"}
 authors = [
   {name = "Artur A. Galstyan", email = "mail@arturgalstyan.dev"},
 ]
 dependencies=[
   "tqdm",
+  "jaxtyping",
+  "progressbar",
   "polars",
+  "beartype",
   "typing_extensions",
   "loguru",
   "kaggle",
   "pandas",
   "pyarrow",
 ]
 [project.optional-dependencies]
```

### Comparing `jaxonloader-0.2.6/PKG-INFO` & `jaxonloader-0.2.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jaxonloader
-Version: 0.2.6
+Version: 0.2.7
 Summary: A dataloader, but for JAX
 Author-email: "Artur A. Galstyan" <mail@arturgalstyan.dev>
 License: MIT License
         
         Copyright (c) 2024 Artur A. Galstyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,18 +22,21 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Requires-Python: ~=3.10
+Requires-Dist: beartype
+Requires-Dist: jaxtyping
 Requires-Dist: kaggle
 Requires-Dist: loguru
 Requires-Dist: pandas
 Requires-Dist: polars
+Requires-Dist: progressbar
 Requires-Dist: pyarrow
 Requires-Dist: tqdm
 Requires-Dist: typing-extensions
 Provides-Extra: dev
 Requires-Dist: mkdocs; extra == 'dev'
 Requires-Dist: nox; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
```

