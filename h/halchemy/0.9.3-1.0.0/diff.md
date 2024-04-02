# Comparing `tmp/halchemy-0.9.3-py3-none-any.whl.zip` & `tmp/halchemy-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 12680 bytes, number of entries: 15
+Zip file size: 11747 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat       22 b- defN 24-Mar-24 15:57 halchemy/__init__.py
--rw-rw-rw-  2.0 fat    13828 b- defN 24-Apr-02 18:50 halchemy/api.py
+-rw-rw-rw-  2.0 fat     6556 b- defN 24-Apr-02 19:33 halchemy/api.py
 -rw-rw-rw-  2.0 fat     2882 b- defN 24-Apr-02 18:50 halchemy/configuration.py
 -rw-rw-rw-  2.0 fat      501 b- defN 24-Apr-02 18:51 halchemy/error_handling.py
 -rw-rw-rw-  2.0 fat      545 b- defN 24-Apr-02 19:19 halchemy/follower.py
 -rw-rw-rw-  2.0 fat      478 b- defN 24-Apr-02 18:53 halchemy/http_model.py
 -rw-rw-rw-  2.0 fat      461 b- defN 24-Apr-02 18:56 halchemy/json_type.py
 -rw-rw-rw-  2.0 fat     6026 b- defN 24-Apr-02 19:20 halchemy/requester.py
 -rw-rw-rw-  2.0 fat     2629 b- defN 24-Apr-02 19:05 halchemy/requests_helper.py
 -rw-rw-rw-  2.0 fat     2735 b- defN 24-Apr-02 19:09 halchemy/resource.py
 -rw-rw-rw-  2.0 fat     1710 b- defN 24-Mar-26 13:12 halchemy/status_codes.py
--rw-rw-rw-  2.0 fat     1822 b- defN 24-Apr-02 19:25 halchemy-0.9.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 19:25 halchemy-0.9.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-02 19:25 halchemy-0.9.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1164 b- defN 24-Apr-02 19:25 halchemy-0.9.3.dist-info/RECORD
-15 files, 34904 bytes uncompressed, 10772 bytes compressed:  69.1%
+-rw-rw-rw-  2.0 fat     1822 b- defN 24-Apr-02 19:33 halchemy-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 19:33 halchemy-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-Apr-02 19:33 halchemy-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1163 b- defN 24-Apr-02 19:33 halchemy-1.0.0.dist-info/RECORD
+15 files, 27631 bytes uncompressed, 9839 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: halchemy/resource.py
 Comment: 
 
 Filename: halchemy/status_codes.py
 Comment: 
 
-Filename: halchemy-0.9.3.dist-info/METADATA
+Filename: halchemy-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: halchemy-0.9.3.dist-info/WHEEL
+Filename: halchemy-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: halchemy-0.9.3.dist-info/top_level.txt
+Filename: halchemy-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: halchemy-0.9.3.dist-info/RECORD
+Filename: halchemy-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## halchemy/api.py

