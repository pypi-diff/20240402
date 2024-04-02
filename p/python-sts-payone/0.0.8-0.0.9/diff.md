# Comparing `tmp/python_sts_payone-0.0.8.tar.gz` & `tmp/python_sts_payone-0.0.9.tar.gz`

## Comparing `python_sts_payone-0.0.8.tar` & `python_sts_payone-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/src/python_sts_payone/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/src/python_sts_payone/base/__init__.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/src/python_sts_payone/base/request_handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/src/python_sts_payone/redirection_model/__init__.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/src/python_sts_payone/redirection_model/redirect_payment.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/src/python_sts_payone/redirection_model/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/src/python_sts_payone/secure_hash/__init__.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/src/python_sts_payone/secure_hash/secure_hash_generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/tests/test_secure_hash_generator.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/LICENSE
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/README.md
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 python_sts_payone-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/base/__init__.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/base/request_handler.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/base/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/redirection_model/__init__.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/redirection_model/redirect_payment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/secure_hash/__init__.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/secure_hash/secure_hash_generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/supporting/__init__.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/src/python_sts_payone/supporting/inquiry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     5876 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/tests/test_secure_hash_generator.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/LICENSE
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/README.md
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 python_sts_payone-0.0.9/PKG-INFO
```

### Comparing `python_sts_payone-0.0.8/src/python_sts_payone/base/request_handler.py` & `python_sts_payone-0.0.9/src/python_sts_payone/base/request_handler.py`

 * *Files identical despite different names*

### Comparing `python_sts_payone-0.0.8/src/python_sts_payone/redirection_model/redirect_payment.py` & `python_sts_payone-0.0.9/src/python_sts_payone/redirection_model/redirect_payment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from requests.models import Response
 from typing import Tuple, List
 from ..base.request_handler import SmartRouteRequestHandler
-from .utils import REDIRECT_MESSAGE_ID, SR_URL_LIVE, SR_URL_TEST
+from ..base.utils import REDIRECT_MESSAGE_ID, SR_URL_LIVE, SR_URL_TEST
 
 
 def redirect_pay(merchant_id: str, auth_token: str, transaction_id: str, amount: int, currency_iso_code: str,
                        response_back_url: str, generate_token: bool=False, payment_method_token: str=None,
                        payment_description: str=None, live_mode: bool=True, version: float=None, message_id: str=REDIRECT_MESSAGE_ID,
                        allowed_payment_methods: List[str]=None) -> Tuple[str, int]:
     params: dict = {
```

### Comparing `python_sts_payone-0.0.8/src/python_sts_payone/secure_hash/secure_hash_generator.py` & `python_sts_payone-0.0.9/src/python_sts_payone/secure_hash/secure_hash_generator.py`

 * *Files identical despite different names*

### Comparing `python_sts_payone-0.0.8/tests/test_secure_hash_generator.py` & `python_sts_payone-0.0.9/tests/test_secure_hash_generator.py`

 * *Files identical despite different names*

### Comparing `python_sts_payone-0.0.8/LICENSE` & `python_sts_payone-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_sts_payone-0.0.8/README.md` & `python_sts_payone-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `python_sts_payone-0.0.8/pyproject.toml` & `python_sts_payone-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_sts_payone"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Kamruzzaman Tauhid", email="tmakpk@gmail.com" },
 ]
 description = "A package that provides utility functions to send payment requests to STS PayOne and interpret the responses"
 readme = "README.md"
 requires-python = ">=3.5"
 dependencies = [
```

### Comparing `python_sts_payone-0.0.8/PKG-INFO` & `python_sts_payone-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: python_sts_payone
-Version: 0.0.8
+Version: 0.0.9
 Summary: A package that provides utility functions to send payment requests to STS PayOne and interpret the responses
 Project-URL: Homepage, https://github.com/Tauhid-UAP/python-sts-payone
 Author-email: Kamruzzaman Tauhid <tmakpk@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

