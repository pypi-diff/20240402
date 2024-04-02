# Comparing `tmp/unifyai-0.3.0.tar.gz` & `tmp/unifyai-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifyai-0.3.0.tar", max compression
+gzip compressed data, was "unifyai-0.3.1.tar", max compression
```

## Comparing `unifyai-0.3.0.tar` & `unifyai-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11336 2024-04-01 15:07:46.559585 unifyai-0.3.0/LICENSE
--rw-r--r--   0        0        0     5260 2024-04-01 15:07:46.627585 unifyai-0.3.0/README.md
--rw-r--r--   0        0        0      998 2024-04-01 17:18:52.581612 unifyai-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       88 2024-04-01 15:09:39.727584 unifyai-0.3.0/unifyai/__init__.py
--rw-r--r--   0        0        0     8405 2024-04-01 15:09:39.731584 unifyai-0.3.0/unifyai/clients.py
--rw-r--r--   0        0        0     1166 2024-04-01 15:09:39.731584 unifyai-0.3.0/unifyai/exceptions.py
--rw-r--r--   0        0        0     4100 2024-04-01 15:09:39.731584 unifyai-0.3.0/unifyai/tests.py
--rw-r--r--   0        0        0     5901 1970-01-01 00:00:00.000000 unifyai-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11336 2024-04-02 01:55:16.865353 unifyai-0.3.1/LICENSE
+-rw-r--r--   0        0        0     5270 2024-04-02 01:55:16.909353 unifyai-0.3.1/README.md
+-rw-r--r--   0        0        0      998 2024-04-02 08:14:37.577337 unifyai-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0       88 2024-04-02 01:55:16.869353 unifyai-0.3.1/unifyai/__init__.py
+-rw-r--r--   0        0        0     8405 2024-04-02 01:55:16.869353 unifyai-0.3.1/unifyai/clients.py
+-rw-r--r--   0        0        0     1166 2024-04-02 01:55:16.873353 unifyai-0.3.1/unifyai/exceptions.py
+-rw-r--r--   0        0        0     4100 2024-04-02 01:55:16.873353 unifyai-0.3.1/unifyai/tests.py
+-rw-r--r--   0        0        0     5911 1970-01-01 00:00:00.000000 unifyai-0.3.1/PKG-INFO
```

### Comparing `unifyai-0.3.0/LICENSE` & `unifyai-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unifyai-0.3.0/README.md` & `unifyai-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ```bash
 pip install unifyai
 ```
 
 ## Basic Usage
 ```python
 import os
-from unify import Unify
+from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
 )
 response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale")
 ```
 
@@ -66,15 +66,15 @@
 
 ## Asynchronous Usage
 For optimal performance in handling multiple user requests simultaneously, such as in a chatbot application, processing them asynchronously is recommended.
 To use the AsyncUnify client, simply import `AsyncUnify` instead
  of `Unify` and use `await` with the `.generate` function.
 
  ```python
-from unify import AsyncUnify
+from unifyai import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
 )
 
@@ -87,28 +87,28 @@
 Functionality wise, the Async and Sync clients are identical.
 
 ## Streaming Responses
 You can enable streaming responses by setting `stream=True` in the `.generate` function.
 
 ```python
 import os
-from unify import Unify
+from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
 )
 stream = unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale", stream=True)
 for chunk in stream:
     print(x, end="")
 ```
 
 It works in exactly the same way with Async clients.
 
  ```python
-from unify import AsyncUnify
+from unifyai import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
 )
 
@@ -121,15 +121,15 @@
 ```
 
 ## Dynamic Routing
 As evidenced by our [benchmarks](https://unify.ai/hub), the optimal provider for each model varies by geographic location and time of day due to fluctuating API performances. With our dynamic routing, we automatically direct your requests to the "top-performing provider" at that moment. To enable this feature, simply replace your query's provider with one of the [available routing modes](https://unify.ai/docs/hub/concepts/runtime_routing.html#available-modes). As an example, you can query the `llama-2-7b-chat` endpoint to get the provider with the lowest input-cost as follows:
 
 ```python
 import os
-from unify import Unify
+from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
 )
 response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="lowest-input-cost")
 ```
 Dynamic routing works with both Synchronous and Asynchronous clients. For more information on Dynamic Routing, check our [documentation](https://unify.ai/docs/hub/concepts/runtime_routing.html#dynamic-routing).
```

### Comparing `unifyai-0.3.0/pyproject.toml` & `unifyai-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unifyai"
-version = "0.3.0"
+version = "0.3.1"
 readme = "README.md"
 description = "A Python package for interacting with the Unify API"
 authors = ["Unify <hello@unify.com>"]
 repository = "https://github.com/unifyai/unify-llm-python"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `unifyai-0.3.0/unifyai/clients.py` & `unifyai-0.3.1/unifyai/clients.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.3.0/unifyai/exceptions.py` & `unifyai-0.3.1/unifyai/exceptions.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.3.0/unifyai/tests.py` & `unifyai-0.3.1/unifyai/tests.py`

 * *Files identical despite different names*

### Comparing `unifyai-0.3.0/PKG-INFO` & `unifyai-0.3.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifyai
-Version: 0.3.0
+Version: 0.3.1
 Summary: A Python package for interacting with the Unify API
 Home-page: https://github.com/unifyai/unify-llm-python
 Author: Unify
 Author-email: hello@unify.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -34,15 +34,15 @@
 ```bash
 pip install unifyai
 ```
 
 ## Basic Usage
 ```python
 import os
-from unify import Unify
+from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
 )
 response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale")
 ```
 
@@ -83,15 +83,15 @@
 
 ## Asynchronous Usage
 For optimal performance in handling multiple user requests simultaneously, such as in a chatbot application, processing them asynchronously is recommended.
 To use the AsyncUnify client, simply import `AsyncUnify` instead
  of `Unify` and use `await` with the `.generate` function.
 
  ```python
-from unify import AsyncUnify
+from unifyai import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
 )
 
@@ -104,28 +104,28 @@
 Functionality wise, the Async and Sync clients are identical.
 
 ## Streaming Responses
 You can enable streaming responses by setting `stream=True` in the `.generate` function.
 
 ```python
 import os
-from unify import Unify
+from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
 )
 stream = unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="anyscale", stream=True)
 for chunk in stream:
     print(x, end="")
 ```
 
 It works in exactly the same way with Async clients.
 
  ```python
-from unify import AsyncUnify
+from unifyai import AsyncUnify
 import os
 import asyncio
 async_unify = AsyncUnify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
 )
 
@@ -138,15 +138,15 @@
 ```
 
 ## Dynamic Routing
 As evidenced by our [benchmarks](https://unify.ai/hub), the optimal provider for each model varies by geographic location and time of day due to fluctuating API performances. With our dynamic routing, we automatically direct your requests to the "top-performing provider" at that moment. To enable this feature, simply replace your query's provider with one of the [available routing modes](https://unify.ai/docs/hub/concepts/runtime_routing.html#available-modes). As an example, you can query the `llama-2-7b-chat` endpoint to get the provider with the lowest input-cost as follows:
 
 ```python
 import os
-from unify import Unify
+from unifyai import Unify
 unify = Unify(
     # This is the default and optional to include.
     api_key=os.environ.get("UNIFY_KEY")
 )
 response = unify.generate(messages="Hello Llama! Who was Isaac Newton?", model="llama-2-13b-chat", provider="lowest-input-cost")
 ```
 Dynamic routing works with both Synchronous and Asynchronous clients. For more information on Dynamic Routing, check our [documentation](https://unify.ai/docs/hub/concepts/runtime_routing.html#dynamic-routing).
```

