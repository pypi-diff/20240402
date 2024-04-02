# Comparing `tmp/apify-1.7.1b1.tar.gz` & `tmp/apify-1.7.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify-1.7.1b1.tar", last modified: Tue Mar 12 16:54:11 2024, max compression
+gzip compressed data, was "apify-1.7.1b2.tar", last modified: Tue Apr  2 13:22:44 2024, max compression
```

## Comparing `apify-1.7.1b1.tar` & `apify-1.7.1b2.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:54:11.442022 apify-1.7.1b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-03-12 16:53:32.000000 apify-1.7.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-03-12 16:54:11.442022 apify-1.7.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-03-12 16:53:32.000000 apify-1.7.1b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-03-12 16:54:08.000000 apify-1.7.1b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 16:54:11.442022 apify-1.7.1b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:54:11.430022 apify-1.7.1b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:54:11.434022 apify-1.7.1b1/src/apify/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_crypto.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:54:11.434022 apify-1.7.1b1/src/apify/_memory_storage/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_memory_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_memory_storage/file_storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10598 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_memory_storage/memory_storage_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:54:11.438022 apify-1.7.1b1/src/apify/_memory_storage/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_memory_storage/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_memory_storage/resource_clients/base_resource_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_memory_storage/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_memory_storage/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_memory_storage/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_memory_storage/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_memory_storage/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    59997 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/event_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/proxy_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:54:11.438022 apify-1.7.1b1/src/apify/scrapy/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/scrapy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:54:11.438022 apify-1.7.1b1/src/apify/scrapy/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/scrapy/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/scrapy/middlewares/apify_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:54:11.438022 apify-1.7.1b1/src/apify/scrapy/pipelines/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/scrapy/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/scrapy/pipelines/actor_dataset_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/scrapy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/scrapy/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/scrapy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:54:11.438022 apify-1.7.1b1/src/apify/storages/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/storages/base_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    23339 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/storages/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/storages/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    28829 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/storages/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-03-12 16:53:32.000000 apify-1.7.1b1/src/apify/storages/storage_client_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 16:54:11.438022 apify-1.7.1b1/src/apify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-03-12 16:54:11.000000 apify-1.7.1b1/src/apify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-03-12 16:54:11.000000 apify-1.7.1b1/src/apify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 16:54:11.000000 apify-1.7.1b1/src/apify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-12 16:54:11.000000 apify-1.7.1b1/src/apify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-12 16:54:11.000000 apify-1.7.1b1/src/apify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:22:44.377393 apify-1.7.1b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-04-02 13:22:04.000000 apify-1.7.1b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-02 13:22:44.377393 apify-1.7.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3635 2024-04-02 13:22:04.000000 apify-1.7.1b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-02 13:22:40.000000 apify-1.7.1b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:22:44.377393 apify-1.7.1b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:22:44.365393 apify-1.7.1b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:22:44.369393 apify-1.7.1b2/src/apify/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_crypto.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:22:44.369393 apify-1.7.1b2/src/apify/_memory_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_memory_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_memory_storage/file_storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10598 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_memory_storage/memory_storage_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:22:44.373393 apify-1.7.1b2/src/apify/_memory_storage/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_memory_storage/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5163 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_memory_storage/resource_clients/base_resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20062 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_memory_storage/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_memory_storage/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20581 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_memory_storage/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_memory_storage/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19700 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_memory_storage/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_memory_storage/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16963 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59997 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2263 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/event_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15735 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/proxy_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:22:44.373393 apify-1.7.1b2/src/apify/scrapy/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/scrapy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:22:44.373393 apify-1.7.1b2/src/apify/scrapy/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/scrapy/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5919 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/scrapy/middlewares/apify_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:22:44.373393 apify-1.7.1b2/src/apify/scrapy/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/scrapy/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/scrapy/pipelines/actor_dataset_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7935 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/scrapy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/scrapy/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/scrapy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:22:44.373393 apify-1.7.1b2/src/apify/storages/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7434 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/storages/base_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23339 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/storages/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10760 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/storages/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28829 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/storages/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-02 13:22:04.000000 apify-1.7.1b2/src/apify/storages/storage_client_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:22:44.373393 apify-1.7.1b2/src/apify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-02 13:22:44.000000 apify-1.7.1b2/src/apify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-04-02 13:22:44.000000 apify-1.7.1b2/src/apify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:22:44.000000 apify-1.7.1b2/src/apify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-02 13:22:44.000000 apify-1.7.1b2/src/apify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 13:22:44.000000 apify-1.7.1b2/src/apify.egg-info/top_level.txt
```

### Comparing `apify-1.7.1b1/LICENSE` & `apify-1.7.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/PKG-INFO` & `apify-1.7.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.7.1b1
+Version: 1.7.1b2
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
```

### Comparing `apify-1.7.1b1/README.md` & `apify-1.7.1b2/README.md`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/pyproject.toml` & `apify-1.7.1b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apify"
-version = "1.7.1b1"
+version = "1.7.1b2"
 description = "Apify SDK for Python"
 readme = "README.md"
 license = { text = "Apache Software License" }
 authors = [{ name = "Apify Technologies s.r.o.", email = "support@apify.com" }]
 keywords = ["apify", "sdk", "actor", "scraping", "automation"]
 
 classifiers = [
```

