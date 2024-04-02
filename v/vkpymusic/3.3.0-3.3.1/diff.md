# Comparing `tmp/vkpymusic-3.3.0.tar.gz` & `tmp/vkpymusic-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vkpymusic-3.3.0.tar", max compression
+gzip compressed data, was "vkpymusic-3.3.1.tar", max compression
```

## Comparing `vkpymusic-3.3.0.tar` & `vkpymusic-3.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1081 2024-01-15 17:40:08.000000 vkpymusic-3.3.0/LICENSE
--rw-r--r--   0        0        0      636 2024-01-21 21:19:32.000000 vkpymusic-3.3.0/pyproject.toml
--rw-r--r--   0        0        0     5430 2024-01-21 21:19:32.000000 vkpymusic-3.3.0/README.md
--rw-r--r--   0        0        0     1292 2024-01-08 23:02:36.000000 vkpymusic-3.3.0/vkpymusic/__init__.py
--rw-r--r--   0        0        0      972 2023-12-24 02:12:52.000000 vkpymusic-3.3.0/vkpymusic/client.py
--rw-r--r--   0        0        0      360 2024-01-21 21:19:32.000000 vkpymusic-3.3.0/vkpymusic/models/__init__.py
--rw-r--r--   0        0        0     2825 2024-01-21 18:12:06.000000 vkpymusic-3.3.0/vkpymusic/models/playlist.py
--rw-r--r--   0        0        0     2432 2024-01-21 21:19:32.000000 vkpymusic-3.3.0/vkpymusic/models/song.py
--rw-r--r--   0        0        0     1806 2024-01-21 21:19:32.000000 vkpymusic-3.3.0/vkpymusic/models/userinfo.py
--rw-r--r--   0        0        0    17442 2024-01-21 21:19:32.000000 vkpymusic-3.3.0/vkpymusic/service.py
--rw-r--r--   0        0        0    17747 2024-01-21 21:19:32.000000 vkpymusic-3.3.0/vkpymusic/service_async.py
--rw-r--r--   0        0        0     9981 2024-01-21 21:19:32.000000 vkpymusic-3.3.0/vkpymusic/token_receiver.py
--rw-r--r--   0        0        0     8827 2024-01-21 21:19:32.000000 vkpymusic-3.3.0/vkpymusic/token_receiver_async.py
--rw-r--r--   0        0        0      322 2024-01-21 18:45:52.000000 vkpymusic-3.3.0/vkpymusic/utils/__init__.py
--rw-r--r--   0        0        0     2258 2024-01-21 21:19:32.000000 vkpymusic-3.3.0/vkpymusic/utils/converter.py
--rw-r--r--   0        0        0     1912 2023-12-24 02:12:52.000000 vkpymusic-3.3.0/vkpymusic/utils/logger.py
--rw-r--r--   0        0        0     6325 1970-01-01 00:00:00.000000 vkpymusic-3.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-01-15 17:40:08.000000 vkpymusic-3.3.1/LICENSE
+-rw-r--r--   0        0        0      636 2024-04-02 14:51:54.000000 vkpymusic-3.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5430 2024-04-02 14:51:54.000000 vkpymusic-3.3.1/README.md
+-rw-r--r--   0        0        0     1292 2024-04-02 14:51:54.000000 vkpymusic-3.3.1/vkpymusic/__init__.py
+-rw-r--r--   0        0        0      972 2023-12-24 02:12:52.000000 vkpymusic-3.3.1/vkpymusic/client.py
+-rw-r--r--   0        0        0      360 2024-01-21 21:19:32.000000 vkpymusic-3.3.1/vkpymusic/models/__init__.py
+-rw-r--r--   0        0        0     2825 2024-01-21 18:12:06.000000 vkpymusic-3.3.1/vkpymusic/models/playlist.py
+-rw-r--r--   0        0        0     2432 2024-01-21 21:19:32.000000 vkpymusic-3.3.1/vkpymusic/models/song.py
+-rw-r--r--   0        0        0     1806 2024-01-21 21:19:32.000000 vkpymusic-3.3.1/vkpymusic/models/userinfo.py
+-rw-r--r--   0        0        0    17442 2024-01-21 21:19:32.000000 vkpymusic-3.3.1/vkpymusic/service.py
+-rw-r--r--   0        0        0    17747 2024-01-21 21:19:32.000000 vkpymusic-3.3.1/vkpymusic/service_async.py
+-rw-r--r--   0        0        0     9981 2024-01-21 21:19:32.000000 vkpymusic-3.3.1/vkpymusic/token_receiver.py
+-rw-r--r--   0        0        0     8827 2024-01-21 21:19:32.000000 vkpymusic-3.3.1/vkpymusic/token_receiver_async.py
+-rw-r--r--   0        0        0      322 2024-01-21 18:45:52.000000 vkpymusic-3.3.1/vkpymusic/utils/__init__.py
+-rw-r--r--   0        0        0     2258 2024-01-21 21:19:32.000000 vkpymusic-3.3.1/vkpymusic/utils/converter.py
+-rw-r--r--   0        0        0     1967 2024-04-02 14:20:32.000000 vkpymusic-3.3.1/vkpymusic/utils/logger.py
+-rw-r--r--   0        0        0     6325 1970-01-01 00:00:00.000000 vkpymusic-3.3.1/PKG-INFO
```

### Comparing `vkpymusic-3.3.0/LICENSE` & `vkpymusic-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vkpymusic-3.3.0/pyproject.toml` & `vkpymusic-3.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vkpymusic"
-version = "3.3.0"
+version = "3.3.1"
 homepage = "https://github.com/issamansur/vkpymusic"
 repository = "https://github.com/issamansur/vkpymusic"
 description = "Python library for VK Audio (API)"
 keywords = ["vk", "api", "music", "downloader", "python"]
 authors = ["Issa Mansur (EDEXADE) <issa_mansur@mail.ru>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `vkpymusic-3.3.0/README.md` & `vkpymusic-3.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![Лицензия](https://img.shields.io/badge/Лицензия-MIT-blue)
 ![Совместимость с Python](https://img.shields.io/badge/Python-3.7--3.9-blue)
-![Версия библиотеки](https://img.shields.io/badge/pip-3.3.0-blue)
+![Версия библиотеки](https://img.shields.io/badge/pip-3.3.1-blue)
 
 # VKpyMusic 
 ### is a Python library that provides a simple interface for interacting with the VKontakte (VK) music service API. The library allows developers to easily perform operations related to music and other functionalities available through the VK API.
 ### это библиотека Python, которая предоставляет простой интерфейс для взаимодействия с API музыкального сервиса ВКонтакте (VK). Библиотека позволяет разработчикам легко выполнять операции, связанные с музыкой и другими функциональными возможностями, доступными через VK API.
 
 # Installation
 ### You can install VKpyMusic using the pip package manager. Open your command prompt or terminal and execute the following command:
```

### Comparing `vkpymusic-3.3.0/vkpymusic/__init__.py` & `vkpymusic-3.3.1/vkpymusic/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     utils: A module that contains utilities for conversion and logging.
 """
 
 __title__ = "vkpymusic"
 __author__ = "issamansur"
 __license__ = "MIT"
 __copyright__ = "Copyright 2023-present issamansur (EDEXADE, inc)"
-__version__ = "3.0.1"
+__version__ = "3.3.1"
 
 from .client import Client, clients
 from .token_receiver import TokenReceiver
 from .token_receiver_async import TokenReceiverAsync
 from .service import Service
 from .service_async import ServiceAsync
```

### Comparing `vkpymusic-3.3.0/vkpymusic/client.py` & `vkpymusic-3.3.1/vkpymusic/client.py`

 * *Files identical despite different names*

### Comparing `vkpymusic-3.3.0/vkpymusic/models/playlist.py` & `vkpymusic-3.3.1/vkpymusic/models/playlist.py`

 * *Files identical despite different names*

### Comparing `vkpymusic-3.3.0/vkpymusic/models/song.py` & `vkpymusic-3.3.1/vkpymusic/models/song.py`

 * *Files identical despite different names*

### Comparing `vkpymusic-3.3.0/vkpymusic/models/userinfo.py` & `vkpymusic-3.3.1/vkpymusic/models/userinfo.py`

 * *Files identical despite different names*

### Comparing `vkpymusic-3.3.0/vkpymusic/service.py` & `vkpymusic-3.3.1/vkpymusic/service.py`

 * *Files identical despite different names*

### Comparing `vkpymusic-3.3.0/vkpymusic/service_async.py` & `vkpymusic-3.3.1/vkpymusic/service_async.py`

 * *Files identical despite different names*

### Comparing `vkpymusic-3.3.0/vkpymusic/token_receiver.py` & `vkpymusic-3.3.1/vkpymusic/token_receiver.py`

 * *Files identical despite different names*

### Comparing `vkpymusic-3.3.0/vkpymusic/token_receiver_async.py` & `vkpymusic-3.3.1/vkpymusic/token_receiver_async.py`

 * *Files identical despite different names*

### Comparing `vkpymusic-3.3.0/vkpymusic/utils/converter.py` & `vkpymusic-3.3.1/vkpymusic/utils/converter.py`

 * *Files identical despite different names*

### Comparing `vkpymusic-3.3.0/vkpymusic/utils/logger.py` & `vkpymusic-3.3.1/vkpymusic/utils/logger.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,22 +50,23 @@
     """
     stream_handler = logging.StreamHandler()
     stream_handler.setLevel(logging.INFO)
     stream_handler.setFormatter(logging.Formatter(_log_format))
     return stream_handler
 
 
-def get_logger(name: str) -> logging.Logger:
+def get_logger(name: str, console_debug: bool = False) -> logging.Logger:
     """
     Returns a logger instance with configured handlers.
 
     Args:
         name (str): The name of the logger.
 
     Returns:
         logger (logging.Logger): A logger instance with configured handlers.
     """
     logger = logging.getLogger(name)
     logger.setLevel(logging.INFO)
     logger.addHandler(_get_file_handler())
-    logger.addHandler(_get_stream_handler())
+    if console_debug:
+        logger.addHandler(_get_stream_handler())
     return logger
```

### Comparing `vkpymusic-3.3.0/PKG-INFO` & `vkpymusic-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vkpymusic
-Version: 3.3.0
+Version: 3.3.1
 Summary: Python library for VK Audio (API)
 Home-page: https://github.com/issamansur/vkpymusic
 License: MIT
 Keywords: vk,api,music,downloader,python
 Author: Issa Mansur (EDEXADE)
 Author-email: issa_mansur@mail.ru
 Requires-Python: >=3.7,<3.12
@@ -20,15 +20,15 @@
 Requires-Dist: httpx (>=0.24)
 Requires-Dist: requests (>=2.31)
 Project-URL: Repository, https://github.com/issamansur/vkpymusic
 Description-Content-Type: text/markdown
 
 ![Лицензия](https://img.shields.io/badge/Лицензия-MIT-blue)
 ![Совместимость с Python](https://img.shields.io/badge/Python-3.7--3.9-blue)
-![Версия библиотеки](https://img.shields.io/badge/pip-3.3.0-blue)
+![Версия библиотеки](https://img.shields.io/badge/pip-3.3.1-blue)
 
 # VKpyMusic 
 ### is a Python library that provides a simple interface for interacting with the VKontakte (VK) music service API. The library allows developers to easily perform operations related to music and other functionalities available through the VK API.
 ### это библиотека Python, которая предоставляет простой интерфейс для взаимодействия с API музыкального сервиса ВКонтакте (VK). Библиотека позволяет разработчикам легко выполнять операции, связанные с музыкой и другими функциональными возможностями, доступными через VK API.
 
 # Installation
 ### You can install VKpyMusic using the pip package manager. Open your command prompt or terminal and execute the following command:
```

