# Comparing `tmp/cheeseapi-0.4.6.tar.gz` & `tmp/cheeseapi-0.4.7.tar.gz`

## Comparing `cheeseapi-0.4.6.tar` & `cheeseapi-0.4.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/__init__.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/app.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/cors.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/exception.py
--rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/file.py
--rw-r--r--   0        0        0    30871 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/handle.py
--rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/protocol.py
--rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/request.py
--rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/response.py
--rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/route.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/server.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/signal.py
--rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/text.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/websocket.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/CheeseAPI/workspace.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/LICENSE
--rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/pyproject.toml
--rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 cheeseapi-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/__init__.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/app.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/cors.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/exception.py
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/file.py
+-rw-r--r--   0        0        0    30883 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/handle.py
+-rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/protocol.py
+-rw-r--r--   0        0        0     2753 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/request.py
+-rw-r--r--   0        0        0    14572 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/response.py
+-rw-r--r--   0        0        0     6814 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/route.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/server.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/signal.py
+-rw-r--r--   0        0        0     7664 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/text.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/websocket.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/CheeseAPI/workspace.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/LICENSE
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/README.md
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0     5024 2020-02-02 00:00:00.000000 cheeseapi-0.4.7/PKG-INFO
```

### Comparing `cheeseapi-0.4.6/CheeseAPI/app.py` & `cheeseapi-0.4.7/CheeseAPI/app.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.6/CheeseAPI/file.py` & `cheeseapi-0.4.7/CheeseAPI/file.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.6/CheeseAPI/handle.py` & `cheeseapi-0.4.7/CheeseAPI/handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,25 +441,25 @@
                 if self._app.signal.websocket_afterRequest.receivers:
                     await self._app.signal.websocket_afterRequest.send_async(**{
                         'request': protocol.request,
                         **protocol.kwargs
                     })
 
                 if e.args[0] == 0:
-                    self.websocket_404(protocol)
+                    await self.websocket_404(protocol)
                     if self._app.signal.websocket_404.receivers:
                         await self._app.signal.websocket_404.send_async(**{
                             'request': protocol.request,
                             'response': protocol.response,
                             **protocol.kwargs
                         })
                     return await self.websocket_response(protocol)
 
                 elif e.args[0] == 1:
-                    self.websocket_405(protocol)
+                    await self.websocket_405(protocol)
                     if self._app.signal.websocket_405.receivers:
                         await self._app.signal.websocket_405.send_async(**{
                             'request': protocol.request,
                             'response': protocol.response,
                             **protocol.kwargs
                         })
                     return await self.websocket_response(protocol)
```

### Comparing `cheeseapi-0.4.6/CheeseAPI/protocol.py` & `cheeseapi-0.4.7/CheeseAPI/protocol.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,28 @@
         self.response: 'BaseResponse' | None = None
         self.kwargs: Dict[str, Any] = {}
 
     def connection_made(self, transport: asyncio.Transport):
         self.transport = transport
 
     def data_received(self, data: bytes) -> None:
-        self.request = None
-        self.response = None
-        self.kwargs = {}
-
         try:
             self.parser.feed_data(data)
         except httptools.HttpParserUpgrade:
             self.request._upgrade()
 
             websocketProtocol = WebsocketProtocol(self)
             websocketProtocol.connection_made(self.transport)
             websocketProtocol.data_received(data)
             self.transport.set_protocol(websocketProtocol)
 
     def on_url(self, url: bytes):
         self.request = Request(http.HTTPMethod(self.parser.get_method().decode()), url.decode())
+        self.response = None
+        self.kwargs = {}
 
     def on_header(self, key: bytes, value: bytes):
         self.request.headers['-'.join([t.capitalize() for t in key.decode().split('-')])] = value.decode()
 
     def on_headers_complete(self):
         self.request.client = self.request.headers.get('X-Real-Ip', self.transport.get_extra_info('socket').getpeername()[0])
         self.request.origin = self.request.headers.get('Origin', f'{self.transport.get_extra_info("socket").getsockname()[0]}:{self.transport.get_extra_info("socket").getsockname()[1]}')
```

### Comparing `cheeseapi-0.4.6/CheeseAPI/request.py` & `cheeseapi-0.4.7/CheeseAPI/request.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.6/CheeseAPI/response.py` & `cheeseapi-0.4.7/CheeseAPI/response.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.6/CheeseAPI/route.py` & `cheeseapi-0.4.7/CheeseAPI/route.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.6/CheeseAPI/server.py` & `cheeseapi-0.4.7/CheeseAPI/server.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.6/CheeseAPI/signal.py` & `cheeseapi-0.4.7/CheeseAPI/signal.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.6/CheeseAPI/text.py` & `cheeseapi-0.4.7/CheeseAPI/text.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.6/CheeseAPI/websocket.py` & `cheeseapi-0.4.7/CheeseAPI/websocket.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.6/CheeseAPI/workspace.py` & `cheeseapi-0.4.7/CheeseAPI/workspace.py`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.6/LICENSE` & `cheeseapi-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.6/README.md` & `cheeseapi-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `cheeseapi-0.4.6/pyproject.toml` & `cheeseapi-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "CheeseAPI"
-version = "0.4.6"
+version = "0.4.7"
 description = "一款web协程框架。"
 readme = "README.md"
 license-files = { paths = [ "LICENSE" ] }
 authors = [
     { name = "Cheese Unknown", email = "cheese@cheese.ren" }
 ]
 keywords = [ 'API', 'BackEnd' ]
```

### Comparing `cheeseapi-0.4.6/PKG-INFO` & `cheeseapi-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: CheeseAPI
-Version: 0.4.6
+Version: 0.4.7
 Summary: 一款web协程框架。
 Project-URL: Source, https://github.com/CheeseUnknown/CheeseAPI
 Author-email: Cheese Unknown <cheese@cheese.ren>
 License-File: LICENSE
 Keywords: API,BackEnd
 Requires-Dist: blinker
 Requires-Dist: cheeselog
```

