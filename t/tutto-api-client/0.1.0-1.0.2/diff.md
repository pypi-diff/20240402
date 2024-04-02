# Comparing `tmp/tutto_api_client-0.1.0.tar.gz` & `tmp/tutto_api_client-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tutto_api_client-0.1.0.tar", max compression
+gzip compressed data, was "tutto_api_client-1.0.2.tar", max compression
```

## Comparing `tutto_api_client-0.1.0.tar` & `tutto_api_client-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1252 2024-03-15 13:23:06.736514 tutto_api_client-0.1.0/README.md
--rw-r--r--   0        0        0      318 2024-03-15 13:23:06.736514 tutto_api_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      290 2024-03-15 13:23:06.736514 tutto_api_client-0.1.0/tutto_api_client/__init__.py
--rw-r--r--   0        0        0     3597 2024-03-15 13:23:06.736514 tutto_api_client-0.1.0/tutto_api_client/core/endpoints_factory.py
--rw-r--r--   0        0        0     2453 2024-03-15 13:23:06.736514 tutto_api_client-0.1.0/tutto_api_client/helpers/http.py
--rw-r--r--   0        0        0    10332 2024-03-15 13:23:06.736514 tutto_api_client-0.1.0/tutto_api_client/main.py
--rw-r--r--   0        0        0     3559 2024-03-15 13:23:06.736514 tutto_api_client-0.1.0/tutto_api_client/models/authorization.py
--rw-r--r--   0        0        0    14644 2024-03-15 13:23:06.736514 tutto_api_client-0.1.0/tutto_api_client/models/endpoints.py
--rw-r--r--   0        0        0     2526 2024-03-15 13:23:06.736514 tutto_api_client-0.1.0/tutto_api_client/models/entities.py
--rw-r--r--   0        0        0     2095 2024-03-15 13:23:06.736514 tutto_api_client-0.1.0/tutto_api_client/utils/filter_clean_utils.py
--rw-r--r--   0        0        0     1783 1970-01-01 00:00:00.000000 tutto_api_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1252 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/README.md
+-rw-r--r--   0        0        0      318 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      290 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/__init__.py
+-rw-r--r--   0        0        0     3597 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/core/endpoints_factory.py
+-rw-r--r--   0        0        0     2295 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/helpers/http.py
+-rw-r--r--   0        0        0    10319 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/main.py
+-rw-r--r--   0        0        0     3553 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/models/authorization.py
+-rw-r--r--   0        0        0    14644 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/models/endpoints.py
+-rw-r--r--   0        0        0     2502 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/models/entities.py
+-rw-r--r--   0        0        0     2113 2024-04-02 21:28:30.310543 tutto_api_client-1.0.2/tutto_api_client/utils/filter_clean_utils.py
+-rw-r--r--   0        0        0     1783 1970-01-01 00:00:00.000000 tutto_api_client-1.0.2/PKG-INFO
```

### Comparing `tutto_api_client-0.1.0/README.md` & `tutto_api_client-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `tutto_api_client-0.1.0/tutto_api_client/core/endpoints_factory.py` & `tutto_api_client-1.0.2/tutto_api_client/core/endpoints_factory.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-0.1.0/tutto_api_client/helpers/http.py` & `tutto_api_client-1.0.2/tutto_api_client/helpers/http.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """Module to handle requests to an API."""
 
 import aiohttp
-
 from urllib.parse import urljoin
 from dataclasses import dataclass, field
 from typing import Any, Literal
 
 
-@dataclass(init=True, frozen=True, slots=True)
+@dataclass(init=True, frozen=True)
 class HTTPRequest:
     """Class to handle requests to an API"""
 
     base_url: str = field(init=True)
 
     async def request(
         self,
@@ -23,59 +22,53 @@
         json: Any = None,
     ) -> dict:
         request_url = urljoin(base=self.base_url, url=endpoint)
         headers = {**headers} if headers else {}
         response = None
 
         async with aiohttp.ClientSession() as session:
-            match method:
-                case "get":
-                    response = await session.get(
-                        url=request_url,
-                        headers=headers,
-                        params=parameters,
-                    )
-
-                case "post":
-                    response = await session.post(
-                        url=request_url,
-                        headers=headers,
-                        params=parameters,
-                        data=data,
-                        json=json,
-                    )
-
-                case "put":
-                    response = await session.put(
-                        url=request_url,
-                        headers=headers,
-                        params=parameters,
-                        data=data,
-                        json=json,
-                    )
-
-                case "patch":
-                    response = await session.patch(
-                        url=request_url,
-                        headers=headers,
-                        params=parameters,
-                        data=data,
-                        json=json,
-                    )
-
-                case "delete":
-                    response = await session.delete(
-                        url=request_url,
-                        headers=headers,
-                        params=parameters,
-                        data=data,
-                        json=json,
-                    )
-
-                case _:
-                    raise ValueError("Invalid HTTP method")
+            if method == "get":
+                response = await session.get(
+                    url=request_url,
+                    headers=headers,
+                    params=parameters,
+                )
+            elif method == "post":
+                response = await session.post(
+                    url=request_url,
+                    headers=headers,
+                    params=parameters,
+                    data=data,
+                    json=json,
+                )
+            elif method == "put":
+                response = await session.put(
+                    url=request_url,
+                    headers=headers,
+                    params=parameters,
+                    data=data,
+                    json=json,
+                )
+            elif method == "patch":
+                response = await session.patch(
+                    url=request_url,
+                    headers=headers,
+                    params=parameters,
+                    data=data,
+                    json=json,
+                )
+            elif method == "delete":
+                response = await session.delete(
+                    url=request_url,
+                    headers=headers,
+                    params=parameters,
+                    data=data,
+                    json=json,
+                )
+            else:
+                raise ValueError("Invalid HTTP method")
 
             # Check response
             response.raise_for_status()
             response_json = await response.json()
 
             return response_json
```

