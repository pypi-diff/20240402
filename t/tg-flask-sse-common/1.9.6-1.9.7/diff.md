# Comparing `tmp/tg_flask_sse_common-1.9.6.tar.gz` & `tmp/tg_flask_sse_common-1.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_flask_sse_common-1.9.6.tar", last modified: Tue Apr  2 02:25:47 2024, max compression
+gzip compressed data, was "tg_flask_sse_common-1.9.7.tar", last modified: Tue Apr  2 12:50:05 2024, max compression
```

## Comparing `tg_flask_sse_common-1.9.6.tar` & `tg_flask_sse_common-1.9.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 02:25:47.684421 tg_flask_sse_common-1.9.6/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 02:25:47.684186 tg_flask_sse_common-1.9.6/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-1.9.6/README.md
--rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-02 02:25:47.684474 tg_flask_sse_common-1.9.6/setup.cfg
--rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-02 02:25:32.000000 tg_flask_sse_common-1.9.6/setup.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 02:25:47.683189 tg_flask_sse_common-1.9.6/tg_flask_sse_common/
--rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-02 02:25:28.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/__init__.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_cache.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    19741 2024-04-02 02:22:34.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_clients.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_constant.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_core.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_message.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_redis_pub_sub.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 02:25:47.683947 tg_flask_sse_common-1.9.6/tg_flask_sse_common.egg-info/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 02:25:47.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common.egg-info/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-02 02:25:47.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common.egg-info/SOURCES.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-02 02:25:47.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common.egg-info/dependency_links.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-02 02:25:47.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common.egg-info/top_level.txt
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 12:50:05.365920 tg_flask_sse_common-1.9.7/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 12:50:05.365718 tg_flask_sse_common-1.9.7/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-1.9.7/README.md
+-rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-02 12:50:05.365968 tg_flask_sse_common-1.9.7/setup.cfg
+-rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-02 12:49:46.000000 tg_flask_sse_common-1.9.7/setup.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 12:50:05.364748 tg_flask_sse_common-1.9.7/tg_flask_sse_common/
+-rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-02 12:49:43.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/__init__.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_cache.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    19733 2024-04-02 12:49:27.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_clients.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_constant.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_core.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_message.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_redis_pub_sub.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 12:50:05.365494 tg_flask_sse_common-1.9.7/tg_flask_sse_common.egg-info/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 12:50:05.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common.egg-info/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-02 12:50:05.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common.egg-info/SOURCES.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-02 12:50:05.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common.egg-info/dependency_links.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-02 12:50:05.000000 tg_flask_sse_common-1.9.7/tg_flask_sse_common.egg-info/top_level.txt
```

### Comparing `tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_cache.py` & `tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_cache.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_clients.py` & `tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_clients.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,15 +299,15 @@
         # 一旦客户端关闭连接，就会收不到心跳包（yield报错），这时候协程将断开连接，while将直接退出，设置LATER_RELEASE=true。
         #
         # 1. 每次心跳包时，将清理已经关闭的连接对象
         # 2. 每次心跳包时，将清理超时连接对象 (额外兜底)
         # 3. 每次心跳包时，将检测消息堆积过多的对象
         self.release_timeout_sse()
 
-        for channel, sse_connect_list in self.sse_global_clients.items():
+        for channel in enumerate(self.sse_global_clients.keys()):
             self.release_sse(channel=channel)
 
         self.release_message_accumulate_sse()
 
         # 移除完失效连接后，往有效连接中添加心跳消息
         for channel, sse_connect_list in self.sse_global_clients.items():
             self.add_message(
```

### Comparing `tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_constant.py` & `tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_constant.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_core.py` & `tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_core.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_message.py` & `tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_message.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_redis_pub_sub.py` & `tg_flask_sse_common-1.9.7/tg_flask_sse_common/sse_redis_pub_sub.py`

 * *Files identical despite different names*