```diff
@@ -10,24 +10,18 @@
 
 from .configuration import load_config
 from .error_handling import ErrorHandling
 from .follower import Follower
 from .requester import Requester, ReadOnlyRequester
 from .resource import Resource, HalResource, HalchemyMetadata
 from .requests_helper import RequestsWithDefaults
-from .json_type import JSON
 from .http_model import Request, Response
 from .status_codes import do_settings_include_status_code
 from requests.exceptions import HTTPError  # TODO: make our own!
 
-##########
-# DEPRECATED
-from urllib.parse import urlencode
-##########
-
 
 class Api:
 
     def __init__(self, base_url: str | None = None, headers: dict[str, Any] | None = None):
         config = load_config()
         self._base_url = base_url if base_url else config['halchemy']['base_url']
         self.parameters_list_style = config['halchemy']['parameters_list_style']
@@ -36,19 +30,14 @@
         self.error_handling.raise_for_network_error = config['error_handling']['raise_for_network_errors']
         self.error_handling.raise_for_status_codes = config['error_handling']['raise_for_status_codes']
         self._headers = CaseInsensitiveDict(config['headers'])
 
         if headers:
             self._headers.update(headers)
 
-        ####################
-        # DEPRECATED
-        self.last_error = {}
-        ####################
-
         if not self._base_url:
             raise ValueError('You must provide a base API URL, either in the constructor or in a config file.')
         self._api = RequestsWithDefaults(url_base=self._base_url, headers=self._headers)
 
     @property
     def base_url(self) -> str:
         return self._base_url
@@ -179,210 +168,7 @@
         return rtn
 
     def _raise_for_status_code(self, status_code, response):
         should_raise = do_settings_include_status_code(self.error_handling.raise_for_status_codes, status_code)
 
         if should_raise:
             raise HTTPError(response)
-
-
-
-
-
-##################################################################################
-    def get(self, url: str = '/', headers: dict[str, Any] | None = None) -> JSON:
-        if headers is None:
-            headers = {}
-
-        response = None
-        try:
-            self.last_error = {}
-
-            response = self._api.get(url, headers=headers)
-            if response.status_code == 404:
-                return {}
-            response.raise_for_status()
-            return response.json()
-        except HTTPError as ex:
-            self._handle_error('GET', url, response, ex)
-
-    def get_from_rel(self, resource,
-                     rel: str,
-                     parameters: dict[str, Any] | None = None,
-                     template: dict[str, Any] | None = None,
-                     headers: dict[str, Any] | None = None
-                     ) -> JSON:
-        if headers is None:
-            headers = {}
-        if template is None:
-            template = {}
-        if parameters is None:
-            parameters = {}
-
-        url = self.url_from_rel(resource, rel, parameters, template)
-        return self.get(url, headers=headers)
-
-    def post_to_rel(self, resource,
-                    rel: str,
-                    data: JSON,
-                    parameters: dict[str, Any] | None = None,
-                    template: dict[str, Any] | None = None,
-                    headers: dict[str, Any] | None = None
-                    ) -> JSON:
-        if headers is None:
-            headers = {}
-        if template is None:
-            template = {}
-        if parameters is None:
-            parameters = {}
-
-        url = self.url_from_rel(resource, rel, parameters, template)
-        return self.post_to_url(url, data, headers=headers)
-
-    def delete_resource(self, resource, headers: dict[str, Any] | None = None) -> JSON:
-        if headers is None:
-            headers = {}
-
-        url = self.url_from_rel(resource, 'self')
-        headers.update({
-            'If-Match': resource['_etag']
-        })
-
-        response = None
-        try:
-            self.last_error = {}
-            response = self._api.delete(url, headers=headers)
-            response.raise_for_status()
-            return response.json()
-        except HTTPError as ex:
-            self._handle_error('DELETE', url, response, ex)
-
-    def patch_resource(self, resource, data: JSON, headers: dict[str, Any] | None = None) -> JSON:
-        if headers is None:
-            headers = {}
-
-        if type(data) is not str:
-            data = json.dumps(data)
-        url = self.url_from_rel(resource, 'self')
-        headers.update({
-            'If-Match': resource['_etag']
-        })
-
-        response = None
-        try:
-            self.last_error = {}
-            response = self._api.patch(url, data=data, headers=headers)
-            response.raise_for_status()
-            return response.json()
-        except HTTPError as ex:
-            self._handle_error('PATCH', url, response, ex)
-
-    def put_to_rel(self, resource,
-                   rel: str,
-                   data: JSON,
-                   parameters: dict[str, Any] | None = None,
-                   template: dict[str, Any] | None = None,
-                   headers: dict[str, Any] | None = None
-                   ) -> JSON:
-        if headers is None:
-            headers = {}
-
-        if type(data) is not str:
-            data = json.dumps(data)
-        url = self.url_from_rel(resource, rel, parameters, template)
-        headers.update({
-            'If-Match': resource['_etag']
-        })
-
-        response = None
-        try:
-            self.last_error = {}
-            response = self._api.put(url, data=data, headers=headers)
-            response.raise_for_status()
-            return response.json()
-        except HTTPError as ex:
-            self._handle_error('PUT', url, response, ex)
-
-    def get_from_rel_with_lookup(self, resource,
-                                 rel: str,
-                                 lookup: str,
-                                 parameters: dict[str, Any] | None = None,
-                                 headers: dict[str, Any] | None = None
-                                 ) -> JSON:
-        # no template because lookup is an implicit template
-        if headers is None:
-            headers = {}
-        if parameters is None:
-            parameters = {}
-
-        url = resource['_links'][rel]['href']
-        if url[-1] != '/':
-            url += '/'
-        url += lookup
-
-        query_string = urlencode(parameters)
-
-        return self.get(f"{url}{'?' if parameters else ''}{query_string}", headers=headers)
-
-    def post_to_url(self, url: str, data: JSON, headers: dict[str, Any] | None = None) -> JSON:
-        if headers is None:
-            headers = {}
-
-        if type(data) is not str:
-            data = json.dumps(data)
-
-        response = None
-        try:
-            self.last_error = {}
-            response = self._api.post(url, data=data, headers=headers)
-            response.raise_for_status()
-            return response.json()
-        except HTTPError as ex:
-            self._handle_error('POST', url, response, ex)
-
-    def delete_url(self, url: str, headers: dict[str, Any] | None = None) -> JSON:
-        if headers is None:
-            headers = {}
-
-        response = None
-        try:
-            self.last_error = {}
-            response = self._api.delete(url, headers=headers)
-            response.raise_for_status()
-            return response.json()
-        except HTTPError as ex:
-            self._handle_error('DELETE', url, response, ex)
-
-    @staticmethod
-    def url_from_rel(resource, rel, parameters=None, template=None):
-        if template is None:
-            template = {}
-        if parameters is None:
-            parameters = {}
-
-        url = resource['_links'][rel]['href']
-        if resource['_links'][rel].get('templated', False):
-            try:
-                url = url.format(**template)
-            except KeyError as ex:
-                print(f'This link is templated.  You must supply a value for {ex}')
-                return ''
-
-        query_string = urlencode(parameters)
-
-        return f"{url}{'?' if parameters else ''}{query_string}"
-
-    def _handle_error(self, method, url, response, error):
-        self.last_error = {
-            'method': method,
-            'url': url,
-            'status_code': response.status_code,
-            'reason': response.reason,
-            'details': response.text,
-            'response': response,
-            'error': error
-        }
-        message = f'{method} {url} - {response.status_code} {response.reason}'
-        details = response.text
-        raise RuntimeError(f'{message}\n{details}\nsee self.last_error for more details')
-
-##################################################################################
```

## Comparing `halchemy-0.9.3.dist-info/METADATA` & `halchemy-1.0.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: halchemy
-Version: 0.9.3
+Version: 1.0.0
 Summary: Toolkit for creating clients of HAL based Hypermedia APIs.
 Home-page: https://github.com/pointw-dev/halchemy
 Author: Michael Ottoson
 Author-email: michael@pointw.com
 License: MIT
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
```

