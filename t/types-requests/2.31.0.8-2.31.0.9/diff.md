# Comparing `tmp/types-requests-2.31.0.8.tar.gz` & `tmp/types-requests-2.31.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-requests-2.31.0.8.tar", last modified: Thu Oct  5 12:30:19 2023, max compression
+gzip compressed data, was "types-requests-2.31.0.9.tar", last modified: Fri Oct 13 18:19:28 2023, max compression
```

## Comparing `types-requests-2.31.0.8.tar` & `types-requests-2.31.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:30:19.344913 types-requests-2.31.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    12980 2023-10-05 12:30:17.000000 types-requests-2.31.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-05 12:30:17.000000 types-requests-2.31.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-10-05 12:30:19.344913 types-requests-2.31.0.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:30:19.344913 types-requests-2.31.0.8/requests-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2023-10-05 12:30:17.000000 types-requests-2.31.0.8/requests-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      169 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/__version__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2868 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/adapters.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4861 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/certs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/compat.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/cookies.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/help.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/hooks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/models.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/packages.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11829 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/sessions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/status_codes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/structures.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-10-05 12:30:05.000000 types-requests-2.31.0.8/requests-stubs/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-05 12:30:19.344913 types-requests-2.31.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2023-10-05 12:30:17.000000 types-requests-2.31.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-05 12:30:19.344913 types-requests-2.31.0.8/types_requests.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2023-10-05 12:30:19.000000 types-requests-2.31.0.8/types_requests.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-10-05 12:30:19.000000 types-requests-2.31.0.8/types_requests.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-05 12:30:19.000000 types-requests-2.31.0.8/types_requests.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-05 12:30:19.000000 types-requests-2.31.0.8/types_requests.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-05 12:30:19.000000 types-requests-2.31.0.8/types_requests.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 18:19:28.737563 types-requests-2.31.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    13218 2023-10-13 18:19:26.000000 types-requests-2.31.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2023-10-13 18:19:26.000000 types-requests-2.31.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-10-13 18:19:28.737563 types-requests-2.31.0.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 18:19:28.737563 types-requests-2.31.0.9/requests-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2023-10-13 18:19:26.000000 types-requests-2.31.0.9/requests-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/__version__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/adapters.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4861 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/certs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/compat.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/cookies.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/help.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/hooks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/models.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/packages.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11829 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/sessions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/status_codes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/structures.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-10-13 18:19:08.000000 types-requests-2.31.0.9/requests-stubs/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-13 18:19:28.737563 types-requests-2.31.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2429 2023-10-13 18:19:26.000000 types-requests-2.31.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-13 18:19:28.737563 types-requests-2.31.0.9/types_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-10-13 18:19:28.000000 types-requests-2.31.0.9/types_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2023-10-13 18:19:28.000000 types-requests-2.31.0.9/types_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-13 18:19:28.000000 types-requests-2.31.0.9/types_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2023-10-13 18:19:28.000000 types-requests-2.31.0.9/types_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2023-10-13 18:19:28.000000 types-requests-2.31.0.9/types_requests.egg-info/top_level.txt
```

### Comparing `types-requests-2.31.0.8/CHANGELOG.md` & `types-requests-2.31.0.9/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 2.31.0.9 (2023-10-13)
+
+[requests] Allow HTTPError.response to be None (#10875)
+
+This aligns with the definition in requests, but means that user code might
+need additional assertions to ensure that `HTTPError.response` is not `None`.
+
 ## 2.31.0.8 (2023-10-05)
 
 `types-requests`, `types-influxdb-client`: add note to the PyPI readme about the `urllib3` pin (#10839)
 
 ## 2.31.0.7 (2023-10-01)
 
 Remove stubs for `urllib3` (#10812)
```

### Comparing `types-requests-2.31.0.8/PKG-INFO` & `types-requests-2.31.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-requests
-Version: 2.31.0.8
+Version: 2.31.0.9
 Summary: Typing stubs for requests
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -12,23 +12,28 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Typing stubs for requests
 
-This is a PEP 561 type stub package for the `requests` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`requests`](https://github.com/psf/requests) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`requests`. The source for this package can be found at
+`requests`.
+
+This version of `types-requests` aims to provide accurate annotations
+for `requests==2.31.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `011f24794d334ecbd6bda104a8e57399bd6bcad8` and was tested
-with mypy 1.5.1, pyright 1.1.328, and
-pytype 2023.8.31.
+This package was generated from typeshed commit `e92bfcbab2d15c407acc6ebaeceda5688e65e280` and was tested
+with mypy 1.5.1, pyright 1.1.330, and
+pytype 2023.10.5.
```

### Comparing `types-requests-2.31.0.8/requests-stubs/__init__.pyi` & `types-requests-2.31.0.9/requests-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.8/requests-stubs/adapters.pyi` & `types-requests-2.31.0.9/requests-stubs/adapters.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.8/requests-stubs/api.pyi` & `types-requests-2.31.0.9/requests-stubs/api.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.8/requests-stubs/auth.pyi` & `types-requests-2.31.0.9/requests-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.8/requests-stubs/compat.pyi` & `types-requests-2.31.0.9/requests-stubs/compat.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.8/requests-stubs/cookies.pyi` & `types-requests-2.31.0.9/requests-stubs/cookies.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.8/requests-stubs/exceptions.pyi` & `types-requests-2.31.0.9/requests-stubs/exceptions.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -8,20 +8,15 @@
     request: Request | PreparedRequest | None
     def __init__(
         self, *args: object, request: Request | PreparedRequest | None = ..., response: Response | None = ...
     ) -> None: ...
 
 class InvalidJSONError(RequestException): ...
 class JSONDecodeError(InvalidJSONError): ...
-
-class HTTPError(RequestException):
-    request: Request | PreparedRequest | None
-    response: Response
-    def __init__(self, *args: object, request: Request | PreparedRequest | None = ..., response: Response) -> None: ...
-
+class HTTPError(RequestException): ...
 class ConnectionError(RequestException): ...
 class ProxyError(ConnectionError): ...
 class SSLError(ConnectionError): ...
 class Timeout(RequestException): ...
 class ConnectTimeout(ConnectionError, Timeout): ...
 class ReadTimeout(Timeout): ...
 class URLRequired(RequestException): ...
```

### Comparing `types-requests-2.31.0.8/requests-stubs/help.pyi` & `types-requests-2.31.0.9/requests-stubs/help.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.8/requests-stubs/models.pyi` & `types-requests-2.31.0.9/requests-stubs/models.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.8/requests-stubs/sessions.pyi` & `types-requests-2.31.0.9/requests-stubs/sessions.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.8/requests-stubs/structures.pyi` & `types-requests-2.31.0.9/requests-stubs/structures.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.8/requests-stubs/utils.pyi` & `types-requests-2.31.0.9/requests-stubs/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-requests-2.31.0.8/setup.py` & `types-requests-2.31.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from setuptools import setup
 
 name = "types-requests"
 description = "Typing stubs for requests"
 long_description = '''
 ## Typing stubs for requests
 
-This is a PEP 561 type stub package for the `requests` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`requests`](https://github.com/psf/requests) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`requests`. The source for this package can be found at
+`requests`.
+
+This version of `types-requests` aims to provide accurate annotations
+for `requests==2.31.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `011f24794d334ecbd6bda104a8e57399bd6bcad8` and was tested
-with mypy 1.5.1, pyright 1.1.328, and
-pytype 2023.8.31.
+This package was generated from typeshed commit `e92bfcbab2d15c407acc6ebaeceda5688e65e280` and was tested
+with mypy 1.5.1, pyright 1.1.330, and
+pytype 2023.10.5.
 '''.lstrip()
 
 setup(name=name,
-      version="2.31.0.8",
+      version="2.31.0.9",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md",
```

### Comparing `types-requests-2.31.0.8/types_requests.egg-info/PKG-INFO` & `types-requests-2.31.0.9/types_requests.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-requests
-Version: 2.31.0.8
+Version: 2.31.0.9
 Summary: Typing stubs for requests
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/requests.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -12,23 +12,28 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Typing stubs for requests
 
-This is a PEP 561 type stub package for the `requests` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`requests`](https://github.com/psf/requests) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`requests`. The source for this package can be found at
+`requests`.
+
+This version of `types-requests` aims to provide accurate annotations
+for `requests==2.31.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/requests. All fixes for
 types and metadata should be contributed there.
 
 Note: `types-requests` has required `urllib3>=2` since v2.31.0.7. If you need to install `types-requests` into an environment that must also have `urllib3<2` installed into it, you will have to use `types-requests<2.31.0.7`.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `011f24794d334ecbd6bda104a8e57399bd6bcad8` and was tested
-with mypy 1.5.1, pyright 1.1.328, and
-pytype 2023.8.31.
+This package was generated from typeshed commit `e92bfcbab2d15c407acc6ebaeceda5688e65e280` and was tested
+with mypy 1.5.1, pyright 1.1.330, and
+pytype 2023.10.5.
```

### Comparing `types-requests-2.31.0.8/types_requests.egg-info/SOURCES.txt` & `types-requests-2.31.0.9/types_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

