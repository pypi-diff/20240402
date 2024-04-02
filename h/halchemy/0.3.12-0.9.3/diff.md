# Comparing `tmp/halchemy-0.3.12-py3-none-any.whl.zip` & `tmp/halchemy-0.9.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 11773 bytes, number of entries: 15
+Zip file size: 12680 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat       22 b- defN 24-Mar-24 15:57 halchemy/__init__.py
--rw-rw-rw-  2.0 fat    13564 b- defN 24-Mar-27 10:43 halchemy/api.py
--rw-rw-rw-  2.0 fat     2683 b- defN 24-Mar-27 10:43 halchemy/configuration.py
--rw-rw-rw-  2.0 fat      364 b- defN 24-Mar-25 23:55 halchemy/error_handling.py
--rw-rw-rw-  2.0 fat      423 b- defN 24-Mar-24 16:34 halchemy/follower.py
--rw-rw-rw-  2.0 fat     1283 b- defN 24-Mar-24 15:57 halchemy/http_model.py
--rw-rw-rw-  2.0 fat      228 b- defN 24-Mar-25 22:43 halchemy/json_type.py
--rw-rw-rw-  2.0 fat     5773 b- defN 24-Mar-24 15:57 halchemy/requester.py
--rw-rw-rw-  2.0 fat     2601 b- defN 24-Mar-24 15:57 halchemy/requests_helper.py
--rw-rw-rw-  2.0 fat     2232 b- defN 24-Mar-26 16:48 halchemy/resource.py
+-rw-rw-rw-  2.0 fat    13828 b- defN 24-Apr-02 18:50 halchemy/api.py
+-rw-rw-rw-  2.0 fat     2882 b- defN 24-Apr-02 18:50 halchemy/configuration.py
+-rw-rw-rw-  2.0 fat      501 b- defN 24-Apr-02 18:51 halchemy/error_handling.py
+-rw-rw-rw-  2.0 fat      545 b- defN 24-Apr-02 19:19 halchemy/follower.py
+-rw-rw-rw-  2.0 fat      478 b- defN 24-Apr-02 18:53 halchemy/http_model.py
+-rw-rw-rw-  2.0 fat      461 b- defN 24-Apr-02 18:56 halchemy/json_type.py
+-rw-rw-rw-  2.0 fat     6026 b- defN 24-Apr-02 19:20 halchemy/requester.py
+-rw-rw-rw-  2.0 fat     2629 b- defN 24-Apr-02 19:05 halchemy/requests_helper.py
+-rw-rw-rw-  2.0 fat     2735 b- defN 24-Apr-02 19:09 halchemy/resource.py
 -rw-rw-rw-  2.0 fat     1710 b- defN 24-Mar-26 13:12 halchemy/status_codes.py
--rw-rw-rw-  2.0 fat     1435 b- defN 24-Mar-27 10:48 halchemy-0.3.12.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-27 10:48 halchemy-0.3.12.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Mar-27 10:48 halchemy-0.3.12.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1169 b- defN 24-Mar-27 10:48 halchemy-0.3.12.dist-info/RECORD
-15 files, 33588 bytes uncompressed, 9857 bytes compressed:  70.7%
+-rw-rw-rw-  2.0 fat     1822 b- defN 24-Apr-02 19:25 halchemy-0.9.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 19:25 halchemy-0.9.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-02 19:25 halchemy-0.9.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1164 b- defN 24-Apr-02 19:25 halchemy-0.9.3.dist-info/RECORD
+15 files, 34904 bytes uncompressed, 10772 bytes compressed:  69.1%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: halchemy/resource.py
 Comment: 
 
 Filename: halchemy/status_codes.py
 Comment: 
 
-Filename: halchemy-0.3.12.dist-info/METADATA
+Filename: halchemy-0.9.3.dist-info/METADATA
 Comment: 
 
-Filename: halchemy-0.3.12.dist-info/WHEEL
+Filename: halchemy-0.9.3.dist-info/WHEEL
 Comment: 
 