### Comparing `apify-1.7.1b1/src/apify/_crypto.py` & `apify-1.7.1b2/src/apify/_crypto.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/_memory_storage/file_storage_utils.py` & `apify-1.7.1b2/src/apify/_memory_storage/file_storage_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/_memory_storage/memory_storage_client.py` & `apify-1.7.1b2/src/apify/_memory_storage/memory_storage_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/_memory_storage/resource_clients/__init__.py` & `apify-1.7.1b2/src/apify/_memory_storage/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/_memory_storage/resource_clients/base_resource_client.py` & `apify-1.7.1b2/src/apify/_memory_storage/resource_clients/base_resource_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py` & `apify-1.7.1b2/src/apify/_memory_storage/resource_clients/base_resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/_memory_storage/resource_clients/dataset.py` & `apify-1.7.1b2/src/apify/_memory_storage/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/_memory_storage/resource_clients/dataset_collection.py` & `apify-1.7.1b2/src/apify/_memory_storage/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/_memory_storage/resource_clients/key_value_store.py` & `apify-1.7.1b2/src/apify/_memory_storage/resource_clients/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/_memory_storage/resource_clients/key_value_store_collection.py` & `apify-1.7.1b2/src/apify/_memory_storage/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/_memory_storage/resource_clients/request_queue.py` & `apify-1.7.1b2/src/apify/_memory_storage/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/_memory_storage/resource_clients/request_queue_collection.py` & `apify-1.7.1b2/src/apify/_memory_storage/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/_utils.py` & `apify-1.7.1b2/src/apify/_utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/actor.py` & `apify-1.7.1b2/src/apify/actor.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/config.py` & `apify-1.7.1b2/src/apify/config.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/consts.py` & `apify-1.7.1b2/src/apify/consts.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/event_manager.py` & `apify-1.7.1b2/src/apify/event_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/log.py` & `apify-1.7.1b2/src/apify/log.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/proxy_configuration.py` & `apify-1.7.1b2/src/apify/proxy_configuration.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/scrapy/middlewares/apify_proxy.py` & `apify-1.7.1b2/src/apify/scrapy/middlewares/apify_proxy.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/scrapy/pipelines/actor_dataset_push.py` & `apify-1.7.1b2/src/apify/scrapy/pipelines/actor_dataset_push.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/scrapy/requests.py` & `apify-1.7.1b2/src/apify/scrapy/requests.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/scrapy/scheduler.py` & `apify-1.7.1b2/src/apify/scrapy/scheduler.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/scrapy/utils.py` & `apify-1.7.1b2/src/apify/scrapy/utils.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/storages/base_storage.py` & `apify-1.7.1b2/src/apify/storages/base_storage.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/storages/dataset.py` & `apify-1.7.1b2/src/apify/storages/dataset.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/storages/key_value_store.py` & `apify-1.7.1b2/src/apify/storages/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/storages/request_queue.py` & `apify-1.7.1b2/src/apify/storages/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify/storages/storage_client_manager.py` & `apify-1.7.1b2/src/apify/storages/storage_client_manager.py`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify.egg-info/PKG-INFO` & `apify-1.7.1b2/src/apify.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify
-Version: 1.7.1b1
+Version: 1.7.1b2
 Summary: Apify SDK for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/sdk/python/
 Project-URL: Documentation, https://docs.apify.com/sdk/python/
 Project-URL: Source, https://github.com/apify/apify-sdk-python
 Project-URL: Issue tracker, https://github.com/apify/apify-sdk-python/issues
```

### Comparing `apify-1.7.1b1/src/apify.egg-info/SOURCES.txt` & `apify-1.7.1b2/src/apify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apify-1.7.1b1/src/apify.egg-info/requires.txt` & `apify-1.7.1b2/src/apify.egg-info/requires.txt`

 * *Files identical despite different names*

