# Comparing `tmp/xibabel-0.0.1a0.tar.gz` & `tmp/xibabel-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xibabel-0.0.1a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "xibabel-0.0.1a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `xibabel-0.0.1a0.tar` & `xibabel-0.0.1a1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     2951 2024-04-01 22:53:59.280176 xibabel-0.0.1a0/README.md
--rw-r--r--   0        0        0     1122 2024-04-01 20:13:24.938093 xibabel-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0      104 2024-04-01 20:13:24.938279 xibabel-0.0.1a0/src/xibabel/__init__.py
--rw-r--r--   0        0        0      571 2024-04-01 20:13:24.938488 xibabel-0.0.1a0/src/xibabel/bench/bench_nib_xib_load.py
--rw-r--r--   0        0        0    18610 2024-04-01 22:51:03.504803 xibabel-0.0.1a0/src/xibabel/loaders.py
--rw-r--r--   0        0        0       20 2024-04-01 20:13:24.938858 xibabel-0.0.1a0/src/xibabel/testing/.gitignore
--rw-r--r--   0        0        0      921 2024-04-01 20:13:24.939016 xibabel-0.0.1a0/src/xibabel/testing/__init__.py
--rw-r--r--   0        0        0      627 2024-04-01 20:13:24.939155 xibabel-0.0.1a0/src/xibabel/testing/__main__.py
--rw-r--r--   0        0        0     5075 2024-04-01 20:13:24.939378 xibabel-0.0.1a0/src/xibabel/testing/fetcher.py
--rw-r--r--   0        0        0      463 2024-04-01 20:13:24.939585 xibabel-0.0.1a0/src/xibabel/testing/test_files.yml
--rw-r--r--   0        0        0      396 2024-04-01 20:13:24.939726 xibabel-0.0.1a0/src/xibabel/testing/test_sets.yml
--rw-r--r--   0        0        0        0 2024-04-01 20:13:24.939864 xibabel-0.0.1a0/src/xibabel/tests/__init__.py
--rw-r--r--   0        0        0     2512 2024-04-01 20:13:24.940151 xibabel-0.0.1a0/src/xibabel/tests/conftest.py
--rw-r--r--   0        0        0     1306 2024-04-01 20:13:24.940358 xibabel-0.0.1a0/src/xibabel/tests/run_server.py
--rw-r--r--   0        0        0    14228 2024-04-01 22:51:03.505743 xibabel-0.0.1a0/src/xibabel/tests/test_loaders.py
--rw-r--r--   0        0        0     1205 2024-04-01 20:13:24.940719 xibabel-0.0.1a0/src/xibabel/tests/test_merge.py
--rw-r--r--   0        0        0     2792 2024-04-01 20:13:24.940931 xibabel-0.0.1a0/src/xibabel/tests/test_scripting.py
--rw-r--r--   0        0        0      794 2024-04-01 20:13:24.941154 xibabel-0.0.1a0/src/xibabel/xutils.py
--rw-r--r--   0        0        0     4452 1970-01-01 00:00:00.000000 xibabel-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0     2951 2024-04-01 22:53:59.280176 xibabel-0.0.1a1/README.md
+-rw-r--r--   0        0        0     1176 2024-04-01 23:00:24.571221 xibabel-0.0.1a1/pyproject.toml
+-rw-r--r--   0        0        0      104 2024-04-01 22:57:23.006276 xibabel-0.0.1a1/src/xibabel/__init__.py
+-rw-r--r--   0        0        0      571 2024-04-01 20:13:24.938488 xibabel-0.0.1a1/src/xibabel/bench/bench_nib_xib_load.py
+-rw-r--r--   0        0        0    18610 2024-04-01 22:51:03.504803 xibabel-0.0.1a1/src/xibabel/loaders.py
+-rw-r--r--   0        0        0       20 2024-04-01 20:13:24.938858 xibabel-0.0.1a1/src/xibabel/testing/.gitignore
+-rw-r--r--   0        0        0      921 2024-04-01 20:13:24.939016 xibabel-0.0.1a1/src/xibabel/testing/__init__.py
+-rw-r--r--   0        0        0      627 2024-04-01 20:13:24.939155 xibabel-0.0.1a1/src/xibabel/testing/__main__.py
+-rw-r--r--   0        0        0     5075 2024-04-01 20:13:24.939378 xibabel-0.0.1a1/src/xibabel/testing/fetcher.py
+-rw-r--r--   0        0        0      463 2024-04-01 20:13:24.939585 xibabel-0.0.1a1/src/xibabel/testing/test_files.yml
+-rw-r--r--   0        0        0      396 2024-04-01 20:13:24.939726 xibabel-0.0.1a1/src/xibabel/testing/test_sets.yml
+-rw-r--r--   0        0        0        0 2024-04-01 20:13:24.939864 xibabel-0.0.1a1/src/xibabel/tests/__init__.py
+-rw-r--r--   0        0        0     2512 2024-04-01 20:13:24.940151 xibabel-0.0.1a1/src/xibabel/tests/conftest.py
+-rw-r--r--   0        0        0     1306 2024-04-01 20:13:24.940358 xibabel-0.0.1a1/src/xibabel/tests/run_server.py
+-rw-r--r--   0        0        0    14228 2024-04-01 22:51:03.505743 xibabel-0.0.1a1/src/xibabel/tests/test_loaders.py
+-rw-r--r--   0        0        0     1205 2024-04-01 20:13:24.940719 xibabel-0.0.1a1/src/xibabel/tests/test_merge.py
+-rw-r--r--   0        0        0     2792 2024-04-01 20:13:24.940931 xibabel-0.0.1a1/src/xibabel/tests/test_scripting.py
+-rw-r--r--   0        0        0      794 2024-04-01 20:13:24.941154 xibabel-0.0.1a1/src/xibabel/xutils.py
+-rw-r--r--   0        0        0     4500 1970-01-01 00:00:00.000000 xibabel-0.0.1a1/PKG-INFO
```

### Comparing `xibabel-0.0.1a0/README.md` & `xibabel-0.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a0/pyproject.toml` & `xibabel-0.0.1a1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,16 @@
     {name = "Paul Ivanov", email = "pi@berkeley.edu"},
     {name = "Christopher J. Markiewicz", email = "markiewicz@stanford.edu"}
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 dynamic = ["version", "description"]
 home-page = "https://github.com/matthew-brett/xibabel"
