# Comparing `tmp/tg_flask_sse_common-1.9.7.tar.gz` & `tmp/tg_flask_sse_common-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_flask_sse_common-1.9.7.tar", last modified: Tue Apr  2 12:50:05 2024, max compression
+gzip compressed data, was "tg_flask_sse_common-1.9.8.tar", last modified: Tue Apr  2 12:57:39 2024, max compression
```

## Comparing `tg_flask_sse_common-1.9.7.tar` & `tg_flask_sse_common-1.9.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 12:50:05.365920 tg_flask_sse_common-1.9.7/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 12:50:05.365718 tg_flask_sse_common-1.9.7/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-1.9.7/README.md
--rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-02 12:50:05.365968 tg_flask_sse_common-1.9.7/setup.cfg
--rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-02 12:49:46.000000 tg_flask_sse_common-1.9.7/setup.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 12:50:05.364748 tg_flask_sse_common-1.9.7/tg_flask_sse_common/
--rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-02 12:49:43.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/__init__.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_cache.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    19733 2024-04-02 12:49:27.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_clients.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_constant.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_core.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_message.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_redis_pub_sub.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 12:50:05.365494 tg_flask_sse_common-1.9.7/tg_flask_sse_common.egg-info/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 12:50:05.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common.egg-info/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-02 12:50:05.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common.egg-info/SOURCES.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-02 12:50:05.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common.egg-info/dependency_links.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-02 12:50:05.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common.egg-info/top_level.txt
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 12:57:39.000839 tg_flask_sse_common-1.9.8/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 12:57:39.000592 tg_flask_sse_common-1.9.8/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-1.9.8/README.md
+-rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-02 12:57:39.000893 tg_flask_sse_common-1.9.8/setup.cfg
+-rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-02 12:57:28.000000 tg_flask_sse_common-1.9.8/setup.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 12:57:38.999665 tg_flask_sse_common-1.9.8/tg_flask_sse_common/
+-rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-02 12:57:25.000000 tg_flask_sse_common-1.9.8/tg_flask_sse_common/__init__.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-1.9.8/tg_flask_sse_common/sse_cache.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    19801 2024-04-02 12:57:04.000000 tg_flask_sse_common-1.9.8/tg_flask_sse_common/sse_clients.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-1.9.8/tg_flask_sse_common/sse_constant.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-1.9.8/tg_flask_sse_common/sse_core.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-1.9.8/tg_flask_sse_common/sse_message.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-1.9.8/tg_flask_sse_common/sse_redis_pub_sub.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 12:57:39.000346 tg_flask_sse_common-1.9.8/tg_flask_sse_common.egg-info/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 12:57:38.000000 tg_flask_sse_common-1.9.8/tg_flask_sse_common.egg-info/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-02 12:57:38.000000 tg_flask_sse_common-1.9.8/tg_flask_sse_common.egg-info/SOURCES.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-02 12:57:38.000000 tg_flask_sse_common-1.9.8/tg_flask_sse_common.egg-info/dependency_links.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-02 12:57:38.000000 tg_flask_sse_common-1.9.8/tg_flask_sse_common.egg-info/top_level.txt
```

### Comparing `tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_cache.py` & `tg_flask_sse_common-1.9.8/tg_flask_sse_common/sse_cache.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_clients.py` & `tg_flask_sse_common-1.9.8/tg_flask_sse_common/sse_clients.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,17 @@
         :param channel: 连接id
         """
         # 移除待释放连接对象
         release_connect_count = 0
         release_channel_list = list()
 
         sse_connect_list = self.sse_global_clients.get(channel)
+        if not sse_connect_list:
+            sse_connect_list = []
+
         for index, sse_connect in enumerate(sse_connect_list):
             if sse_connect.get(self.Field.LATER_RELEASE):
                 sse_connect_list.pop(index)
                 release_connect_count += 1
 
         if len(sse_connect_list) == 0:
             self.sse_global_clients.pop(channel)
```

### Comparing `tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_constant.py` & `tg_flask_sse_common-1.9.8/tg_flask_sse_common/sse_constant.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_core.py` & `tg_flask_sse_common-1.9.8/tg_flask_sse_common/sse_core.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_message.py` & `tg_flask_sse_common-1.9.8/tg_flask_sse_common/sse_message.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_redis_pub_sub.py` & `tg_flask_sse_common-1.9.8/tg_flask_sse_common/sse_redis_pub_sub.py`

 * *Files identical despite different names*

