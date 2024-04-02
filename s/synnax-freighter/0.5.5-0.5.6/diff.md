# Comparing `tmp/synnax_freighter-0.5.5.tar.gz` & `tmp/synnax_freighter-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synnax_freighter-0.5.5.tar", max compression
+gzip compressed data, was "synnax_freighter-0.5.6.tar", max compression
```

## Comparing `synnax_freighter-0.5.5.tar` & `synnax_freighter-0.5.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1233 2023-10-31 15:49:45.975596 synnax_freighter-0.5.5/freighter/__init__.py
--rw-r--r--   0        0        0     2101 2023-10-31 15:49:45.976004 synnax_freighter-0.5.5/freighter/alamos.py
--rw-r--r--   0        0        0     1521 2023-10-31 15:49:45.976289 synnax_freighter-0.5.5/freighter/context.py
--rw-r--r--   0        0        0     2652 2023-10-31 15:49:45.976569 synnax_freighter-0.5.5/freighter/encoder.py
--rw-r--r--   0        0        0     4170 2024-03-10 00:38:28.327850 synnax_freighter-0.5.5/freighter/exceptions.py
--rw-r--r--   0        0        0     4130 2023-10-31 15:49:45.976879 synnax_freighter-0.5.5/freighter/http.py
--rw-r--r--   0        0        0     6923 2023-10-31 15:49:45.977182 synnax_freighter-0.5.5/freighter/stream.py
--rw-r--r--   0        0        0     8026 2024-03-10 00:38:28.328180 synnax_freighter-0.5.5/freighter/sync.py
--rw-r--r--   0        0        0     4649 2023-10-31 15:49:45.978088 synnax_freighter-0.5.5/freighter/transport.py
--rw-r--r--   0        0        0     2048 2023-10-31 15:49:45.978371 synnax_freighter-0.5.5/freighter/unary.py
--rw-r--r--   0        0        0     2143 2023-10-11 16:45:00.246234 synnax_freighter-0.5.5/freighter/url.py
--rw-r--r--   0        0        0      694 2023-10-11 16:45:00.246255 synnax_freighter-0.5.5/freighter/util/__init__.py
--rw-r--r--   0        0        0     1005 2023-10-11 16:45:00.246271 synnax_freighter-0.5.5/freighter/util/asyncio.py
--rw-r--r--   0        0        0      969 2023-10-11 16:45:00.246481 synnax_freighter-0.5.5/freighter/util/threading.py
--rw-r--r--   0        0        0     6349 2024-03-09 17:29:59.302832 synnax_freighter-0.5.5/freighter/websocket.py
--rw-r--r--   0        0        0      844 2024-03-10 01:21:20.024922 synnax_freighter-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 synnax_freighter-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0     1233 2023-10-31 15:49:45.975596 synnax_freighter-0.5.6/freighter/__init__.py
+-rw-r--r--   0        0        0     2101 2023-10-31 15:49:45.976004 synnax_freighter-0.5.6/freighter/alamos.py
+-rw-r--r--   0        0        0     1521 2023-10-31 15:49:45.976289 synnax_freighter-0.5.6/freighter/context.py
+-rw-r--r--   0        0        0     2652 2023-10-31 15:49:45.976569 synnax_freighter-0.5.6/freighter/encoder.py
+-rw-r--r--   0        0        0     4170 2024-03-10 00:38:28.327850 synnax_freighter-0.5.6/freighter/exceptions.py
+-rw-r--r--   0        0        0     4130 2023-10-31 15:49:45.976879 synnax_freighter-0.5.6/freighter/http.py
+-rw-r--r--   0        0        0     6923 2023-10-31 15:49:45.977182 synnax_freighter-0.5.6/freighter/stream.py
+-rw-r--r--   0        0        0     8026 2024-03-10 00:38:28.328180 synnax_freighter-0.5.6/freighter/sync.py
+-rw-r--r--   0        0        0     4649 2023-10-31 15:49:45.978088 synnax_freighter-0.5.6/freighter/transport.py
+-rw-r--r--   0        0        0     2048 2023-10-31 15:49:45.978371 synnax_freighter-0.5.6/freighter/unary.py
+-rw-r--r--   0        0        0     2143 2023-10-11 16:45:00.246234 synnax_freighter-0.5.6/freighter/url.py
+-rw-r--r--   0        0        0      694 2023-10-11 16:45:00.246255 synnax_freighter-0.5.6/freighter/util/__init__.py
+-rw-r--r--   0        0        0     1005 2023-10-11 16:45:00.246271 synnax_freighter-0.5.6/freighter/util/asyncio.py
+-rw-r--r--   0        0        0      969 2023-10-11 16:45:00.246481 synnax_freighter-0.5.6/freighter/util/threading.py
+-rw-r--r--   0        0        0     6349 2024-03-09 17:29:59.302832 synnax_freighter-0.5.6/freighter/websocket.py
+-rw-r--r--   0        0        0      844 2024-03-10 01:21:49.844252 synnax_freighter-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      552 1970-01-01 00:00:00.000000 synnax_freighter-0.5.6/PKG-INFO
```

### Comparing `synnax_freighter-0.5.5/freighter/__init__.py` & `synnax_freighter-0.5.6/freighter/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/alamos.py` & `synnax_freighter-0.5.6/freighter/alamos.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/context.py` & `synnax_freighter-0.5.6/freighter/context.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/encoder.py` & `synnax_freighter-0.5.6/freighter/encoder.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/exceptions.py` & `synnax_freighter-0.5.6/freighter/exceptions.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/http.py` & `synnax_freighter-0.5.6/freighter/http.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/stream.py` & `synnax_freighter-0.5.6/freighter/stream.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/sync.py` & `synnax_freighter-0.5.6/freighter/sync.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/transport.py` & `synnax_freighter-0.5.6/freighter/transport.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/unary.py` & `synnax_freighter-0.5.6/freighter/unary.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/url.py` & `synnax_freighter-0.5.6/freighter/url.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/util/__init__.py` & `synnax_freighter-0.5.6/freighter/util/__init__.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/util/asyncio.py` & `synnax_freighter-0.5.6/freighter/util/asyncio.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/util/threading.py` & `synnax_freighter-0.5.6/freighter/util/threading.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/freighter/websocket.py` & `synnax_freighter-0.5.6/freighter/websocket.py`

 * *Files identical despite different names*

### Comparing `synnax_freighter-0.5.5/pyproject.toml` & `synnax_freighter-0.5.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "synnax-freighter"
-version = "0.5.5"
+version = "0.5.6"
 description = ""
 authors = ["emiliano bonilla <emilbon99@gmail.com>"]
 packages = [
     { include = "freighter/**/*.py" }
 ]
 
 [tool.mypy]
@@ -17,15 +17,15 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 websockets = "^11.0.3"
 msgpack = "^1.0.4"
 urllib3 = "^2.0.3"
 janus = "^1.0.0"
 pydantic = "^1.10.0"
-alamos = "^0.2.4"
+alamos = "^0.2.5"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 pytest = "^7.3.2"
 pytest-asyncio = "^0.21.0"
 mypy = "^1.3.0"
 pytest-cov = "^4.1.0"
```

### Comparing `synnax_freighter-0.5.5/PKG-INFO` & `synnax_freighter-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: synnax-freighter
-Version: 0.5.5
+Version: 0.5.6
 Summary: 
 Author: emiliano bonilla
 Author-email: emilbon99@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: alamos (>=0.2.4,<0.3.0)
+Requires-Dist: alamos (>=0.2.5,<0.3.0)
 Requires-Dist: janus (>=1.0.0,<2.0.0)
 Requires-Dist: msgpack (>=1.0.4,<2.0.0)
 Requires-Dist: pydantic (>=1.10.0,<2.0.0)
 Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
```

