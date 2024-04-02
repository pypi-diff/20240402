# Comparing `tmp/comfy_catapult-1.0.2.tar.gz` & `tmp/comfy_catapult-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comfy_catapult-1.0.2.tar", last modified: Mon Mar  4 02:23:44 2024, max compression
+gzip compressed data, was "comfy_catapult-2.0.0.tar", last modified: Tue Apr  2 19:24:00 2024, max compression
```

## Comparing `comfy_catapult-1.0.2.tar` & `comfy_catapult-2.0.0.tar`

### file list

```diff
@@ -1,35 +1,34 @@
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-03-04 02:23:44.166710 comfy_catapult-1.0.2/
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-01-11 16:26:42.000000 comfy_catapult-1.0.2/LICENSE.md
--rwxrwxrwx   0 realz     (1000) realz     (1000)    12515 2024-03-04 02:23:44.159150 comfy_catapult-1.0.2/PKG-INFO
--r-xr-xr-x   0 realz     (1000) realz     (1000)    11414 2024-03-04 02:20:57.000000 comfy_catapult-1.0.2/README.md
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-03-04 02:23:44.031974 comfy_catapult-1.0.2/comfy_catapult/
--rwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-01-11 16:26:42.000000 comfy_catapult-1.0.2/comfy_catapult/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    11679 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/api_client.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     6464 2024-02-19 01:20:59.000000 comfy_catapult-1.0.2/comfy_catapult/api_client_base.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    29814 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/catapult.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     3282 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/catapult_base.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1600 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/comfy_config.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    14219 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/comfy_schema.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)      821 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/comfy_schema_test.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    14545 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/comfy_utils.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     2195 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/errors.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     5983 2024-01-06 03:17:37.000000 comfy_catapult-1.0.2/comfy_catapult/eta_estimator.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     2405 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/remote_file_api_base.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)    11488 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/remote_file_api_comfy.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     8109 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/remote_file_api_comfy_test.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     5111 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/remote_file_api_generic.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     5627 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/remote_file_api_local.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     6090 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/url_utils.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     7533 2024-03-04 02:18:35.000000 comfy_catapult-1.0.2/comfy_catapult/url_utils_test.py
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-03-04 02:23:44.150053 comfy_catapult-1.0.2/comfy_catapult.egg-info/
--rwxrwxrwx   0 realz     (1000) realz     (1000)    12515 2024-03-04 02:23:43.000000 comfy_catapult-1.0.2/comfy_catapult.egg-info/PKG-INFO
--rwxrwxrwx   0 realz     (1000) realz     (1000)      893 2024-03-04 02:23:43.000000 comfy_catapult-1.0.2/comfy_catapult.egg-info/SOURCES.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-03-04 02:23:43.000000 comfy_catapult-1.0.2/comfy_catapult.egg-info/dependency_links.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)      339 2024-03-04 02:23:43.000000 comfy_catapult-1.0.2/comfy_catapult.egg-info/requires.txt
--rwxrwxrwx   0 realz     (1000) realz     (1000)       24 2024-03-04 02:23:43.000000 comfy_catapult-1.0.2/comfy_catapult.egg-info/top_level.txt
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-03-04 02:23:43.792022 comfy_catapult-1.0.2/examples/
-drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-03-04 02:23:44.132470 comfy_catapult-1.0.2/examples/utilities/
--rwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-01-11 16:26:42.000000 comfy_catapult-1.0.2/examples/utilities/__init__.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)     6227 2024-02-01 21:10:02.000000 comfy_catapult-1.0.2/examples/utilities/sdxlturbo_parse_args.py
--rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-03-04 02:23:44.168716 comfy_catapult-1.0.2/setup.cfg
--rwxrwxrwx   0 realz     (1000) realz     (1000)     1262 2024-03-04 02:19:09.000000 comfy_catapult-1.0.2/setup.py
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-02 19:24:00.272452 comfy_catapult-2.0.0/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1102 2024-01-11 16:26:42.000000 comfy_catapult-2.0.0/LICENSE.md
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    24255 2024-04-02 19:24:00.263341 comfy_catapult-2.0.0/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    17215 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/README.md
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-02 19:24:00.123517 comfy_catapult-2.0.0/comfy_catapult/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-01-11 16:26:42.000000 comfy_catapult-2.0.0/comfy_catapult/__init__.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    13665 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/api_client.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     6464 2024-02-19 01:20:59.000000 comfy_catapult-2.0.0/comfy_catapult/api_client_base.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    30008 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/catapult.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     3291 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/catapult_base.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    16582 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/comfy_schema.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     4859 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/comfy_schema_test.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    15682 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/comfy_utils.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     2237 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/errors.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     5983 2024-01-06 03:17:37.000000 comfy_catapult-2.0.0/comfy_catapult/eta_estimator.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     2325 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/remote_file_api_base.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    11630 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/remote_file_api_comfy.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     8441 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/remote_file_api_comfy_test.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     5634 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/remote_file_api_generic.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     5772 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/remote_file_api_local.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     4188 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/url_utils.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      377 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/comfy_catapult/url_utils_test.py
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-02 19:24:00.245200 comfy_catapult-2.0.0/comfy_catapult.egg-info/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)    24255 2024-04-02 19:23:59.000000 comfy_catapult-2.0.0/comfy_catapult.egg-info/PKG-INFO
+-rwxrwxrwx   0 realz     (1000) realz     (1000)      868 2024-04-02 19:23:59.000000 comfy_catapult-2.0.0/comfy_catapult.egg-info/SOURCES.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)        1 2024-04-02 19:23:59.000000 comfy_catapult-2.0.0/comfy_catapult.egg-info/dependency_links.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     1929 2024-04-02 19:23:59.000000 comfy_catapult-2.0.0/comfy_catapult.egg-info/requires.txt
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       15 2024-04-02 19:23:59.000000 comfy_catapult-2.0.0/comfy_catapult.egg-info/top_level.txt
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-02 19:23:59.860027 comfy_catapult-2.0.0/examples/
+drwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-04-02 19:24:00.225127 comfy_catapult-2.0.0/examples/utilities/
+-rwxrwxrwx   0 realz     (1000) realz     (1000)        0 2024-01-11 16:26:42.000000 comfy_catapult-2.0.0/examples/utilities/__init__.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     6227 2024-02-01 21:10:02.000000 comfy_catapult-2.0.0/examples/utilities/sdxlturbo_parse_args.py
+-rwxrwxrwx   0 realz     (1000) realz     (1000)     4122 2024-04-02 19:19:54.000000 comfy_catapult-2.0.0/pyproject.toml
+-rwxrwxrwx   0 realz     (1000) realz     (1000)       38 2024-04-02 19:24:00.273961 comfy_catapult-2.0.0/setup.cfg
```

### Comparing `comfy_catapult-1.0.2/LICENSE.md` & `comfy_catapult-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `comfy_catapult-1.0.2/comfy_catapult/api_client.py` & `comfy_catapult-2.0.0/comfy_catapult/api_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,92 +3,130 @@
 #
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
 import base64
 import json
+import logging
 import textwrap
 from typing import Any, Dict, List, Type, TypeVar
 from urllib.parse import urlencode, urlparse
 
 import aiohttp
+from anyio import Path
 from pydantic import BaseModel
 
 from comfy_catapult.api_client_base import ComfyAPIClientBase
 from comfy_catapult.comfy_schema import (APIHistory, APIObjectInfo,
                                          APIQueueInfo, APISystemStats,
                                          APIUploadImageResp, APIWorkflowTicket,
                                          ClientID, PromptID)
-from comfy_catapult.comfy_utils import TryParseAsModel, YamlDump, _WatchVar
+from comfy_catapult.comfy_utils import TryParseAsModel, WatchVar, YamlDump
 from comfy_catapult.url_utils import JoinToBaseURL
 
+logger = logging.getLogger(__name__)
+
 T = TypeVar('T')
 
 
+async def _TryGetContent(*, resp: aiohttp.ClientResponse) -> str | Exception:
+  try:
+    return await resp.text(errors='replace')
+  except Exception as e:
+    logger.exception('Error getting content', exc_info=e, stack_info=True)
+    return e
+
+
+async def _RaiseForStatus(*,
+                          resp: aiohttp.ClientResponse,
+                          extra: Any | None = None):
+  """Same as raise_for_status(), but also dumps any content in the response into the exception"""
+  try:
+    resp.raise_for_status()
+  except aiohttp.ClientResponseError as e:
+    content_or_exc = await _TryGetContent(resp=resp)
+
+    message = e.message
+    if isinstance(content_or_exc, str):
+      message += f'\n\nContent (raw): {textwrap.indent(content_or_exc, prefix="  ")}'
+    else:
+      message += f'\n\nError getting content: {content_or_exc}'
+    if extra is not None:
+      message += f'\n\nExtra info: {textwrap.indent(YamlDump(extra), prefix="  ")}'
+
+    raise aiohttp.ClientResponseError(request_info=e.request_info,
+                                      history=e.history,
+                                      code=e.code,
+                                      status=e.status,
+                                      message=message,
+                                      headers=e.headers) from e
+
+
 async def _TryParseAsJson(*, content: str, json_type: Type[T]) -> T:
   try:
     result = json.loads(content)
     if not isinstance(result, json_type):
       raise TypeError(f'Expected {json_type}, got {type(result)}')
     return result
   except json.JSONDecodeError as e:
     raise Exception(
         f'Error: {e}\n\nContent (raw): {textwrap.indent(content, prefix="  ")}'
     ) from e
 
 
 async def _TryParseRespAsJson(*, resp: aiohttp.ClientResponse,
                               json_type: Type[T]) -> T:
-  # Raise if error
-  resp.raise_for_status()
-
   content_bytes = b''
   content_str: str = ''
   content: T | None = None
   try:
     content_bytes = await resp.content.read()
     content_str = content_bytes.decode('utf-8')
     if resp.content_type != 'application/json':
       raise Exception(
           f'Error: {resp.status} {resp.reason}'
           f'\n\nExpected content-type: application/json, got {resp.content_type}'
           f'\n\nContent (raw):\n{textwrap.indent(content_str, prefix="  ")}')
 
     content = await _TryParseAsJson(content=content_str, json_type=json_type)
-    if resp.status != 200:
-      raise Exception(
-          f'Error: {resp.status} {resp.reason}'
-          f'\n\nContent (yaml):\n{textwrap.indent(YamlDump(content), prefix="  ")}'
-      )
+    if resp.ok:
+      await _RaiseForStatus(resp=resp, extra=content)
     return content
   except Exception as e:
     contentb64 = base64.b64encode(content_bytes).decode('utf-8')
     raise Exception(
         f'Error: {resp.status} {resp.reason}'
         f'\n\nContent (raw):\n{textwrap.indent(content_str, prefix="  ")}'
         f'\n\nContent (yaml):\n{textwrap.indent(YamlDump(content), prefix="  ")}'
         f'\n\nContent (base64):\n{textwrap.indent(contentb64, prefix="  ")}'
     ) from e
 
 
 _BaseModelT = TypeVar('_BaseModelT', bound=BaseModel)
 
 
-async def _TryParseRespAsModel(*, resp: aiohttp.ClientResponse,
-                               model_type: Type[_BaseModelT]) -> _BaseModelT:
+async def _TryParseRespAsModel(
+    *, resp: aiohttp.ClientResponse, model_type: Type[_BaseModelT],
+    errors_dump_directory: Path | None) -> _BaseModelT:
   content: Any = await _TryParseRespAsJson(resp=resp, json_type=dict)
-  return await TryParseAsModel(content=content, model_type=model_type)
+  return await TryParseAsModel(content=content,
+                               model_type=model_type,
+                               errors_dump_directory=errors_dump_directory)
 
 
 class ComfyAPIClient(ComfyAPIClientBase):
 
-  def __init__(self, *, comfy_api_url: str):
+  def __init__(self,
+               comfy_api_url: str,
+               *,
+               errors_dump_directory: Path | None = None):
     self._comfy_api_url = comfy_api_url
     self._session = aiohttp.ClientSession()
+    self._errors_dump_directory = errors_dump_directory
 
   async def __aenter__(self):
     await self._session.__aenter__()
     return self
 
   async def __aexit__(self, exc_type, exc, tb):
     await self._session.__aexit__(exc_type, exc, tb)
@@ -98,39 +136,45 @@
     await self._session.close()
 
   def GetURL(self) -> str:
     return self._comfy_api_url
 
   async def GetSystemStatsRaw(self) -> dict:
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'system_stats'))
-    with _WatchVar(url=url.geturl()):
+    with WatchVar(url=url.geturl()):
       async with self._session.get(url.geturl()) as resp:
         return await _TryParseRespAsJson(resp=resp, json_type=dict)
 
   async def GetSystemStats(self) -> APISystemStats:
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'system_stats'))
-    with _WatchVar(url=url.geturl()):
+    with WatchVar(url=url.geturl()):
       async with self._session.get(url.geturl()) as resp:
-        return await _TryParseRespAsModel(resp=resp, model_type=APISystemStats)
+        return await _TryParseRespAsModel(
+            resp=resp,
+            model_type=APISystemStats,
+            errors_dump_directory=self._errors_dump_directory)
 
   async def GetObjectInfoRaw(self) -> dict:
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'object_info'))
-    with _WatchVar(url=url.geturl()):
+    with WatchVar(url=url.geturl()):
       async with self._session.get(url.geturl()) as resp:
         return await _TryParseRespAsJson(resp=resp, json_type=dict)
 
   async def GetObjectInfo(self) -> APIObjectInfo:
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'object_info'))
-    with _WatchVar(url=url.geturl()):
+    with WatchVar(url=url.geturl()):
       async with self._session.get(url.geturl()) as resp:
-        return await _TryParseRespAsModel(resp=resp, model_type=APIObjectInfo)
+        return await _TryParseRespAsModel(
+            resp=resp,
+            model_type=APIObjectInfo,
+            errors_dump_directory=self._errors_dump_directory)
 
   async def GetPromptRaw(self) -> dict:
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'prompt'))
-    with _WatchVar(url=url.geturl()):
+    with WatchVar(url=url.geturl()):
       async with self._session.get(url.geturl()) as resp:
         return await _TryParseRespAsJson(resp=resp, json_type=dict)
 
   async def PostPromptRaw(self,
                           *,
                           prompt_workflow: dict,
                           number: int | None = None,
@@ -146,15 +190,15 @@
     if prompt_id is not None:
       body['prompt_id'] = prompt_id
     if extra_data is not None:
       body['extra_data'] = extra_data
 
     data: bytes = json.dumps(body).encode('utf-8')
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'prompt'))
-    with _WatchVar(url=url.geturl()):
+    with WatchVar(url=url.geturl()):
       async with self._session.post(url.geturl(), data=data) as resp:
         return await _TryParseRespAsJson(resp=resp, json_type=dict)
 
   async def PostPrompt(self,
                        *,
                        prompt_workflow: dict,
                        number: int | None = None,
@@ -162,46 +206,55 @@
                        prompt_id: PromptID | None = None,
                        extra_data: dict | None = None) -> APIWorkflowTicket:
     ticket = await self.PostPromptRaw(prompt_workflow=prompt_workflow,
                                       number=number,
                                       client_id=client_id,
                                       prompt_id=prompt_id,
                                       extra_data=extra_data)
-    return await TryParseAsModel(content=ticket, model_type=APIWorkflowTicket)
+    return await TryParseAsModel(
+        content=ticket,
+        model_type=APIWorkflowTicket,
+        errors_dump_directory=self._errors_dump_directory)
 
   async def GetHistoryRaw(self,
                           *,
                           prompt_id: PromptID | None = None,
                           max_items: int | None = None) -> dict:
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'history'))
     if max_items is not None:
       url = url._replace(query=f'max_items={max_items}')
     if prompt_id is not None:
       url = url._replace(path=f'{url.path}/{prompt_id}')
 
-    with _WatchVar(url=url.geturl()):
+    with WatchVar(url=url.geturl()):
       async with self._session.get(url.geturl()) as resp:
         return await _TryParseRespAsJson(resp=resp, json_type=dict)
 
   async def GetHistory(self,
                        *,
                        prompt_id: PromptID | None = None,
                        max_items: int | None = None) -> APIHistory:
     history = await self.GetHistoryRaw(prompt_id=prompt_id, max_items=max_items)
-    return await TryParseAsModel(content=history, model_type=APIHistory)
+    return await TryParseAsModel(
+        content=history,
+        model_type=APIHistory,
+        errors_dump_directory=self._errors_dump_directory)
 
   async def GetQueueRaw(self) -> dict:
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'queue'))
-    with _WatchVar(url=url.geturl()):
+    with WatchVar(url=url.geturl()):
       async with self._session.get(url.geturl()) as resp:
         return await _TryParseRespAsJson(resp=resp, json_type=dict)
 
   async def GetQueue(self) -> APIQueueInfo:
     queue: dict = await self.GetQueueRaw()
-    return await TryParseAsModel(content=queue, model_type=APIQueueInfo)
+    return await TryParseAsModel(
+        content=queue,
+        model_type=APIQueueInfo,
+        errors_dump_directory=self._errors_dump_directory)
 
   async def PostUploadImageRaw(self, *, folder_type: str, subfolder: str,
                                filename: str, data: bytes,
                                overwrite: bool) -> dict:
     """
 
     * See https://github.com/comfyanonymous/ComfyUI/blob/0c2c9fbdfa53c2ad3b7658a7f2300da831830388/server.py#L203
@@ -214,29 +267,29 @@
         filename (str): _description_
         data (bytes): _description_
         overwrite (bool): _description_
 
     Returns:
         dict: _description_
     """
-    with _WatchVar(folder_type=folder_type,
-                   subfolder=subfolder,
-                   filename=filename,
-                   overwrite=overwrite):
+    with WatchVar(folder_type=folder_type,
+                  subfolder=subfolder,
+                  filename=filename,
+                  overwrite=overwrite):
       fdata = aiohttp.FormData()
       fdata.add_field('image',
                       data,
                       filename=filename,
                       content_type='application/octet-stream')
       fdata.add_field('overwrite', str(overwrite).lower())
       fdata.add_field('subfolder', subfolder)
       fdata.add_field('type', folder_type)
       fdata.add_field('filename', filename)
       post_url = urlparse(JoinToBaseURL(self._comfy_api_url, 'upload/image'))
-      with _WatchVar(post_url=post_url.geturl(), fdata=fdata):
+      with WatchVar(post_url=post_url.geturl(), fdata=fdata):
         async with self._session.post(post_url.geturl(), data=fdata) as resp:
           result = await _TryParseRespAsJson(resp=resp, json_type=dict)
           if not isinstance(result, dict):
             # Server should never return a list or something other than a
             # dictionary.
             raise TypeError(f'Expected dict, got {type(result)}')
           return result
@@ -245,39 +298,43 @@
                             filename: str, data: bytes,
                             overwrite: bool) -> APIUploadImageResp:
     result = await self.PostUploadImageRaw(folder_type=folder_type,
                                            subfolder=subfolder,
                                            filename=filename,
                                            data=data,
                                            overwrite=overwrite)
-    return await TryParseAsModel(content=result, model_type=APIUploadImageResp)
+    return await TryParseAsModel(
+        content=result,
+        model_type=APIUploadImageResp,
+        errors_dump_directory=self._errors_dump_directory)
 
   async def GetView(self, *, folder_type: str, subfolder: str,
                     filename: str) -> bytes:
     data = {'filename': filename, 'subfolder': subfolder, 'type': folder_type}
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'view'))
     url = url._replace(query=urlencode(data))
 
-    with _WatchVar(url=url.geturl()):
+    with WatchVar(url=url.geturl()):
       async with self._session.get(url.geturl()) as resp:
+        await _RaiseForStatus(resp=resp)
         return await resp.content.read()
 
   async def PostFree(self, *, unload_models: bool, free_memory: bool):
     data = {'unload_models': unload_models, 'free_memory': free_memory}
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'free'))
-    with _WatchVar(url=url.geturl()):
+    with WatchVar(url=url.geturl()):
       async with self._session.post(url.geturl(), data=data) as resp:
-        resp.raise_for_status()
+        await _RaiseForStatus(resp=resp)
 
   async def PostInterrupt(self):
     # TODO(realazthat/comfy-catapult#5): change the API to take a prompt_id.
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'interrupt'))
-    with _WatchVar(url=url.geturl()):
+    with WatchVar(url=url.geturl()):
       async with self._session.post(url.geturl()) as resp:
         resp.raise_for_status()
 
   async def PostQueue(self, *, delete: List[PromptID], clear: bool):
     url = urlparse(JoinToBaseURL(self._comfy_api_url, 'queue'))
     data = {'delete': delete, 'clear': clear}
-    with _WatchVar(url=url.geturl()):
+    with WatchVar(url=url.geturl()):
       async with self._session.post(url.geturl(), data=data) as resp:
         resp.raise_for_status()
```

