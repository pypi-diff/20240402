# Comparing `tmp/tg_flask_sse_common-1.9.5.tar.gz` & `tmp/tg_flask_sse_common-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tg_flask_sse_common-1.9.5.tar", last modified: Fri Mar 29 06:37:05 2024, max compression
+gzip compressed data, was "tg_flask_sse_common-1.9.6.tar", last modified: Tue Apr  2 02:25:47 2024, max compression
```

## Comparing `tg_flask_sse_common-1.9.5.tar` & `tg_flask_sse_common-1.9.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-03-29 06:37:05.337172 tg_flask_sse_common-1.9.5/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-03-29 06:37:05.336939 tg_flask_sse_common-1.9.5/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-1.9.5/README.md
--rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-03-29 06:37:05.337217 tg_flask_sse_common-1.9.5/setup.cfg
--rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-03-29 06:36:58.000000 tg_flask_sse_common-1.9.5/setup.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-03-29 06:37:05.336005 tg_flask_sse_common-1.9.5/tg_flask_sse_common/
--rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-03-29 06:36:54.000000 tg_flask_sse_common-1.9.5/tg_flask_sse_common/__init__.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-1.9.5/tg_flask_sse_common/sse_cache.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    17091 2024-03-29 06:36:28.000000 tg_flask_sse_common-1.9.5/tg_flask_sse_common/sse_clients.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-1.9.5/tg_flask_sse_common/sse_constant.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-1.9.5/tg_flask_sse_common/sse_core.py
--rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-1.9.5/tg_flask_sse_common/sse_message.py
--rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-1.9.5/tg_flask_sse_common/sse_redis_pub_sub.py
-drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-03-29 06:37:05.336705 tg_flask_sse_common-1.9.5/tg_flask_sse_common.egg-info/
--rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-03-29 06:37:05.000000 tg_flask_sse_common-1.9.5/tg_flask_sse_common.egg-info/PKG-INFO
--rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-03-29 06:37:05.000000 tg_flask_sse_common-1.9.5/tg_flask_sse_common.egg-info/SOURCES.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-03-29 06:37:05.000000 tg_flask_sse_common-1.9.5/tg_flask_sse_common.egg-info/dependency_links.txt
--rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-03-29 06:37:05.000000 tg_flask_sse_common-1.9.5/tg_flask_sse_common.egg-info/top_level.txt
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 02:25:47.684421 tg_flask_sse_common-1.9.6/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 02:25:47.684186 tg_flask_sse_common-1.9.6/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)       69 2024-02-07 02:00:45.000000 tg_flask_sse_common-1.9.6/README.md
+-rw-r--r--   0 iamtsm     (501) staff       (20)       38 2024-04-02 02:25:47.684474 tg_flask_sse_common-1.9.6/setup.cfg
+-rw-r--r--   0 iamtsm     (501) staff       (20)      510 2024-04-02 02:25:32.000000 tg_flask_sse_common-1.9.6/setup.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 02:25:47.683189 tg_flask_sse_common-1.9.6/tg_flask_sse_common/
+-rw-r--r--   0 iamtsm     (501) staff       (20)       94 2024-04-02 02:25:28.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/__init__.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5167 2024-03-29 05:44:23.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_cache.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    19741 2024-04-02 02:22:34.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_clients.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     2384 2024-03-29 06:07:56.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_constant.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     5233 2024-03-29 06:36:35.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_core.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)     1387 2024-03-29 06:10:28.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_message.py
+-rw-r--r--   0 iamtsm     (501) staff       (20)    14831 2024-03-29 05:49:11.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_redis_pub_sub.py
+drwxr-xr-x   0 iamtsm     (501) staff       (20)        0 2024-04-02 02:25:47.683947 tg_flask_sse_common-1.9.6/tg_flask_sse_common.egg-info/
+-rw-r--r--   0 iamtsm     (501) staff       (20)      285 2024-04-02 02:25:47.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common.egg-info/PKG-INFO
+-rw-r--r--   0 iamtsm     (501) staff       (20)      434 2024-04-02 02:25:47.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common.egg-info/SOURCES.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)        1 2024-04-02 02:25:47.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common.egg-info/dependency_links.txt
+-rw-r--r--   0 iamtsm     (501) staff       (20)       20 2024-04-02 02:25:47.000000 tg_flask_sse_common-1.9.6/tg_flask_sse_common.egg-info/top_level.txt
```

### Comparing `tg_flask_sse_common-1.9.5/tg_flask_sse_common/sse_cache.py` & `tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_cache.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.5/tg_flask_sse_common/sse_clients.py` & `tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_clients.py`

 * *Files 12% similar despite different names*

```diff
@@ -96,83 +96,138 @@
             self.Field.LATER_RELEASE: False,
         })
 
         self.sse_global_clients[channel] = sse_connect_list
 
         return True, "ok", client_id
 
