# Comparing `tmp/telegram_collector-0.0.7.tar.gz` & `tmp/telegram_collector-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "telegram_collector-0.0.7.tar", last modified: Mon Apr  1 15:17:48 2024, max compression
+gzip compressed data, was "telegram_collector-0.0.8.tar", last modified: Tue Apr  2 06:47:02 2024, max compression
```

## Comparing `telegram_collector-0.0.7.tar` & `telegram_collector-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 15:17:48.137176 telegram_collector-0.0.7/
--rw-rw-rw-   0        0        0      287 2024-04-01 15:17:48.134959 telegram_collector-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-01 15:17:48.137687 telegram_collector-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      735 2024-04-01 15:17:04.000000 telegram_collector-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-01 15:17:48.119829 telegram_collector-0.0.7/telegram_collector/
--rw-rw-rw-   0        0        0     5168 2024-04-01 15:17:04.000000 telegram_collector-0.0.7/telegram_collector/__init__.py
--rw-rw-rw-   0        0        0      361 2024-04-01 07:25:42.000000 telegram_collector-0.0.7/telegram_collector/__main__.py
--rw-rw-rw-   0        0        0     2528 2024-04-01 05:08:12.000000 telegram_collector-0.0.7/telegram_collector/util.py
-drwxrwxrwx   0        0        0        0 2024-04-01 15:17:48.133582 telegram_collector-0.0.7/telegram_collector.egg-info/
--rw-rw-rw-   0        0        0      287 2024-04-01 15:17:48.000000 telegram_collector-0.0.7/telegram_collector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2024-04-01 15:17:48.000000 telegram_collector-0.0.7/telegram_collector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 15:17:48.000000 telegram_collector-0.0.7/telegram_collector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      248 2024-04-01 15:17:48.000000 telegram_collector-0.0.7/telegram_collector.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-04-01 15:17:48.000000 telegram_collector-0.0.7/telegram_collector.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-04-01 15:17:48.000000 telegram_collector-0.0.7/telegram_collector.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-02 06:47:02.797426 telegram_collector-0.0.8/
+-rw-rw-rw-   0        0        0      287 2024-04-02 06:47:02.795966 telegram_collector-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-04-02 06:47:02.797426 telegram_collector-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      735 2024-04-02 06:47:00.000000 telegram_collector-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:47:02.780718 telegram_collector-0.0.8/telegram_collector/
+-rw-rw-rw-   0        0        0     5170 2024-04-02 06:45:49.000000 telegram_collector-0.0.8/telegram_collector/__init__.py
+-rw-rw-rw-   0        0        0      361 2024-04-01 07:25:42.000000 telegram_collector-0.0.8/telegram_collector/__main__.py
+-rw-rw-rw-   0        0        0     2528 2024-04-01 05:08:12.000000 telegram_collector-0.0.8/telegram_collector/util.py
+drwxrwxrwx   0        0        0        0 2024-04-02 06:47:02.794681 telegram_collector-0.0.8/telegram_collector.egg-info/
+-rw-rw-rw-   0        0        0      287 2024-04-02 06:47:02.000000 telegram_collector-0.0.8/telegram_collector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2024-04-02 06:47:02.000000 telegram_collector-0.0.8/telegram_collector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 06:47:02.000000 telegram_collector-0.0.8/telegram_collector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      248 2024-04-02 06:47:02.000000 telegram_collector-0.0.8/telegram_collector.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-04-02 06:47:02.000000 telegram_collector-0.0.8/telegram_collector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-02 06:47:02.000000 telegram_collector-0.0.8/telegram_collector.egg-info/top_level.txt
```

### Comparing `telegram_collector-0.0.7/setup.py` & `telegram_collector-0.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding: utf-8
 
 from setuptools import setup
 
 setup(
     name='telegram_collector',
-    version='0.0.7',
+    version='0.0.8',
     author='fengleicn',
     author_email='fengleisemail@gmail.com',
     url='https://github.com/fengleicn/telegram_collector',
     description=u'收集电报群组的视频图片消息',
     packages=['telegram_collector'],
     install_requires=['telethon', 'python_socks'],
     entry_points={
```

### Comparing `telegram_collector-0.0.7/telegram_collector/__init__.py` & `telegram_collector-0.0.8/telegram_collector/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,14 +116,15 @@
         src_dialog_id = event.message.chat_id
         print('get: ', message)
         if message_is_video_or_photo(message) and src_dialog_id in self.src_dialog_ids:
             await self.__send_messages([message])
 
     # 流式汇总增量消息
     async def __send_current_message_src_to_dest(self):
+
         self.client.add_event_handler(self.callback, events.NewMessage(incoming=True))
         try:
             while True:
                 await asyncio.sleep(1)
         finally:
             await self.__terminate_client()
```

### Comparing `telegram_collector-0.0.7/telegram_collector/util.py` & `telegram_collector-0.0.8/telegram_collector/util.py`

 * *Files identical despite different names*

