# Comparing `tmp/waifuvault-1.3.3.tar.gz` & `tmp/waifuvault-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waifuvault-1.3.3.tar", last modified: Tue Apr  2 16:35:30 2024, max compression
+gzip compressed data, was "waifuvault-1.3.4.tar", last modified: Tue Apr  2 16:46:56 2024, max compression
```

## Comparing `waifuvault-1.3.3.tar` & `waifuvault-1.3.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:35:30.316700 waifuvault-1.3.3/
--rw-r--r--   0 walker     (501) staff       (20)     1071 2024-03-11 13:55:18.000000 waifuvault-1.3.3/LICENSE
--rw-r--r--   0 walker     (501) staff       (20)     8464 2024-04-02 16:35:30.315367 waifuvault-1.3.3/PKG-INFO
--rw-r--r--   0 walker     (501) staff       (20)     7772 2024-03-24 14:27:53.000000 waifuvault-1.3.3/README.md
--rw-r--r--   0 walker     (501) staff       (20)      741 2024-04-02 16:33:02.000000 waifuvault-1.3.3/pyproject.toml
--rw-r--r--   0 walker     (501) staff       (20)       38 2024-04-02 16:35:30.316944 waifuvault-1.3.3/setup.cfg
-drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:35:30.304127 waifuvault-1.3.3/src/
-drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:35:30.308924 waifuvault-1.3.3/src/waifuvault/
--rw-r--r--   0 walker     (501) staff       (20)      133 2024-03-20 19:19:23.000000 waifuvault-1.3.3/src/waifuvault/__init__.py
--rw-r--r--   0 walker     (501) staff       (20)     1695 2024-04-02 16:24:50.000000 waifuvault-1.3.3/src/waifuvault/waifumodels.py
--rw-r--r--   0 walker     (501) staff       (20)     3568 2024-04-02 16:29:36.000000 waifuvault-1.3.3/src/waifuvault/waifuvault.py
-drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:35:30.313810 waifuvault-1.3.3/src/waifuvault.egg-info/
--rw-r--r--   0 walker     (501) staff       (20)     8464 2024-04-02 16:35:30.000000 waifuvault-1.3.3/src/waifuvault.egg-info/PKG-INFO
--rw-r--r--   0 walker     (501) staff       (20)      332 2024-04-02 16:35:30.000000 waifuvault-1.3.3/src/waifuvault.egg-info/SOURCES.txt
--rw-r--r--   0 walker     (501) staff       (20)        1 2024-04-02 16:35:30.000000 waifuvault-1.3.3/src/waifuvault.egg-info/dependency_links.txt
--rw-r--r--   0 walker     (501) staff       (20)       53 2024-04-02 16:35:30.000000 waifuvault-1.3.3/src/waifuvault.egg-info/requires.txt
--rw-r--r--   0 walker     (501) staff       (20)       11 2024-04-02 16:35:30.000000 waifuvault-1.3.3/src/waifuvault.egg-info/top_level.txt
-drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:35:30.312978 waifuvault-1.3.3/tests/
--rw-r--r--   0 walker     (501) staff       (20)     7852 2024-04-02 16:33:02.000000 waifuvault-1.3.3/tests/test_waifuvault.py
+drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:46:56.527014 waifuvault-1.3.4/
+-rw-r--r--   0 walker     (501) staff       (20)     1071 2024-03-11 13:55:18.000000 waifuvault-1.3.4/LICENSE
+-rw-r--r--   0 walker     (501) staff       (20)     8464 2024-04-02 16:46:56.526095 waifuvault-1.3.4/PKG-INFO
+-rw-r--r--   0 walker     (501) staff       (20)     7772 2024-03-24 14:27:53.000000 waifuvault-1.3.4/README.md
+-rw-r--r--   0 walker     (501) staff       (20)      741 2024-04-02 16:46:48.000000 waifuvault-1.3.4/pyproject.toml
+-rw-r--r--   0 walker     (501) staff       (20)       38 2024-04-02 16:46:56.527192 waifuvault-1.3.4/setup.cfg
+drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:46:56.515194 waifuvault-1.3.4/src/
+drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:46:56.519739 waifuvault-1.3.4/src/waifuvault/
+-rw-r--r--   0 walker     (501) staff       (20)      133 2024-03-20 19:19:23.000000 waifuvault-1.3.4/src/waifuvault/__init__.py
+-rw-r--r--   0 walker     (501) staff       (20)     1695 2024-04-02 16:24:50.000000 waifuvault-1.3.4/src/waifuvault/waifumodels.py
+-rw-r--r--   0 walker     (501) staff       (20)     3585 2024-04-02 16:46:29.000000 waifuvault-1.3.4/src/waifuvault/waifuvault.py
+drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:46:56.524457 waifuvault-1.3.4/src/waifuvault.egg-info/
+-rw-r--r--   0 walker     (501) staff       (20)     8464 2024-04-02 16:46:56.000000 waifuvault-1.3.4/src/waifuvault.egg-info/PKG-INFO
+-rw-r--r--   0 walker     (501) staff       (20)      332 2024-04-02 16:46:56.000000 waifuvault-1.3.4/src/waifuvault.egg-info/SOURCES.txt
+-rw-r--r--   0 walker     (501) staff       (20)        1 2024-04-02 16:46:56.000000 waifuvault-1.3.4/src/waifuvault.egg-info/dependency_links.txt
+-rw-r--r--   0 walker     (501) staff       (20)       53 2024-04-02 16:46:56.000000 waifuvault-1.3.4/src/waifuvault.egg-info/requires.txt
+-rw-r--r--   0 walker     (501) staff       (20)       11 2024-04-02 16:46:56.000000 waifuvault-1.3.4/src/waifuvault.egg-info/top_level.txt
+drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:46:56.523409 waifuvault-1.3.4/tests/
+-rw-r--r--   0 walker     (501) staff       (20)     7852 2024-04-02 16:33:02.000000 waifuvault-1.3.4/tests/test_waifuvault.py
```

### Comparing `waifuvault-1.3.3/LICENSE` & `waifuvault-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `waifuvault-1.3.3/PKG-INFO` & `waifuvault-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waifuvault
-Version: 1.3.3
+Version: 1.3.4
 Summary: waifuVault Python API module
 Author-email: Walker Aldridge <walker@waifuvault.moe>
 Project-URL: Homepage, https://github.com/waifuvault/waifuVault-python-api
 Project-URL: Issues, https://github.com/waifuvault/waifuVault-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `waifuvault-1.3.3/README.md` & `waifuvault-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `waifuvault-1.3.3/pyproject.toml` & `waifuvault-1.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waifuvault"
-version = "1.3.3"
+version = "1.3.4"
 authors = [
     { name="Walker Aldridge", email="walker@waifuvault.moe" },
 ]
 description = "waifuVault Python API module"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `waifuvault-1.3.3/src/waifuvault/waifumodels.py` & `waifuvault-1.3.4/src/waifuvault/waifumodels.py`

 * *Files identical despite different names*

### Comparing `waifuvault-1.3.3/src/waifuvault/waifuvault.py` & `waifuvault-1.3.4/src/waifuvault/waifuvault.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,11 +105,11 @@
 
 def __dict_to_obj(dict_obj: any):
     return FileResponse(
         dict_obj["token"],
         dict_obj["url"],
         dict_obj["retentionPeriod"],
         FileOptions(
-            dict_obj["options.hideFileName"],
-            dict_obj["options.oneTimeDownload"],
-            dict_obj["protected"]
+            dict_obj["options"]["hideFileName"],
+            dict_obj["options"]["oneTimeDownload"],
+            dict_obj["options"]["protected"]
         ))
```

### Comparing `waifuvault-1.3.3/src/waifuvault.egg-info/PKG-INFO` & `waifuvault-1.3.4/src/waifuvault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waifuvault
-Version: 1.3.3
+Version: 1.3.4
 Summary: waifuVault Python API module
 Author-email: Walker Aldridge <walker@waifuvault.moe>
 Project-URL: Homepage, https://github.com/waifuvault/waifuVault-python-api
 Project-URL: Issues, https://github.com/waifuvault/waifuVault-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `waifuvault-1.3.3/tests/test_waifuvault.py` & `waifuvault-1.3.4/tests/test_waifuvault.py`

 * *Files identical despite different names*