-    def get_sse(self, channel):
-        """
-        获取连接对象
-        :param channel: 连接id
-        """
-        sse_connect_list = self.sse_global_clients.get(channel)
-
-        if not sse_connect_list:
-            sse_connect_list = []
-
-        return sse_connect_list
-
     def release_sse(self, channel):
         """
         移除待释放连接对象
         :param channel: 连接id
         """
         # 移除待释放连接对象
-        release_count = 0
+        release_connect_count = 0
+        release_channel_list = list()
 
         sse_connect_list = self.sse_global_clients.get(channel)
         for index, sse_connect in enumerate(sse_connect_list):
             if sse_connect.get(self.Field.LATER_RELEASE):
                 sse_connect_list.pop(index)
-                release_count += 1
+                release_connect_count += 1
 
         if len(sse_connect_list) == 0:
             self.sse_global_clients.pop(channel)
+            release_channel_list.append(channel)
+
+        if release_connect_count > 0 or len(release_channel_list) > 0:
+            print({
+                'title': 'sse-log',
+                'msg': '移除待释放连接/频道',
+                'ln_id': self.local_node_id,
+                'channel': channel,
+                'release_connect_count': release_connect_count,
+                'release_channel_list': release_channel_list,
+                'channel_connect_count': len(sse_connect_list),
+                'channel_count': self.count(),
+                'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
+            })
+
+    def release_timeout_sse(self):
+        """
+        移除超时连接对象
+        """
+        release_channel_list = list()
+
+        for channel in enumerate(self.sse_global_clients.keys()):
+            release_connect_count = 0
+
+            sse_connect_list = self.sse_global_clients.get(channel)
+            if sse_connect_list is None:
+                continue
+
+            for index, sse_connect in enumerate(sse_connect_list):
+                if not sse_connect:
+                    continue
+
+                connect_time = sse_connect.get(self.Field.CONNECT_TIME, datetime.now())
+                if (datetime.now() - connect_time).seconds > self.max_connect_time:
+                    sse_connect_list.pop(index)
+                    release_connect_count += 1
+
+            if len(sse_connect_list) == 0:
+                self.sse_global_clients.pop(channel)
+                release_channel_list.append(channel)
+
+            if release_connect_count > 0:
+                print({
+                    'title': 'sse-log',
+                    'msg': '移除超时连接',
+                    'ln_id': self.local_node_id,
+                    'channel': channel,
+                    'release_connect_count': release_connect_count,
+                    'channel_connect_count': len(sse_connect_list),
+                    'channel_count': self.count(),
+                    'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
+                })
 
         print({
             'title': 'sse-log',
-            'msg': '移除待释放连接',
+            'msg': '移除超时频道',
             'ln_id': self.local_node_id,
-            'channel': channel,
-            'release_count': release_count,
-            'channel_connect_count': len(sse_connect_list),
+            'release_channel_list': release_channel_list,
             'channel_count': self.count(),
             'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
         })
 
-    def release_timeout_sse(self):
+    def release_message_accumulate_sse(self):
         """
-        移除超时连接对象
+        移除消息堆积过多的连接对象
         """
-        for channel, sse_connect_list in self.sse_global_clients.items():
-            release_count = 0
+        release_channel_list = list()
+
+        for channel in enumerate(self.sse_global_clients.keys()):
+            release_connect_count = 0
+
+            sse_connect_list = self.sse_global_clients.get(channel)
+            if sse_connect_list is None:
+                continue
 
             for index, sse_connect in enumerate(sse_connect_list):
                 if not sse_connect:
                     continue
 
-                connect_time = sse_connect.get(self.Field.CONNECT_TIME, datetime.now())
-                if (datetime.now() - connect_time).seconds > self.max_connect_time:
+                message_list = sse_connect.get(self.Field.MESSAGE_LIST, [])
+                if len(message_list) > 200:
                     sse_connect_list.pop(index)
