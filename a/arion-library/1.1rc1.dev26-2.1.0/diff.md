# Comparing `tmp/arion_library-1.1rc1.dev26.tar.gz` & `tmp/arion_library-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arion_library-1.1rc1.dev26.tar", last modified: Tue Apr  2 13:08:57 2024, max compression
+gzip compressed data, was "arion_library-2.1.0.tar", last modified: Tue Mar 26 12:35:37 2024, max compression
```

## Comparing `arion_library-1.1rc1.dev26.tar` & `arion_library-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:57.595188 arion_library-1.1rc1.dev26/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 13:08:57.595188 arion_library-1.1rc1.dev26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:57.591188 arion_library-1.1rc1.dev26/arion_library.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 13:08:57.000000 arion_library-1.1rc1.dev26/arion_library.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-02 13:08:57.000000 arion_library-1.1rc1.dev26/arion_library.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:08:57.000000 arion_library-1.1rc1.dev26/arion_library.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-02 13:08:57.000000 arion_library-1.1rc1.dev26/arion_library.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 13:08:57.000000 arion_library-1.1rc1.dev26/arion_library.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:57.591188 arion_library-1.1rc1.dev26/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:57.591188 arion_library-1.1rc1.dev26/processors/azure_storage_provider/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/azure_storage_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:57.595188 arion_library-1.1rc1.dev26/processors/azure_storage_provider/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/azure_storage_provider/lib/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/azure_storage_provider/lib/azureBlobStorage.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4930 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/azure_storage_provider/lib/azureTableStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/azure_storage_provider/lib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:57.595188 arion_library-1.1rc1.dev26/processors/azure_storage_provider/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/azure_storage_provider/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/azure_storage_provider/tests/test_blob.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/azure_storage_provider/tests/test_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:57.595188 arion_library-1.1rc1.dev26/processors/msserversql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/msserversql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:57.595188 arion_library-1.1rc1.dev26/processors/msserversql/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/msserversql/lib/MsServerSQL.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/msserversql/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:57.595188 arion_library-1.1rc1.dev26/processors/msserversql/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/msserversql/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/msserversql/tests/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-02 13:08:53.000000 arion_library-1.1rc1.dev26/processors/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:08:57.595188 arion_library-1.1rc1.dev26/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:37.267429 arion_library-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-26 12:35:37.267429 arion_library-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-26 12:35:31.000000 arion_library-2.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:37.267429 arion_library-2.1.0/arion_library.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-26 12:35:37.000000 arion_library-2.1.0/arion_library.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-03-26 12:35:37.000000 arion_library-2.1.0/arion_library.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 12:35:37.000000 arion_library-2.1.0/arion_library.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-03-26 12:35:37.000000 arion_library-2.1.0/arion_library.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-26 12:35:37.000000 arion_library-2.1.0/arion_library.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:37.267429 arion_library-2.1.0/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:37.267429 arion_library-2.1.0/processors/azure_storage_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/azure_storage_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:37.267429 arion_library-2.1.0/processors/azure_storage_provider/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/azure_storage_provider/lib/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3072 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/azure_storage_provider/lib/azureBlobStorage.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4930 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/azure_storage_provider/lib/azureTableStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/azure_storage_provider/lib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:37.267429 arion_library-2.1.0/processors/azure_storage_provider/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/azure_storage_provider/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/azure_storage_provider/tests/test_blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/azure_storage_provider/tests/test_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:37.267429 arion_library-2.1.0/processors/msserversql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/msserversql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:37.267429 arion_library-2.1.0/processors/msserversql/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/msserversql/lib/MsServerSQL.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/msserversql/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:37.267429 arion_library-2.1.0/processors/msserversql/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/msserversql/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/msserversql/tests/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-26 12:35:31.000000 arion_library-2.1.0/processors/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 12:35:37.267429 arion_library-2.1.0/setup.cfg
```

### Comparing `arion_library-1.1rc1.dev26/arion_library.egg-info/SOURCES.txt` & `arion_library-2.1.0/arion_library.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev26/processors/azure_storage_provider/lib/azureBlobStorage.py` & `arion_library-2.1.0/processors/azure_storage_provider/lib/azureBlobStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev26/processors/azure_storage_provider/lib/azureTableStorage.py` & `arion_library-2.1.0/processors/azure_storage_provider/lib/azureTableStorage.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev26/processors/azure_storage_provider/lib/config.py` & `arion_library-2.1.0/processors/azure_storage_provider/lib/config.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev26/processors/azure_storage_provider/tests/test_blob.py` & `arion_library-2.1.0/processors/azure_storage_provider/tests/test_blob.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev26/processors/azure_storage_provider/tests/test_env.py` & `arion_library-2.1.0/processors/azure_storage_provider/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev26/processors/msserversql/lib/MsServerSQL.py` & `arion_library-2.1.0/processors/msserversql/lib/MsServerSQL.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev26/processors/msserversql/tests/test_methods.py` & `arion_library-2.1.0/processors/msserversql/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `arion_library-1.1rc1.dev26/processors/setup.py` & `arion_library-2.1.0/processors/setup.py`

 * *Files identical despite different names*