-Filename: halchemy-0.3.12.dist-info/top_level.txt
+Filename: halchemy-0.9.3.dist-info/top_level.txt
 Comment: 
 
-Filename: halchemy-0.3.12.dist-info/RECORD
+Filename: halchemy-0.9.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## halchemy/api.py

```diff
@@ -1,7 +1,11 @@
+"""
+This module defines the Api class, which is the main class for interacting with HAL-based APIs.
+"""
+
 import json
 from typing import Any
 
 from requests import JSONDecodeError
 from requests.structures import CaseInsensitiveDict
 
 from .configuration import load_config
@@ -21,15 +25,14 @@
 ##########
 
 
 class Api:
 
     def __init__(self, base_url: str | None = None, headers: dict[str, Any] | None = None):
         config = load_config()
-
         self._base_url = base_url if base_url else config['halchemy']['base_url']
         self.parameters_list_style = config['halchemy']['parameters_list_style']
         self.etag_field = config['halchemy']['etag_field']
         self.error_handling = ErrorHandling()
         self.error_handling.raise_for_network_error = config['error_handling']['raise_for_network_errors']
         self.error_handling.raise_for_status_codes = config['error_handling']['raise_for_status_codes']
         self._headers = CaseInsensitiveDict(config['headers'])
@@ -43,24 +46,24 @@
         ####################
 
         if not self._base_url:
             raise ValueError('You must provide a base API URL, either in the constructor or in a config file.')
         self._api = RequestsWithDefaults(url_base=self._base_url, headers=self._headers)
 
     @property
-    def base_url(self):
+    def base_url(self) -> str:
         return self._base_url
 
     @base_url.setter
     def base_url(self, base_url: str):
         self._base_url = base_url
         self._api = RequestsWithDefaults(url_base=self._base_url, headers=self._headers)
 
     @property
-    def headers(self):
+    def headers(self) -> CaseInsensitiveDict:
         return self._headers
 
     @headers.setter
     def headers(self, headers: dict[str, Any]):
         self._headers = headers
         self._api = RequestsWithDefaults(url_base=self._base_url, headers=self._headers)
 
@@ -70,32 +73,32 @@
 
     def remove_headers(self, headers: list[str]):
         for header in headers:
             self._headers.pop(header, None)
         self._api = RequestsWithDefaults(url_base=self._base_url, headers=self._headers)
 
     @property
-    def root(self):
+    def root(self) -> Requester:
         return self.using_endpoint('/', is_root=True)
 
-    def follow(self, resource: HalResource):
+    def follow(self, resource: HalResource) -> Follower:
         return Follower(self, resource)
 
-    def get_optimistic_concurrency_header(self, resource: HalResource):
+    def get_optimistic_concurrency_header(self, resource: HalResource) -> CaseInsensitiveDict:
         etag = None
         try:
             etag = resource._halchemy.response.headers.get('Etag')
         except AttributeError:
             pass
         if etag is None:
             etag = resource.get(self.etag_field)
 
-        return {'If-Match': etag} if etag else {}
+        return CaseInsensitiveDict({'If-Match': etag}) if etag else {}
 
-    def using_endpoint(self, url, is_root=False):
+    def using_endpoint(self, url: str, is_root: bool=False) -> Requester | ReadOnlyRequester:
         if is_root:
             return ReadOnlyRequester(self, url)
         return Requester(self, url)
 
     def request(self,
                 method: str,
                 url: str,
@@ -130,15 +133,15 @@
         )
 
         try:
             result = self._api.request(method, url, data=data, headers=headers)
             request = Request(
                 method=method,
                 url=result.url,
-                headers=CaseInsensitiveDict(result.headers),
+                headers=CaseInsensitiveDict(dict(result.request.headers)),
                 body=result.request.body
             )
         except Exception as e:
             response = Response(
                 status_code=0,
                 reason='Did not receive a response from the server',
                 headers=CaseInsensitiveDict({}),
```

## halchemy/configuration.py

