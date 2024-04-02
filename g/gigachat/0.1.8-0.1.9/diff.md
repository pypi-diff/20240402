# Comparing `tmp/gigachat-0.1.8.tar.gz` & `tmp/gigachat-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gigachat-0.1.8.tar", max compression
+gzip compressed data, was "gigachat-0.1.9.tar", max compression
```

## Comparing `gigachat-0.1.8.tar` & `gigachat-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1067 2023-10-23 08:52:02.844741 gigachat-0.1.8/LICENSE
--rw-r--r--   0        0        0     4779 2023-11-01 09:43:49.393627 gigachat-0.1.8/README.md
--rw-r--r--   0        0        0     1538 2023-11-07 13:44:44.710937 gigachat-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      135 2023-10-23 08:52:02.847056 gigachat-0.1.8/src/gigachat/__init__.py
--rw-r--r--   0        0        0        0 2023-10-23 08:52:02.847213 gigachat-0.1.8/src/gigachat/api/__init__.py
--rw-r--r--   0        0        0     2157 2023-11-01 09:43:49.398381 gigachat-0.1.8/src/gigachat/api/get_model.py
--rw-r--r--   0        0        0     2109 2023-11-01 09:43:49.399438 gigachat-0.1.8/src/gigachat/api/get_models.py
--rw-r--r--   0        0        0     1438 2023-11-01 09:43:49.400786 gigachat-0.1.8/src/gigachat/api/post_auth.py
--rw-r--r--   0        0        0     2076 2023-11-01 09:43:49.402001 gigachat-0.1.8/src/gigachat/api/post_chat.py
--rw-r--r--   0        0        0     1672 2023-11-01 09:43:49.402921 gigachat-0.1.8/src/gigachat/api/post_token.py
--rw-r--r--   0        0        0     3027 2023-11-01 09:43:49.403970 gigachat-0.1.8/src/gigachat/api/stream_chat.py
--rw-r--r--   0        0        0    11282 2023-11-01 09:43:49.405113 gigachat-0.1.8/src/gigachat/client.py
--rw-r--r--   0        0        0      424 2023-11-01 09:43:49.406056 gigachat-0.1.8/src/gigachat/context.py
--rw-r--r--   0        0        0      146 2023-10-23 08:52:02.850081 gigachat-0.1.8/src/gigachat/exceptions.py
--rw-r--r--   0        0        0      879 2023-10-23 08:52:02.850360 gigachat-0.1.8/src/gigachat/models/__init__.py
--rw-r--r--   0        0        0      315 2023-10-23 08:52:02.850555 gigachat-0.1.8/src/gigachat/models/access_token.py
--rw-r--r--   0        0        0     1504 2023-11-01 09:43:49.407052 gigachat-0.1.8/src/gigachat/models/chat.py
--rw-r--r--   0        0        0      701 2023-10-23 08:52:02.850974 gigachat-0.1.8/src/gigachat/models/chat_completion.py
--rw-r--r--   0        0        0      629 2023-10-23 08:52:02.851216 gigachat-0.1.8/src/gigachat/models/chat_completion_chunk.py
--rw-r--r--   0        0        0      468 2023-10-23 08:52:02.851390 gigachat-0.1.8/src/gigachat/models/choices.py
--rw-r--r--   0        0        0      489 2023-10-23 08:52:02.851557 gigachat-0.1.8/src/gigachat/models/choices_chunk.py
--rw-r--r--   0        0        0      338 2023-10-23 08:52:02.851715 gigachat-0.1.8/src/gigachat/models/messages.py
--rw-r--r--   0        0        0      181 2023-10-23 08:52:02.851877 gigachat-0.1.8/src/gigachat/models/messages_chunk.py
--rw-r--r--   0        0        0      175 2023-10-23 08:52:02.852029 gigachat-0.1.8/src/gigachat/models/messages_role.py
--rw-r--r--   0        0        0      371 2023-10-23 08:52:02.852178 gigachat-0.1.8/src/gigachat/models/model.py
--rw-r--r--   0        0        0      422 2023-10-23 08:52:02.852409 gigachat-0.1.8/src/gigachat/models/models.py
--rw-r--r--   0        0        0      293 2023-10-23 08:52:02.852686 gigachat-0.1.8/src/gigachat/models/token.py
--rw-r--r--   0        0        0      447 2023-10-23 08:52:02.853259 gigachat-0.1.8/src/gigachat/models/usage.py
--rw-r--r--   0        0        0        0 2023-10-26 13:59:08.940960 gigachat-0.1.8/src/gigachat/py.typed
--rw-r--r--   0        0        0      897 2023-10-23 08:52:02.854107 gigachat-0.1.8/src/gigachat/pydantic_v1/__init__.py
--rw-r--r--   0        0        0      134 2023-10-23 08:52:02.854600 gigachat-0.1.8/src/gigachat/pydantic_v1/dataclasses.py
--rw-r--r--   0        0        0      120 2023-10-23 08:52:02.854879 gigachat-0.1.8/src/gigachat/pydantic_v1/main.py
--rw-r--r--   0        0        0      936 2023-10-27 06:23:48.335598 gigachat-0.1.8/src/gigachat/settings.py
--rw-r--r--   0        0        0     5513 1970-01-01 00:00:00.000000 gigachat-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-09-25 12:23:58.359238 gigachat-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4779 2023-12-01 11:48:41.249030 gigachat-0.1.9/README.md
+-rw-r--r--   0        0        0     1536 2023-12-07 08:58:40.936271 gigachat-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      135 2023-09-26 09:45:19.754655 gigachat-0.1.9/src/gigachat/__init__.py
+-rw-r--r--   0        0        0        0 2023-09-26 09:45:19.754840 gigachat-0.1.9/src/gigachat/api/__init__.py
+-rw-r--r--   0        0        0     2438 2023-12-06 08:14:59.760841 gigachat-0.1.9/src/gigachat/api/get_model.py
+-rw-r--r--   0        0        0     2390 2023-12-06 07:54:47.554181 gigachat-0.1.9/src/gigachat/api/get_models.py
+-rw-r--r--   0        0        0     1438 2023-12-01 11:48:41.275789 gigachat-0.1.9/src/gigachat/api/post_auth.py
+-rw-r--r--   0        0        0     2357 2023-12-06 08:16:22.247590 gigachat-0.1.9/src/gigachat/api/post_chat.py
+-rw-r--r--   0        0        0     1924 2023-12-06 07:54:47.551839 gigachat-0.1.9/src/gigachat/api/post_token.py
+-rw-r--r--   0        0        0     3308 2023-12-06 08:14:59.761238 gigachat-0.1.9/src/gigachat/api/stream_chat.py
+-rw-r--r--   0        0        0    11282 2023-12-01 11:48:41.282640 gigachat-0.1.9/src/gigachat/client.py
+-rw-r--r--   0        0        0      606 2023-12-06 07:46:16.132357 gigachat-0.1.9/src/gigachat/context.py
+-rw-r--r--   0        0        0      146 2023-09-26 09:45:19.758413 gigachat-0.1.9/src/gigachat/exceptions.py
+-rw-r--r--   0        0        0      879 2023-12-01 11:48:38.453798 gigachat-0.1.9/src/gigachat/models/__init__.py
+-rw-r--r--   0        0        0      315 2023-12-01 11:48:38.456346 gigachat-0.1.9/src/gigachat/models/access_token.py
+-rw-r--r--   0        0        0     1504 2023-12-01 11:48:41.285379 gigachat-0.1.9/src/gigachat/models/chat.py
+-rw-r--r--   0        0        0      701 2023-12-01 11:48:38.459340 gigachat-0.1.9/src/gigachat/models/chat_completion.py
+-rw-r--r--   0        0        0      629 2023-12-01 11:48:38.460913 gigachat-0.1.9/src/gigachat/models/chat_completion_chunk.py
+-rw-r--r--   0        0        0      468 2023-12-01 11:48:38.462572 gigachat-0.1.9/src/gigachat/models/choices.py
+-rw-r--r--   0        0        0      489 2023-12-01 11:48:38.464121 gigachat-0.1.9/src/gigachat/models/choices_chunk.py
+-rw-r--r--   0        0        0      338 2023-12-01 11:48:38.465744 gigachat-0.1.9/src/gigachat/models/messages.py
+-rw-r--r--   0        0        0      181 2023-12-01 11:48:38.467902 gigachat-0.1.9/src/gigachat/models/messages_chunk.py
+-rw-r--r--   0        0        0      175 2023-12-01 11:48:38.469563 gigachat-0.1.9/src/gigachat/models/messages_role.py
+-rw-r--r--   0        0        0      371 2023-12-01 11:48:38.471168 gigachat-0.1.9/src/gigachat/models/model.py
+-rw-r--r--   0        0        0      422 2023-12-01 11:48:38.472916 gigachat-0.1.9/src/gigachat/models/models.py
+-rw-r--r--   0        0        0      293 2023-12-01 11:48:38.474674 gigachat-0.1.9/src/gigachat/models/token.py
+-rw-r--r--   0        0        0      447 2023-12-01 11:48:38.476757 gigachat-0.1.9/src/gigachat/models/usage.py
+-rw-r--r--   0        0        0        0 2023-12-01 11:48:41.285507 gigachat-0.1.9/src/gigachat/py.typed
+-rw-r--r--   0        0        0      897 2023-12-06 08:24:35.368439 gigachat-0.1.9/src/gigachat/pydantic_v1/__init__.py
+-rw-r--r--   0        0        0      134 2023-09-26 09:45:19.765764 gigachat-0.1.9/src/gigachat/pydantic_v1/dataclasses.py
+-rw-r--r--   0        0        0      120 2023-09-26 09:45:19.766221 gigachat-0.1.9/src/gigachat/pydantic_v1/main.py
+-rw-r--r--   0        0        0      936 2023-12-01 11:48:41.287628 gigachat-0.1.9/src/gigachat/settings.py
+-rw-r--r--   0        0        0     5562 1970-01-01 00:00:00.000000 gigachat-0.1.9/PKG-INFO
```

### Comparing `gigachat-0.1.8/LICENSE` & `gigachat-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gigachat-0.1.8/README.md` & `gigachat-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gigachat-0.1.8/pyproject.toml` & `gigachat-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "gigachat"
-version = "0.1.8"
-description = "GigaChat. Python-библиотека для GigaChain"
+version = "0.1.9"
+description = "GigaChat. Python-library for GigaChain and LangChain"
 authors = ["Konstantin Krestnikov <rai220@gmail.com>", "Sergey Malyshev <in1t@ya.ru>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ai-forever/gigachat"
 packages = [{include = "gigachat", from = "src"}]
 
 [tool.poetry.dependencies]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `gigachat-0.1.8/src/gigachat/api/get_model.py` & `gigachat-0.1.9/src/gigachat/api/get_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
-from gigachat.context import authorization_cvar, client_id_cvar, request_id_cvar, session_id_cvar
+from gigachat.context import (
+    authorization_cvar,
+    client_id_cvar,
+    operation_id_cvar,
+    request_id_cvar,
+    service_id_cvar,
+    session_id_cvar,
+)
 from gigachat.exceptions import AuthenticationError, ResponseError
 from gigachat.models import Model
 
 
 def _get_kwargs(
     *,
     model: str,
@@ -18,23 +25,29 @@
     if access_token:
         headers["Authorization"] = f"Bearer {access_token}"
 
     authorization = authorization_cvar.get()
     client_id = client_id_cvar.get()
     session_id = session_id_cvar.get()
     request_id = request_id_cvar.get()
+    service_id = service_id_cvar.get()
+    operation_id = operation_id_cvar.get()
 
     if authorization:
         headers["Authorization"] = authorization
     if client_id:
         headers["X-Client-ID"] = client_id
     if session_id:
         headers["X-Session-ID"] = session_id
     if request_id:
         headers["X-Request-ID"] = request_id
+    if service_id:
+        headers["X-Service-ID"] = service_id
+    if operation_id:
+        headers["X-Operation-ID"] = operation_id
 
     return {
         "method": "GET",
         "url": f"/models/{model}",
         "headers": headers,
     }
```

### Comparing `gigachat-0.1.8/src/gigachat/api/get_models.py` & `gigachat-0.1.9/src/gigachat/api/get_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
-from gigachat.context import authorization_cvar, client_id_cvar, request_id_cvar, session_id_cvar
+from gigachat.context import (
+    authorization_cvar,
+    client_id_cvar,
+    operation_id_cvar,
+    request_id_cvar,
+    service_id_cvar,
+    session_id_cvar,
+)
 from gigachat.exceptions import AuthenticationError, ResponseError
 from gigachat.models import Models
 
 
 def _get_kwargs(
     *,
     access_token: Optional[str] = None,
@@ -17,23 +24,29 @@
     if access_token:
         headers["Authorization"] = f"Bearer {access_token}"
 
     authorization = authorization_cvar.get()
     client_id = client_id_cvar.get()
     session_id = session_id_cvar.get()
     request_id = request_id_cvar.get()
+    service_id = service_id_cvar.get()
+    operation_id = operation_id_cvar.get()
 
     if authorization:
         headers["Authorization"] = authorization
     if client_id:
         headers["X-Client-ID"] = client_id
     if session_id:
         headers["X-Session-ID"] = session_id
     if request_id:
         headers["X-Request-ID"] = request_id
+    if service_id:
+        headers["X-Service-ID"] = service_id
+    if operation_id:
+        headers["X-Operation-ID"] = operation_id
 
     return {
         "method": "GET",
         "url": "/models",
         "headers": headers,
     }
```

### Comparing `gigachat-0.1.8/src/gigachat/api/post_auth.py` & `gigachat-0.1.9/src/gigachat/api/post_auth.py`

 * *Files identical despite different names*

### Comparing `gigachat-0.1.8/src/gigachat/api/post_chat.py` & `gigachat-0.1.9/src/gigachat/api/post_chat.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
-from gigachat.context import authorization_cvar, client_id_cvar, request_id_cvar, session_id_cvar
+from gigachat.context import (
+    authorization_cvar,
+    client_id_cvar,
+    operation_id_cvar,
+    request_id_cvar,
+    service_id_cvar,
+    session_id_cvar,
+)
 from gigachat.exceptions import AuthenticationError, ResponseError
 from gigachat.models import Chat, ChatCompletion
 
 
 def _get_kwargs(
     *,
     chat: Chat,
@@ -18,23 +25,29 @@
     if access_token:
         headers["Authorization"] = f"Bearer {access_token}"
 
     authorization = authorization_cvar.get()
     client_id = client_id_cvar.get()
     session_id = session_id_cvar.get()
     request_id = request_id_cvar.get()
+    service_id = service_id_cvar.get()
+    operation_id = operation_id_cvar.get()
 
     if authorization:
         headers["Authorization"] = authorization
     if client_id:
         headers["X-Client-ID"] = client_id
     if session_id:
         headers["X-Session-ID"] = session_id
     if request_id:
         headers["X-Request-ID"] = request_id
+    if service_id:
+        headers["X-Service-ID"] = service_id
+    if operation_id:
+        headers["X-Operation-ID"] = operation_id
 
     return {
         "method": "POST",
         "url": "/chat/completions",
         "json": chat.dict(exclude_none=True, exclude={"stream"}),
         "headers": headers,
     }
```

### Comparing `gigachat-0.1.8/src/gigachat/api/post_token.py` & `gigachat-0.1.9/src/gigachat/api/post_token.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 from http import HTTPStatus
 from typing import Any, Dict
 
 import httpx
 
-from gigachat.context import client_id_cvar, request_id_cvar, session_id_cvar
+from gigachat.context import client_id_cvar, operation_id_cvar, request_id_cvar, service_id_cvar, session_id_cvar
 from gigachat.exceptions import AuthenticationError, ResponseError
 from gigachat.models import Token
 
 
 def _get_kwargs(
     *,
     user: str,
     password: str,
 ) -> Dict[str, Any]:
     headers = {}
 
     client_id = client_id_cvar.get()
     session_id = session_id_cvar.get()
     request_id = request_id_cvar.get()
+    service_id = service_id_cvar.get()
+    operation_id = operation_id_cvar.get()
 
     if client_id:
         headers["X-Client-ID"] = client_id
     if session_id:
         headers["X-Session-ID"] = session_id
     if request_id:
         headers["X-Request-ID"] = request_id
+    if service_id:
+        headers["X-Service-ID"] = service_id
+    if operation_id:
+        headers["X-Operation-ID"] = operation_id
 
     return {
         "method": "POST",
         "url": "/token",
         "auth": (user, password),
         "headers": headers,
     }
```

### Comparing `gigachat-0.1.8/src/gigachat/api/stream_chat.py` & `gigachat-0.1.9/src/gigachat/api/stream_chat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from http import HTTPStatus
 from typing import Any, AsyncIterator, Dict, Iterator, Optional
 
 import httpx
 
-from gigachat.context import authorization_cvar, client_id_cvar, request_id_cvar, session_id_cvar
+from gigachat.context import (
+    authorization_cvar,
+    client_id_cvar,
+    operation_id_cvar,
+    request_id_cvar,
+    service_id_cvar,
+    session_id_cvar,
+)
 from gigachat.exceptions import AuthenticationError, ResponseError
 from gigachat.models import Chat, ChatCompletionChunk
 
 EVENT_STREAM = "text/event-stream"
 
 
 def _get_kwargs(
@@ -22,23 +29,29 @@
     if access_token:
         headers["Authorization"] = f"Bearer {access_token}"
 
     authorization = authorization_cvar.get()
     client_id = client_id_cvar.get()
     session_id = session_id_cvar.get()
     request_id = request_id_cvar.get()
+    service_id = service_id_cvar.get()
+    operation_id = operation_id_cvar.get()
 
     if authorization:
         headers["Authorization"] = authorization
     if client_id:
         headers["X-Client-ID"] = client_id
     if session_id:
         headers["X-Session-ID"] = session_id
     if request_id:
         headers["X-Request-ID"] = request_id
+    if service_id:
+        headers["X-Service-ID"] = service_id
+    if operation_id:
+        headers["X-Operation-ID"] = operation_id
 
     return {
         "method": "POST",
         "url": "/chat/completions",
         "json": {**chat.dict(exclude_none=True), **{"stream": True}},
         "headers": headers,
     }
```

### Comparing `gigachat-0.1.8/src/gigachat/client.py` & `gigachat-0.1.9/src/gigachat/client.py`

 * *Files identical despite different names*

### Comparing `gigachat-0.1.8/src/gigachat/models/__init__.py` & `gigachat-0.1.9/src/gigachat/models/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachat-0.1.8/src/gigachat/models/chat.py` & `gigachat-0.1.9/src/gigachat/models/chat.py`

 * *Files identical despite different names*

### Comparing `gigachat-0.1.8/src/gigachat/models/chat_completion.py` & `gigachat-0.1.9/src/gigachat/models/chat_completion.py`

 * *Files identical despite different names*

### Comparing `gigachat-0.1.8/src/gigachat/models/chat_completion_chunk.py` & `gigachat-0.1.9/src/gigachat/models/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `gigachat-0.1.8/src/gigachat/pydantic_v1/__init__.py` & `gigachat-0.1.9/src/gigachat/pydantic_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `gigachat-0.1.8/src/gigachat/settings.py` & `gigachat-0.1.9/src/gigachat/settings.py`

 * *Files identical despite different names*

### Comparing `gigachat-0.1.8/PKG-INFO` & `gigachat-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: gigachat
-Version: 0.1.8
-Summary: GigaChat. Python-библиотека для GigaChain
+Version: 0.1.9
+Summary: GigaChat. Python-library for GigaChain and LangChain
 Home-page: https://github.com/ai-forever/gigachat
 License: MIT
 Author: Konstantin Krestnikov
 Author-email: rai220@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: httpx (<1)
 Requires-Dist: pydantic (>=1,<3)
 Project-URL: Repository, https://github.com/ai-forever/gigachat
 Description-Content-Type: text/markdown
 
 # GigaChat. Python-библиотека для GigaChain
```