-classifiers = ['License :: OSI Approved :: BSD License']
+classifiers = ['License :: OSI Approved :: BSD License',
+               'Development Status :: 2 - Pre-Alpha']
 dependencies = [
     'xarray',
     'dask',
     'nibabel',
     'nipy',
     'psutil'
 ]
```

### Comparing `xibabel-0.0.1a0/src/xibabel/bench/bench_nib_xib_load.py` & `xibabel-0.0.1a1/src/xibabel/bench/bench_nib_xib_load.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a0/src/xibabel/loaders.py` & `xibabel-0.0.1a1/src/xibabel/loaders.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a0/src/xibabel/testing/__init__.py` & `xibabel-0.0.1a1/src/xibabel/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a0/src/xibabel/testing/__main__.py` & `xibabel-0.0.1a1/src/xibabel/testing/__main__.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a0/src/xibabel/testing/fetcher.py` & `xibabel-0.0.1a1/src/xibabel/testing/fetcher.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a0/src/xibabel/tests/conftest.py` & `xibabel-0.0.1a1/src/xibabel/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a0/src/xibabel/tests/run_server.py` & `xibabel-0.0.1a1/src/xibabel/tests/run_server.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a0/src/xibabel/tests/test_loaders.py` & `xibabel-0.0.1a1/src/xibabel/tests/test_loaders.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a0/src/xibabel/tests/test_merge.py` & `xibabel-0.0.1a1/src/xibabel/tests/test_merge.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a0/src/xibabel/tests/test_scripting.py` & `xibabel-0.0.1a1/src/xibabel/tests/test_scripting.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a0/src/xibabel/xutils.py` & `xibabel-0.0.1a1/src/xibabel/xutils.py`

 * *Files identical despite different names*

### Comparing `xibabel-0.0.1a0/PKG-INFO` & `xibabel-0.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: xibabel
-Version: 0.0.1a0
+Version: 0.0.1a1
 Summary: Init for Xibabel package
 Author-email: Matthew Brett <matthew.brett@gmail.com>, Paul Ivanov <pi@berkeley.edu>, "Christopher J. Markiewicz" <markiewicz@stanford.edu>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: BSD License
+Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Dist: xarray
 Requires-Dist: dask
 Requires-Dist: nibabel
 Requires-Dist: nipy
 Requires-Dist: psutil
 Requires-Dist: pre-commit ; extra == "developer"
 Requires-Dist: nbclassic ; extra == "developer"
```

