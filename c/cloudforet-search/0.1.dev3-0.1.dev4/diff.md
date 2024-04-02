# Comparing `tmp/cloudforet-search-0.1.dev3.tar.gz` & `tmp/cloudforet-search-0.1.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudforet-search-0.1.dev3.tar", last modified: Thu Mar 21 08:39:42 2024, max compression
+gzip compressed data, was "cloudforet-search-0.1.dev4.tar", last modified: Tue Apr  2 01:10:09 2024, max compression
```

## Comparing `cloudforet-search-0.1.dev3.tar` & `cloudforet-search-0.1.dev4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:41.999373 cloudforet-search-0.1.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-21 08:39:41.999373 cloudforet-search-0.1.dev3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:41.995373 cloudforet-search-0.1.dev3/cloudforet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:41.995373 cloudforet-search-0.1.dev3/cloudforet/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:41.995373 cloudforet-search-0.1.dev3/cloudforet/search/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/conf/global_conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/conf/search_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:41.995373 cloudforet-search-0.1.dev3/cloudforet/search/interface/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:41.995373 cloudforet-search-0.1.dev3/cloudforet/search/interface/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/interface/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/interface/grpc/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:41.995373 cloudforet-search-0.1.dev3/cloudforet/search/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/lib/pymongo_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:41.995373 cloudforet-search-0.1.dev3/cloudforet/search/manager/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/manager/identity_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/manager/resource_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:41.999373 cloudforet-search-0.1.dev3/cloudforet/search/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:41.999373 cloudforet-search-0.1.dev3/cloudforet/search/model/resource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/model/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/model/resource/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/model/resource/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:41.999373 cloudforet-search-0.1.dev3/cloudforet/search/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15104 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/cloudforet/search/service/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 08:39:41.999373 cloudforet-search-0.1.dev3/cloudforet_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-21 08:39:41.000000 cloudforet-search-0.1.dev3/cloudforet_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-21 08:39:41.000000 cloudforet-search-0.1.dev3/cloudforet_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 08:39:41.000000 cloudforet-search-0.1.dev3/cloudforet_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 08:39:41.000000 cloudforet-search-0.1.dev3/cloudforet_search.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-21 08:39:41.000000 cloudforet-search-0.1.dev3/cloudforet_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-21 08:39:41.000000 cloudforet-search-0.1.dev3/cloudforet_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 08:39:41.999373 cloudforet-search-0.1.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-03-21 08:39:31.000000 cloudforet-search-0.1.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:10:09.838300 cloudforet-search-0.1.dev4/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-02 01:10:09.838300 cloudforet-search-0.1.dev4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:10:09.834300 cloudforet-search-0.1.dev4/cloudforet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:10:09.834300 cloudforet-search-0.1.dev4/cloudforet/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:10:09.838300 cloudforet-search-0.1.dev4/cloudforet/search/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/conf/global_conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4480 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/conf/search_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:10:09.838300 cloudforet-search-0.1.dev4/cloudforet/search/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:10:09.838300 cloudforet-search-0.1.dev4/cloudforet/search/interface/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/interface/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/interface/grpc/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:10:09.838300 cloudforet-search-0.1.dev4/cloudforet/search/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/lib/pymongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:10:09.838300 cloudforet-search-0.1.dev4/cloudforet/search/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/manager/identity_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8887 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/manager/resource_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:10:09.838300 cloudforet-search-0.1.dev4/cloudforet/search/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:10:09.838300 cloudforet-search-0.1.dev4/cloudforet/search/model/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/model/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/model/resource/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/model/resource/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:10:09.838300 cloudforet-search-0.1.dev4/cloudforet/search/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15104 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/cloudforet/search/service/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 01:10:09.838300 cloudforet-search-0.1.dev4/cloudforet_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-02 01:10:09.000000 cloudforet-search-0.1.dev4/cloudforet_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-02 01:10:09.000000 cloudforet-search-0.1.dev4/cloudforet_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:10:09.000000 cloudforet-search-0.1.dev4/cloudforet_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 01:10:09.000000 cloudforet-search-0.1.dev4/cloudforet_search.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-02 01:10:09.000000 cloudforet-search-0.1.dev4/cloudforet_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 01:10:09.000000 cloudforet-search-0.1.dev4/cloudforet_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 01:10:09.838300 cloudforet-search-0.1.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-04-02 01:09:51.000000 cloudforet-search-0.1.dev4/setup.py
```

### Comparing `cloudforet-search-0.1.dev3/cloudforet/search/conf/global_conf.py` & `cloudforet-search-0.1.dev4/cloudforet/search/conf/global_conf.py`

 * *Files identical despite different names*

### Comparing `cloudforet-search-0.1.dev3/cloudforet/search/conf/search_conf.py` & `cloudforet-search-0.1.dev4/cloudforet/search/conf/search_conf.py`

 * *Files identical despite different names*

### Comparing `cloudforet-search-0.1.dev3/cloudforet/search/interface/grpc/resource.py` & `cloudforet-search-0.1.dev4/cloudforet/search/interface/grpc/resource.py`

 * *Files identical despite different names*

### Comparing `cloudforet-search-0.1.dev3/cloudforet/search/lib/pymongo_client.py` & `cloudforet-search-0.1.dev4/cloudforet/search/lib/pymongo_client.py`

 * *Files identical despite different names*

### Comparing `cloudforet-search-0.1.dev3/cloudforet/search/lib/utils.py` & `cloudforet-search-0.1.dev4/cloudforet/search/lib/utils.py`

 * *Files identical despite different names*

### Comparing `cloudforet-search-0.1.dev3/cloudforet/search/manager/identity_manager.py` & `cloudforet-search-0.1.dev4/cloudforet/search/manager/identity_manager.py`

 * *Files identical despite different names*

### Comparing `cloudforet-search-0.1.dev3/cloudforet/search/manager/resource_manager.py` & `cloudforet-search-0.1.dev4/cloudforet/search/manager/resource_manager.py`

 * *Files identical despite different names*

### Comparing `cloudforet-search-0.1.dev3/cloudforet/search/service/resource.py` & `cloudforet-search-0.1.dev4/cloudforet/search/service/resource.py`

 * *Files identical despite different names*

### Comparing `cloudforet-search-0.1.dev3/cloudforet_search.egg-info/SOURCES.txt` & `cloudforet-search-0.1.dev4/cloudforet_search.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudforet-search-0.1.dev3/setup.py` & `cloudforet-search-0.1.dev4/setup.py`

 * *Files identical despite different names*

