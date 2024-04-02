# Comparing `tmp/miservice_fork-2.4.0.tar.gz` & `tmp/miservice_fork-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miservice_fork-2.4.0.tar", last modified: Fri Mar 29 07:20:03 2024, max compression
+gzip compressed data, was "miservice_fork-2.4.1.tar", last modified: Tue Apr  2 14:00:29 2024, max compression
```

## Comparing `miservice_fork-2.4.0.tar` & `miservice_fork-2.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-03-29 07:20:03.449387 miservice_fork-2.4.0/
--rw-r--r--   0 hyi        (502) staff       (20)     1067 2023-03-11 14:21:43.000000 miservice_fork-2.4.0/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)      529 2024-03-29 07:20:03.448517 miservice_fork-2.4.0/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     4476 2024-03-29 07:18:13.000000 miservice_fork-2.4.0/README.md
--rwxr-xr-x   0 hyi        (502) staff       (20)       96 2023-07-31 09:48:54.000000 miservice_fork-2.4.0/micli.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-03-29 07:20:03.437077 miservice_fork-2.4.0/miservice/
--rwxr-xr-x   0 hyi        (502) staff       (20)      178 2023-03-12 07:11:31.000000 miservice_fork-2.4.0/miservice/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       95 2023-03-11 14:21:43.000000 miservice_fork-2.4.0/miservice/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)     7559 2024-03-29 07:15:35.000000 miservice_fork-2.4.0/miservice/cli.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     5647 2023-10-23 08:06:30.000000 miservice_fork-2.4.0/miservice/miaccount.py
--rwxr-xr-x   0 hyi        (502) staff       (20)     3818 2024-01-07 08:08:03.000000 miservice_fork-2.4.0/miservice/miiocommand.py
--rwxr-xr-x   0 hyi        (502) staff       (20)    10620 2024-01-29 05:33:41.000000 miservice_fork-2.4.0/miservice/miioservice.py
--rw-r--r--   0 hyi        (502) staff       (20)     4251 2024-01-24 14:39:17.000000 miservice_fork-2.4.0/miservice/minaservice.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-03-29 07:20:03.447820 miservice_fork-2.4.0/miservice_fork.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)      529 2024-03-29 07:20:03.000000 miservice_fork-2.4.0/miservice_fork.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)      424 2024-03-29 07:20:03.000000 miservice_fork-2.4.0/miservice_fork.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2024-03-29 07:20:03.000000 miservice_fork-2.4.0/miservice_fork.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       46 2024-03-29 07:20:03.000000 miservice_fork-2.4.0/miservice_fork.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)       21 2024-03-29 07:20:03.000000 miservice_fork-2.4.0/miservice_fork.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)       10 2024-03-29 07:20:03.000000 miservice_fork-2.4.0/miservice_fork.egg-info/top_level.txt
--rw-r--r--   0 hyi        (502) staff       (20)       38 2024-03-29 07:20:03.449437 miservice_fork-2.4.0/setup.cfg
--rwxr-xr-x   0 hyi        (502) staff       (20)      919 2024-03-29 07:14:59.000000 miservice_fork-2.4.0/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-02 14:00:29.302715 miservice_fork-2.4.1/
+-rw-r--r--   0 hyi        (502) staff       (20)     1067 2023-03-11 14:21:43.000000 miservice_fork-2.4.1/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)      529 2024-04-02 14:00:29.302225 miservice_fork-2.4.1/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     4541 2024-04-02 13:57:51.000000 miservice_fork-2.4.1/README.md
+-rwxr-xr-x   0 hyi        (502) staff       (20)       96 2023-07-31 09:48:54.000000 miservice_fork-2.4.1/micli.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-02 14:00:29.290848 miservice_fork-2.4.1/miservice/
+-rwxr-xr-x   0 hyi        (502) staff       (20)      178 2023-03-12 07:11:31.000000 miservice_fork-2.4.1/miservice/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       95 2023-03-11 14:21:43.000000 miservice_fork-2.4.1/miservice/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)     7930 2024-04-02 14:00:08.000000 miservice_fork-2.4.1/miservice/cli.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)     5647 2023-10-23 08:06:30.000000 miservice_fork-2.4.1/miservice/miaccount.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)     3818 2024-01-07 08:08:03.000000 miservice_fork-2.4.1/miservice/miiocommand.py
+-rwxr-xr-x   0 hyi        (502) staff       (20)    10620 2024-01-29 05:33:41.000000 miservice_fork-2.4.1/miservice/miioservice.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4251 2024-01-24 14:39:17.000000 miservice_fork-2.4.1/miservice/minaservice.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-02 14:00:29.301142 miservice_fork-2.4.1/miservice_fork.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)      529 2024-04-02 14:00:29.000000 miservice_fork-2.4.1/miservice_fork.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)      424 2024-04-02 14:00:29.000000 miservice_fork-2.4.1/miservice_fork.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2024-04-02 14:00:29.000000 miservice_fork-2.4.1/miservice_fork.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       46 2024-04-02 14:00:29.000000 miservice_fork-2.4.1/miservice_fork.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       21 2024-04-02 14:00:29.000000 miservice_fork-2.4.1/miservice_fork.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       10 2024-04-02 14:00:29.000000 miservice_fork-2.4.1/miservice_fork.egg-info/top_level.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2024-04-02 14:00:29.302763 miservice_fork-2.4.1/setup.cfg
+-rwxr-xr-x   0 hyi        (502) staff       (20)      919 2024-04-02 14:00:19.000000 miservice_fork-2.4.1/setup.py
```

### Comparing `miservice_fork-2.4.0/LICENSE` & `miservice_fork-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.0/PKG-INFO` & `miservice_fork-2.4.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miservice_fork
-Version: 2.4.0
+Version: 2.4.1
 Summary: XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService
 Home-page: https://github.com/yihong0618/MiService
 Author: Yonsm, yihong0618
 Author-email: Yonsm@qq.com, zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `miservice_fork-2.4.0/README.md` & `miservice_fork-2.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,20 @@
 
 ## -> 播放 suno.ai trending
 
 ```
 micli suno 
 ```
 
+## -> 播放 suno.ai trending random
+
+```
+micli suno_random
+```
+
 ## Install
 ```
 pip3 install -U miservice_fork
 or 
 pip3 install .
 ```
```