```diff
@@ -1,52 +1,57 @@
+"""
+This module provides functions to load configuration from an .ini file.
+It is intended only for internal use by the library.
+"""
+
 import inspect
 import os
 import configparser
 
 
-def get_caller_file():
+def get_caller_file() -> str | None:
     # Get the current stack frame and go back one level to find the caller
     # The 0-index is the current function, 1-index is the caller
     caller_frame = inspect.stack()[4]
     caller_module = inspect.getmodule(caller_frame[0])
     if caller_module is not None and hasattr(caller_module, '__file__'):
         # Return the path of the caller's file
         return caller_module.__file__
     else:
         # Caller does not have a __file__ attribute, or inspection failed
         return None
 
 
-def find_project_root(current_dir=None):
+def find_project_root(current_dir: str =None) -> str | None:
     current_dir = current_dir or os.path.dirname(get_caller_file())
     root_indicators = [
         '.git', 'pyproject.toml', 'requirements.txt',
         'setup.py', 'setup.cfg', '.venv', 'venv',
         '.project', '.idea', '.vscode',
         'Pipfile', 'poetry.lock', '.halchemy'
     ]
     while current_dir != os.path.dirname(current_dir):  # Stop at the filesystem root
         if any(os.path.exists(os.path.join(current_dir, indicator)) for indicator in root_indicators):
             return current_dir
         current_dir = os.path.dirname(current_dir)
     return None
 
 
-def ini_to_dict(config_filename, project_root):
+def ini_to_dict(config_filename: str, project_root: str) -> dict:
     config = {}
     config_path = os.path.join(project_root, config_filename)
     if os.path.exists(config_path):
         parser = configparser.ConfigParser()
         parser.read(config_path)
         for section in parser.sections():
             config[section] = dict(parser.items(section))
     return config
 
 
-def load_config():
+def load_config() -> dict:
     config_filename = '.halchemy'
     project_root = find_project_root()
     rtn = {
         'halchemy': {
             'base_url': 'http://localhost:2112',
             'parameters_list_style': 'repeat_key',
             'etag_field': '_etag'
```

## halchemy/error_handling.py

```diff
@@ -1,10 +1,15 @@
+"""
+This module defines the ErrorHandling class which the Api class uses to determine how to handle errors.
+"""
+
+
 class ErrorHandling:
     def __init__(self):
-        self.raise_for_network_error = True
-        self.raise_for_status_codes = None
+        self.raise_for_network_error: bool = True
+        self.raise_for_status_codes: str | None = None
 
     def __str__(self):
         return f'raise_on_network_error: {self.raise_for_network_error}, raise_for_status_codes: {self.raise_for_status_codes}'
 
     def __repr__(self):
         return f'ErrorSettings({str(self)})'
```

## halchemy/follower.py

```diff
@@ -1,13 +1,17 @@
+"""
+This module provides the Follower class, which is used to follow links from a HalResource.
+"""
+
 from .resource import HalResource
 from .requester import Requester
 
 
 class Follower:
     def __init__(self, api, resource: HalResource):
         self.api = api
         self.resource = resource
 
-    def to(self, rel):
+    def to(self, rel: str) -> Requester:
         if rel not in self.resource['_links']:
             raise KeyError(f"This resource does not have a link relation named '{rel}'")
         return Requester(self.api, (self.resource, rel))
```

## halchemy/http_model.py

```diff
@@ -1,8 +1,12 @@
-from typing import Dict, NamedTuple, Optional
+"""
+This module contains the data model for HTTP requests and responses.  Intended only for internal use.
+"""
+
+from typing import NamedTuple, Optional
 
 from requests.structures import CaseInsensitiveDict
 
 
 class Request(NamedTuple):
     method: str
     url: str
@@ -11,31 +15,7 @@
 
 
 class Response(NamedTuple):
     status_code: int
     reason: str
     headers: CaseInsensitiveDict
     body: Optional[str] = None
-
-# from typing import Dict, Optional, Union
-#
-#
-# class HttpRequest:
-#     def __init__(self, method: str, url: str, headers: Optional[Dict[str, str]] = None, body: Optional[Union[str, bytes]] = None):
-#         self.method = method
-#         self.url = url
-#         self.headers = headers if headers is not None else {}
-#         self.body = body
-#
-#     def __repr__(self):
-#         return f"HttpRequest(method={self.method}, url={self.url}"
-#
-#
-# class HttpResponse:
-#     def __init__(self, status_code: int, reason: str, headers: Optional[Dict[str, str]] = None, body: Optional[Union[str, bytes]] = None):
-#         self.status_code = status_code
-#         self.reason = reason
-#         self.headers = headers if headers is not None else {}
-#         self.body = body
-#
-#     def __repr__(self):
-#         return f"HttpResponse(status_code={self.status_code}, reason={self.reason}"
```

