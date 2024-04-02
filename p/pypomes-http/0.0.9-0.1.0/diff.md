# Comparing `tmp/pypomes_http-0.0.9.tar.gz` & `tmp/pypomes_http-0.1.0.tar.gz`

## Comparing `pypomes_http-0.0.9.tar` & `pypomes_http-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1253 2020-02-02 00:00:00.000000 pypomes_http-0.0.9/src/pypomes_http/__init__.py
--rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 pypomes_http-0.0.9/src/pypomes_http/http_async.py
--rw-r--r--   0        0        0    10660 2020-02-02 00:00:00.000000 pypomes_http-0.0.9/src/pypomes_http/http_pomes.py
--rw-r--r--   0        0        0    22949 2020-02-02 00:00:00.000000 pypomes_http-0.0.9/src/pypomes_http/http_statuses.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.0.9/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.0.9/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.0.9/README.md
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.0.9/pyproject.toml
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/src/pypomes_http/__init__.py
+-rw-r--r--   0        0        0     4829 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/src/pypomes_http/http_async.py
+-rw-r--r--   0        0        0    12440 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/src/pypomes_http/http_pomes.py
+-rw-r--r--   0        0        0    22949 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/src/pypomes_http/http_statuses.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/README.md
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pypomes_http-0.1.0/PKG-INFO
```

### Comparing `pypomes_http-0.0.9/src/pypomes_http/__init__.py` & `pypomes_http-0.1.0/src/pypomes_http/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 )
 from .http_pomes import (
     HTTP_DELETE_TIMEOUT, HTTP_GET_TIMEOUT, HTTP_POST_TIMEOUT, HTTP_PUT_TIMEOUT,
     MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
     MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
     MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
     http_status_code, http_status_name, http_status_description,
-    http_json_from_request, http_get, http_post, http_put,
+    http_json_from_request, http_delete, http_get, http_post, http_put,
 )
 
 __all__ = [
     # http_async
     "HttpAsync",
     # http_pomes
     "HTTP_DELETE_TIMEOUT", "HTTP_GET_TIMEOUT", "HTTP_POST_TIMEOUT", "HTTP_PUT_TIMEOUT",
     "MIMETYPE_BINARY", "MIMETYPE_CSS", "MIMETYPE_CSV", "MIMETYPE_HTML", "MIMETYPE_JAVASCRIPT",
     "MIMETYPE_JSON", "MIMETYPE_MULTIPART", "MIMETYPE_PDF", "MIMETYPE_PKCS7", "MIMETYPE_SOAP",
     "MIMETYPE_TEXT", "MIMETYPE_URLENCODED", "MIMETYPE_XML", "MIMETYPE_ZIP",
     "http_status_code", "http_status_name", "http_status_description",
-    "http_json_from_request", "http_get", "http_post", "http_put",
+    "http_json_from_request", "http_delete", "http_get", "http_post", "http_put",
 ]
 
 from importlib.metadata import version
 __version__ = version("pypomes_http")
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_http-0.0.9/src/pypomes_http/http_async.py` & `pypomes_http-0.1.0/src/pypomes_http/http_async.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.0.9/src/pypomes_http/http_pomes.py` & `pypomes_http-0.1.0/src/pypomes_http/http_pomes.py`

 * *Files 9% similar despite different names*

```diff
@@ -77,53 +77,79 @@
 
     :param request: the Request object
     :return: dict containing the input parameters (empty, if no input data exist)
     """
     # declare the return variable
     result: dict
 
-    # is JSON the content-type of the request ?
+    # is JSON the content type of the request ?
     if request.mimetype == MIMETYPE_JSON:
         # yes, retrieve it
         result = request.get_json()
     else:
         # no, try parameters in URL query
         result = request.values  # noqa (bug: Ruff reports PD011)
         if len(result) == 0:
             # no query parameters, try the form
             result = request.form  # empty dictionary, if no form or empty form
 
     return result
 
 
-def http_get(errors: list[str] | None, url: str, headers: dict = None, params: dict = None,
-             auth: str = None, timeout: int | None = HTTP_GET_TIMEOUT, logger: logging.Logger = None) -> Response:
+def http_delete(errors: list[str] | None, url: str, headers: dict = None,
+                params: dict = None, data: dict = None, json: dict = None, auth: str = None,
+                timeout: int | None = HTTP_DELETE_TIMEOUT, logger: logging.Logger = None) -> Response:
     """
-    Issue a *GET* request to the given *url*, and retriever the returned response.
+    Issue a *DELETE* request to the given *url*,and retrieve the returned response.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
     :param params: optional parameters