### Comparing `tutto_api_client-0.1.0/tutto_api_client/main.py` & `tutto_api_client-1.0.2/tutto_api_client/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     def __init__(
         self,
         base_url: str,
         authorization: Authorization,
     ) -> None:
         self.__base_url = base_url
         self.__authorization = authorization
-        pass
 
     def get_deductions(
         self,
         reference: str,
         type: str = "",
         start_date: str = "",
         end_date: str = "",
```

### Comparing `tutto_api_client-0.1.0/tutto_api_client/models/authorization.py` & `tutto_api_client-1.0.2/tutto_api_client/models/authorization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """This module handles authorization into Tutto API."""
 
 import asyncio
 
 from typing import Union, Literal, List, Optional
 from dataclasses import dataclass
-from enum import Enum
+from enum import Enum, auto
 
 from tutto_api_client.helpers.http import HTTPRequest
 from tutto_api_client.utils.filter_clean_utils import split_str_to_list
 
 
 class _TOKEN_ORIGIN(Enum):
-    USER = "user"
-    API = "api"
+    USER = auto()
+    API = auto()
 
 
 @dataclass(slots=True, init=True)
 class _Auth:
     status: int
     message: str
     type: str
@@ -57,15 +57,14 @@
         self.__user = user
         self.__user_type = user_type
         self.__password = password
         self.__basic_auth_token = basic_auth_token
         self.__bearer_token = bearer_token
         # Check initialization
         self.__check_init()
-        pass
 
     def __check_init(self) -> None:
         # Errors
         if not self.__basic_auth_token and not self.__bearer_token:
             raise ValueError("Basic auth token or bearer token are required.")
         if not self.__bearer_token and not (self.__user and self.__password):
             raise ValueError("User and password are required to get a bearer token.")
```

### Comparing `tutto_api_client-0.1.0/tutto_api_client/models/endpoints.py` & `tutto_api_client-1.0.2/tutto_api_client/models/endpoints.py`

 * *Files identical despite different names*

### Comparing `tutto_api_client-0.1.0/tutto_api_client/models/entities.py` & `tutto_api_client-1.0.2/tutto_api_client/models/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module to define the entities of Tutto API, a class-like to the body of requests."""
 
 from dataclasses import dataclass, field
 from datetime import date
 
 
 ### Entities ###
-@dataclass(init=True, frozen=True, slots=True)
+@dataclass(init=True, frozen=True)
 class Relative:
     """Class to represent a relative entity.\n
     Args:
         name (str, optional): Relative name.
         code (str, optional): Relative code.
         birthday_date (date, optional): Relative birthday date.
         vat (str, optional): Relative VAT number.
@@ -41,15 +41,15 @@
     sus_card: str = field(default="")
     mother_name: str = field(default="")
     father_name: str = field(default="")
     race: str = field(default="")
     species: str = field(default="")
 
 
-@dataclass(init=True, frozen=True, slots=True)
+@dataclass(init=True, frozen=True)
 class Occurrence:
     """Class to represent an occurrence entity.\n
     Args:
         type (str, optional): Occurrence type.
         start_date (date, optional): Occurrence date.
         end_date (date, optional): Occurrence end date.
         absence_reason_code (str, optional): Absence reason code.
```

### Comparing `tutto_api_client-0.1.0/tutto_api_client/utils/filter_clean_utils.py` & `tutto_api_client-1.0.2/tutto_api_client/utils/filter_clean_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     Args:
         dictionary (dict): The dictionary to convert.
 
     Returns:
         dict: The dictionary with date values converted to ISO 8601 format.
     """
 
+    @staticmethod
     def convert_value(value):
         if isinstance(value, date):
             return value.isoformat()
         elif isinstance(value, dict):
             return convert_dict_dates_to_isoformat(value)
         elif isinstance(value, list):
             return [convert_value(item) for item in value]
```

### Comparing `tutto_api_client-0.1.0/PKG-INFO` & `tutto_api_client-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutto-api-client
-Version: 0.1.0
+Version: 1.0.2
 Summary: 
 Author: rapha-pereira
 Author-email: raphaelpgomes1@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

