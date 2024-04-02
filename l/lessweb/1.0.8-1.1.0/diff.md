# Comparing `tmp/lessweb-1.0.8.tar.gz` & `tmp/lessweb-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lessweb-1.0.8.tar", last modified: Sat Jul  1 14:50:29 2023, max compression
+gzip compressed data, was "lessweb-1.1.0.tar", last modified: Tue Apr  2 03:30:00 2024, max compression
```

## Comparing `lessweb-1.0.8.tar` & `lessweb-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,62 @@
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-07-01 14:50:29.005907 lessweb-1.0.8/
--rw-r--r--   0 zhangji    (501) staff       (20)      556 2022-11-14 08:34:51.000000 lessweb-1.0.8/LICENSE.txt
--rw-r--r--   0 zhangji    (501) staff       (20)     1924 2023-07-01 14:50:29.005356 lessweb-1.0.8/PKG-INFO
--rw-r--r--   0 zhangji    (501) staff       (20)     1649 2022-12-06 09:47:53.000000 lessweb-1.0.8/README.md
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-07-01 14:50:28.995933 lessweb-1.0.8/lessweb/
--rw-r--r--   0 zhangji    (501) staff       (20)      255 2023-04-23 13:41:17.000000 lessweb-1.0.8/lessweb/__init__.py
--rw-r--r--   0 zhangji    (501) staff       (20)    14244 2023-04-23 13:41:06.000000 lessweb-1.0.8/lessweb/bridge.py
--rw-r--r--   0 zhangji    (501) staff       (20)        0 2023-01-14 08:15:49.000000 lessweb-1.0.8/lessweb/py.typed
--rw-r--r--   0 zhangji    (501) staff       (20)     7860 2023-01-14 07:25:23.000000 lessweb-1.0.8/lessweb/typecast.py
-drwxr-xr-x   0 zhangji    (501) staff       (20)        0 2023-07-01 14:50:29.004679 lessweb-1.0.8/lessweb.egg-info/
--rw-r--r--   0 zhangji    (501) staff       (20)     1924 2023-07-01 14:50:28.000000 lessweb-1.0.8/lessweb.egg-info/PKG-INFO
--rw-r--r--   0 zhangji    (501) staff       (20)      265 2023-07-01 14:50:28.000000 lessweb-1.0.8/lessweb.egg-info/SOURCES.txt
--rw-r--r--   0 zhangji    (501) staff       (20)        1 2023-07-01 14:50:28.000000 lessweb-1.0.8/lessweb.egg-info/dependency_links.txt
--rw-r--r--   0 zhangji    (501) staff       (20)       43 2023-07-01 14:50:28.000000 lessweb-1.0.8/lessweb.egg-info/requires.txt
--rw-r--r--   0 zhangji    (501) staff       (20)        8 2023-07-01 14:50:28.000000 lessweb-1.0.8/lessweb.egg-info/top_level.txt
--rw-r--r--   0 zhangji    (501) staff       (20)      520 2023-07-01 14:36:46.000000 lessweb-1.0.8/pyproject.toml
--rw-r--r--   0 zhangji    (501) staff       (20)       38 2023-07-01 14:50:29.006080 lessweb-1.0.8/setup.cfg
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.389198 lessweb-1.1.0/
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.380889 lessweb-1.1.0/.github/
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.382704 lessweb-1.1.0/.github/workflows/
+-rw-r--r--   0 zhangji    (502) staff       (20)      941 2024-03-28 06:37:50.000000 lessweb-1.1.0/.github/workflows/python-package.yml
+-rw-r--r--   0 zhangji    (502) staff       (20)     1093 2024-03-28 06:00:47.000000 lessweb-1.1.0/.gitignore
+-rw-r--r--   0 zhangji    (502) staff       (20)      556 2024-03-28 00:41:05.000000 lessweb-1.1.0/LICENSE.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)     2099 2024-04-02 03:30:00.388945 lessweb-1.1.0/PKG-INFO
+-rw-r--r--   0 zhangji    (502) staff       (20)     1706 2024-03-28 00:41:05.000000 lessweb-1.1.0/README.md
+-rw-r--r--   0 zhangji    (502) staff       (20)      315 2024-03-28 06:43:43.000000 lessweb-1.1.0/changelog.md
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.381551 lessweb-1.1.0/examples/
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.382949 lessweb-1.1.0/examples/100_hello_world/
+-rw-r--r--   0 zhangji    (502) staff       (20)      244 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/100_hello_world/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.383380 lessweb-1.1.0/examples/100_hello_world_config/
+-rw-r--r--   0 zhangji    (502) staff       (20)       21 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/100_hello_world_config/config.toml
+-rw-r--r--   0 zhangji    (502) staff       (20)      264 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/100_hello_world_config/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.383592 lessweb-1.1.0/examples/101_handle_request/
+-rw-r--r--   0 zhangji    (502) staff       (20)      676 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/101_handle_request/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.384201 lessweb-1.1.0/examples/102_response/
+-rw-r--r--   0 zhangji    (502) staff       (20)     1284 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/102_response/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.384399 lessweb-1.1.0/examples/103_get_request/
+-rw-r--r--   0 zhangji    (502) staff       (20)      772 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/103_get_request/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.384737 lessweb-1.1.0/examples/205_mysql_crud/
+-rw-r--r--   0 zhangji    (502) staff       (20)      169 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/config.toml
+-rw-r--r--   0 zhangji    (502) staff       (20)      370 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.384978 lessweb-1.1.0/examples/205_mysql_crud/myapp/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/myapp/__init__.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.385406 lessweb-1.1.0/examples/205_mysql_crud/myapp/endpoint/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/myapp/endpoint/__init__.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      211 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/myapp/endpoint/create_pet.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      225 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/myapp/endpoint/get_pet_detail.py
+-rw-r--r--   0 zhangji    (502) staff       (20)      295 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/myapp/endpoint/get_pet_total.py
+-rw-r--r--   0 zhangji    (502) staff       (20)     1544 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/myapp/mapper.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.385526 lessweb-1.1.0/examples/205_mysql_crud/schema/
+-rw-r--r--   0 zhangji    (502) staff       (20)      307 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/205_mysql_crud/schema/pet.sql
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.385639 lessweb-1.1.0/examples/302_cookie/
+-rw-r--r--   0 zhangji    (502) staff       (20)      550 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/302_cookie/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.385834 lessweb-1.1.0/examples/303_middleware/
+-rw-r--r--   0 zhangji    (502) staff       (20)      533 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/303_middleware/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.386017 lessweb-1.1.0/examples/304_websocket/
+-rw-r--r--   0 zhangji    (502) staff       (20)     1198 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/304_websocket/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.386602 lessweb-1.1.0/examples/305_schedule_task/
+-rw-r--r--   0 zhangji    (502) staff       (20)      814 2024-03-28 00:41:05.000000 lessweb-1.1.0/examples/305_schedule_task/index.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.387241 lessweb-1.1.0/lessweb/
+-rw-r--r--   0 zhangji    (502) staff       (20)      232 2024-03-28 00:41:05.000000 lessweb-1.1.0/lessweb/__init__.py
+-rw-r--r--   0 zhangji    (502) staff       (20)    14739 2024-03-28 06:00:47.000000 lessweb-1.1.0/lessweb/bridge.py
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 00:41:05.000000 lessweb-1.1.0/lessweb/py.typed
+-rw-r--r--   0 zhangji    (502) staff       (20)     8932 2024-03-28 06:06:02.000000 lessweb-1.1.0/lessweb/typecast.py
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.388551 lessweb-1.1.0/lessweb.egg-info/
+-rw-r--r--   0 zhangji    (502) staff       (20)     2099 2024-04-02 03:30:00.000000 lessweb-1.1.0/lessweb.egg-info/PKG-INFO
+-rw-r--r--   0 zhangji    (502) staff       (20)     1178 2024-04-02 03:30:00.000000 lessweb-1.1.0/lessweb.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)        1 2024-04-02 03:30:00.000000 lessweb-1.1.0/lessweb.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)       43 2024-04-02 03:30:00.000000 lessweb-1.1.0/lessweb.egg-info/requires.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)        8 2024-04-02 03:30:00.000000 lessweb-1.1.0/lessweb.egg-info/top_level.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)       62 2024-03-28 06:00:47.000000 lessweb-1.1.0/mypy.ini
+-rw-r--r--   0 zhangji    (502) staff       (20)      538 2024-03-28 06:40:38.000000 lessweb-1.1.0/pyproject.toml
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.388116 lessweb-1.1.0/requirements/
+-rw-r--r--   0 zhangji    (502) staff       (20)       42 2024-03-28 06:00:47.000000 lessweb-1.1.0/requirements/base.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)       66 2024-03-28 06:00:47.000000 lessweb-1.1.0/requirements/test.txt
+-rw-r--r--   0 zhangji    (502) staff       (20)       38 2024-04-02 03:30:00.389232 lessweb-1.1.0/setup.cfg
+drwxr-xr-x   0 zhangji    (502) staff       (20)        0 2024-04-02 03:30:00.388292 lessweb-1.1.0/tests/
+-rw-r--r--   0 zhangji    (502) staff       (20)        0 2024-03-28 06:00:47.000000 lessweb-1.1.0/tests/__init__.py
+-rw-r--r--   0 zhangji    (502) staff       (20)     3916 2024-03-28 06:12:06.000000 lessweb-1.1.0/tests/test_typecast.py
```

### Comparing `lessweb-1.0.8/LICENSE.txt` & `lessweb-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lessweb-1.0.8/PKG-INFO` & `lessweb-1.1.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: lessweb
-Version: 1.0.8
+Version: 1.1.0
 Summary: A pythonic web framework
 Author-email: qorzj <goodhorsezxj@gmail.com>
 License: Apache 2
 Keywords: lessweb,web,web.py,aiohttp
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: aiohttp
+Requires-Dist: toml
+Requires-Dist: orjson
+Requires-Dist: lesscli
+Requires-Dist: typing_inspect
 
 # lessweb
 >「嘞是web」
 
 Lessweb is an extremely easy-to-use python web framework with the following goals.
 
 * Simple and efficient: based on the aiohttp library IOC capabilities, native support for configuration loading and logging settings to meet production-level development requirements