### Comparing `comfy_catapult-1.0.2/comfy_catapult/api_client_base.py` & `comfy_catapult-2.0.0/comfy_catapult/api_client_base.py`

 * *Files identical despite different names*

### Comparing `comfy_catapult-1.0.2/comfy_catapult/catapult.py` & `comfy_catapult-2.0.0/comfy_catapult/catapult.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
 import asyncio
 import datetime
 import enum
 import json
-import sys
+import logging
 import textwrap
 import threading
-import traceback
 import traceback as tb
 import uuid
 from copy import deepcopy
 from dataclasses import dataclass
 from pprint import pformat
 from typing import Any, Dict, Generic, List, Sequence, Tuple, TypeVar
 from urllib.parse import ParseResult, urlparse
@@ -25,31 +24,33 @@
 from anyio import Path
 from slugify import slugify
 from websockets import WebSocketClientProtocol, connect
 
 from comfy_catapult.api_client import ComfyAPIClientBase, YamlDump
 from comfy_catapult.catapult_base import ComfyCatapultBase, JobStatus, Progress
 from comfy_catapult.comfy_schema import (APIHistory, APIHistoryEntry,
-                                         APIHistoryEntryStatusNote,
+                                         APIHistoryEntryStatusNote, APINodeID,
                                          APIQueueInfo, APISystemStats,
-                                         APIWorkflowTicket, NodeID, WSMessage)
+                                         APIWorkflowTicket, WSMessage)
 from comfy_catapult.comfy_utils import TryParseAsModel
 from comfy_catapult.errors import NodesNotExecuted, WorkflowSubmissionError
 
+logger = logging.getLogger(__name__)
+
 
 @dataclass
 class _Job:
 
   class RemoteStatus(enum.Enum):
     NONE = enum.auto()
     PENDING_OR_RUNNING = enum.auto()
 
   job_id: str
   prepared_workflow: dict
-  important_nodes: Tuple[NodeID, ...]
+  important_nodes: Tuple[APINodeID, ...]
   ticket: APIWorkflowTicket | None
   status: JobStatus
   # Exceptions that should be in status but aren't because they're not pickable
   # or deepcopyable.
   errors: List[Exception]
   future: asyncio.Future[dict]
   remote_job_status: RemoteStatus
