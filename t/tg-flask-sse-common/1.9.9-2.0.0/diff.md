# Comparing `tmp/tg_flask_sse_common-1.9.9.tar.gz` & `tmp/tg_flask_sse_common-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_flask_sse_common-1.9.9.tar", last modified: Tue Apr  2 13:07:32 2024, max compression
+gzip compressed data, was "tg_flask_sse_common-2.0.0.tar", last modified: Tue Apr  2 13:19:30 2024, max compression
```

## Comparing `tg_flask_sse_common-1.9.9.tar` & `tg_flask_sse_common-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 13:07:32.046105 tg_flask_sse_common-1.9.9/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 13:07:32.045882 tg_flask_sse_common-1.9.9/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-1.9.9/README.md
--rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-02 13:07:32.046145 tg_flask_sse_common-1.9.9/setup.cfg
--rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-02 13:07:29.000000 tg_flask_sse_common-1.9.9/setup.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 13:07:32.045002 tg_flask_sse_common-1.9.9/tg_flask_sse_common/
--rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-02 13:07:27.000000 tg_flask_sse_common-1.9.9/tg_flask_sse_common/__init__.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-1.9.9/tg_flask_sse_common/sse_cache.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    19810 2024-04-02 13:06:54.000000 tg_flask_sse_common-1.9.9/tg_flask_sse_common/sse_clients.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-1.9.9/tg_flask_sse_common/sse_constant.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-1.9.9/tg_flask_sse_common/sse_core.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-1.9.9/tg_flask_sse_common/sse_message.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-1.9.9/tg_flask_sse_common/sse_redis_pub_sub.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 13:07:32.045638 tg_flask_sse_common-1.9.9/tg_flask_sse_common.egg-info/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 13:07:32.000000 tg_flask_sse_common-1.9.9/tg_flask_sse_common.egg-info/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-02 13:07:32.000000 tg_flask_sse_common-1.9.9/tg_flask_sse_common.egg-info/SOURCES.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-02 13:07:32.000000 tg_flask_sse_common-1.9.9/tg_flask_sse_common.egg-info/dependency_links.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-02 13:07:32.000000 tg_flask_sse_common-1.9.9/tg_flask_sse_common.egg-info/top_level.txt
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 13:19:30.532188 tg_flask_sse_common-2.0.0/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 13:19:30.531958 tg_flask_sse_common-2.0.0/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-2.0.0/README.md
+-rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-02 13:19:30.532242 tg_flask_sse_common-2.0.0/setup.cfg
+-rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-02 13:19:14.000000 tg_flask_sse_common-2.0.0/setup.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 13:19:30.531022 tg_flask_sse_common-2.0.0/tg_flask_sse_common/
+-rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-02 13:19:10.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/__init__.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_cache.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    19958 2024-04-02 13:18:29.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_clients.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_constant.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_core.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_message.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_redis_pub_sub.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 13:19:30.531725 tg_flask_sse_common-2.0.0/tg_flask_sse_common.egg-info/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 13:19:30.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common.egg-info/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-02 13:19:30.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common.egg-info/SOURCES.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-02 13:19:30.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common.egg-info/dependency_links.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-02 13:19:30.000000 tg_flask_sse_common-2.0.0/tg_flask_sse_common.egg-info/top_level.txt
```

### Comparing `tg_flask_sse_common-1.9.9/tg_flask_sse_common/sse_cache.py` & `tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_cache.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.9/tg_flask_sse_common/sse_clients.py` & `tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,22 +169,23 @@
                     'channel': channel,
                     'release_connect_count': release_connect_count,
                     'channel_connect_count': len(sse_connect_list),
                     'channel_count': self.count(),
                     'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
                 })
 
-        print({
-            'title': 'sse-log',
-            'msg': '移除超时频道',
-            'ln_id': self.local_node_id,
-            'release_channel_list': release_channel_list,
-            'channel_count': self.count(),
-            'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
-        })
+        if len(release_channel_list) > 0:
+            print({
+                'title': 'sse-log',
+                'msg': '移除超时频道',
+                'ln_id': self.local_node_id,
+                'release_channel_list': release_channel_list,
+                'channel_count': self.count(),
+                'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
+            })
 
     def release_message_accumulate_sse(self):
         """
         移除消息堆积过多的连接对象
         """
         release_channel_list = list()
 
@@ -215,22 +216,23 @@
                     'channel': channel,
                     'release_connect_count': release_connect_count,
                     'channel_connect_count': len(sse_connect_list),
                     'channel_count': self.count(),
                     'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
                 })
 
-        print({
-            'title': 'sse-log',
-            'msg': '移除消息堆积过多频道',
-            'ln_id': self.local_node_id,
-            'release_channel_list': release_channel_list,
-            'channel_count': self.count(),
-            'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
-        })
+        if len(release_channel_list) > 0:
+            print({
+                'title': 'sse-log',
+                'msg': '移除消息堆积过多频道',
+                'ln_id': self.local_node_id,
+                'release_channel_list': release_channel_list,
+                'channel_count': self.count(),
+                'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
+            })
 
     def disconnect_sse(self, channel, client_id):
         """
         监听到推送消息异常后，可以判断客户端是断开连接
         需注意 :
             这个事件的触发是非实时，所以在执行清理的时候，sse_connect_list中可能存在多个连接对象
         :param channel: 连接id
```

### Comparing `tg_flask_sse_common-1.9.9/tg_flask_sse_common/sse_constant.py` & `tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_constant.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.9/tg_flask_sse_common/sse_core.py` & `tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_core.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.9/tg_flask_sse_common/sse_message.py` & `tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_message.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.9/tg_flask_sse_common/sse_redis_pub_sub.py` & `tg_flask_sse_common-2.0.0/tg_flask_sse_common/sse_redis_pub_sub.py`

 * *Files identical despite different names*