### Comparing `miservice_fork-2.4.0/miservice/cli.py` & `miservice_fork-2.4.1/miservice/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from aiohttp import ClientSession
 import asyncio
 import logging
 import json
 import os
 import sys
 import tempfile
+import random
 from pathlib import Path
 
 import aiohttp
 from rich import print
 from mutagen.mp3 import MP3
 from miservice import (
     MiAccount,
@@ -110,38 +111,45 @@
             # TODO refactor this shit
             elif args.split(" ")[0].strip() in [
                 "play",
                 "pause",
                 "loop",
                 "play_list",
                 "suno",
-            ]:
+                "suno_random"
+                ]:
                 arg = args.split(" ")[0].strip()
                 result = await mina_service.device_list()
                 if not env.get("MI_DID"):
                     raise Exception("Please export MI_DID in your env")
                 device_id = find_device_id(result, env.get("MI_DID", ""))
                 # tricky add it to global
                 device_id_list.append(device_id)
                 args_list = args.split(" ")
                 if len(args_list) == 1:
                     if args_list[0] == "pause":
                         await mina_service.player_pause(device_id)
-                    elif args_list[0] == "suno":
+                    elif "suno" in args_list[0]:
                         song_dict = await get_suno_playlist()
-                        print("Will play suno trending list")
                         print(song_dict)
-                        for song_url, title in song_dict.items():
+                        song_urls = list(song_dict.keys())
+                        if args_list[0] == "suno_random":
+                            random.shuffle(song_urls)
+                            print("Will play suno trending list randomly")
+                        else:
+                            print("Will play suno trending list")
+                        for song_url in song_urls:
+                            title = song_dict[song_url]
                             print(f"Will play {song_url.strip()} title {title}")
                             await mina_service.play_by_url(device_id, song_url.strip())
                             duration = await _get_duration(song_url)
                             await asyncio.sleep(duration)
                         await mina_service.player_pause(device_id)
                     else:
-                        print("Please provice play url")
+                        print("Please provide a play URL")
                     return
                 # make device_id
                 if arg == "loop":
                     url = args_list[1]
                     await mina_service.play_by_url(device_id, url)
                     # set loop single mp3
                     await mina_service.player_set_loop(device_id, 0)
```

### Comparing `miservice_fork-2.4.0/miservice/miaccount.py` & `miservice_fork-2.4.1/miservice/miaccount.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.0/miservice/miiocommand.py` & `miservice_fork-2.4.1/miservice/miiocommand.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.0/miservice/miioservice.py` & `miservice_fork-2.4.1/miservice/miioservice.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.0/miservice/minaservice.py` & `miservice_fork-2.4.1/miservice/minaservice.py`

 * *Files identical despite different names*

### Comparing `miservice_fork-2.4.0/miservice_fork.egg-info/PKG-INFO` & `miservice_fork-2.4.1/miservice_fork.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miservice_fork
-Version: 2.4.0
+Version: 2.4.1
 Summary: XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService
 Home-page: https://github.com/yihong0618/MiService
 Author: Yonsm, yihong0618
 Author-email: Yonsm@qq.com, zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `miservice_fork-2.4.0/setup.py` & `miservice_fork-2.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 from setuptools import setup
 
 setup(
     name="miservice_fork",
     description="XiaoMi Cloud Service fork from https://github.com/Yonsm/MiService",
-    version="2.4.0",
+    version="2.4.1",
     license="MIT",
     author="Yonsm, yihong0618",
     author_email="Yonsm@qq.com, zouzou0208@gmail.com",
     url="https://github.com/yihong0618/MiService",
     packages=["miservice"],
     scripts=["micli.py"],
     python_requires=">=3.7",
```