## halchemy/json_type.py

```diff
@@ -1,7 +1,12 @@
+"""
+This module contains the type alias for JSON and JSON_NULL.  Use JSON_NULL when you want to explicitly include
+a null value in your request body, instead of using a regular null|None which will result in an empty body.
+"""
+
 from typing import TypeAlias
 
 JSON: TypeAlias = dict[str, "JSON"] | list["JSON"] | str | int | float | bool | None
 
 
 class JsonNullType:
     def __repr__(self):
```

## halchemy/requester.py

```diff
@@ -1,11 +1,19 @@
+"""
+This module defines the Requester set of classes, which can be used as the end of the fluent chain, or extended
+to provide more specific details.  Intended primarily to be used internally, but may be useful to manipulate
+outside a fluent chain.
+"""
+
 from typing import Any, Tuple
 from urllib.parse import quote_plus
+
+import uritemplate
 from requests.structures import CaseInsensitiveDict
-from .resource import HalResource
+from .resource import HalResource, Resource
 
 
 class BaseRequester:
     def __init__(self, api, target: str | Tuple[HalResource, str]):
         self._api = api
         self._headers = CaseInsensitiveDict({})
         self._parameters = {}
@@ -20,46 +28,34 @@
 
         resource, rel = target
         self._url = resource['_links'][rel]['href']
         self._is_templated = resource['_links'][rel].get('templated', False)
         self.resource = resource
 
     @property
-    def url(self):
-        url = self._url
-        # ASSERT: the href IS a URL
-
-        if self._is_templated:
-            missing_keys = [k.strip("{}") for k in url.split("/")
-                            if "{" in k and k.strip("{}") not in self._template_values]
-
-            if not self._template_values:
-                raise ValueError("This link is templated, but no template values were provided. "
-                                 f"Missing template values for link: {', '.join(missing_keys)}")
-
-            if missing_keys:
-                raise ValueError(f"Not enough template values were provided. "
-                                 f"Missing template values for link: {', '.join(missing_keys)}")
-
-            url = url.format(**self._template_values)
+    def url(self) -> str:
+        try:
+            url = uritemplate.expand(self._url, self._template_values or {})
+        except Exception as e:
+            raise ValueError(f"Error expanding template: {e}")
 
         if self._parameters:
-            url = self._add_parameters_to_url(url, self._parameters)
+            url = self._add_parameters_to_url(url)
 
         return url
 
-    def with_headers(self, headers: dict[str, Any]):
+    def with_headers(self, headers: dict[str, Any]) -> 'BaseRequester':
         self._headers.update(headers)
         return self
 
-    def with_parameters(self, parameters: dict[str, Any]):
+    def with_parameters(self, parameters: dict[str, Any]) -> 'BaseRequester':
         self._parameters.update(parameters)
         return self
 
-    def with_template_values(self, template_values: dict[str, Any]):
+    def with_template_values(self, template_values: dict[str, Any]) -> 'BaseRequester':
         self._template_values.update(template_values)
         return self
 
     def _handle_list(self, key: str, array: list) -> list:
         list_style = self._api.parameters_list_style
 
         if list_style == "repeat_key":
@@ -87,65 +83,75 @@
                 flattened.extend(self._flatten_parameters(full_key, value))
             elif isinstance(value, bool):
                 flattened.append((full_key, str(value).lower()))
             else:
                 flattened.append((full_key, quote_plus(str(value))))
         return flattened
 
-    def _add_parameters_to_url(self, url: str, parameters: dict) -> str:
-        query_params = self._flatten_parameters('', parameters)
+    def _add_parameters_to_url(self, url: str) -> str:
+        query_params = self._flatten_parameters('', self._parameters)
 
         query_string_parts = []
         for key, value in query_params:
             part = key if value is None else f"{key}={value}"
             query_string_parts.append(part)
         query_string = '&'.join(query_string_parts)
 
         if '?' in url and not url.endswith('?'):
             return f"{url}&{query_string}"
         else:
             return f"{url}{'' if url.endswith('?') else '?'}{query_string}"
 
-    def _request(self, method: str):
+    def _request(self, method: str) -> Resource:
         return self._api.request(method, self.url, data=self._data, headers=self._headers)
 
 
 class ReadOnlyRequester(BaseRequester):
+    """
+    This class extends the ABC BaseRequester with the read-only HTTP methods: GET, HEAD, and OPTIONS.
+    """
+
     def __init__(self, api, target: str | Tuple[HalResource, str]):
         super().__init__(api, target)
 
-    def get(self):
+    def get(self) -> Resource:
         return self._request('GET')
 
-    def head(self):
+    def head(self) -> Resource:
         return self._request('HEAD')
 
-    def options(self):
+    def options(self) -> Resource:
         return self._request('OPTIONS')
 
 
 class Requester(ReadOnlyRequester):
+    """
+    This class extends the ReadOnlyRequester adding the "writeable" methods: POST, PUT, PATCH, and DELETE.
+    Notice the slight differences between "Payload" methods: POST, PUT, PATCH,
+    and the "Optimistic Concurrency aware" methods: PUT, PATCH, DELETE.
+    """
+
     def __init__(self, api, target: str | Tuple[HalResource, str]):
         super().__init__(api, target)
 
-    def post(self, data=None, content_type=None):
+    def post(self, data=None, content_type=None) -> Resource:
         self._prepare_payload(data, content_type)
         return self._request('POST')
 
-    def put(self, data=None, content_type=None):
+    def put(self, data=None, content_type=None) -> Resource:
         self._prepare_payload(data, content_type)
         self._prepare_modify_header()
         return self._request('PUT')
 
-    def patch(self, data=None, content_type=None):
+    def patch(self, data=None, content_type=None) -> Resource:
         self._prepare_payload(data, content_type)
         self._prepare_modify_header()
         return self._request('PATCH')
 
-    def delete(self):
+    def delete(self) -> Resource:
         self._prepare_modify_header()
         return self._request('DELETE')
 
     def _prepare_payload(self, data, content_type):
         self._data = data
         if content_type:
             self._headers['Content-type'] = content_type
```