@@ -64,16 +65,16 @@
   value: T | None
   updated: datetime.datetime
 
 
 class ComfyCatapult(ComfyCatapultBase):
 
   def __init__(self,
-               *,
                comfy_client: ComfyAPIClientBase,
+               *,
                debug_path: Path | None,
                debug_save_all: bool = False):
     """_summary_
 
     Args:
         comfy_client (ComfyAPIClientBase): _description_
         debug_path (Path | None): For logging of certain debug information, in
@@ -140,15 +141,15 @@
       pass
 
   async def Catapult(
       self,
       *,
       job_id: str,
       prepared_workflow: dict,
-      important: Sequence[NodeID],
+      important: Sequence[APINodeID],
       job_debug_path: Path | None = None,
   ) -> dict:
     async with self._lock:
       if job_id in self._jobs:
         raise KeyError(f'User job id {repr(job_id)} already exists')
       if not slugify(job_id) == job_id:
         raise ValueError(
@@ -176,18 +177,16 @@
                            errored=None,
                            cancelled=None),
           errors=[],
           remote_job_status=_Job.RemoteStatus.PENDING_OR_RUNNING,
           job_debug_path=job_debug_path)
 
     async with _JobContext(job_id=job_id, comfy=self):
-      print('self._client.PostPrompt()', file=sys.stderr)
       ticket: APIWorkflowTicket = await self._comfy_client.PostPrompt(
           prompt_workflow=prepared_workflow)
-      print('self._client.PostPrompt(), done', file=sys.stderr)
 
       async with self._lock:
         self._jobs[job_id].ticket = ticket
         if ticket.prompt_id is not None:
           self._prompt_id_index[ticket.prompt_id] = job_id
 
       has_errors = False
@@ -274,23 +273,25 @@
     async with self._lock:
       self._jobs[job_id].status = self._jobs[job_id].status._replace(
           job_history=job_history)
 
     ##########################################################################
     # Get outputs_to_execute, outputs_with_data, extra_data
     extra_data: dict | None = None
-    outputs_to_execute: List[NodeID] = []
-    outputs_with_data: List[NodeID] = []
+    outputs_to_execute: List[APINodeID] = []
+    outputs_with_data: List[APINodeID] = []
     if job_history.outputs is not None:
       outputs_with_data = list(job_history.outputs.keys())
     if job_history.prompt is not None:
       if job_history.prompt.extra_data is not None:
         extra_data = job_history.prompt.extra_data
       if job_history.prompt.outputs_to_execute is not None:
         outputs_to_execute = job_history.prompt.outputs_to_execute
+    logger.debug('extra_data: %s', YamlDump(extra_data))
+
     if job_history.status is not None:
       if job_history.status.completed is False:
         notes: List[str] = []
         if job_history.status.messages is not None:
           note: APIHistoryEntryStatusNote
           for note in job_history.status.messages:
             notes.append(textwrap.indent(pformat(note._asdict()), prefix='  '))
@@ -298,55 +299,50 @@
         # TODO: Make all exceptions going forward contain the metadata that
         # NodesNotExecuted does.
         raise Exception('Job has failed'
                         f'\n  status: {repr(job_history.status)}'
                         f'\n  notes:' + '\n'.join(notes))
 
     ##########################################################################
-    print('job_history.prompt.extra_data.model_dump():', file=sys.stderr)
-    print(YamlDump(extra_data), file=sys.stderr)
+    logger.debug('job_history.prompt.extra_data.model_dump(): %s',
+                 YamlDump(extra_data))
+    logger.debug('job_history.prompt.outputs_to_execute.model_dump(): %s',
+                 YamlDump(outputs_to_execute))
 
-    print('job_history.prompt.outputs_to_execute.model_dump():',
-          file=sys.stderr)
-    print(YamlDump(outputs_to_execute), file=sys.stderr)
-
-    print('outputs_to_execute:', file=sys.stderr)
-    print(YamlDump(outputs_to_execute), file=sys.stderr)
-    print('outputs_that_executed:', file=sys.stderr)
-    print(YamlDump(outputs_with_data), file=sys.stderr)
+    logger.debug('outputs_to_execute: %s', YamlDump(outputs_to_execute))
+    logger.debug('outputs_that_executed: %s', YamlDump(outputs_with_data))
 
     bad_dataless_outputs = [
         node_id for node_id in outputs_to_execute
         if node_id not in outputs_with_data
     ]
 
-    def _GetTitles(node_ids: List[NodeID]) -> List[str | None]:
+    def _GetTitles(node_ids: List[APINodeID]) -> List[str | None]:
       titles = []
       for node_id in node_ids:
         node_info: dict = prepared_workflow.get(node_id, {})
         meta: dict = node_info.get('_meta', {})
         title: str | None = meta.get('title', None)
         titles.append(title)
       return titles
 
     if len(bad_dataless_outputs) > 0:
-      print('bad_dataless_outputs:', file=sys.stderr)
-      print(YamlDump(bad_dataless_outputs), file=sys.stderr)
-      print('_GetTitles(bad_dataless_outputs):', file=sys.stderr)
-      print(YamlDump(_GetTitles(bad_dataless_outputs)), file=sys.stderr)
+      logger.error('bad_dataless_outputs: %s', YamlDump(bad_dataless_outputs))
+      logger.error('_GetTitles(bad_dataless_outputs): %s',
+                   YamlDump(_GetTitles(bad_dataless_outputs)))
 
     dataless_important_outputs = [
         node_id for node_id in bad_dataless_outputs
         if node_id in important_nodes
     ]
     if len(dataless_important_outputs) > 0:
-      print('dataless_important_outputs:', file=sys.stderr)
-      print(YamlDump(dataless_important_outputs), file=sys.stderr)
-      print('_GetTitles(dataless_important_outputs):', file=sys.stderr)
-      print(YamlDump(_GetTitles(dataless_important_outputs)), file=sys.stderr)
+      logger.error('dataless_important_outputs: %s',
+                   YamlDump(dataless_important_outputs))
+      logger.error('_GetTitles(dataless_important_outputs): %s',
+                   YamlDump(_GetTitles(dataless_important_outputs)))
       raise NodesNotExecuted(nodes=list(dataless_important_outputs),
                              titles=_GetTitles(dataless_important_outputs))
 
     # await self._eta_estimator.RecordFinished(job_id=job_id)
 
     now = self._Now()
     async with self._lock:
@@ -373,15 +369,15 @@
         async with self._lock:
           job = self._jobs[job_id]
           # See if an error occurred.
           job.future.result()
           job.status = job.status._replace(success=self._Now())
     ############################################################################
     system_stats: APISystemStats = await self._comfy_client.GetSystemStats()
-    print(YamlDump(system_stats.model_dump()), file=sys.stderr)
+    logger.info('system_stats: %s', YamlDump(system_stats.model_dump()))
     ############################################################################
     queue_info: APIQueueInfo = await self._comfy_client.GetQueue()
 
     prompt_id_2_status: Dict[str, str] = {}
     for pending in queue_info.queue_running:
       prompt_id_2_status[pending.prompt_id] = 'running'
     for running in queue_info.queue_pending:
@@ -389,16 +385,16 @@
     pending_count = sum(
         [1 for status in prompt_id_2_status.values() if status == 'pending'],
         start=0)
     running_count = sum(
         [1 for status in prompt_id_2_status.values() if status == 'running'],
         start=0)
 
-    print('pending_count:', pending_count, file=sys.stderr)
-    print('running_count:', running_count, file=sys.stderr)
+    logger.info('pending_count: %s', pending_count)
+    logger.info('running_count: %s', running_count)
 
     for prompt_id, status in prompt_id_2_status.items():
       async with self._lock:
         job_id = self._prompt_id_index.get(prompt_id, None)
         if job_id is None:
           continue
         job: _Job = self._jobs[job_id]
@@ -411,26 +407,27 @@
           self._guess_currently_running_job_id = _Guess(value=job_id,
                                                         updated=self._Now())
           self._guess_currently_running_node_id = _Guess(value=None,
                                                          updated=self._Now())
           self._guess_currently_running_node_progress = _Guess(
               value=None, updated=self._Now())
 
+    # TODO: Reenable this or remove it.
     # print('self._jobs:', file=sys.stderr)
     # pprint(self._jobs, indent=2, stream=sys.stderr)
 
     ############################################################################
     prompt_info: dict = await self._comfy_client.GetPromptRaw()
 
     exec_info = prompt_info['exec_info']
     queue_remaining = exec_info['queue_remaining']
     if not isinstance(queue_remaining, int):
       raise AssertionError(
           f'queue_remaining must be int, not {type(queue_remaining)}')
-    print('queue_remaining:', queue_remaining, file=sys.stderr)
+    logger.info('queue_remaining: %s', queue_remaining)
     ############################################################################
     # Check the /history endpoint to see if there are any updates on our jobs.
 
     # Update job.remote_job_status.
     for job_id in await self._GetJobIDs():
       async with self._lock:
         new_remote_job_status = (_Job.RemoteStatus.NONE
@@ -454,22 +451,28 @@
         prompt_id: str | None = None
         if ticket is not None:
           prompt_id = ticket.prompt_id
 
         if prompt_id is None:
           # This should never happen, but :shrug:.
           continue
+        job_debug_path = self._jobs[job_id].job_debug_path
+        errors_dump_directory: Path | None = None
+        if job_debug_path is not None:
+          errors_dump_directory = job_debug_path / 'errors'
 
       ##########################################################################
       async with _JobContext(job_id=job_id, comfy=self) as job_context:
         history_raw: dict = await self._comfy_client.GetHistoryRaw(
             prompt_id=prompt_id)
         await job_context.WatchVar(history_raw=history_raw)
-        history: APIHistory = await TryParseAsModel(content=history_raw,
-                                                    model_type=APIHistory)
+        history: APIHistory = await TryParseAsModel(
+            content=history_raw,
+            model_type=APIHistory,
+            errors_dump_directory=errors_dump_directory)
         await self._ReceivedJobHistory(job_id=job_id,
                                        history=history,
                                        job_context=job_context)
       ##########################################################################
 
   def _Now(self) -> datetime.datetime:
     return datetime.datetime.now(datetime.timezone.utc)
@@ -482,25 +485,30 @@
 
     if guess_currently_running_job_id.value is not None:
       pass
 
   async def _LoopWS(self, *, ws: WebSocketClientProtocol):
     while True:
       try:
-        print('websocket recv', file=sys.stderr)
+        logger.debug('websocket recv')
         out = await ws.recv()
         if not isinstance(out, str):
-          print('websocket type(out):', type(out), file=sys.stderr)
+          logger.debug('websocket type(out): %s', type(out))
           continue
-        print('websocket raw:', file=sys.stderr)
-        print(YamlDump(out), file=sys.stderr)
-        message = await TryParseAsModel(content=json.loads(out),
-                                        model_type=WSMessage)
-        print('websocket message:', file=sys.stderr)
-        print(YamlDump(message.__dict__), file=sys.stderr)
+        logger.debug('websocket raw: %s', YamlDump(out))
+        errors_dump_directory: Path | None = None
+        async with self._lock:
+          if self._debug_path is not None:
+            errors_dump_directory = self._debug_path / 'errors'
+
+        message = await TryParseAsModel(
+            content=json.loads(out),
+            model_type=WSMessage,
+            errors_dump_directory=errors_dump_directory)
+        logger.debug('websocket message: %s', YamlDump(message.__dict__))
 
         if message.type == 'executing' and 'last_node_id' in message.data:
           last_node_id = message.data['last_node_id']
 
           async with self._lock:
             self._guess_currently_running_node_id = _Guess(value=last_node_id,
                                                            updated=self._Now())
@@ -595,25 +603,25 @@
               self._guess_currently_running_node_progress = _Guess(
                   value=Progress(value=value, max_value=max_value),
                   updated=self._Now())
             await self._Record()
       except asyncio.CancelledError:
         raise
       except Exception:
-        traceback.print_exc(file=sys.stderr)
+        logger.exception('Error in _LoopWS')
 
   async def _PollLoop(self):
     while not self._stop_event.is_set():
       try:
         await asyncio.sleep(5)
         await self._Poll()
       except asyncio.CancelledError:
         raise
       except Exception:
-        traceback.print_exc(file=sys.stderr)
+        logger.exception('Error in _PollLoop')
 
   async def _MonitoringThread(self):
 
     async with self._lock:
       client_id = self._client_id
       comfy_api_url: str = self._comfy_client.GetURL()
       ws_connect_interval: float = self._ws_connect_interval
@@ -633,25 +641,25 @@
           await asyncio.wait_for(self._LoopWS(ws=ws),
                                  timeout=ws_connect_interval)
       except asyncio.TimeoutError:
         pass
       except asyncio.CancelledError:
         raise
       except Exception:
-        traceback.print_exc(file=sys.stderr)
+        logger.exception('Error in _MonitoringThreadLoopOnce')
 
     while not self._stop_event.is_set():
       try:
         await _MonitoringThreadLoopOnce()
       except asyncio.TimeoutError:
         pass
       except asyncio.CancelledError:
         raise
       except Exception:
-        traceback.print_exc(file=sys.stderr)
+        logger.exception('Error in _MonitoringThreadLoopOnce')
 
   async def _CheckError(self):
     async with self._lock:
       if self._monitoring_task.done():
         self._monitoring_task.result()
       if self._poll_task.done():
         self._poll_task.result()
@@ -741,9 +749,8 @@
             'watch_vars': self._watch_vars,
             'workflow': workflow,
         }
         job_dump_path = job_debug_path / 'context-dumps' / f'{slugify(dt)}.dump.yaml'
         await job_dump_path.parent.mkdir(parents=True, exist_ok=True)
         async with aiofiles.open(job_dump_path, 'w') as f:
           await f.write(YamlDump(dump))
-        print(f'Wrote job status to {repr(str(job_dump_path))}.',
-              file=sys.stderr)
+        logger.error(f'Wrote job status to {repr(str(job_dump_path))}.')
```

### Comparing `comfy_catapult-1.0.2/comfy_catapult/catapult_base.py` & `comfy_catapult-2.0.0/comfy_catapult/catapult_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import asyncio
 import datetime
 from abc import ABC, abstractmethod
 from typing import Dict, List, NamedTuple, Sequence, Tuple
 
 from anyio import Path
 
-from comfy_catapult.comfy_schema import NodeID
+from comfy_catapult.comfy_schema import APINodeID
 
 
 class Progress(NamedTuple):
   value: int
   max_value: int
 
 
@@ -62,25 +62,25 @@
 
   @abstractmethod
   async def Catapult(
       self,
       *,
       job_id: str,
       prepared_workflow: dict,
-      important: Sequence[NodeID],
+      important: Sequence[APINodeID],
       job_debug_path: Path | None = None,
   ) -> dict:
     """Schedule a ComfyUI workflow job.
 
     Args:
         job_id (str): A unique identifier for the job. Note: This string must
           be unique, and must be slugified! Use python-slugify to slugify the
           string.
         prepared_workflow (dict): Workflow to submit.