+    :param data: optionaL data to send in the body of the request
+    :param json: optional JSON to send in the body of the request
+    :param auth: optional authentication scheme to use
+    :param timeout: timeout, in seconds (defaults to HTTP_POST_TIMEOUT - use None to omit)
+    :param logger: optional logger to log the operation with
+    :return: the response to the PUT operation
+    """
+    return _http_rest(errors, "DELETE", url, headers, params, data, json, auth, timeout, logger)
+
+
+def http_get(errors: list[str] | None, url: str, headers: dict = None,
+             params: dict = None, data: dict = None, json: dict = None, auth: str = None,
+             timeout: int | None = HTTP_GET_TIMEOUT, logger: logging.Logger = None) -> Response:
+    """
+    Issue a *GET* request to the given *url*,and retrieve the returned response.
+
+    The returned response might be *None*.
+    The request might contain *headers* and *parameters*.
+
+    :param errors: incidental error messages
+    :param url: the destination URL
+    :param headers: optional headers
+    :param params: optional parameters
+    :param data: optionaL data to send in the body of the request
+    :param json: optional JSON to send in the body of the request
     :param auth: optional authentication scheme to use
     :param timeout: timeout, in seconds (defaults to HTTP_GET_TIMEOUT - use None to omit)
     :param logger: optional logger
     :return: the response to the GET operation
     """
-    return _http_rest(errors, "GET", url, headers, params, None, None, auth, timeout, logger)
+    return _http_rest(errors, "GET", url, headers, params, data, json, auth, timeout, logger)
 
 
 def http_post(errors: list[str] | None, url: str, headers: dict = None,
               params: dict = None, data: dict = None, json: dict = None, auth: str = None,
               timeout: int | None = HTTP_POST_TIMEOUT, logger: logging.Logger = None) -> Response:
     """
-    Issue a *POST* request to the given *url*, and retriever the returned response.
+    Issue a *POST* request to the given *url*,and retrieve the returned response.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
@@ -138,15 +164,15 @@
     return _http_rest(errors, "POST", url, headers, params, data, json, auth, timeout, logger)
 
 
 def http_put(errors: list[str] | None, url: str, headers: dict = None,
              params: dict = None, data: dict = None, json: dict = None, auth: str = None,
              timeout: int | None = HTTP_POST_TIMEOUT, logger: logging.Logger = None) -> Response:
     """
-    Issue a *PUT* request to the given *url*, and retriever the returned response.
+    Issue a *PUT* request to the given *url*,and retrieve the returned response.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
@@ -161,15 +187,15 @@
     return _http_rest(errors, "PUT", url, headers, params, data, json, auth, timeout, logger)
 
 
 def _http_rest(errors: list[str], method: str, url: str, headers: dict,
                params: dict, data: dict | None, json: dict | None,
                auth: str | None, timeout: int, logger: logging.Logger) -> Response:
     """
-    Issue a *REST* request to the given *url*, and retriever the returned response.
+    Issue a *REST* request to the given *url*,and retrieve the returned response.
 
     The returned response might be *None*.
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param method: the REST method to use (GET, POST or PUT)
     :param url: the destination URL
@@ -215,18 +241,27 @@
             else:
                 err_msg = f"Authentication scheme '{auth}' not implemented"
 
         # were there errors ?
         if not err_msg and not op_errors:
             # no, send the REST request
             match method:
+                case "DELETE":
+                    result = requests.delete(url=url,
+                                             headers=op_headers,
+                                             params=params,
+                                             data=data,
+                                             json=json,
+                                             timeout=timeout)
                 case "GET":
                     result = requests.get(url=url,
                                           headers=op_headers,
                                           params=params,
+                                          data=data,
+                                          json=json,
                                           timeout=timeout)
                 case "POST":
                     result = requests.post(url=url,
                                            headers=op_headers,
                                            params=params,
                                            data=data,
                                            json=json,
```

### Comparing `pypomes_http-0.0.9/src/pypomes_http/http_statuses.py` & `pypomes_http-0.1.0/src/pypomes_http/http_statuses.py`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.0.9/LICENSE` & `pypomes_http-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_http-0.0.9/pyproject.toml` & `pypomes_http-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,30 +2,30 @@
 requires = [
     "hatchling>=1.22.2"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_http"
-version = "0.0.9"
+version = "0.1.0"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (HTTP modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=3.0.2",
     "pip>=24.0",
-    "pypomes_core>=0.7.1",
+    "pypomes_core>=0.7.3",
     "pypomes_security>=0.1.3",
     "requests>=2.31.0",
     "setuptools>=68.0.0",
     "wheel>=0.42.0"
 ]
 
 [project.urls]
```

### Comparing `pypomes_http-0.0.9/PKG-INFO` & `pypomes_http-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.3
 Name: pypomes_http
-Version: 0.0.9
+Version: 0.1.0
 Summary: A collection of Python pomes, pennyeach (HTTP modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-HTTP
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-HTTP/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=3.0.2
 Requires-Dist: pip>=24.0
-Requires-Dist: pypomes-core>=0.7.1
+Requires-Dist: pypomes-core>=0.7.3
 Requires-Dist: pypomes-security>=0.1.3
 Requires-Dist: requests>=2.31.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.42.0
```