## halchemy/requests_helper.py

```diff
@@ -1,8 +1,8 @@
-"""Extends requests.Session to add url_base and default headers to requests
+"""Extends requests.Session to add url_base (to resolve relative paths) and default headers to requests
 
 Usage:
     Pass url_base and/or headers to constructor
 
 Examples:
     api =  RequestsWithDefaults(url_base='https://example.org/my-api', headers={
         'Content-type': 'application/json',
```

## halchemy/resource.py

```diff
@@ -1,16 +1,24 @@
+"""
+The Resource class extends a plain dictionary to include a metadata object containing details
+about the HTTP request and response.  This lets the metadata stay "out of the way" allowing
+the client code to use the result of a request directly as a resource without losing access
+to the request details, response details, and any error details.  If the resource is a HAL
+representation, the HalResource class also provides extra functionality.
+"""
+
 from typing import Iterator
 
 from .http_model import Response, Request
 from .status_codes import do_settings_include_status_code
 from requests.exceptions import HTTPError
 
 
 class HalchemyMetadata:
-    def __init__(self, request, response, error):
+    def __init__(self, request: Request, response: Response, error: Exception | None = None):
         self.response: Response | None = response
         self.request: Request | None = request
         self.error = error
 
     def raise_for_status_codes(self, settings: str = '>399'):
         status_code = self.response.status_code
         should_raise = do_settings_include_status_code(settings, status_code)
```