-        important (List[NodeID]): List of important nodes (e.g output nodes we
+        important (List[APINodeID]): List of important nodes (e.g output nodes we
           are interested in).
         job_debug_path (Path, optional): Path to save debug information. If
           None, will use sensible defaults.
 
     Raises:
         WorkflowSubmissionError: Failed to submit workflow.
```

### Comparing `comfy_catapult-1.0.2/comfy_catapult/comfy_schema.py` & `comfy_catapult-2.0.0/comfy_catapult/comfy_schema.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,67 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 #
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
-from typing import Any, Dict, List, NamedTuple
+from typing import Any, Dict, List, Literal, NamedTuple
+from urllib.parse import urljoin
 
-from pydantic import BaseModel, ConfigDict, Field, RootModel
+from pydantic import BaseModel, ConfigDict, Field, RootModel, field_validator
 from typing_extensions import Annotated
 
 EXTRA = 'allow'
 
-NodeID = Annotated[str, Field(alias='node_id')]
-PromptID = Annotated[str, Field(alias='prompt_id')]
+APINodeID = Annotated[
+    str,
+    Field(alias='node_id', description='The ID of a node in a workflow.')]
+PromptID = Annotated[
+    str,
+    Field(
+        alias='prompt_id',
+        description=
+        'The ID of a prompt (submission of a api workflow to the server to be executed). You can choose this yourself when submitting.'
+    )]
 ClientID = Annotated[str, Field(alias='client_id')]
-OutputName = Annotated[str, Field(alias='output_name')]
+OutputName = Annotated[
+    str,
+    Field(
+        alias='output_name',
+        description=
+        'The name of an output in a node, in /history/, /history/{prompt_id} endpoints.'
+    )]
 # This is BOOLEAN, INT etc.
-OutputType = Annotated[str, Field(alias='output_type')]
+OutputType = Annotated[
+    str,
+    Field(
+        alias='output_type',
+        description=
+        'The type of a named output of a node, in /object_info endpoint, and also can be seen/found in {node,custom node} implementations.'
+    )]
 
 # This is BOOLEAN, INT etc.
-NamedInputType = Annotated[str, Field(alias='input_type')]
+NamedInputType = Annotated[
+    str,
+    Field(
+        alias='input_type',
+        description=
+        'The type of a named input of a node, in /object_info endpoint, and also can be seen/found in {node,custom node} implementations.'
+    )]
 # This is a list of valid *values* for a combo input.
 ComboInputType = Annotated[List[Any], Field(alias='combo_input_class')]
+ComfyFolderType = Literal['input', 'output', 'temp']
+VALID_FOLDER_TYPES: List[ComfyFolderType] = ['input', 'output', 'temp']
 
 
 ################################################################################
 class APIWorkflowInConnection(NamedTuple):
   """Represents a connection between two nodes in a workflow. This is used in the input of a node."""
-  output_node_id: NodeID
+  output_node_id: APINodeID
   output_index: int
 
 
 class APIWorkflowNodeMeta(BaseModel):
   """Nodes are allowed to have a `_meta` field.
 
   The meta field was was added in
@@ -60,21 +89,21 @@
   """
 
   inputs: Dict[str, str | int | float | bool | APIWorkflowInConnection | dict]
   class_type: str
   meta: APIWorkflowNodeMeta | None = Field(None, alias='_meta')
 
 
-class APIWorkflow(RootModel[Dict[NodeID, APIWorkflowNodeInfo]]):
+class APIWorkflow(RootModel[Dict[APINodeID, APIWorkflowNodeInfo]]):
   """This is the API format, you get it from `Save (API Format)` in the UI.
 
 
   See test_data/sdxlturbo_example_api.json for an example of this format in json.
   """
-  root: Dict[NodeID, APIWorkflowNodeInfo]
+  root: Dict[APINodeID, APIWorkflowNodeInfo]
 
 
 ################################################################################
 class APISystemStatsSystem(BaseModel):
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
@@ -117,15 +146,15 @@
 
 ################################################################################
 class APIQueueInfoEntry(NamedTuple):
   number: int
   prompt_id: PromptID
   prompt: APIWorkflow
   extra_data: dict
-  outputs_to_execute: List[NodeID]
+  outputs_to_execute: List[APINodeID]
 
 
 class APIQueueInfo(BaseModel):
   """Returned from /queue endpoint."""
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
@@ -155,36 +184,36 @@
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
   class_type: str
-  dependent_outputs: List[NodeID]
+  dependent_outputs: List[APINodeID]
   errors: List[NodeErrorInfo]
 
 
 class APIWorkflowTicket(BaseModel):
   """Return from post /prompt endpoint."""
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
-  node_errors: Dict[NodeID, NodeErrors] | None = None
+  node_errors: Dict[APINodeID, NodeErrors] | None = None
   number: int | None = None
   prompt_id: PromptID | None = None
   error: str | None = None
 
 
 ################################################################################
 
 
-class APIOutputUI(RootModel[Dict[OutputName, Any]]):
+class APIOutputUI(RootModel[Dict[OutputName, List[Any]]]):
   root: Dict[OutputName, List[Any]]
 
 
 class APIHistoryEntryStatusNote(NamedTuple):
   name: str
   data: Any
 
@@ -222,15 +251,15 @@
 class APIHistoryEntry(BaseModel):
   model_config = ConfigDict(extra=EXTRA)
   """This is a pydantic thing, to configure the model, it is not an accessible field.
 
   extra: This is just to future proof the schema so it won't break if extra
   fields are added. They'll be stored dynamically.
   """
-  outputs: Dict[NodeID, APIOutputUI] | None = None
+  outputs: Dict[APINodeID, APIOutputUI] | None = None
   prompt: APIQueueInfoEntry | None = None
   status: APIHistoryEntryStatus | None = None
 
 
 class APIHistory(RootModel[Dict[PromptID, APIHistoryEntry]]):
   """Returned if you call /history and /history/{prompt_id} endpoints.
 
@@ -463,15 +492,15 @@
   root: Dict[APIObjectKey, APIObjectInfoEntry]
 
 
 ################################################################################
 class APIUploadImageResp(BaseModel):
   name: str
   subfolder: str
-  type: str
+  type: ComfyFolderType
 
 
 ################################################################################
 class WSExecutingData(BaseModel):
   """Websocket "executing" message.
   See:
 
@@ -501,7 +530,57 @@
   fields are added. They'll be stored dynamically.
   """
   type: str
   data: dict
 
 
 ################################################################################
+
+
+class ComfyUIPathTriplet(BaseModel):
+  """
+  Represents a folder_type/subfolder/filename triplet, which ComfyUI API and
+  some nodes use as file paths.
+  """
+  model_config = ConfigDict(frozen=True)
+
+  type: ComfyFolderType
+  subfolder: str
+  filename: str
+
+  @field_validator('type')
+  @classmethod
+  def validate_folder_type(cls, v: str):
+    if v not in VALID_FOLDER_TYPES:
+      raise ValueError(
+          f'folder_type {repr(v)} is not one of {VALID_FOLDER_TYPES}')
+    return v
+
+  @field_validator('subfolder')
+  @classmethod
+  def validate_subfolder(cls, v: str):
+    if v.startswith('/'):
+      raise ValueError(f'subfolder {repr(v)} must not start with a slash')
+    return v
+
+  @field_validator('filename')
+  @classmethod
+  def validate_filename(cls, v: str):
+    if '/' in v:
+      raise ValueError(f'filename {repr(v)} must not contain a slash')
+    if v == '':
+      raise ValueError(f'filename {repr(v)} must not be empty')
+    return v
+
+  def ToLocalPathStr(self, *, include_folder_type: bool) -> str:
+    """Converts this triplet to something like `input/subfolder/filename`.
+    """
+    subfolder = self.subfolder
+    if subfolder == '':
+      subfolder = '.'
+    if not subfolder.endswith('/'):
+      subfolder += '/'
+
+    local_path = urljoin(subfolder, self.filename)
+    if include_folder_type:
+      local_path = urljoin(f'{self.type}/', local_path)
+    return local_path
```

### Comparing `comfy_catapult-1.0.2/comfy_catapult/comfy_utils.py` & `comfy_catapult-2.0.0/comfy_catapult/comfy_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,47 +3,47 @@
 #
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
 import dataclasses
 import datetime
-import sys
+import logging
 import textwrap
 from dataclasses import is_dataclass
 from typing import (Any, Generator, Hashable, List, Literal, NamedTuple, Type,
-                    TypeVar)
+                    TypeVar, cast)
 
 import aiofiles
 import pydantic_core
 import pydash
 import yaml
 from anyio import Path
 from pydantic import BaseModel
 from pydash import slugify
 
-from comfy_catapult.comfy_schema import (APIHistoryEntry, APIOutputUI,
-                                         APIWorkflow, APIWorkflowNodeInfo,
-                                         NodeID)
+from comfy_catapult.comfy_schema import (APIHistoryEntry, APINodeID,
+                                         APIOutputUI, APIWorkflow,
+                                         APIWorkflowNodeInfo,
+                                         ComfyUIPathTriplet)
 from comfy_catapult.errors import MultipleNodesFound, NodeNotFound
 from comfy_catapult.remote_file_api_base import RemoteFileAPIBase
-from comfy_catapult.url_utils import ComfyUIPathTriplet
 
 MAX_DUMP_LINES: int | None = 200
-DUMP_DIR: Path = Path('.logs/dumps')
+logger = logging.getLogger(__name__)
 
 
 class NodeIDAndNode(NamedTuple):
-  node_id: NodeID
+  node_id: APINodeID
   node_info: APIWorkflowNodeInfo
 
 
 def FindNodesByTitle(*, workflow: APIWorkflow,
                      title: str) -> Generator[NodeIDAndNode, None, None]:
-  node_id: NodeID
+  node_id: APINodeID
   node_info: APIWorkflowNodeInfo
   for node_id, node_info in workflow.root.items():
     if node_info.meta is not None and node_info.meta.title == title:
       yield NodeIDAndNode(node_id=node_id, node_info=node_info)
 
 
 def FindNodeByTitle(*, workflow: APIWorkflow,
@@ -67,75 +67,79 @@
                              found_nodes=[node_id for node_id, _ in nodes])
   node_id, node_info = nodes[0]
 
   return NodeIDAndNode(node_id=node_id, node_info=node_info)
 
 
 def FindNode(*, workflow: APIWorkflow,
-             id_or_title: str) -> NodeIDAndNode | None:
-  id_node_id: NodeID | None = None
+             id_or_title: int | str) -> NodeIDAndNode | None:
+  id_node_id: APINodeID | None = None
   # id_node_error: Exception | None = None
 
-  title_node_id: NodeID | None = None
+  title_node_id: APINodeID | None = None
   # title_node_error: Exception | None = None
 
   try:
-    title_node_id, _ = GetNodeByTitle(workflow=workflow, title=id_or_title)
+    if isinstance(id_or_title, str):
+      title_node_id, _ = GetNodeByTitle(workflow=workflow, title=id_or_title)
 
   except NodeNotFound:
     # id_node_error = e
     pass
 
+  id_or_title_str = str(id_or_title)
   try:
-    id_node_id = NodeID(id_or_title)
-    # node = workflow.root[id_node_id]
+    id_node_id_: APINodeID = cast(APINodeID, id_or_title_str)
+    if id_node_id_ in workflow.root:
+      id_node_id = id_node_id_
   except ValueError:
     # title_node_error = e
     pass
 
   if title_node_id is None and id_node_id is None:
     return None
   elif title_node_id is not None and id_node_id is not None:
-    raise MultipleNodesFound(search_titles=[id_or_title],
+    raise MultipleNodesFound(search_titles=[id_or_title_str],
                              search_nodes=[id_node_id],
-                             found_titles=[id_or_title],
+                             found_titles=[title_node_id],
                              found_nodes=[id_node_id])
   elif title_node_id is not None:
     return NodeIDAndNode(node_id=title_node_id,
                          node_info=workflow.root[title_node_id])
   else:
     if id_node_id is None:
       raise AssertionError('id_node_id is None')
 
     return NodeIDAndNode(node_id=id_node_id,
                          node_info=workflow.root[id_node_id])
 
 
-def GetNode(*, workflow: APIWorkflow, id_or_title: str) -> NodeIDAndNode:
+def GetNode(*, workflow: APIWorkflow, id_or_title: str | int) -> NodeIDAndNode:
   node = FindNode(workflow=workflow, id_or_title=id_or_title)
   if node is None:
     raise NodeNotFound(title=id_or_title, node_id=id_or_title)
   return node
 
 
-def GenerateNewNodeID(*, workflow: APIWorkflow) -> NodeID:
+def GenerateNewNodeID(*, workflow: APIWorkflow) -> APINodeID:
   all_keys = workflow.root.keys()
   max_integer = 0
 
   # Filter all keys that fail to convert to int
   for key in all_keys:
     try:
       max_integer = max(int(key), max_integer)
     except ValueError:
       continue
 
-  return NodeID(str(max_integer + 1))
+  return cast(APINodeID, str(max_integer + 1))
 
 
-async def DownloadPreviewImage(*, node_id: NodeID, job_history: APIHistoryEntry,
+async def DownloadPreviewImage(*, node_id: APINodeID,
+                               job_history: APIHistoryEntry,
                                field_path: Hashable | List[Hashable],
                                comfy_api_url: str, remote: RemoteFileAPIBase,
                                local_dst_path: Path):
   """Downloads something that looks like an Preview Image node's outputs.
 
   * field_path=='gifs[0]' works for Video Combine
   * field_path=='images[0]' works for Preview Image
@@ -205,19 +209,19 @@
   folder_type: Literal['temp', 'output'] = file_dict['type']
   if not isinstance(folder_type, str):
     raise Exception(f'Expected "type" to be str, got {type(folder_type)}')
   if folder_type not in ['temp', 'output']:
     raise Exception(
         f'Expected "type" to be "temp" or "output", got {folder_type}')
 
-  triplet = ComfyUIPathTriplet(comfy_api_url=comfy_api_url,
-                               folder_type=folder_type,
+  triplet = ComfyUIPathTriplet(type=folder_type,
                                subfolder=subfolder,
                                filename=filename)
-  return await remote.DownloadTriplet(untrusted_src_triplet=triplet,
+  return await remote.DownloadTriplet(untrusted_comfy_api_url=comfy_api_url,
+                                      untrusted_src_triplet=triplet,
                                       dst_path=local_dst_path)
 
 
 class _CustomDumper(yaml.Dumper):
 
   def represent_tuple(self, data):
     return self.represent_list(data)
@@ -233,14 +237,15 @@
 async def _GetNewPath(*, parent_path: Path) -> Path:
   name = datetime.datetime.now().strftime('%Y-%m-%d_%H-%M-%S_%f')
   path = parent_path / name
   index = 1
   while await path.exists():
     path = parent_path / f'{name}_{index}'
     index += 1
+  await path.mkdir(parents=True, exist_ok=True)
   return path
 
 
 async def BigYamlDump(data: Any, *, max_lines: int | None, path: Path) -> str:
   yaml_str = YamlDump(data)
   line_count = len(yaml_str.splitlines())
   if max_lines is None or line_count <= max_lines:
@@ -270,18 +275,14 @@
 _BaseModelT = TypeVar('_BaseModelT', bound=BaseModel)
 
 
 def _IsDataclassInstance(instance):
   return is_dataclass(instance) and not isinstance(instance, type)
 
 
-def _IsNamedTuple(instance):
-  return isinstance(instance, tuple) and hasattr(instance, '_fields')
-
-
 class _ExtraFieldWarning(NamedTuple):
   path: List[Any]
   thing: Any
   message: str
 
 
 def _WarnModelExtras(*, path: List[Any],
@@ -320,120 +321,139 @@
     pass
 
 
 async def TryParseAsModel(
     *,
     content: Any,
     model_type: Type[_BaseModelT],
+    errors_dump_directory: Path | None,
     strict: Literal['yes', 'no', 'warn'] = 'warn') -> _BaseModelT:
 
-  async def _Internal():
-    dump_path: Path | None = None
+  async def _Internal(errors_dump_directory: Path | None):
+    error_dump_path: Path | None = None
 
     try:
       try:
         return model_type.model_validate(content,
                                          strict=strict in ['yes', 'warn'])
       except pydantic_core.ValidationError as e:
         if strict == 'yes':
           # Go to the except below which just prints the error.
           raise
         # Try parsing it non-strictly, and then warn about the error if it
         # succeeds. If it errors, then we'll go to the except below which
         # prints the error.
         model = model_type.model_validate(content, strict=False)
-        if dump_path is None:
-          dump_path = await _GetNewPath(parent_path=DUMP_DIR)
+        if error_dump_path is None and errors_dump_directory is not None:
+          error_dump_path = await _GetNewPath(parent_path=errors_dump_directory)
 
-        error_line = await BigErrorStrDump(
-            exception=e,
-            max_lines=MAX_DUMP_LINES,
-            path=dump_path / f'{slugify(str(model_type))}-error_str.txt')
+        if error_dump_path is not None:
+          error_line = await BigErrorStrDump(
+              exception=e,
+              max_lines=MAX_DUMP_LINES,
+              path=error_dump_path /
+              f'{slugify(str(model_type))}-error_str.txt')
+
+          model_dump_yaml = await BigYamlDump(
+              model.model_dump(),
+              max_lines=MAX_DUMP_LINES,
+              path=error_dump_path /
+              f'{slugify(str(model_type))}-model_dump.yaml')
+          input_content_yaml = await BigYamlDump(
+              content,
+              max_lines=MAX_DUMP_LINES,
+              path=error_dump_path /
+              f'{slugify(str(model_type))}-input_content.yaml')
+        else:
+          error_line = str(e)
+          model_dump_yaml = YamlDump(model.model_dump())
+          input_content_yaml = YamlDump(content)
 
-        model_dump_yaml = await BigYamlDump(
-            model.model_dump(),
-            max_lines=MAX_DUMP_LINES,
-            path=dump_path / f'{slugify(str(model_type))}-model_dump.yaml')
-        input_content_yaml = await BigYamlDump(
-            content,
-            max_lines=MAX_DUMP_LINES,
-            path=dump_path / f'{slugify(str(model_type))}-input_content.yaml')
         msg = f'Warning: Error parsing {model_type} with strict=True: {error_line}'
-        print(
+        logger.error(
             f'{msg}:'
             f'\n\n{textwrap.indent(str(e), prefix="  ")}'
             f'\nParsed Model:\n{textwrap.indent(model_dump_yaml, prefix="  ")}'
             f'\nInput content\n{textwrap.indent(input_content_yaml, prefix="  ")}'
-            f'\n{msg}',
-            file=sys.stderr)
+            f'\n{msg}')
         return model
     except pydantic_core.ValidationError as e:
       # It failed strictly or non-strictly. Print the error and raise.
 
-      if dump_path is None:
-        dump_path = await _GetNewPath(parent_path=DUMP_DIR)
-        await dump_path.mkdir(parents=True, exist_ok=True)
-
-      error_line = await BigErrorStrDump(
-          exception=e,
-          max_lines=MAX_DUMP_LINES,
-          path=dump_path / f'{slugify(str(model_type))}-error_str.txt')
-      msg = f'Error parsing {model_type}: {error_line}'
-
-      input_content_yaml = await BigYamlDump(
-          content,
-          max_lines=MAX_DUMP_LINES,
-          path=dump_path / f'{slugify(str(model_type))}-input_content.yaml')
-      errors_yaml = await BigYamlDump(e.errors(),
-                                      max_lines=MAX_DUMP_LINES,
-                                      path=dump_path /
-                                      f'{slugify(str(model_type))}-errors.yaml')
-
-      raise Exception(
-          f'{msg}'
-          f'\nInput content\n{textwrap.indent(input_content_yaml, prefix="  ")}'
-          f'\nError details\n{textwrap.indent(errors_yaml, prefix="  ")}'
-          f'\n{msg}') from e
+      if error_dump_path is None and errors_dump_directory is not None:
+        error_dump_path = await _GetNewPath(parent_path=errors_dump_directory)
+
+      if error_dump_path is not None:
+        error_line = await BigErrorStrDump(
+            exception=e,
+            max_lines=MAX_DUMP_LINES,
+            path=error_dump_path / f'{slugify(str(model_type))}-error_str.txt')
+      else:
+        error_line = str(e)
+      msg_summary = f'Error parsing {model_type}: {error_line}'
+      msg = f'{msg_summary}'
+      if error_dump_path is not None:
+        input_content_yaml = await BigYamlDump(
+            content,
+            max_lines=MAX_DUMP_LINES,
+            path=error_dump_path /
+            f'{slugify(str(model_type))}-input_content.yaml')
+        msg += '\nInput content\n' + textwrap.indent(input_content_yaml,
+                                                     prefix='  ')
+        errors_yaml = await BigYamlDump(
+            e.errors(),
+            max_lines=MAX_DUMP_LINES,
+            path=error_dump_path / f'{slugify(str(model_type))}-errors.yaml')
+        msg += '\nError details\n' + textwrap.indent(errors_yaml, prefix='  ')
+      else:
+        msg += '\nInput content\n' + textwrap.indent(YamlDump(content),
+                                                     prefix='  ')
+        msg += '\nError details\n' + textwrap.indent(YamlDump(e.errors()),
+                                                     prefix='  ')
+
+      msg += f'\n{msg_summary}'
+      raise Exception(msg) from e
 
-  model = await _Internal()
-  warnings = _WarnModelExtras(path=[], thing=model)
+  model = await _Internal(errors_dump_directory=errors_dump_directory)
+  extra_fields_warnings = _WarnModelExtras(path=[], thing=model)
   if strict == 'warn':
-    for warning in warnings:
-      print(warning.message, file=sys.stderr)
+    for warning in extra_fields_warnings:
+      logger.warn(warning.message)
   elif strict == 'yes':
-    for warning in warnings:
+    for warning in extra_fields_warnings:
       raise Exception(warning.message)
 
+  # TODO: Renable this or remove it.
   # model_dump: Dict[str, Any] = model.model_dump()
   # differences = list(diff(model_dump, content))
   # if len(differences) > 0:
   #   print('Warning: Model parsed with differences from the content', file=sys.stderr)
   #   print('content:', file=sys.stderr)
   #   print(textwrap.indent(_YamlDump(content), prefix='  '), file=sys.stderr)
   #   print('model_dump:', file=sys.stderr)
   #   print(textwrap.indent(_YamlDump(model_dump), prefix='  '), file=sys.stderr)
   #   print('differences:', file=sys.stderr)
   #   print(textwrap.indent(_YamlDump(differences), prefix='  '), file=sys.stderr)
   return model
 
 
-class _WatchVar:
+class WatchVar:
 
   def __init__(self, **kwargs):
     self._kwargs = kwargs
 
   def __enter__(self):
     pass
 
   def __exit__(self, exc_type, exc, tb):
     if exc is not None:
-      print(
-          f'{type(self).__name__}: Error occurred, and you are watching these variables:',
-          file=sys.stderr)
+      logger.error(
+          f'{type(self).__name__}: Error occurred, and you are watching these variables:'
+      )
       for key, value in self._kwargs.items():
         value_lines = str(value).split('\n')
         if len(value_lines) > 1:
           value = '\n' + textwrap.indent(value, prefix='    ')
         else:
           if isinstance(value, str):
             value = repr(value)
-        print(f'  {key}: {value}', file=sys.stderr)
+        logger.error(f'  {key}: {value}')
```

### Comparing `comfy_catapult-1.0.2/comfy_catapult/errors.py` & `comfy_catapult-2.0.0/comfy_catapult/errors.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,44 +4,45 @@
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
 from copy import deepcopy
 from typing import Sequence
 
-from comfy_catapult.comfy_schema import APIWorkflowTicket, NodeID
+from comfy_catapult.comfy_schema import APINodeID, APIWorkflowTicket
 
 
 class NodeNotFound(RuntimeError):
 
-  def __init__(self, *, node_id: NodeID | None, title: str | None):
+  def __init__(self, *, node_id: APINodeID | int | None,
+               title: str | int | None):
     super().__init__(
         f'Node with title=={repr(title)}, node_id=={repr(node_id)} not found')
     self.node_id = node_id
     self.title = title
 
 
 class MultipleNodesFound(RuntimeError):
 
   def __init__(self, *, search_titles: Sequence[str],
-               search_nodes: Sequence[NodeID], found_titles: Sequence[str],
-               found_nodes: Sequence[NodeID]):
+               search_nodes: Sequence[APINodeID], found_titles: Sequence[str],
+               found_nodes: Sequence[APINodeID]):
     super().__init__(
         f'Found multiple nodes with titles=={repr(found_titles)}, node_ids=={list(found_nodes)}'
         f' when searching for titles=={repr(search_titles)}, node_ids=={list(search_nodes)}'
     )
     self.search_titles = list(search_titles)
     self.search_node_ids = list(search_nodes)
     self.found_titles = list(found_titles)
     self.found_node_ids = list(found_nodes)
 
 
 class NodesNotExecuted(RuntimeError):
 
-  def __init__(self, *, nodes: Sequence[NodeID],
+  def __init__(self, *, nodes: Sequence[APINodeID],
                titles: Sequence[str | None] | None):
     if titles is None:
       titles = [None] * len(nodes)
     if len(nodes) != len(titles):
       raise ValueError(
           f'len(nodes) != len(titles): {len(nodes)} != {len(titles)}')
```

### Comparing `comfy_catapult-1.0.2/comfy_catapult/eta_estimator.py` & `comfy_catapult-2.0.0/comfy_catapult/eta_estimator.py`

 * *Files identical despite different names*

### Comparing `comfy_catapult-1.0.2/comfy_catapult/remote_file_api_base.py` & `comfy_catapult-2.0.0/comfy_catapult/remote_file_api_base.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,26 +2,19 @@
 # SPDX-License-Identifier: MIT
 #
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
 from abc import ABC, abstractmethod
-from urllib.parse import ParseResult
+from typing import Tuple
 
 from anyio import Path
 
-from comfy_catapult.url_utils import ComfyUIPathTriplet
-
-EMPTY_URL = ParseResult(scheme='',
-                        netloc='',
-                        path='',
-                        params='',
-                        query='',
-                        fragment='')
+from comfy_catapult.comfy_schema import ComfyUIPathTriplet
 
 
 class RemoteFileAPIBase(ABC):
 
   @abstractmethod
   async def UploadFile(self, *, src_path: Path, untrusted_dst_url: str) -> str:
     """Upload a file.
@@ -34,15 +27,15 @@
     Returns:
         str: A new URL, sometimes the stored URL is not the same as the uploaded
         one, e.g if there is already an existing file there.
     """
     raise NotImplementedError()
 
   async def UploadToTriplet(
-      self, *, src_path: Path,
+      self, *, src_path: Path, untrusted_comfy_api_url: str,
       untrusted_dst_triplet: ComfyUIPathTriplet) -> ComfyUIPathTriplet:
     """Upload a file to a (comfy api server, folder_type, subfolder, filename).
 
     Raises:
         NotImplementedError: _description_
 
     Returns:
@@ -53,25 +46,27 @@
     raise NotImplementedError()
 
   @abstractmethod
   async def DownloadFile(self, *, untrusted_src_url: str, dst_path: Path):
     raise NotImplementedError()
 
   @abstractmethod
-  async def DownloadTriplet(self, *, untrusted_src_triplet: ComfyUIPathTriplet,
+  async def DownloadTriplet(self, *, untrusted_comfy_api_url: str,
+                            untrusted_src_triplet: ComfyUIPathTriplet,
                             dst_path: Path):
     raise NotImplementedError()
 
   @abstractmethod
-  def TripletToURL(self, *, triplet: ComfyUIPathTriplet) -> str:
+  def TripletToURL(self, *, comfy_api_url: str,
+                   triplet: ComfyUIPathTriplet) -> str:
     """Convert a triplet, that this API can handle, to a URL that this API can handle."""
     raise NotImplementedError()
 
   @abstractmethod
-  def URLToTriplet(self, *, url: str) -> ComfyUIPathTriplet:
+  def URLToTriplet(self, *, url: str) -> Tuple[str, ComfyUIPathTriplet]:
     """Convert a URL that this API can handle to a triplet, that this API can handle."""
     raise NotImplementedError()
 
   @abstractmethod
   def GetBases(self) -> list[str]:
     """Return a list of base URLs that this API can handle."""
     raise NotImplementedError()
```

### Comparing `comfy_catapult-1.0.2/comfy_catapult/remote_file_api_comfy.py` & `comfy_catapult-2.0.0/comfy_catapult/remote_file_api_comfy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 #
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
-from typing import List
+from typing import List, Tuple
 from urllib.parse import ParseResult
 
 from anyio import Path
 
 from comfy_catapult.api_client import ComfyAPIClient
-from comfy_catapult.comfy_schema import APIUploadImageResp
+from comfy_catapult.comfy_schema import (VALID_FOLDER_TYPES,
+                                         APIUploadImageResp,
+                                         ComfyUIPathTriplet)
 from comfy_catapult.remote_file_api_base import RemoteFileAPIBase
-from comfy_catapult.url_utils import (VALID_COMFY_API_SCHEMES,
-                                      VALID_FOLDER_TYPES, ComfyUIPathTriplet,
-                                      SmartURLJoin, ToParseResult,
-                                      ValidateIsBasedURL,
+from comfy_catapult.url_utils import (VALID_COMFY_API_SCHEMES, SmartURLJoin,
+                                      ToParseResult, ValidateIsBasedURL,
                                       ValidateIsComfyAPITargetURL)
 
 VALID_COMFY_SCHEME_SCHEMES = ['comfy+http', 'comfy+https']
 
 
 def _ValidateComfyAPITargetURL(url: str, *,
                                any_api_targets: List[str] | None) -> str:
@@ -47,28 +47,28 @@
   # TODO: check the path
 
   if any_bases is not None:
     return ValidateIsBasedURL(url=url, any_bases=any_bases)
   return url
 
 
-def ComfySchemeURLToTriplet(url: str,
-                            *,
-                            inversion_check: bool = __debug__
-                            ) -> ComfyUIPathTriplet:
+def ComfySchemeURLToTriplet(
+    url: str,
+    *,
+    inversion_check: bool = __debug__) -> Tuple[str, ComfyUIPathTriplet]:
   """Turns a custom URL scheme into a triplet.
 
   Args:
-      url (str): URL in the form of:
-        comfy+http://comfy-server-host:port/folder_type/subfolder/sub/filename
+    url (str): URL in the form of:
+      comfy+http://comfy-server-host:port/folder_type/subfolder/sub/filename
   Raises:
-      ValueError: When something is wrong with the URL.
+    ValueError: When something is wrong with the URL.
 
   Returns:
-      ComfyUIPathTriplet: The triplet.
+    Tuple[str, ComfyUIPathTriplet]: The ComfyUI API URL, and the triplet.
   """
   url_pr = ToParseResult(url=url)
   url_path = url_pr.path
 
   if url_pr.scheme not in ['comfy+http', 'comfy+https']:
     raise ValueError(
         f'URL {repr(url)} does not start with one of {VALID_COMFY_SCHEME_SCHEMES}'
@@ -91,56 +91,54 @@
     raise ValueError(
         f'URL {repr(url)} path {repr(url_path)} does not start with one of {VALID_FOLDER_TYPES}'
     )
   subfolder, _, filename = rest.rpartition('/')
 
   comfy_api_url_pr = url_pr._replace(scheme=api_scheme, path='')
 
-  triplet = ComfyUIPathTriplet(comfy_api_url=comfy_api_url_pr.geturl(),
-                               folder_type=folder_type,
+  triplet = ComfyUIPathTriplet(type=folder_type,
                                subfolder=subfolder,
                                filename=filename)
   if inversion_check:
-    inverted_url = TripletToComfySchemeURL(triplet=triplet,
-                                           inversion_check=False)
+    inverted_url = TripletToComfySchemeURL(
+        comfy_api_url=comfy_api_url_pr.geturl(),
+        triplet=triplet,
+        inversion_check=False)
     if inverted_url != url:
       raise ValueError(
           f'\nurl: {repr(url)}\ntriplet: {repr(triplet)}\ninverted_url: {repr(inverted_url)}'
       )
-  return triplet
+  return comfy_api_url_pr.geturl(), triplet
 
 
-def TripletToComfySchemeURL(triplet: ComfyUIPathTriplet,
+def TripletToComfySchemeURL(comfy_api_url: str,
+                            triplet: ComfyUIPathTriplet,
                             *,
                             inversion_check: bool = __debug__) -> str:
-  comfy_api_url = ValidateIsComfyAPITargetURL(triplet.comfy_api_url)
+  comfy_api_url = ValidateIsComfyAPITargetURL(comfy_api_url)
   comfy_api_url_pr = ToParseResult(comfy_api_url)
   api_scheme = comfy_api_url_pr.scheme
   # ComfyUIPathTriplet validation should have already caught this.
   # trunk-ignore(bandit/B101)
   assert api_scheme in VALID_COMFY_API_SCHEMES
   # ComfyUIPathTriplet validation should have already caught this.
   # trunk-ignore(bandit/B101)
-  assert triplet.folder_type in VALID_FOLDER_TYPES
+  assert triplet.type in VALID_FOLDER_TYPES
   # ComfyUIPathTriplet validation should have already caught this.
   # trunk-ignore(bandit/B101)
   assert '/' not in triplet.filename
   # ComfyUIPathTriplet validation should have already caught this.
   # trunk-ignore(bandit/B101)
   assert triplet.filename != ''
   # ComfyUIPathTriplet validation should have already caught this.
   # trunk-ignore(bandit/B101)
   assert not triplet.subfolder.startswith('/')
 
-  path = f'{triplet.folder_type}/{triplet.subfolder}'
-  if not path.endswith('/'):
-    path += '/'
-
-  path = SmartURLJoin(path, triplet.filename)
-  comfy_scheme = f'comfy+{ToParseResult(triplet.comfy_api_url).scheme}'
+  path = triplet.ToLocalPathStr(include_folder_type=True)
+  comfy_scheme = f'comfy+{ToParseResult(comfy_api_url).scheme}'
   # Sanity check, since api_scheme is in VALID_COMFY_API_SCHEMES, this should
   # always be true.
   # trunk-ignore(bandit/B101)
   assert comfy_scheme in VALID_COMFY_SCHEME_SCHEMES
 
   url_pr = comfy_api_url_pr._replace(scheme=comfy_scheme,
                                      path=SmartURLJoin(comfy_api_url_pr.path,
@@ -186,93 +184,99 @@
       self._comfy_api_urls = [
           _ValidateComfyAPITargetURL(url, any_api_targets=None)
           for url in comfy_api_urls
       ]
 
     self._overwrite = overwrite
 
-  def _ToTrustedTriplet(self, *,
-                        untrusted_comfy_scheme_url: str) -> ComfyUIPathTriplet:
-    triplet = ComfySchemeURLToTriplet(url=untrusted_comfy_scheme_url)
-    return ComfyUIPathTriplet(comfy_api_url=_ValidateComfyAPITargetURL(
-        triplet.comfy_api_url, any_api_targets=self._comfy_api_urls),
-                              folder_type=triplet.folder_type,
-                              subfolder=triplet.subfolder,
-                              filename=triplet.filename)
+  def _ToTrustedTriplet(
+      self, *,
+      untrusted_comfy_scheme_url: str) -> Tuple[str, ComfyUIPathTriplet]:
+    comfy_api_url, triplet = ComfySchemeURLToTriplet(
+        url=untrusted_comfy_scheme_url)
+    comfy_api_url = _ValidateComfyAPITargetURL(
+        comfy_api_url, any_api_targets=self._comfy_api_urls)
+    return comfy_api_url, triplet
 
   def _ValidateTriplet(
-      self, *, untrusted_triplet: ComfyUIPathTriplet) -> ComfyUIPathTriplet:
-    return ComfyUIPathTriplet(comfy_api_url=_ValidateComfyAPITargetURL(
-        untrusted_triplet.comfy_api_url, any_api_targets=self._comfy_api_urls),
-                              folder_type=untrusted_triplet.folder_type,
-                              subfolder=untrusted_triplet.subfolder,
-                              filename=untrusted_triplet.filename)
+      self, *, untrusted_comfy_api_url: str,
+      untrusted_triplet: ComfyUIPathTriplet) -> Tuple[str, ComfyUIPathTriplet]:
+    comfy_api_url = _ValidateComfyAPITargetURL(
+        untrusted_comfy_api_url, any_api_targets=self._comfy_api_urls)
+    triplet = untrusted_triplet
+    return comfy_api_url, triplet
 
   async def DownloadFile(self, *, untrusted_src_url: str, dst_path: Path):
-    trusted_src_triplet = self._ToTrustedTriplet(
+    trusted_comfy_api_url, trusted_src_triplet = self._ToTrustedTriplet(
         untrusted_comfy_scheme_url=untrusted_src_url)
-    await self.DownloadTriplet(untrusted_src_triplet=trusted_src_triplet,
+    await self.DownloadTriplet(untrusted_comfy_api_url=trusted_comfy_api_url,
+                               untrusted_src_triplet=trusted_src_triplet,
                                dst_path=dst_path)
 
   async def UploadFile(self, *, src_path: Path, untrusted_dst_url: str) -> str:
     # Validate andt turn the URL into the form:
     #   comfy+http://api_host:port/folder_type/subfolder/filename
-    trusted_dst_triplet = self._ToTrustedTriplet(
+    trusted_comfy_api_url, trusted_dst_triplet = self._ToTrustedTriplet(
         untrusted_comfy_scheme_url=untrusted_dst_url)
     new_triplet = await self.UploadToTriplet(
-        src_path=src_path, untrusted_dst_triplet=trusted_dst_triplet)
+        src_path=src_path,
+        untrusted_comfy_api_url=trusted_comfy_api_url,
+        untrusted_dst_triplet=trusted_dst_triplet)
     # Turn the triplet back into the form:
     #   comfy+http://api_host:port/folder_type/subfolder/filename
-    return TripletToComfySchemeURL(triplet=new_triplet)
+    return TripletToComfySchemeURL(comfy_api_url=trusted_comfy_api_url,
+                                   triplet=new_triplet)
 
-  async def DownloadTriplet(self, *, untrusted_src_triplet: ComfyUIPathTriplet,
+  async def DownloadTriplet(self, *, untrusted_comfy_api_url: str,
+                            untrusted_src_triplet: ComfyUIPathTriplet,
                             dst_path: Path):
-    trusted_src_triplet = self._ValidateTriplet(
+    trusted_comfy_api_url, trusted_src_triplet = self._ValidateTriplet(
+        untrusted_comfy_api_url=untrusted_comfy_api_url,
         untrusted_triplet=untrusted_src_triplet)
 
-    async with ComfyAPIClient(
-        comfy_api_url=trusted_src_triplet.comfy_api_url) as client:
+    async with ComfyAPIClient(comfy_api_url=trusted_comfy_api_url) as client:
       data: bytes = await client.GetView(
-          folder_type=trusted_src_triplet.folder_type,
+          folder_type=trusted_src_triplet.type,
           subfolder=trusted_src_triplet.subfolder,
           filename=trusted_src_triplet.filename)
 
     await dst_path.parent.mkdir(parents=True, exist_ok=True)
     async with await dst_path.open('wb') as f:
       await f.write(data)
 
   async def UploadToTriplet(
-      self, *, src_path: Path,
+      self, *, src_path: Path, untrusted_comfy_api_url: str,
       untrusted_dst_triplet: ComfyUIPathTriplet) -> ComfyUIPathTriplet:
-    trusted_dst_triplet = self._ValidateTriplet(
+    trusted_comfy_api_url, trusted_dst_triplet = self._ValidateTriplet(
+        untrusted_comfy_api_url=untrusted_comfy_api_url,
         untrusted_triplet=untrusted_dst_triplet)
 
     async with await src_path.open('rb') as f:
       data = await f.read()
 
-    async with ComfyAPIClient(
-        comfy_api_url=trusted_dst_triplet.comfy_api_url) as client:
+    async with ComfyAPIClient(comfy_api_url=trusted_comfy_api_url) as client:
       resp: APIUploadImageResp = await client.PostUploadImage(
-          folder_type=trusted_dst_triplet.folder_type,
+          folder_type=trusted_dst_triplet.type,
           subfolder=trusted_dst_triplet.subfolder,
           filename=trusted_dst_triplet.filename,
           data=data,
           overwrite=self._overwrite)
     # If the server renamed the file, we need to update the triplet.
     return trusted_dst_triplet.model_copy(update={
         'filename': resp.name,
         'subfolder': resp.subfolder,
         'folder_type': resp.type
     },
                                           deep=True)
 
-  def TripletToURL(self, *, triplet: ComfyUIPathTriplet) -> str:
-    return TripletToComfySchemeURL(triplet=triplet)
+  def TripletToURL(self, *, comfy_api_url: str,
+                   triplet: ComfyUIPathTriplet) -> str:
+    return TripletToComfySchemeURL(comfy_api_url=comfy_api_url, triplet=triplet)
 
-  def URLToTriplet(self, *, url: str) -> ComfyUIPathTriplet:
+  def URLToTriplet(self, *, url: str) -> Tuple[str, ComfyUIPathTriplet]:
     return ComfySchemeURLToTriplet(url=url)
 
   def GetBases(self) -> list[str]:
     if self._comfy_api_urls is None:
       return [f'comfy+{scheme}://' for scheme in VALID_COMFY_API_SCHEMES]
 
     return [
```

### Comparing `comfy_catapult-1.0.2/comfy_catapult/remote_file_api_comfy_test.py` & `comfy_catapult-2.0.0/comfy_catapult/remote_file_api_comfy_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 from tempfile import TemporaryDirectory
 from typing import List
 from unittest import IsolatedAsyncioTestCase
 
 import pydantic
 from anyio import Path
 
+from comfy_catapult.comfy_schema import (VALID_FOLDER_TYPES, ComfyFolderType,
+                                         ComfyUIPathTriplet)
+from comfy_catapult.comfy_schema_test import VALID_SUBFOLDER_EDGES
 from comfy_catapult.remote_file_api_comfy import (ComfySchemeRemoteFileAPI,
                                                   TripletToComfySchemeURL)
-from comfy_catapult.url_utils import (VALID_FOLDER_TYPES, ComfyFolderType,
-                                      ComfyUIPathTriplet, SmartURLJoin)
-from comfy_catapult.url_utils_test import VALID_SUBFOLDER_EDGES
+from comfy_catapult.url_utils import SmartURLJoin
 
 COMFY_API_URL = os.environ.get('COMFY_API_URL')
 if COMFY_API_URL is None:
   raise ValueError('Please set COMFY_API_URL in the environment')
 
 
 class TestRemoteFileApiComfy(IsolatedAsyncioTestCase):
@@ -33,22 +34,24 @@
     self._comfy_api_url: str = COMFY_API_URL
     self._remote = ComfySchemeRemoteFileAPI(comfy_api_urls=[COMFY_API_URL],
                                             overwrite=True)
 
   async def asyncTearDown(self):
     pass
 
-  async def _test_UploadFile(self, *, triplet: ComfyUIPathTriplet):
+  async def _test_UploadFile(self, *, comfy_api_url: str,
+                             triplet: ComfyUIPathTriplet):
     with TemporaryDirectory() as tmp_dir:
       path = Path(tmp_dir) / 'local-file.txt'
       local_download_path = Path(tmp_dir) / 'local-downloaded.txt'
       contents = 'hello world'
       await path.write_text(contents)
 
-      input_url = TripletToComfySchemeURL(triplet=triplet)
+      input_url = TripletToComfySchemeURL(comfy_api_url=comfy_api_url,
+                                          triplet=triplet)
 
       uploaded_url = await self._remote.UploadFile(src_path=path,
                                                    untrusted_dst_url=input_url)
 
       await self._remote.DownloadFile(untrusted_src_url=uploaded_url,
                                       dst_path=local_download_path)
 
@@ -57,125 +60,126 @@
 
   async def test_UploadFile(self):
     folder_type: ComfyFolderType
     folder_types: List[ComfyFolderType] = ['input']
     for folder_type in folder_types:
       for subfolder, _ in VALID_SUBFOLDER_EDGES:
         with self.subTest(folder_type=folder_type, subfolder=subfolder):
-          await self._test_UploadFile(
-              triplet=ComfyUIPathTriplet(comfy_api_url=self._comfy_api_url,
-                                         folder_type=folder_type,
-                                         subfolder=subfolder,
-                                         filename='remote-file.txt'))
+          await self._test_UploadFile(comfy_api_url=self._comfy_api_url,
+                                      triplet=ComfyUIPathTriplet(
+                                          type=folder_type,
+                                          subfolder=subfolder,
+                                          filename='remote-file.txt'))
 
-  async def _test_UploadToTriplet(self, *, triplet: ComfyUIPathTriplet):
+  async def _test_UploadToTriplet(self, *, comfy_api_url: str,
+                                  triplet: ComfyUIPathTriplet):
     with TemporaryDirectory() as tmp_dir:
       path = Path(tmp_dir) / 'local-file.txt'
       local_download_path = Path(tmp_dir) / 'local-downloaded.txt'
       contents = 'hello world'
       await path.write_text(contents)
 
       uploaded_triplet = await self._remote.UploadToTriplet(
-          src_path=path, untrusted_dst_triplet=triplet)
+          src_path=path,
+          untrusted_comfy_api_url=comfy_api_url,
+          untrusted_dst_triplet=triplet)
 
-      await self._remote.DownloadTriplet(untrusted_src_triplet=uploaded_triplet,
+      await self._remote.DownloadTriplet(untrusted_comfy_api_url=comfy_api_url,
+                                         untrusted_src_triplet=uploaded_triplet,
                                          dst_path=local_download_path)
 
       downloaded_contents = await local_download_path.read_text()
       self.assertEqual(contents, downloaded_contents)
 
   async def test_UploadToTriplet(self):
     folder_type: ComfyFolderType
     folder_types: List[ComfyFolderType] = ['input']
     for folder_type in folder_types:
       for subfolder, _ in VALID_SUBFOLDER_EDGES:
         with self.subTest(folder_type=folder_type, subfolder=subfolder):
 
-          await self._test_UploadToTriplet(
-              triplet=ComfyUIPathTriplet(comfy_api_url=self._comfy_api_url,
-                                         folder_type=folder_type,
-                                         subfolder=subfolder,
-                                         filename='remote-file.txt'))
+          await self._test_UploadToTriplet(comfy_api_url=self._comfy_api_url,
+                                           triplet=ComfyUIPathTriplet(
+                                               type=folder_type,
+                                               subfolder=subfolder,
+                                               filename='remote-file.txt'))
 
   async def test__TripletToComfySchemeURL(self):
     comfy_api_url = 'http://comfy_host:23534/'
     comfy_scheme_url = 'comfy+http://comfy_host:23534/'
 
     self.assertEqual(
-        TripletToComfySchemeURL(
-            triplet=ComfyUIPathTriplet(comfy_api_url=comfy_api_url,
-                                       folder_type='input',
-                                       subfolder='',
-                                       filename='remote-file.txt')),
+        TripletToComfySchemeURL(comfy_api_url=comfy_api_url,
+                                triplet=ComfyUIPathTriplet(
+                                    type='input',
+                                    subfolder='',
+                                    filename='remote-file.txt')),
         SmartURLJoin(comfy_scheme_url, 'input/remote-file.txt'))
     with self.assertRaises(pydantic.ValidationError):
-      _ = ComfyUIPathTriplet(comfy_api_url=comfy_api_url,
-                             folder_type='input',
+      _ = ComfyUIPathTriplet(type='input',
                              subfolder='/',
                              filename='remote-file.txt')
 
     self.assertEqual(
-        TripletToComfySchemeURL(
-            triplet=ComfyUIPathTriplet(comfy_api_url=comfy_api_url,
-                                       folder_type='input',
-                                       subfolder='subfolder',
-                                       filename='remote-file.txt')),
+        TripletToComfySchemeURL(comfy_api_url=comfy_api_url,
+                                triplet=ComfyUIPathTriplet(
+                                    type='input',
+                                    subfolder='subfolder',
+                                    filename='remote-file.txt')),
         SmartURLJoin(comfy_scheme_url, 'input/subfolder/remote-file.txt'))
     with self.assertRaises(pydantic.ValidationError):
-      _ = ComfyUIPathTriplet(comfy_api_url=comfy_api_url,
-                             folder_type='input',
+      _ = ComfyUIPathTriplet(type='input',
                              subfolder='/subfolder',
                              filename='remote-file.txt')
     with self.assertRaises(pydantic.ValidationError):
-      _ = ComfyUIPathTriplet(comfy_api_url=comfy_api_url,
-                             folder_type='input',
+      _ = ComfyUIPathTriplet(type='input',
                              subfolder='/subfolder/',
                              filename='remote-file.txt')
     self.assertEqual(
-        TripletToComfySchemeURL(
-            triplet=ComfyUIPathTriplet(comfy_api_url=comfy_api_url,
-                                       folder_type='input',
-                                       subfolder='subfolder/subsubfolder',
-                                       filename='remote-file.txt')),
+        TripletToComfySchemeURL(comfy_api_url=comfy_api_url,
+                                triplet=ComfyUIPathTriplet(
+                                    type='input',
+                                    subfolder='subfolder/subsubfolder',
+                                    filename='remote-file.txt')),
         SmartURLJoin(comfy_scheme_url,
                      'input/subfolder/subsubfolder/remote-file.txt'))
 
   async def test_TripletToComfySchemeURL(self):
     for comfy_api_url in [
         'http://comfy_host:23534',
     ]:
       for folder_type in VALID_FOLDER_TYPES:
         with self.subTest(folder_type=folder_type):
           self.assertEqual(
-              TripletToComfySchemeURL(
-                  triplet=ComfyUIPathTriplet(comfy_api_url=comfy_api_url,
-                                             folder_type=folder_type,
-                                             subfolder='',
-                                             filename='remote-file.txt')),
+              TripletToComfySchemeURL(comfy_api_url=comfy_api_url,
+                                      triplet=ComfyUIPathTriplet(
+                                          type=folder_type,
+                                          subfolder='',
+                                          filename='remote-file.txt')),
               f'comfy+{comfy_api_url}/{folder_type}/remote-file.txt')
           self.assertEqual(
-              TripletToComfySchemeURL(
-                  triplet=ComfyUIPathTriplet(comfy_api_url=comfy_api_url,
-                                             folder_type=folder_type,
-                                             subfolder='subfolder',
-                                             filename='remote-file.txt')),
+              TripletToComfySchemeURL(comfy_api_url=comfy_api_url,
+                                      triplet=ComfyUIPathTriplet(
+                                          type=folder_type,
+                                          subfolder='subfolder',
+                                          filename='remote-file.txt')),
               f'comfy+{comfy_api_url}/{folder_type}/subfolder/remote-file.txt')
           self.assertEqual(
-              TripletToComfySchemeURL(
-                  triplet=ComfyUIPathTriplet(comfy_api_url=comfy_api_url,
-                                             folder_type=folder_type,
-                                             subfolder='subfolder/subsubfolder',
-                                             filename='remote-file.txt')),
+              TripletToComfySchemeURL(comfy_api_url=comfy_api_url,
+                                      triplet=ComfyUIPathTriplet(
+                                          type=folder_type,
+                                          subfolder='subfolder/subsubfolder',
+                                          filename='remote-file.txt')),
               f'comfy+{comfy_api_url}/{folder_type}/subfolder/subsubfolder/remote-file.txt'
           )
           self.assertEqual(
-              TripletToComfySchemeURL(triplet=ComfyUIPathTriplet(
-                  comfy_api_url=comfy_api_url,
-                  folder_type=folder_type,
-                  subfolder='subfolder/subsubfolder/',
-                  filename='remote-file.txt')),
+              TripletToComfySchemeURL(comfy_api_url=comfy_api_url,
+                                      triplet=ComfyUIPathTriplet(
+                                          type=folder_type,
+                                          subfolder='subfolder/subsubfolder/',
+                                          filename='remote-file.txt')),
               f'comfy+{comfy_api_url}/{folder_type}/subfolder/subsubfolder/remote-file.txt'
           )
 
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `comfy_catapult-1.0.2/comfy_catapult/remote_file_api_generic.py` & `comfy_catapult-2.0.0/comfy_catapult/remote_file_api_generic.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 # SPDX-License-Identifier: MIT
 #
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
 from collections import defaultdict
-from typing import Dict, List
+from typing import Dict, List, Tuple
 
 from anyio import Path
 
+from comfy_catapult.comfy_schema import ComfyUIPathTriplet
 from comfy_catapult.remote_file_api_base import RemoteFileAPIBase
-from comfy_catapult.url_utils import ComfyUIPathTriplet, IsWeaklyRelativeTo
+from comfy_catapult.url_utils import IsWeaklyRelativeTo
 
 
 class GenericRemoteFileAPI(RemoteFileAPIBase):
   """Download or upload files from a URL, using multiple schemss.
   """
 
   def __init__(self):
@@ -34,30 +35,31 @@
     if apis:
       return apis
     raise ValueError(f'URL {url} is not relative to any of'
                      f' {self._base_to_api.keys()}, there is no API registered'
                      f' to handle such URLs')
 
   def _GetAPIsForTriplet(
-      self, *, triplet: ComfyUIPathTriplet) -> List[RemoteFileAPIBase]:
+      self, *, comfy_api_url: str,
+      triplet: ComfyUIPathTriplet) -> List[RemoteFileAPIBase]:
     relevant_apis = []
     convered_urls = []
     for base, base_apis in self._base_to_api.items():
       for api in base_apis:
         try:
-          url = api.TripletToURL(triplet=triplet)
+          url = api.TripletToURL(comfy_api_url=comfy_api_url, triplet=triplet)
         except NotImplementedError:
           continue
 
         convered_urls.append({'base': base, 'url': url})
         if IsWeaklyRelativeTo(base=base, url=url):
           relevant_apis.append(api)
     if relevant_apis:
       return relevant_apis
-    raise ValueError(f'ComfyUI API server URL {repr(triplet.comfy_api_url)}:'
+    raise ValueError(f'ComfyUI API server URL {repr(comfy_api_url)}:'
                      ' there is no API registered to handle this URL'
                      f'\n triplet: {triplet}'
                      f'\n convered_urls: {convered_urls}')
 
   async def UploadFile(self, *, src_path: Path, untrusted_dst_url: str) -> str:
     if not await src_path.exists():
       raise ValueError(f'File {src_path} does not exist')
@@ -71,28 +73,30 @@
                                     untrusted_dst_url=untrusted_dst_url)
       except ValueError:
         if i + 1 >= len(apis):
           raise
     raise AssertionError('unreachable')
 
   async def UploadToTriplet(
-      self, *, src_path: Path,
+      self, *, src_path: Path, untrusted_comfy_api_url: str,
       untrusted_dst_triplet: ComfyUIPathTriplet) -> ComfyUIPathTriplet:
     if not await src_path.exists():
       raise ValueError(f'File {src_path} does not exist')
     if not await src_path.is_file():
       raise ValueError(f'File {src_path} is not a file')
 
     apis: List[RemoteFileAPIBase] = self._GetAPIsForTriplet(
-        triplet=untrusted_dst_triplet)
+        comfy_api_url=untrusted_comfy_api_url, triplet=untrusted_dst_triplet)
 
     for i, api in enumerate(apis):
       try:
         return await api.UploadToTriplet(
-            src_path=src_path, untrusted_dst_triplet=untrusted_dst_triplet)
+            untrusted_comfy_api_url=untrusted_comfy_api_url,
+            src_path=src_path,
+            untrusted_dst_triplet=untrusted_dst_triplet)
       except ValueError:
         if i + 1 >= len(apis):
           raise
     raise AssertionError('unreachable')
 
   async def DownloadFile(self, *, untrusted_src_url: str, dst_path: Path):
     apis: List[RemoteFileAPIBase] = self._GetAPIsForURL(url=untrusted_src_url)
@@ -101,38 +105,43 @@
         return await api.DownloadFile(untrusted_src_url=untrusted_src_url,
                                       dst_path=dst_path)
       except ValueError:
         if i + 1 >= len(apis):
           raise
     raise AssertionError('unreachable')
 
-  async def DownloadTriplet(self, *, untrusted_src_triplet: ComfyUIPathTriplet,
+  async def DownloadTriplet(self, *, untrusted_comfy_api_url: str,
+                            untrusted_src_triplet: ComfyUIPathTriplet,
                             dst_path: Path):
     apis: List[RemoteFileAPIBase] = self._GetAPIsForTriplet(
-        triplet=untrusted_src_triplet)
+        comfy_api_url=untrusted_comfy_api_url, triplet=untrusted_src_triplet)
     for i, api in enumerate(apis):
       try:
         return await api.DownloadTriplet(
-            untrusted_src_triplet=untrusted_src_triplet, dst_path=dst_path)
+            untrusted_comfy_api_url=untrusted_comfy_api_url,
+            untrusted_src_triplet=untrusted_src_triplet,
+            dst_path=dst_path)
       except ValueError:
         if i + 1 >= len(apis):
           raise
     raise AssertionError('unreachable')
 
-  def TripletToURL(self, *, triplet: ComfyUIPathTriplet) -> str:
-    apis: List[RemoteFileAPIBase] = self._GetAPIsForTriplet(triplet=triplet)
+  def TripletToURL(self, *, comfy_api_url: str,
+                   triplet: ComfyUIPathTriplet) -> str:
+    apis: List[RemoteFileAPIBase] = self._GetAPIsForTriplet(
+        comfy_api_url=comfy_api_url, triplet=triplet)
     for i, api in enumerate(apis):
       try:
-        return api.TripletToURL(triplet=triplet)
+        return api.TripletToURL(comfy_api_url=comfy_api_url, triplet=triplet)
       except ValueError:
         if i + 1 >= len(apis):
           raise
     raise AssertionError('unreachable')
 
-  def URLToTriplet(self, *, url: str) -> ComfyUIPathTriplet:
+  def URLToTriplet(self, *, url: str) -> Tuple[str, ComfyUIPathTriplet]:
     apis: List[RemoteFileAPIBase] = self._GetAPIsForURL(url=url)
     for i, api in enumerate(apis):
       try:
         return api.URLToTriplet(url=url)
       except (NotImplementedError, ValueError):
         if i + 1 >= len(apis):
           raise
```

### Comparing `comfy_catapult-1.0.2/comfy_catapult/remote_file_api_local.py` & `comfy_catapult-2.0.0/comfy_catapult/remote_file_api_local.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # -*- coding: utf-8 -*-
 # SPDX-License-Identifier: MIT
 #
 # The Comfy Catapult project requires contributions made to this file be licensed
 # under the MIT license or a compatible open source license. See LICENSE.md for
 # the license text.
 
-from typing import List
+from typing import List, Tuple
 
 import aioshutil
 from anyio import Path
 
+from comfy_catapult.comfy_schema import ComfyUIPathTriplet
 from comfy_catapult.remote_file_api_base import RemoteFileAPIBase
-from comfy_catapult.url_utils import (ComfyUIPathTriplet, ToParseResult,
-                                      ValidateIsBasedURL)
+from comfy_catapult.url_utils import ToParseResult, ValidateIsBasedURL
 
 
 async def _LocalFileURLToLocalPath(url: str) -> Path:
   url_pr = ToParseResult(url)
   if url_pr.scheme != 'file':
     raise ValueError(f'URL {repr(url)} is not a file:// URL')
   if url_pr.netloc != '':
@@ -103,34 +103,36 @@
       raise ValueError(f'File {trusted_src_path} does not exist')
     if not await trusted_src_path.is_file():
       raise ValueError(f'File {trusted_src_path} is not a file')
 
     await dst_path.parent.mkdir(parents=True, exist_ok=True)
     await aioshutil.copy(trusted_src_path, dst_path)
 
-  async def DownloadTriplet(self, *, untrusted_src_triplet: ComfyUIPathTriplet,
+  async def DownloadTriplet(self, *, untrusted_comfy_api_url: str,
+                            untrusted_src_triplet: ComfyUIPathTriplet,
                             dst_path: Path):
     # TODO: Maybe we can make a mapper that maps triplets to urls, and then
     # download the file from the URL. But this is not necessary right now,
     # because you can use the ComfyAPIRemoteFileAPI to download triplets,
     # and the GenericRemoteFileAPI to handle it transparently by choosing
     # the RemoteAPIFileBase.
     raise NotImplementedError('Local files do not support triplets')
 
   async def UploadToTriplet(
-      self, *, src_triplet: ComfyUIPathTriplet,
+      self, *, src_triplet: ComfyUIPathTriplet, untrusted_comfy_api_url: str,
       untrusted_dst_triplet: ComfyUIPathTriplet) -> ComfyUIPathTriplet:
     # TODO: Maybe we can make a mapper that maps triplets to urls, and then
     # download the file from the URL. But this is not necessary right now,
     # because you can use the ComfyAPIRemoteFileAPI to download triplets,
     # and the GenericRemoteFileAPI to handle it transparently by choosing
     # the RemoteAPIFileBase.
     raise NotImplementedError('Local files do not support triplets')
 
-  def TripletToURL(self, *, triplet: ComfyUIPathTriplet) -> str:
+  def TripletToURL(self, *, comfy_api_url: str,
+                   triplet: ComfyUIPathTriplet) -> str:
     raise NotImplementedError('Local files do not support triplets')
 
-  def URLToTriplet(self, *, url: str) -> ComfyUIPathTriplet:
+  def URLToTriplet(self, *, url: str) -> Tuple[str, ComfyUIPathTriplet]:
     raise NotImplementedError('Local files do not support triplets')
 
   def GetBases(self) -> list[str]:
     return list(self._upload_to_bases + self._download_from_bases)
```

### Comparing `comfy_catapult-1.0.2/comfy_catapult.egg-info/SOURCES.txt` & `comfy_catapult-2.0.0/comfy_catapult.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 LICENSE.md
 README.md
-setup.py
+pyproject.toml
 comfy_catapult/__init__.py
 comfy_catapult/api_client.py
 comfy_catapult/api_client_base.py
 comfy_catapult/catapult.py
 comfy_catapult/catapult_base.py
-comfy_catapult/comfy_config.py
 comfy_catapult/comfy_schema.py
 comfy_catapult/comfy_schema_test.py
 comfy_catapult/comfy_utils.py
 comfy_catapult/errors.py
 comfy_catapult/eta_estimator.py
 comfy_catapult/remote_file_api_base.py
 comfy_catapult/remote_file_api_comfy.py
```

### Comparing `comfy_catapult-1.0.2/examples/utilities/sdxlturbo_parse_args.py` & `comfy_catapult-2.0.0/examples/utilities/sdxlturbo_parse_args.py`

 * *Files identical despite different names*