-                    release_count += 1
 
             if len(sse_connect_list) == 0:
                 self.sse_global_clients.pop(channel)
+                release_channel_list.append(channel)
 
-            print({
-                'title': 'sse-log',
-                'msg': '移除超时连接',
-                'ln_id': self.local_node_id,
-                'channel': channel,
-                'release_count': release_count,
-                'channel_connect_count': len(sse_connect_list),
-                'channel_count': self.count(),
-                'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
-            })
+            if release_connect_count > 0:
+                print({
+                    'title': 'sse-log',
+                    'msg': '移除消息堆积过多连接',
+                    'ln_id': self.local_node_id,
+                    'channel': channel,
+                    'release_connect_count': release_connect_count,
+                    'channel_connect_count': len(sse_connect_list),
+                    'channel_count': self.count(),
+                    'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
+                })
+
+        print({
+            'title': 'sse-log',
+            'msg': '移除消息堆积过多频道',
+            'ln_id': self.local_node_id,
+            'release_channel_list': release_channel_list,
+            'channel_count': self.count(),
+            'time': datetime.now().strftime('%Y-%m-%d %H:%M:%S'),
+        })
 
     def disconnect_sse(self, channel, client_id):
         """
         监听到推送消息异常后，可以判断客户端是断开连接
         需注意 :
             这个事件的触发是非实时，所以在执行清理的时候，sse_connect_list中可能存在多个连接对象
         :param channel: 连接id
@@ -215,15 +270,18 @@
 
     def add_message(self, channel, message):
         """
         添加消息到连接对象，监听到redis-pub-sub消息时调用
         :param channel: 连接id
         :param message: 消息
         """
-        sse_connect_list = self.get_sse(channel)
+        sse_connect_list = self.sse_global_clients.get(channel)
+        if not sse_connect_list:
+            sse_connect_list = []
+
         for sse_connect in sse_connect_list:
             if not sse_connect:
                 continue
 
             message_list = sse_connect.get(self.Field.MESSAGE_LIST, [])
             message_list.append(message)
             sse_connect.update({
@@ -238,19 +296,22 @@
         """
         # 问题:
         # 因为flask是无法主动监听到连接是否关闭的(或者说客户端关闭事件，flask是不会向上抛出异常)，所以需要定时发送心跳包
         # 一旦客户端关闭连接，就会收不到心跳包（yield报错），这时候协程将断开连接，while将直接退出，设置LATER_RELEASE=true。
         #
         # 1. 每次心跳包时，将清理已经关闭的连接对象
         # 2. 每次心跳包时，将清理超时连接对象 (额外兜底)
+        # 3. 每次心跳包时，将检测消息堆积过多的对象
         self.release_timeout_sse()
 
         for channel, sse_connect_list in self.sse_global_clients.items():
             self.release_sse(channel=channel)
 
+        self.release_message_accumulate_sse()
+
         # 移除完失效连接后，往有效连接中添加心跳消息
         for channel, sse_connect_list in self.sse_global_clients.items():
             self.add_message(
                 channel=channel,
                 message=SseMessage(
                     channel=channel,
                     data=SseSystemEventType.HEARTBEAT,
@@ -261,15 +322,18 @@
             )
 
     def listen_message(self, channel):
         """
         监听消息
         """
         latest_sse_connect = None
-        sse_connect_list = self.get_sse(channel)
+
+        sse_connect_list = self.sse_global_clients.get(channel)
+        if not sse_connect_list:
+            sse_connect_list = []
 
         for sse_connect in sse_connect_list:
             if not sse_connect:
                 continue
             if sse_connect.get(self.Field.LATER_RELEASE):
                 continue
```

### Comparing `tg_flask_sse_common-1.9.5/tg_flask_sse_common/sse_constant.py` & `tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_constant.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.5/tg_flask_sse_common/sse_core.py` & `tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_core.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.5/tg_flask_sse_common/sse_message.py` & `tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_message.py`

 * *Files identical despite different names*

### Comparing `tg_flask_sse_common-1.9.5/tg_flask_sse_common/sse_redis_pub_sub.py` & `tg_flask_sse_common-1.9.6/tg_flask_sse_common/sse_redis_pub_sub.py`

 * *Files identical despite different names*