@@ -77,9 +82,12 @@
 
 Lessweb is offered under the Apache 2 license.
 
 ## Source code
 
 The latest developer version is available in a GitHub repository: https://github.com/lessweb/lessweb
 
+## Cookbook
+### https://github.com/lessweb/lessweb/wiki
+
 ## Cookbook【中文】：
 ### http://www.lessweb.cn
```

### Comparing `lessweb-1.0.8/README.md` & `lessweb-1.1.0/lessweb.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: lessweb
+Version: 1.1.0
+Summary: A pythonic web framework
+Author-email: qorzj <goodhorsezxj@gmail.com>
+License: Apache 2
+Keywords: lessweb,web,web.py,aiohttp
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: aiohttp
+Requires-Dist: toml
+Requires-Dist: orjson
+Requires-Dist: lesscli
+Requires-Dist: typing_inspect
+
 # lessweb
 >「嘞是web」
 
 Lessweb is an extremely easy-to-use python web framework with the following goals.
 
 * Simple and efficient: based on the aiohttp library IOC capabilities, native support for configuration loading and logging settings to meet production-level development requirements
 * Pythonic: support for the latest python version and the latest python syntax
@@ -66,9 +82,12 @@
 
 Lessweb is offered under the Apache 2 license.
 
 ## Source code
 
 The latest developer version is available in a GitHub repository: https://github.com/lessweb/lessweb
 
