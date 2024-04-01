# Comparing `tmp/py_cachify-1.0.6.tar.gz` & `tmp/py_cachify-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_cachify-1.0.6.tar", max compression
+gzip compressed data, was "py_cachify-1.0.7.tar", max compression
```

## Comparing `py_cachify-1.0.6.tar` & `py_cachify-1.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1064 2024-03-14 16:18:25.427548 py_cachify-1.0.6/LICENSE
--rw-r--r--   0        0        0     3316 2024-03-14 16:18:25.427548 py_cachify-1.0.6/README.md
--rw-r--r--   0        0        0      460 2024-03-14 16:18:25.431548 py_cachify-1.0.6/py_cachify/__init__.py
--rw-r--r--   0        0        0        0 2024-03-14 16:18:25.431548 py_cachify-1.0.6/py_cachify/backend/__init__.py
--rw-r--r--   0        0        0     1210 2024-03-14 16:18:25.431548 py_cachify-1.0.6/py_cachify/backend/clients.py
--rw-r--r--   0        0        0       81 2024-03-14 16:18:25.431548 py_cachify-1.0.6/py_cachify/backend/exceptions.py
--rw-r--r--   0        0        0     1916 2024-03-14 16:18:25.431548 py_cachify-1.0.6/py_cachify/backend/lib.py
--rw-r--r--   0        0        0      719 2024-03-14 16:18:25.431548 py_cachify-1.0.6/py_cachify/backend/types.py
--rw-r--r--   0        0        0      676 2024-03-14 16:18:25.431548 py_cachify-1.0.6/py_cachify/base.py
--rw-r--r--   0        0        0     1420 2024-03-14 16:18:25.431548 py_cachify-1.0.6/py_cachify/cached.py
--rw-r--r--   0        0        0       44 2024-03-14 16:18:25.431548 py_cachify-1.0.6/py_cachify/exceptions.py
--rw-r--r--   0        0        0     2549 2024-03-14 16:18:25.431548 py_cachify-1.0.6/py_cachify/lock.py
--rw-r--r--   0        0        0        0 2024-03-14 16:18:25.431548 py_cachify-1.0.6/py_cachify/py.typed
--rw-r--r--   0        0        0     4017 2024-03-14 16:18:25.431548 py_cachify-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 py_cachify-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-01 23:43:20.047584 py_cachify-1.0.7/LICENSE
+-rw-r--r--   0        0        0     3316 2024-04-01 23:43:20.047584 py_cachify-1.0.7/README.md
+-rw-r--r--   0        0        0      460 2024-04-01 23:43:20.047584 py_cachify-1.0.7/py_cachify/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:43:20.047584 py_cachify-1.0.7/py_cachify/backend/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-01 23:43:20.047584 py_cachify-1.0.7/py_cachify/backend/clients.py
+-rw-r--r--   0        0        0       81 2024-04-01 23:43:20.047584 py_cachify-1.0.7/py_cachify/backend/exceptions.py
+-rw-r--r--   0        0        0     1941 2024-04-01 23:43:20.047584 py_cachify-1.0.7/py_cachify/backend/lib.py
+-rw-r--r--   0        0        0      719 2024-04-01 23:43:20.051584 py_cachify-1.0.7/py_cachify/backend/types.py
+-rw-r--r--   0        0        0      693 2024-04-01 23:43:20.051584 py_cachify-1.0.7/py_cachify/base.py
+-rw-r--r--   0        0        0     1420 2024-04-01 23:43:20.051584 py_cachify-1.0.7/py_cachify/cached.py
+-rw-r--r--   0        0        0       44 2024-04-01 23:43:20.051584 py_cachify-1.0.7/py_cachify/exceptions.py
+-rw-r--r--   0        0        0     2549 2024-04-01 23:43:20.051584 py_cachify-1.0.7/py_cachify/lock.py
+-rw-r--r--   0        0        0        0 2024-04-01 23:43:20.051584 py_cachify-1.0.7/py_cachify/py.typed
+-rw-r--r--   0        0        0     4017 2024-04-01 23:43:20.051584 py_cachify-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     3981 1970-01-01 00:00:00.000000 py_cachify-1.0.7/PKG-INFO
```

### Comparing `py_cachify-1.0.6/LICENSE` & `py_cachify-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.6/README.md` & `py_cachify-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.6/py_cachify/backend/clients.py` & `py_cachify-1.0.7/py_cachify/backend/clients.py`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.6/py_cachify/backend/lib.py` & `py_cachify-1.0.7/py_cachify/backend/lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 from py_cachify.backend.clients import AsyncWrapper, MemoryCache
 from py_cachify.backend.exceptions import CachifyInitError
 from py_cachify.backend.types import AsyncClient, SyncClient
 
 
 class Cachify:
     def __init__(
-        self, sync_client: Union[SyncClient, MemoryCache], async_client: Union[AsyncClient, AsyncWrapper], prefix: str
+        self,
+        sync_client: Union[SyncClient, MemoryCache],
+        async_client: Union[AsyncClient, AsyncWrapper],
+        prefix: str,
     ) -> None:
         self._sync_client = sync_client
         self._async_client = async_client
         self._prefix = prefix
 
     def set(self, key: str, val: Any, ttl: Union[int, None] = None) -> Any:
         self._sync_client.set(name=f'{self._prefix}{key}', value=pickle.dumps(val), ex=ttl)
```

### Comparing `py_cachify-1.0.6/py_cachify/backend/types.py` & `py_cachify-1.0.7/py_cachify/backend/types.py`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.6/py_cachify/base.py` & `py_cachify-1.0.7/py_cachify/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import inspect
-from typing import Any, Awaitable, Callable, Union
+from typing import Awaitable, Callable, TypeVar, Union
 
 from typing_extensions import ParamSpec
 
 
+T = TypeVar('T')
 P = ParamSpec('P')
-SyncFunc = Callable[P, Any]
-AsyncFunc = Callable[P, Awaitable[Any]]
+SyncFunc = Callable[P, T]
+AsyncFunc = Callable[P, Awaitable[T]]
 DecoratorFunc = Callable[[Union[SyncFunc, AsyncFunc]], Union[AsyncFunc, SyncFunc]]
 
 
 def get_full_key_from_signature(bound_args: inspect.BoundArguments, key: str) -> str:
     args_dict = bound_args.arguments
     args = args_dict.pop('args', ())
     kwargs = args_dict.pop('kwargs', {})
```

### Comparing `py_cachify-1.0.6/py_cachify/cached.py` & `py_cachify-1.0.7/py_cachify/cached.py`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.6/py_cachify/lock.py` & `py_cachify-1.0.7/py_cachify/lock.py`

 * *Files identical despite different names*

### Comparing `py_cachify-1.0.6/pyproject.toml` & `py_cachify-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-cachify"
-version = "1.0.6"
+version = "1.0.7"
 homepage = "https://github.com/EzyGang/py-cachify"
 repository = "https://github.com/EzyGang/py-cachify"
 license = "MIT"
 description = ""
 authors = ["Galtozzy <galtozzy+git@gmail.com>"]
 readme = "README.md"
 include = ["README.md"]
```

### Comparing `py_cachify-1.0.6/PKG-INFO` & `py_cachify-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-cachify
-Version: 1.0.6
+Version: 1.0.7
 Summary: 
 Home-page: https://github.com/EzyGang/py-cachify
 License: MIT
 Author: Galtozzy
 Author-email: galtozzy+git@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

