# Comparing `tmp/scmallet-0.0.1.tar.gz` & `tmp/scmallet-0.0.2.tar.gz`

## Comparing `scmallet-0.0.1.tar` & `scmallet-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.0.1/.codecov.yaml
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scmallet-0.0.1/.cruft.json
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 scmallet-0.0.1/.editorconfig
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 scmallet-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 scmallet-0.0.1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 scmallet-0.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scmallet-0.0.1/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 scmallet-0.0.1/.github/workflows/build.yaml
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 scmallet-0.0.1/.github/workflows/release.yaml
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 scmallet-0.0.1/.github/workflows/test.yaml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 scmallet-0.0.1/src/scmallet/__init__.py
--rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 scmallet-0.0.1/src/scmallet/binarize.py
--rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 scmallet-0.0.1/src/scmallet/infer.py
--rw-r--r--   0        0        0     7905 2020-02-02 00:00:00.000000 scmallet-0.0.1/src/scmallet/input.py
--rw-r--r--   0        0        0    20237 2020-02-02 00:00:00.000000 scmallet-0.0.1/src/scmallet/mallet.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 scmallet-0.0.1/src/scmallet/utils.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 scmallet-0.0.1/tests/test_basic.py
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.0.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 scmallet-0.0.1/LICENSE
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 scmallet-0.0.1/README.md
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scmallet-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 scmallet-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.0.2/.codecov.yaml
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 scmallet-0.0.2/.cruft.json
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 scmallet-0.0.2/.editorconfig
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 scmallet-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 scmallet-0.0.2/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 scmallet-0.0.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 scmallet-0.0.2/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 scmallet-0.0.2/.github/workflows/build.yaml
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 scmallet-0.0.2/.github/workflows/release.yaml
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 scmallet-0.0.2/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/__init__.py
+-rw-r--r--   0        0        0     4426 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/binarize.py
+-rw-r--r--   0        0        0    10190 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/eval_model.py
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/infer.py
+-rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/input.py
+-rw-r--r--   0        0        0    20237 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/mallet.py
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/topic_metrices.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 scmallet-0.0.2/src/scmallet/utils.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 scmallet-0.0.2/tests/test_basic.py
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 scmallet-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 scmallet-0.0.2/LICENSE
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 scmallet-0.0.2/README.md
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 scmallet-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 scmallet-0.0.2/PKG-INFO
```

### Comparing `scmallet-0.0.1/.cruft.json` & `scmallet-0.0.2/.cruft.json`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.1/.pre-commit-config.yaml` & `scmallet-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.1/.github/ISSUE_TEMPLATE/bug_report.yml` & `scmallet-0.0.2/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.1/.github/workflows/build.yaml` & `scmallet-0.0.2/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.1/.github/workflows/release.yaml` & `scmallet-0.0.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.1/.github/workflows/test.yaml` & `scmallet-0.0.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.1/src/scmallet/binarize.py` & `scmallet-0.0.2/src/scmallet/binarize.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.1/src/scmallet/infer.py` & `scmallet-0.0.2/src/scmallet/infer.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.1/src/scmallet/input.py` & `scmallet-0.0.2/src/scmallet/input.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 def convert_input(
     data: csc_matrix,
     output_prefix: str,
     train_mallet_file: Union[str, Path] = None,
     train_id2word_file: Union[str, Path] = None,
     mem_gb: int = 4,
+    binarize_data=False,
 ):
     """
     Convert sparse.csc_matrix to Mallet format and save it to a binary file, also save the id2word dictionary.
 
     Parameters
     ----------
     data : sparse.csc_matrix
@@ -46,14 +47,17 @@
         Path to the id2word dictionary. If the model is trained, this will be the same as the train_id2word_file.
     """
     if not issparse(data):
         raise ValueError("data should be a sparse matrix")
     if not isinstance(data, csc_matrix):
         data = data.tocsc()
 
+    if binarize_data:
+        data.data = np.ones_like(data.data, dtype=bool)
+
     corpus = matutils.Sparse2Corpus(data)
 
     if train_mallet_file is not None or train_id2word_file is not None:
         trained = True
         assert train_id2word_file is not None, "train_id2word_file and train_mallet_file have to be provided together"
         assert train_mallet_file is not None, "train_id2word_file and train_mallet_file have to be provided together"
         train_mallet_path = pathlib.Path(train_mallet_file)
```

### Comparing `scmallet-0.0.1/src/scmallet/mallet.py` & `scmallet-0.0.2/src/scmallet/mallet.py`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.1/src/scmallet/utils.py` & `scmallet-0.0.2/src/scmallet/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 
 def get_mallet_path():
     """Get the path to the Mallet executable."""
     try:
         path = subprocess.check_output(["which", "mallet"], encoding="utf8")
     except subprocess.CalledProcessError:
         print(
-            "LDA package Mallet not found. Please install it with `conda install -c conda-forge mallet` or `mamba install -c conda-forge mallet`"
+            "LDA package Mallet not found. "
+            "Please install it with `conda install -c conda-forge mallet` "
+            "or `mamba install -c conda-forge mallet`"
         )
         exit(1)
     return path.strip()
 
 
 MALLET_PATH = get_mallet_path()
 MALLET_PATH = pathlib.Path(MALLET_PATH)
```

### Comparing `scmallet-0.0.1/LICENSE` & `scmallet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.1/README.md` & `scmallet-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.1/pyproject.toml` & `scmallet-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scmallet-0.0.1/PKG-INFO` & `scmallet-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: scmallet
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python wrapper of MALLET for LDA analysis on single-cell data
 Project-URL: Source, https://github.com/lhqing/scmallet
 Project-URL: Home-page, https://github.com/lhqing/scmallet
 Author: Hanqing Liu
 Maintainer-email: Hanqing Liu <hanqingliu@fas.harvard.edu>
 License: MIT License
```