+## Cookbook
+### https://github.com/lessweb/lessweb/wiki
+
 ## Cookbook【中文】：
 ### http://www.lessweb.cn
```

### Comparing `lessweb-1.0.8/lessweb/bridge.py` & `lessweb-1.1.0/lessweb/bridge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
-from aiohttp.web import Request, Application, Response, middleware, HTTPBadRequest, HTTPError, run_app
-from aiohttp.typedefs import LooseHeaders
-from dataclasses import dataclass, is_dataclass
 import importlib
 import inspect
 import logging
-from logging.handlers import TimedRotatingFileHandler
-import orjson
-from os import environ, listdir
 import re
 import sys
+from dataclasses import dataclass, is_dataclass
+from logging.handlers import TimedRotatingFileHandler
+from os import environ, listdir
+from typing import Any, Dict, Optional, Type, TypeVar, Union
+
+import orjson
 import toml
-from typing import Union, Type, TypeVar, Any, Optional, Dict
-from .typecast import typecast, isinstance_safe, is_typeddict
+from aiohttp.typedefs import LooseHeaders
+from aiohttp.web import (Application, HTTPBadRequest, HTTPError, Request,
+                         Response, middleware, run_app)
+
+from .typecast import is_typeddict, isinstance_safe, typecast
 
 T = TypeVar('T')
 ORJSON_OPTION = 0
 POSITIONAL_ONLY = 0
 KEYWORD_ONLY = 3
 
 
