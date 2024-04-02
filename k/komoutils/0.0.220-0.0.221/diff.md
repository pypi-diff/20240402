# Comparing `tmp/komoutils-0.0.220.tar.gz` & `tmp/komoutils-0.0.221.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "komoutils-0.0.220.tar", max compression
+gzip compressed data, was "komoutils-0.0.221.tar", max compression
```

## Comparing `komoutils-0.0.220.tar` & `komoutils-0.0.221.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2024-02-22 16:30:36.997703 komoutils-0.0.220/README.md
--rw-r--r--   0        0        0      294 2024-02-23 05:43:36.448362 komoutils-0.0.220/komoutils/__init__.py
--rw-r--r--   0        0        0     1793 2024-04-02 05:04:28.069377 komoutils-0.0.220/komoutils/core/__init__.py
--rw-r--r--   0        0        0        1 2024-02-25 11:24:54.905290 komoutils-0.0.220/komoutils/core/base/__init__.py
--rw-r--r--   0        0        0      579 2024-02-25 11:24:54.909290 komoutils-0.0.220/komoutils/core/base/komo_base.py
--rw-r--r--   0        0        0      973 2024-01-07 07:39:27.992568 komoutils-0.0.220/komoutils/core/base/publish_queue.py
--rw-r--r--   0        0        0     2289 2024-02-22 16:53:53.243852 komoutils-0.0.220/komoutils/core/time/__init__.py
--rw-r--r--   0        0        0        0 2024-02-22 16:55:04.304573 komoutils-0.0.220/komoutils/db/__init__.py
--rw-r--r--   0        0        0     1996 2024-03-11 04:12:22.829593 komoutils-0.0.220/komoutils/db/mongodb_reader_writer.py
--rw-r--r--   0        0        0      577 2024-02-23 05:43:36.436362 komoutils-0.0.220/komoutils/logger/__init__.py
--rw-r--r--   0        0        0      743 2023-03-16 15:19:40.459000 komoutils-0.0.220/komoutils/logger/logger.py
--rw-r--r--   0        0        0     1254 2024-02-23 05:43:36.400362 komoutils-0.0.220/komoutils/logger/struct_logger.py
--rw-r--r--   0        0        0      380 2024-04-02 05:00:11.383586 komoutils-0.0.220/pyproject.toml
--rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 komoutils-0.0.220/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-22 16:30:36.997703 komoutils-0.0.221/README.md
+-rw-r--r--   0        0        0      294 2024-02-23 05:43:36.448362 komoutils-0.0.221/komoutils/__init__.py
+-rw-r--r--   0        0        0     1805 2024-04-02 06:03:17.149307 komoutils-0.0.221/komoutils/core/__init__.py
+-rw-r--r--   0        0        0        1 2024-02-25 11:24:54.905290 komoutils-0.0.221/komoutils/core/base/__init__.py
+-rw-r--r--   0        0        0      579 2024-02-25 11:24:54.909290 komoutils-0.0.221/komoutils/core/base/komo_base.py
+-rw-r--r--   0        0        0      973 2024-01-07 07:39:27.992568 komoutils-0.0.221/komoutils/core/base/publish_queue.py
+-rw-r--r--   0        0        0     2289 2024-02-22 16:53:53.243852 komoutils-0.0.221/komoutils/core/time/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-22 16:55:04.304573 komoutils-0.0.221/komoutils/db/__init__.py
+-rw-r--r--   0        0        0     1996 2024-03-11 04:12:22.829593 komoutils-0.0.221/komoutils/db/mongodb_reader_writer.py
+-rw-r--r--   0        0        0      577 2024-02-23 05:43:36.436362 komoutils-0.0.221/komoutils/logger/__init__.py
+-rw-r--r--   0        0        0      743 2023-03-16 15:19:40.459000 komoutils-0.0.221/komoutils/logger/logger.py
+-rw-r--r--   0        0        0     1254 2024-02-23 05:43:36.400362 komoutils-0.0.221/komoutils/logger/struct_logger.py
+-rw-r--r--   0        0        0      380 2024-04-02 06:03:27.253416 komoutils-0.0.221/pyproject.toml
+-rw-r--r--   0        0        0      586 1970-01-01 00:00:00.000000 komoutils-0.0.221/PKG-INFO
```

### Comparing `komoutils-0.0.220/komoutils/core/__init__.py` & `komoutils-0.0.221/komoutils/core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 class SubscribeRequest(BaseModel):
     type: str = ""
     topics: list = []
     heartbeat: bool = True
 
 
 class TradeRecord(BaseModel):
-    data: tuple = [float, float, float, float]  # price, amount, trade_ts, age
-    symbol: str = ""
+    data: tuple = [float, float, float, float, str]  # price, amount, trade_ts, age, symbol
+    topic: str = ""
     timestamp: str = ""
 
 
 async def safe_wrapper(c):
     try:
         return await c
     except asyncio.CancelledError:
```

### Comparing `komoutils-0.0.220/komoutils/core/base/komo_base.py` & `komoutils-0.0.221/komoutils/core/base/komo_base.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.220/komoutils/core/base/publish_queue.py` & `komoutils-0.0.221/komoutils/core/base/publish_queue.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.220/komoutils/core/time/__init__.py` & `komoutils-0.0.221/komoutils/core/time/__init__.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.220/komoutils/db/mongodb_reader_writer.py` & `komoutils-0.0.221/komoutils/db/mongodb_reader_writer.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.220/komoutils/logger/__init__.py` & `komoutils-0.0.221/komoutils/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.220/komoutils/logger/logger.py` & `komoutils-0.0.221/komoutils/logger/logger.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.220/komoutils/logger/struct_logger.py` & `komoutils-0.0.221/komoutils/logger/struct_logger.py`

 * *Files identical despite different names*

### Comparing `komoutils-0.0.220/PKG-INFO` & `komoutils-0.0.221/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: komoutils
-Version: 0.0.220
+Version: 0.0.221
 Summary: 
 Author: Makhosonke Morafo
 Author-email: makhosonke@komokun.org
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

