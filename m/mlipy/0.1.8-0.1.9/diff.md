# Comparing `tmp/mlipy-0.1.8.tar.gz` & `tmp/mlipy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlipy-0.1.8.tar", max compression
+gzip compressed data, was "mlipy-0.1.9.tar", max compression
```

## Comparing `mlipy-0.1.8.tar` & `mlipy-0.1.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-11-15 19:16:24.084400 mlipy-0.1.8/LICENSE
--rw-r--r--   0        0        0     5012 2023-11-26 16:10:37.765074 mlipy-0.1.8/README.md
--rw-r--r--   0        0        0      175 2023-11-26 12:40:33.538687 mlipy-0.1.8/mli/__init__.py
--rw-r--r--   0        0        0    10023 2023-11-26 17:31:47.331931 mlipy-0.1.8/mli/client.py
--rw-r--r--   0        0        0     1617 2023-11-26 13:42:16.968835 mlipy-0.1.8/mli/params.py
--rw-r--r--   0        0        0    22068 2023-11-26 17:35:04.619397 mlipy-0.1.8/mli/server.py
--rw-r--r--   0        0        0      568 2023-11-26 17:35:51.170373 mlipy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5739 1970-01-01 00:00:00.000000 mlipy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-11-15 19:16:24.084400 mlipy-0.1.9/LICENSE
+-rw-r--r--   0        0        0     5012 2023-11-26 16:10:37.765074 mlipy-0.1.9/README.md
+-rw-r--r--   0        0        0      175 2023-11-26 12:40:33.538687 mlipy-0.1.9/mli/__init__.py
+-rw-r--r--   0        0        0    10095 2023-11-26 17:55:45.915381 mlipy-0.1.9/mli/client.py
+-rw-r--r--   0        0        0     1617 2023-11-26 13:42:16.968835 mlipy-0.1.9/mli/params.py
+-rw-r--r--   0        0        0    22068 2023-11-26 17:35:04.619397 mlipy-0.1.9/mli/server.py
+-rw-r--r--   0        0        0      568 2023-11-26 17:58:56.492747 mlipy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5739 1970-01-01 00:00:00.000000 mlipy-0.1.9/PKG-INFO
```

### Comparing `mlipy-0.1.8/LICENSE` & `mlipy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mlipy-0.1.8/README.md` & `mlipy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mlipy-0.1.8/mli/client.py` & `mlipy-0.1.9/mli/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,35 +122,35 @@
 
 
 class AsyncMLIClient(BaseMLIClient):
     async def text(self, **kwargs: Unpack[LLMParams]) -> str:
         url: str = f'{self.endpoint}/text/completions'
 
         async with ClientSession() as session:
-            async with session.post(url, json=kwargs) as resp:
+            async with session.post(url, json=kwargs, verify_ssl=False) as resp:
                 data = await resp.json()
 
         return data
 
 
     async def chat(self, **kwargs: Unpack[LLMParams]) -> str:
         url: str = f'{self.endpoint}/chat/completions'
 
         async with ClientSession() as session:
-            async with session.post(url, json=kwargs) as resp:
+            async with session.post(url, json=kwargs, verify_ssl=False) as resp:
                 data = await resp.json()
 
         return data
 
 
     async def iter_text(self, **kwargs: Unpack[LLMParams]) -> AsyncIterator[str]:
         url: str = f'{self.ws_endpoint}/text/completions'
         
         async with ClientSession() as session:
-            async with session.ws_connect(url) as ws:
+            async with session.ws_connect(url, verify_ssl=False) as ws:
                 await ws.send_json(kwargs)
 
                 async for msg in ws:
                     if msg.type == WSMsgType.PING:
                         await ws.pong(msg.data)
                     elif msg.type == WSMsgType.TEXT:
                         data = json.loads(msg.data)
@@ -160,15 +160,15 @@
                         break
 
 
     async def iter_chat(self, **kwargs: Unpack[LLMParams]) -> AsyncIterator[str]:
         url: str = f'{self.ws_endpoint}/chat/completions'
         
         async with ClientSession() as session:
-            async with session.ws_connect(url) as ws:
+            async with session.ws_connect(url, verify_ssl=False) as ws:
                 await ws.send_json(kwargs)
 
                 async for msg in ws:
                     if msg.type == WSMsgType.PING:
                         await ws.pong(msg.data)
                     elif msg.type == WSMsgType.TEXT:
                         data = json.loads(msg.data)
```

### Comparing `mlipy-0.1.8/mli/params.py` & `mlipy-0.1.9/mli/params.py`

 * *Files identical despite different names*

### Comparing `mlipy-0.1.8/mli/server.py` & `mlipy-0.1.9/mli/server.py`

 * *Files identical despite different names*

### Comparing `mlipy-0.1.8/pyproject.toml` & `mlipy-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlipy"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python-based Machine Learning Interface"
 homepage = "https://github.com/mtasic85/mlipy"
 repository = "https://github.com/mtasic85/mlipy"
 authors = ["Marko Tasic <mtasic85@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "mli"}]
```

### Comparing `mlipy-0.1.8/PKG-INFO` & `mlipy-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlipy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python-based Machine Learning Interface
 Home-page: https://github.com/mtasic85/mlipy
 License: MIT
 Author: Marko Tasic
 Author-email: mtasic85@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

