# Comparing `tmp/openicite-0.1.5.tar.gz` & `tmp/openicite-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openicite-0.1.5.tar", last modified: Mon Apr  1 08:35:22 2024, max compression
+gzip compressed data, was "openicite-0.1.6.tar", last modified: Tue Apr  2 15:08:56 2024, max compression
```

## Comparing `openicite-0.1.5.tar` & `openicite-0.1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 Zyh       (1002) Zyh       (1002)        0 2024-04-01 08:35:22.205515 openicite-0.1.5/
--rw-rw-r--   0 Zyh       (1002) Zyh       (1002)     1088 2024-04-01 08:27:38.000000 openicite-0.1.5/LICENSE
--rw-r--r--   0 Zyh       (1002) Zyh       (1002)     7909 2024-04-01 08:35:22.205515 openicite-0.1.5/PKG-INFO
--rw-rw-r--   0 Zyh       (1002) Zyh       (1002)     7519 2024-04-01 08:27:38.000000 openicite-0.1.5/README.md
-drwxrwxr-x   0 Zyh       (1002) Zyh       (1002)        0 2024-04-01 08:35:22.201515 openicite-0.1.5/openicite/
--rw-rw-r--   0 Zyh       (1002) Zyh       (1002)     3428 2024-04-01 08:34:09.000000 openicite-0.1.5/openicite/__init__.py
-drwxrwxr-x   0 Zyh       (1002) Zyh       (1002)        0 2024-04-01 08:35:22.205515 openicite-0.1.5/openicite.egg-info/
--rw-r--r--   0 Zyh       (1002) Zyh       (1002)     7909 2024-04-01 08:35:22.000000 openicite-0.1.5/openicite.egg-info/PKG-INFO
--rw-rw-r--   0 Zyh       (1002) Zyh       (1002)      218 2024-04-01 08:35:22.000000 openicite-0.1.5/openicite.egg-info/SOURCES.txt
--rw-rw-r--   0 Zyh       (1002) Zyh       (1002)        1 2024-04-01 08:35:22.000000 openicite-0.1.5/openicite.egg-info/dependency_links.txt
--rw-rw-r--   0 Zyh       (1002) Zyh       (1002)        9 2024-04-01 08:35:22.000000 openicite-0.1.5/openicite.egg-info/requires.txt
--rw-rw-r--   0 Zyh       (1002) Zyh       (1002)       10 2024-04-01 08:35:22.000000 openicite-0.1.5/openicite.egg-info/top_level.txt
--rw-rw-r--   0 Zyh       (1002) Zyh       (1002)      649 2024-04-01 08:35:12.000000 openicite-0.1.5/pyproject.toml
--rw-rw-r--   0 Zyh       (1002) Zyh       (1002)       38 2024-04-01 08:35:22.205515 openicite-0.1.5/setup.cfg
+drwxrwxr-x   0 Zyh       (1002) Zyh       (1002)        0 2024-04-02 15:08:56.841413 openicite-0.1.6/
+-rw-rw-r--   0 Zyh       (1002) Zyh       (1002)     1088 2024-04-01 08:27:38.000000 openicite-0.1.6/LICENSE
+-rw-r--r--   0 Zyh       (1002) Zyh       (1002)     7909 2024-04-02 15:08:56.841413 openicite-0.1.6/PKG-INFO
+-rw-rw-r--   0 Zyh       (1002) Zyh       (1002)     7519 2024-04-01 08:27:38.000000 openicite-0.1.6/README.md
+drwxrwxr-x   0 Zyh       (1002) Zyh       (1002)        0 2024-04-02 15:08:56.841413 openicite-0.1.6/openicite/
+-rw-rw-r--   0 Zyh       (1002) Zyh       (1002)     4852 2024-04-02 15:08:23.000000 openicite-0.1.6/openicite/__init__.py
+drwxrwxr-x   0 Zyh       (1002) Zyh       (1002)        0 2024-04-02 15:08:56.841413 openicite-0.1.6/openicite.egg-info/
+-rw-r--r--   0 Zyh       (1002) Zyh       (1002)     7909 2024-04-02 15:08:56.000000 openicite-0.1.6/openicite.egg-info/PKG-INFO
+-rw-rw-r--   0 Zyh       (1002) Zyh       (1002)      218 2024-04-02 15:08:56.000000 openicite-0.1.6/openicite.egg-info/SOURCES.txt
+-rw-rw-r--   0 Zyh       (1002) Zyh       (1002)        1 2024-04-02 15:08:56.000000 openicite-0.1.6/openicite.egg-info/dependency_links.txt
+-rw-rw-r--   0 Zyh       (1002) Zyh       (1002)        9 2024-04-02 15:08:56.000000 openicite-0.1.6/openicite.egg-info/requires.txt
+-rw-rw-r--   0 Zyh       (1002) Zyh       (1002)       10 2024-04-02 15:08:56.000000 openicite-0.1.6/openicite.egg-info/top_level.txt
+-rw-rw-r--   0 Zyh       (1002) Zyh       (1002)      649 2024-04-02 15:08:45.000000 openicite-0.1.6/pyproject.toml
+-rw-rw-r--   0 Zyh       (1002) Zyh       (1002)       38 2024-04-02 15:08:56.841413 openicite-0.1.6/setup.cfg
```

### Comparing `openicite-0.1.5/LICENSE` & `openicite-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openicite-0.1.5/PKG-INFO` & `openicite-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openicite
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python wrapper for interacting with the iCite API
 Author-email: phage-GP <mirscope@outlook.com>
 Project-URL: Homepage, https://github.com/opendoicom/openicite/
 Project-URL: Issues, https://github.com/opendoicom/openicite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openicite-0.1.5/README.md` & `openicite-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `openicite-0.1.5/openicite.egg-info/PKG-INFO` & `openicite-0.1.6/openicite.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openicite
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python wrapper for interacting with the iCite API
 Author-email: phage-GP <mirscope@outlook.com>
 Project-URL: Homepage, https://github.com/opendoicom/openicite/
 Project-URL: Issues, https://github.com/opendoicom/openicite/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `openicite-0.1.5/pyproject.toml` & `openicite-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openicite"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="phage-GP", email="mirscope@outlook.com" },
 ]
 description = "A python wrapper for interacting with the iCite API"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

