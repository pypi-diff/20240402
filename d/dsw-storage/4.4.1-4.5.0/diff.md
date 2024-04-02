# Comparing `tmp/dsw-storage-4.4.1.tar.gz` & `tmp/dsw-storage-4.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsw-storage-4.4.1.tar", last modified: Tue Mar 19 11:37:40 2024, max compression
+gzip compressed data, was "dsw-storage-4.5.0.tar", last modified: Tue Apr  2 10:29:09 2024, max compression
```

## Comparing `dsw-storage-4.4.1.tar` & `dsw-storage-4.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:40.359862 dsw-storage-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-03-19 11:37:35.000000 dsw-storage-4.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-19 11:37:40.355862 dsw-storage-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-19 11:37:35.000000 dsw-storage-4.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:40.355862 dsw-storage-4.4.1/dsw/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:40.355862 dsw-storage-4.4.1/dsw/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-19 11:37:35.000000 dsw-storage-4.4.1/dsw/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-19 11:37:40.000000 dsw-storage-4.4.1/dsw/storage/build_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-03-19 11:37:35.000000 dsw-storage-4.4.1/dsw/storage/s3storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 11:37:40.355862 dsw-storage-4.4.1/dsw_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-19 11:37:40.000000 dsw-storage-4.4.1/dsw_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-19 11:37:40.000000 dsw-storage-4.4.1/dsw_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 11:37:40.000000 dsw-storage-4.4.1/dsw_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 11:37:40.000000 dsw-storage-4.4.1/dsw_storage.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-19 11:37:40.000000 dsw-storage-4.4.1/dsw_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-19 11:37:40.000000 dsw-storage-4.4.1/dsw_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-03-19 11:37:35.000000 dsw-storage-4.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 11:37:40.359862 dsw-storage-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 11:37:35.000000 dsw-storage-4.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:09.080476 dsw-storage-4.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-04-02 10:29:01.000000 dsw-storage-4.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-02 10:29:09.080476 dsw-storage-4.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-04-02 10:29:01.000000 dsw-storage-4.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:09.076476 dsw-storage-4.5.0/dsw/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:09.076476 dsw-storage-4.5.0/dsw/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-02 10:29:01.000000 dsw-storage-4.5.0/dsw/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 10:29:08.000000 dsw-storage-4.5.0/dsw/storage/build_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-02 10:29:01.000000 dsw-storage-4.5.0/dsw/storage/s3storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 10:29:09.080476 dsw-storage-4.5.0/dsw_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-02 10:29:09.000000 dsw-storage-4.5.0/dsw_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-02 10:29:09.000000 dsw-storage-4.5.0/dsw_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:29:09.000000 dsw-storage-4.5.0/dsw_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 10:29:09.000000 dsw-storage-4.5.0/dsw_storage.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 10:29:09.000000 dsw-storage-4.5.0/dsw_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-02 10:29:09.000000 dsw-storage-4.5.0/dsw_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-02 10:29:01.000000 dsw-storage-4.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:29:09.080476 dsw-storage-4.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 10:29:01.000000 dsw-storage-4.5.0/setup.py
```

### Comparing `dsw-storage-4.4.1/LICENSE` & `dsw-storage-4.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dsw-storage-4.4.1/PKG-INFO` & `dsw-storage-4.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-storage
-Version: 4.4.1
+Version: 4.5.0
 Summary: Library for managing DSW S3 storage
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,s3,bucket,storage
@@ -16,15 +16,15 @@
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: minio
 Requires-Dist: tenacity
-Requires-Dist: dsw-config==4.4.1
+Requires-Dist: dsw-config==4.5.0
 
 # Data Stewardship Wizard: Storage
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-storage)](https://pypi.org/project/dsw-storage/)
 [![LICENSE](https://img.shields.io/github/license/ds-wizard/engine-tools)](LICENSE)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4975/badge)](https://bestpractices.coreinfrastructure.org/projects/4975)
```

### Comparing `dsw-storage-4.4.1/README.md` & `dsw-storage-4.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dsw-storage-4.4.1/dsw/storage/s3storage.py` & `dsw-storage-4.5.0/dsw/storage/s3storage.py`

 * *Files identical despite different names*

### Comparing `dsw-storage-4.4.1/dsw_storage.egg-info/PKG-INFO` & `dsw-storage-4.5.0/dsw_storage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dsw-storage
-Version: 4.4.1
+Version: 4.5.0
 Summary: Library for managing DSW S3 storage
 Author-email: Marek Suchánek <marek.suchanek@ds-wizard.org>
 License: Apache License 2.0
 Project-URL: Homepage, https://ds-wizard.org
 Project-URL: Repository, https://github.com/ds-wizard/engine-tools
 Project-URL: Documentation, https://guide.ds-wizard.org
 Keywords: dsw,s3,bucket,storage
@@ -16,15 +16,15 @@
 Classifier: Topic :: Communications :: File Sharing
 Classifier: Topic :: Utilities
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: minio
 Requires-Dist: tenacity
-Requires-Dist: dsw-config==4.4.1
+Requires-Dist: dsw-config==4.5.0
 
 # Data Stewardship Wizard: Storage
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/ds-wizard/engine-tools)](https://github.com/ds-wizard/engine-tools/releases)
 [![PyPI](https://img.shields.io/pypi/v/dsw-storage)](https://pypi.org/project/dsw-storage/)
 [![LICENSE](https://img.shields.io/github/license/ds-wizard/engine-tools)](LICENSE)
 [![CII Best Practices](https://bestpractices.coreinfrastructure.org/projects/4975/badge)](https://bestpractices.coreinfrastructure.org/projects/4975)
```

### Comparing `dsw-storage-4.4.1/pyproject.toml` & `dsw-storage-4.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'dsw-storage'
-version = "4.4.1"
+version = "4.5.0"
 description = 'Library for managing DSW S3 storage'
 readme = 'README.md'
 keywords = ['dsw', 's3', 'bucket', 'storage']
 license = { text = 'Apache License 2.0' }
 authors = [
     { name = 'Marek Suchánek', email = 'marek.suchanek@ds-wizard.org' }
 ]
@@ -22,15 +22,15 @@
     'Topic :: Utilities',
 ]
 requires-python = '>=3.10, <4'
 dependencies = [
     'minio',
     'tenacity',
     # DSW
-    "dsw-config==4.4.1",
+    "dsw-config==4.5.0",
 ]
 
 [project.urls]
 Homepage = 'https://ds-wizard.org'
 Repository = 'https://github.com/ds-wizard/engine-tools'
 Documentation = 'https://guide.ds-wizard.org'
```