## Comparing `halchemy-0.3.12.dist-info/RECORD` & `halchemy-0.9.3.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 halchemy/__init__.py,sha256=ckzAcd6WlzwEgKWsiH99POnUIfboAPjhzeiFvXL8dCM,22
-halchemy/api.py,sha256=yEeeNppF68h2Lf8v0E4u_t1hTLQMy2hXvjxV8el7m4o,13564
-halchemy/configuration.py,sha256=bUPicyZ28gehhTaiBzXqKn2vGHvmYrnKACbaJp4Dyc8,2683
-halchemy/error_handling.py,sha256=hl-bjOrWM7KcPr_-IEwWm4BNCEKZHqVU_ZDJ_uxK5Tg,364
-halchemy/follower.py,sha256=mvJ-PAI2tgl8p1tiF8U-me0NLfYGdB6-adCbrQq92xI,423
-halchemy/http_model.py,sha256=qsdLgwv1P8t9n0zRrZjrmhMNlHY7yg1dAtWcD7AEy_Q,1283
-halchemy/json_type.py,sha256=q28gY69MjMGt4yaiCauFFFFs5jvJO0J8TPlDWM635Z8,228
-halchemy/requester.py,sha256=Ld36RZE6XmHFP9SU_fH8pEXou8xGexFC59341BCXLv8,5773
-halchemy/requests_helper.py,sha256=IqpZZIL5520KW5cUnyTmt-as7L6Mu3SPWZm7CiMjslU,2601
-halchemy/resource.py,sha256=S5-450PUUs1zCcPvYCWo_EIGbPHAipo9o6lU1VqFQ3I,2232
+halchemy/api.py,sha256=LQEmzl6CqGcBEebUlNppyQ9ThsU6g9AJ5C3TgbamgPM,13828
+halchemy/configuration.py,sha256=w-EZZac6_ZjagNRSqM7jfebx2SdXPClHC2Zzczjsr8o,2882
+halchemy/error_handling.py,sha256=Dc8wcVRNW2SKkf6hNjuclUmbK2Mcyom7gfEs78_qP8A,501
+halchemy/follower.py,sha256=xVo5f5j6stzdvnOgjwCXcXuA_a902SE7hx-Gg6HUZPk,545
+halchemy/http_model.py,sha256=z65_W7xKqSIuqyiUWQTkmYyC-DdCLNGcA4m-m3C-R_g,478
+halchemy/json_type.py,sha256=jkrC5A_WFb3O6Nz9Zt2730hOwRsf7LBteyY6boxyz4o,461
+halchemy/requester.py,sha256=JYF61YwPros1xM-BHpy659qPKujEvvUm_Ji_IeUzfEI,6026
+halchemy/requests_helper.py,sha256=fR3aL4qIDzkrbdVB0dfp0H9jmJESMw_zyQ5m9NvKoJc,2629
+halchemy/resource.py,sha256=TjLgSjwuveITwdmyEsjSs3Ykz45ewZBWibF6UjCoDEs,2735
 halchemy/status_codes.py,sha256=UXE4WtHkfcQ9wRSITerVDe3ofk7kBlM9Erq2tOUgjh4,1710
-halchemy-0.3.12.dist-info/METADATA,sha256=WGl446othpG1JxJcPYCW47NzxG6hEXQn4Gj6wLfr8tA,1435
-halchemy-0.3.12.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-halchemy-0.3.12.dist-info/top_level.txt,sha256=QDAX4T2q2TC09LWO_LgEyuEBr-lPTU86p48miwnpfzw,9
-halchemy-0.3.12.dist-info/RECORD,,
+halchemy-0.9.3.dist-info/METADATA,sha256=ph2tOBsIY5EMMMSDXbZZjGq5UePZ3vslapslaUphnnI,1822
+halchemy-0.9.3.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+halchemy-0.9.3.dist-info/top_level.txt,sha256=QDAX4T2q2TC09LWO_LgEyuEBr-lPTU86p48miwnpfzw,9
+halchemy-0.9.3.dist-info/RECORD,,
```