@@ -77,16 +80,16 @@
     return ORJSON_OPTION
 
 
 def rest_response(
         data,
         *,
         status: int = 200,
-        reason: str = None,
-        headers: LooseHeaders = None,
+        reason: Optional[str] = None,
+        headers: Optional[LooseHeaders] = None,
 ) -> Response:
     resp = Response(
         body=orjson.dumps(data, option=ORJSON_OPTION),
         status=status,
         reason=reason,
         headers=headers,
         content_type='application/json',
@@ -95,15 +98,15 @@
     return resp
 
 
 def rest_error(
         error: Type[HTTPError],
         data,
         *,
-        headers: LooseHeaders = None,
+        headers: Optional[LooseHeaders] = None,
         **kwargs,
 ) -> HTTPError:
     return error(
         body=orjson.dumps(data, option=ORJSON_OPTION),
         headers=headers,
         content_type='application/json',
         **kwargs,
@@ -111,23 +114,23 @@
 
 
 def service(f: T) -> T:
     f.__lessweb_service__ = 1  # type: ignore[attr-defined]
     return f
 
 
-def autowire(ctx: Union[Application, Request], cls: Type[T], name: str = None) -> T:
+def autowire(ctx: Union[Application, Request], cls: Type[T], name: Optional[str] = None) -> T:
     """
     依赖注入。
     通过注入完成后，调用__init__实例化。后续直接使用实例化结果。
     实例生命范围分为应用级(application)和请求级(request)。
     特别地，依赖Application和Request不需要加载模块。
     """
     ref = absolute_ref(cls)
-    app_ctx = ctx.app if isinstance_safe(ctx, Request) else ctx
+    app_ctx = ctx.app if isinstance(ctx, Request) else ctx
     assert ref != 'config', f'Cannot inject {cls} since `config` is reserved word!'
     if name:  # try to inject by name
         if name == 'config' and is_typeddict(cls):
             name_ref = f'{name}:{ref}'
             if name_ref in app_ctx:
                 return app_ctx[name_ref]
             else:
@@ -141,17 +144,17 @@
             return ctx.config_dict[name]
     if ref in ctx:
         return ctx[ref]
     elif isinstance(ctx, Request) and ref in ctx.config_dict:
         return ctx.config_dict[ref]
     logging.debug('autowire-> %s %s', ctx, cls)
     if isinstance_safe(ctx, cls):
-        return ctx
+        return ctx  # type: ignore
     elif isinstance(ctx, Request) and cls is Application:
-        return ctx.app
+        return ctx.app  # type: ignore
     elif not hasattr(cls, '__lessweb_service__'):
         raise TypeError(f'cannot autowire ({ref}) {ctx=} {cls=})')
     depends_on = get_depends_on(cls.__init__)
     args: list = []
     for name, depends_type in depends_on:
         args.append(autowire(ctx, depends_type, name))
     ctx[ref] = singleton = cls(*args)
@@ -186,33 +189,34 @@
 
 def make_app_signal(sp_handler):
     """
     :return: 形如foo(app)这样的函数
     """
 
     async def aio_handler(app):
-        args, kwargs = [], {}
+        kwargs = {}
         for name, (depends_type, _, kind) in func_arg_spec(sp_handler).items():
             kwargs[name] = autowire(app, depends_type, name)
-        return await sp_handler(*args, **kwargs)
+        return await sp_handler(**kwargs)
 
     return aio_handler
 
 
 def getdoc(obj) -> str:
     """
     获得模块或对象的docstring
     实现了递归包含，只需要以「:include 」开头
     """
     if isinstance(obj, str):
         try:
             module_or_object = importlib.import_module(obj)
         except ModuleNotFoundError:
             module_name, object_name = obj.rsplit('.', 1)
-            module_or_object = getattr(importlib.import_module(module_name), object_name)
+            module_or_object = getattr(
+                importlib.import_module(module_name), object_name)
         return getdoc(module_or_object)
     result = []
     docstring = inspect.getdoc(obj) or ''
     for line in docstring.splitlines():
         if line.strip().startswith(':include '):
             include_doc = getdoc(line.replace(':include ', '').strip())
             result.append(include_doc)
@@ -227,39 +231,45 @@
         1.POSITIONAL_ONLY参数表示requestbody
         2.int和str类型参数表示路径参数
         3.其他参数支持可注入类型
     :return: 形如foo(request)这样的函数
     """
 
     async def aio_endpoint(request: Request):
-        assert inspect.iscoroutinefunction(sp_endpoint), f'{sp_endpoint} must be coroutine function'
+        assert inspect.iscoroutinefunction(
+            sp_endpoint), f'{sp_endpoint} must be coroutine function'
         args = []
         kwargs: Dict[str, Any] = {}
         for name, (depends_type, default, kind) in func_arg_spec(sp_endpoint).items():
             if kind == POSITIONAL_ONLY:
                 try:
                     data = orjson.loads(await request.text())
                 except orjson.JSONDecodeError:
-                    raise HTTPBadRequest(text=f'BadRequest: request body raise JSONDecodeError')
+                    raise HTTPBadRequest(
+                        text=f'BadRequest: request body raise JSONDecodeError')
                 try:
                     args.append(typecast(data, depends_type))
                 except Exception as e:
-                    raise HTTPBadRequest(text=f'BadRequest: request body decoding error: {e}')
+                    raise HTTPBadRequest(
+                        text=f'BadRequest: request body decoding error: {e}')
             elif kind == KEYWORD_ONLY:
-                chosen_value = request.match_info[name] if name in request.match_info else request.query.get(name)
+                chosen_value = request.match_info[name] if name in request.match_info else request.query.get(
+                    name)
                 if chosen_value is None:
                     if default is not None:
-                        raise HTTPBadRequest(text=f'BadRequest: missing required parameter: {name}')
+                        raise HTTPBadRequest(
+                            text=f'BadRequest: missing required parameter: {name}')
                     else:
                         kwargs[name] = None
                 else:
                     try:
                         kwargs[name] = typecast(chosen_value, depends_type)
                     except Exception:
-                        raise HTTPBadRequest(text=f'BadRequest: invalid parameter: {name}')
+                        raise HTTPBadRequest(
+                            text=f'BadRequest: invalid parameter: {name}')
             else:
                 kwargs[name] = autowire(request, depends_type, name)
         result = await sp_endpoint(*args, **kwargs)
         if isinstance(result, (dict, list)) or is_dataclass(result):
             return rest_response(result)
         else:
             return result
@@ -321,15 +331,15 @@
     return g
 
 
 class Bridge:
     app: Application
     config: Optional[str]
 
-    def __init__(self, config: str = None, app: Application = None):
+    def __init__(self, config: Optional[str] = None, app: Optional[Application] = None):
         if app is None:
             self.app = Application()
         else:
             self.app = app
         self.config = config
         self._load_config()
 
@@ -383,15 +393,16 @@
             stream = sys.stdout if stream_str == 'stdout' else sys.stderr
             stream_handler = logging.StreamHandler(stream)
             if formatter:
                 stream_handler.setFormatter(formatter)
             logger.addHandler(stream_handler)
 
     def _load_orjson(self):
-        init_orjson_option(self.app['config']['bootstrap'].get('orjson_option', ''))
+        init_orjson_option(self.app['config']
+                           ['bootstrap'].get('orjson_option', ''))
 
     def add_middleware(self, handler):
         self.app.middlewares.append(make_middleware(handler))
 
     def add_on_startup(self, handler):
         self.app.on_startup.append(make_app_signal(handler))
 
@@ -407,21 +418,25 @@
         self.app.cleanup_ctx.append(aio_handler)
 
     def add_on_shutdown(self, handler):
         self.app.on_shutdown.append(make_app_signal(handler))
 
     def add_route(self, route):
         for path in route.paths:
-            self.app.router.add_route(method=route.method, path=path, handler=route.handler)
+            self.app.router.add_route(
+                method=route.method, path=path, handler=route.handler)
 
     def add_route_scan(self, endpoint_package: str):
         endpoint_mdl = importlib.import_module(endpoint_package)
+        if endpoint_mdl.__spec__ is None or not endpoint_mdl.__spec__.submodule_search_locations:
+            raise ImportError(f'{endpoint_package} is an empty package')
         for filename in listdir(endpoint_mdl.__spec__.submodule_search_locations[0]):
             if filename.endswith('.py'):
-                sub_mdl = importlib.import_module(f'{endpoint_package}.{filename[:-3]}')
+                sub_mdl = importlib.import_module(
+                    f'{endpoint_package}.{filename[:-3]}')
                 for item in sub_mdl.__dict__.values():
                     if isinstance(item, Route):
                         self.add_route(item)
 
     def run_app(self, **kwargs):
         port = int(self.app['config']['bootstrap'].get('port', 8080))
         run_app(app=self.app, port=port, **kwargs)
```

### Comparing `lessweb-1.0.8/lessweb/typecast.py` & `lessweb-1.1.0/lessweb/typecast.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import csv
 import datetime
 import enum
 import inspect
-from typing import Any, Union, get_type_hints, List, Type, Dict
-import typing_inspect
-import csv
 import json
+import re
+import sys
+from typing import Any, Dict, List, Literal, Type, Union, get_type_hints
+
+import typing_inspect
 
 
-class JSONDecodeError(Exception):
+class TypeCastError(Exception):
     pass
 
 
 NoneType = type(None)
 
 
 classname_dict: Dict[str, Type] = {}
@@ -50,51 +53,64 @@
 
 def is_typeddict(tp) -> bool:
     return issubclass_safe(tp, dict) and future_typed_dict_keys(tp)
 
 
 def inspect_type(tp):
     """
-    inspect_type(int) => int
-    inspect_type(list) => list
+    inspect_type(int) => (int,)
+    inspect_type(list) => (list,)
     inspect_type(list[int]) => (list, int)
     inspect_type(int | None) => (Union, (int, NoneType))
     inspect_type(int | str) => (Union, (int, str))
     inspect_type(int | str | None) => (Union, (int, str, NoneType))
-    inspect_type(dict) => dict
+    inspect_type(Literal['a', 'b']) => (Literal, ('a', 'b'))
+    inspect_type(dict) => (dict,)
     inspect_type(dict[str, int]) => NotImplementedError
     inspect_type(typeddict) => (dict, __annotations__)
-    inspect_type(else) => NotImplementedError
+    inspect_type(cls) => (cls,)
+    inspect_type(_else_) => NotImplementedError
     """
     if isinstance_safe(tp, str):
         tp = classname_dict[tp]
     tp_origin = typing_inspect.get_origin(tp)
     tp_args = typing_inspect.get_args(tp)
     if tp_origin is None and tp_args == ():
         if is_typeddict(tp):
             classname_dict[tp.__qualname__] = tp
             return dict, get_type_hints(tp)
-        return tp
+        return (tp,)
     if tp_origin is list:
         return list, tp_args[0]
     if (tp_origin is None or tp_origin == Union) and tp_args:
         return Union, tp_args
+    if tp_origin == Literal and tp_args:
+        return Literal, tp_args
     raise NotImplementedError(f'cannot inspect type {tp=}')
 
 
 def is_list_type(tp):
     return tp is list or typing_inspect.get_origin(tp) is list
 
 
 def typecast(data, tp):
     if isinstance_safe(tp, str):
         if tp not in classname_dict:
-            raise JSONDecodeError(f'typename {tp=} is not valid ref')
+            raise TypeCastError(
+                f'typename {tp=} is not valid ref')  # 5xx Error in fact
         else:
             tp = classname_dict[tp]
+    type_inspect_seed = inspect_type(tp)
+    if type_inspect_seed[0] == Literal:
+        if len(type_inspect_seed) != 2 or not type_inspect_seed[1]:
+            raise TypeCastError(f'{tp=} is empty')  # 5xx Error in fact
+        for item in type_inspect_seed[1]:
+            if item == data:
+                return data
+        raise TypeCastError(f'{data=} is not member of {tp=}')
     if isinstance_safe(data, tp):
         return data
     elif issubclass_safe(tp, enum.Enum):
         return tp(data)
     elif issubclass_safe(tp, datetime.datetime):
         return datetime.datetime.fromisoformat(data)
     elif issubclass_safe(tp, datetime.date):
@@ -104,56 +120,63 @@
     elif isinstance(data, str):
         if issubclass_safe(tp, str):
             return tp(data)
         elif is_list_type(tp):
             data = parse_csv(data)
             return typecast(data, tp)
         else:
-            data = json.loads(data)
-            return typecast(data, tp)
+            try:
+                data = json.loads(data)
+                return typecast(data, tp)
+            except:
+                if re.match(r'^\w*$', data):
+                    raise TypeCastError(f'{data=} is not an instance of {tp=}')
+                raise
     else:
-        type_inspect_seed = inspect_type(tp)
-        if isinstance(type_inspect_seed, tuple):
-            origin_type, type_args = type_inspect_seed
-            if origin_type is list:
-                assert isinstance(data, list)
-                return [typecast(item, type_args) for item in data]
-            elif origin_type == Union:
-                error_list = []
-                for type_arg in type_args:
-                    try:
-                        return typecast(data, type_arg)
-                    except Exception as e:
-                        error_list.append(str(e))
-                raise JSONDecodeError(f'{data=} is not any instance of {tp=}: ' + '; '.join(error_list))
-            elif origin_type == dict:
-                assert isinstance(data, dict)
-                optional_keys = getattr(tp, '__optional_keys__')
-                if optional_keys:
-                    required_keys = set(type_args.keys()) - optional_keys
-                else:
-                    required_keys = getattr(tp, '__required_keys__', set())
-                missing_keys = required_keys - set(data.keys())
-                none_value_keys = set()
-                result = {}
-                for item_key, item_value in data.items():
-                    if item_key not in type_args:
-                        raise JSONDecodeError(f'{item_key=} is not member of {tp=}')
-                    result[item_key] = typecast(item_value, type_args[item_key])
-                for item_key in missing_keys:
-                    if typing_inspect.is_optional_type(type_args[item_key]):
-                        result[item_key] = None
-                        none_value_keys.add(item_key)
-                if missing_keys - none_value_keys:
-                    raise JSONDecodeError(f'missing required keys {list(missing_keys - none_value_keys)}')
-                return result
+        if len(type_inspect_seed) != 2:
+            raise TypeCastError(f'{data=} is not instance of {tp=}')
+        origin_type, type_args = type_inspect_seed
+        if origin_type is list:
+            assert isinstance(data, list)
+            return [typecast(item, type_args) for item in data]
+        elif origin_type == Union:
+            error_list = []
+            for type_arg in type_args:
+                try:
+                    return typecast(data, type_arg)
+                except Exception as e:
+                    error_list.append(str(e))
+            raise TypeCastError(
+                f'{data=} is not any instance of {tp=}: ' + '; '.join(error_list))
+        elif origin_type == dict:
+            assert isinstance(data, dict)
+            optional_keys = getattr(tp, '__optional_keys__')
+            if optional_keys:
+                required_keys = set(type_args.keys()) - optional_keys
             else:
-                raise JSONDecodeError(f'type {tp=} is not supported ({data=})')
+                required_keys = getattr(tp, '__required_keys__', set())
+            missing_keys = required_keys - set(data.keys())
+            none_value_keys = set()
+            result = {}
+            for item_key, item_value in data.items():
+                if item_key not in type_args:
+                    raise TypeCastError(
+                        f'{item_key=} is not member of {tp=}')
+                result[item_key] = typecast(
+                    item_value, type_args[item_key])
+            for item_key in missing_keys:
+                if typing_inspect.is_optional_type(type_args[item_key]):
+                    result[item_key] = None
+                    none_value_keys.add(item_key)
+            if missing_keys - none_value_keys:
+                raise TypeCastError(
+                    f'missing required keys {list(missing_keys - none_value_keys)}')
+            return result
         else:
-            raise JSONDecodeError(f'{data=} is not instance of {tp=}')
+            raise TypeCastError(f'type {tp=} is not supported ({data=})')
 
 
 def echo_typing_inspect():
     import typing
     int_args = typing_inspect.get_args(int)
     int_origin = typing_inspect.get_origin(int)
     print(f'{int_args=}')  # int_args=()
@@ -162,49 +185,65 @@
     list_origin = typing_inspect.get_origin(list)
     print(f'{list_args=}')  # list_args=()
     print(f'{list_origin=}')  # list_origin=None
     list_int_args = typing_inspect.get_args(list[int])
     list_int_origin = typing_inspect.get_origin(list[int])
     print(f'{list_int_args=}')  # list_int_args=(<class 'int'>,)
     print(f'{list_int_origin=}')  # list_int_origin=<class 'list'>
-    int_optional_args = typing_inspect.get_args(int | None)
-    int_optional_origin = typing_inspect.get_origin(int | None)
-    is_optional = typing_inspect.is_optional_type(int | None)
-    print(f'{int_optional_args=}')  # int_optional_args=(<class 'int'>, <class 'NoneType'>)
-    print(f'{int_optional_origin=}')  # int_optional_origin=None
-    print(f'{is_optional=}')  # is_optional=True
-    union_optional_args = typing_inspect.get_args(int | str)
-    union_optional_origin = typing_inspect.get_origin(int | str)
-    print(f'{union_optional_args=}')  # union_optional_args=(<class 'int'>, <class 'str'>)
-    print(f'{union_optional_origin=}')  # union_optional_origin=None
+    if sys.version_info[:2] >= (3, 11):
+        int_optional_args = typing_inspect.get_args(int | None)
+        int_optional_origin = typing_inspect.get_origin(int | None)
+        is_optional = typing_inspect.is_optional_type(int | None)
+        # int_optional_args=(<class 'int'>, <class 'NoneType'>)
+        print(f'{int_optional_args=}')
+        print(f'{int_optional_origin=}')  # int_optional_origin=None
+        print(f'{is_optional=}')  # is_optional=True
+
+        union_optional_args = typing_inspect.get_args(int | str)
+        union_optional_origin = typing_inspect.get_origin(int | str)
+        # union_optional_args=(<class 'int'>, <class 'str'>)
+        print(f'{union_optional_args=}')
+        print(f'{union_optional_origin=}')  # union_optional_origin=None
+
     union_optional_args = typing_inspect.get_args(Union[int, str])
     union_optional_origin = typing_inspect.get_origin(Union[int, str])
-    print(f'{union_optional_args=}')  # union_optional_args=(<class 'int'>, <class 'str'>)
+    # union_optional_args=(<class 'int'>, <class 'str'>)
+    print(f'{union_optional_args=}')
     print(f'{union_optional_origin=}')  # union_optional_origin=typing.Union
+
+    literral_args = typing_inspect.get_args(Literal['a', 'b'])
+    literal_origin = typing_inspect.get_origin(Literal['a', 'b'])
+    print(f'{literral_args=}')  # literral_args=('a', 'b')
+    print(f'{literal_origin=}')  # literal_origin=typing.Literal
+
     class Pet(typing.TypedDict):
         name: str
         age: int
     pet_optional_args = typing_inspect.get_args(Pet)
     pet_optional_origin = typing_inspect.get_origin(Pet)
     is_dict = issubclass_safe(Pet, dict)
     print(f'{pet_optional_args=}')  # pet_optional_args=()
     print(f'{pet_optional_origin=}')  # pet_optional_origin=None
-    print(f'{is_dict=} {get_type_hints(Pet)} {get_type_hints(dict)}')  # is_dict=True {'name': <class 'str'>, 'age': <class 'int'>} {}
+    # is_dict=True {'name': <class 'str'>, 'age': <class 'int'>} {}
+    print(f'{is_dict=} {get_type_hints(Pet)} {get_type_hints(dict)}')
     is_list = issubclass_safe(list[int], list)
     print(f'{is_list=}')  # is_list=False
-    print(f'is_list={is_list_type(List[int])} {is_list_type(List)}')  # is_list=True
+    # is_list=True
+    print(f'is_list={is_list_type(List[int])} {is_list_type(List)}')
 
 
 def test_typecast():
     import typing
+
     class Pet(typing.TypedDict):
         name: str
         size: list[int]
-        child: Union[list['test_typecast.<locals>.Pet'], None]
-    data = {'name': 'duck', 'size': '10,20,15', 'child': [{'name': 'duckII', 'size': '5,10,8', 'child': None}]}
+        child: Union[list['test_typecast.<locals>.Pet'], None]  # type: ignore
+    data = {'name': 'duck', 'size': '10,20,15', 'child': [
+        {'name': 'duckII', 'size': '5,10,8', 'child': None}]}
     pet = typecast(data, Pet)
     print(pet)
 
 
 if __name__ == '__main__':
-    # echo_typing_inspect()
-    test_typecast()
+    echo_typing_inspect()
+    # test_typecast()
```

### Comparing `lessweb-1.0.8/pyproject.toml` & `lessweb-1.1.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
-requires = ["setuptools"]
+requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lessweb"
-version = "1.0.8"
+version = "1.1.0"
 description = 'A pythonic web framework'
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 keywords = ['lessweb', 'web', 'web.py', 'aiohttp']
 authors = [
     {name = "qorzj", email = "goodhorsezxj@gmail.com"},
 ]
 license = {text = "Apache 2"}
 dependencies = [
     "aiohttp",
```

