# Comparing `tmp/netdata-1.1.0.tar.gz` & `tmp/netdata-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netdata-1.1.0.tar", max compression
+gzip compressed data, was "netdata-1.2.0.tar", max compression
```

## Comparing `netdata-1.1.0.tar` & `netdata-1.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1110 2023-05-31 22:55:56.813574 netdata-1.1.0/LICENSE
--rw-r--r--   0        0        0     1116 2022-01-04 08:24:16.663550 netdata-1.1.0/README.rst
--rw-r--r--   0        0        0     2958 2023-05-31 22:55:56.814574 netdata-1.1.0/netdata/__init__.py
--rw-r--r--   0        0        0      248 2020-08-15 11:47:01.963105 netdata-1.1.0/netdata/exceptions.py
--rw-r--r--   0        0        0     1126 2023-05-31 23:12:49.817386 netdata-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     2364 1970-01-01 00:00:00.000000 netdata-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1110 2024-01-01 21:59:10.147009 netdata-1.2.0/LICENSE
+-rw-r--r--   0        0        0     1116 2022-01-04 08:24:16.663550 netdata-1.2.0/README.rst
+-rw-r--r--   0        0        0     3017 2023-11-17 12:09:06.284059 netdata-1.2.0/netdata/__init__.py
+-rw-r--r--   0        0        0      248 2020-08-15 11:47:01.963105 netdata-1.2.0/netdata/exceptions.py
+-rw-r--r--   0        0        0     1122 2024-04-02 21:45:16.990113 netdata-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2215 1970-01-01 00:00:00.000000 netdata-1.2.0/PKG-INFO
```

### Comparing `netdata-1.1.0/LICENSE` & `netdata-1.2.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2023 Fabian Affolter <fabian@affolter-engineering.ch>
+Copyright (c) 2018-2024 Fabian Affolter <fabian@affolter-engineering.ch>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `netdata-1.1.0/README.rst` & `netdata-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `netdata-1.1.0/netdata/__init__.py` & `netdata-1.2.0/netdata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,17 @@
             )
 
     async def get_data(self, url) -> Dict:
         """Execute a request to a data endpoint."""
         try:
             async with httpx.AsyncClient() as client:
                 response = await client.get(str(url), timeout = self.timeout)
-        except httpx.ConnectError:
+        except httpx.TimeoutException:
+            raise
+        except httpx.TransportError:
             raise exceptions.NetdataConnectionError(
                 f"Connection to {self.scheme}://{self.host}:{self.port} failed"
             )
 
         if response.status_code == httpx.codes.OK:
             _LOGGER.debug(response.json())
             try:
```

### Comparing `netdata-1.1.0/pyproject.toml` & `netdata-1.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netdata"
-version = "1.1.0"
+version = "1.2.0"
 description = "Python API for interacting with Netdata"
 authors = ["Fabian Affolter <mail@fabian-affolter.ch>"]
 license = "MIT"
 homepage = "https://github.com/home-assistant-ecosystem/python-netdata"
 repository = "https://github.com/home-assistant-ecosystem/python-netdata"
 readme = "README.rst"
 classifiers = [
@@ -24,15 +24,15 @@
 
 [tool.poetry.dependencies]
 python = "^3.9"
 httpx = ">=0.23,<1"
 yarl = "^1.8.0"
 
 [tool.poetry.dev-dependencies]
-black = "^23.3.0"
-pytest = "^6.2.5"
+black = "^24.3.0"
+pytest = "^8"
 pytest-httpx = ">0.15,<1"
 pytest-asyncio = "^0.15.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `netdata-1.1.0/PKG-INFO` & `netdata-1.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netdata
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python API for interacting with Netdata
 Home-page: https://github.com/home-assistant-ecosystem/python-netdata
 License: MIT
 Author: Fabian Affolter
 Author-email: mail@fabian-affolter.ch
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,18 +14,15 @@
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Utilities
 Requires-Dist: httpx (>=0.23,<1)
 Requires-Dist: yarl (>=1.8.0,<2.0.0)
 Project-URL: Repository, https://github.com/home-assistant-ecosystem/python-netdata
 Description-Content-Type: text/x-rst
```

