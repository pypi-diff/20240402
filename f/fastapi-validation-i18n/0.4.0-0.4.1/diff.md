# Comparing `tmp/fastapi_validation_i18n-0.4.0.tar.gz` & `tmp/fastapi_validation_i18n-0.4.1.tar.gz`

## Comparing `fastapi_validation_i18n-0.4.0.tar` & `fastapi_validation_i18n-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/py.typed
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/.github/workflows/checker.yml
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/example/main.py
--rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/example/locale/en-US/message.json
--rw-r--r--   0        0        0    15165 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/example/locale/ja-JP/message.json
--rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/example/locale/zh-TW/message.json
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/__init__.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/_helpers.py
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/handler.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/middleware.py
--rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/translator.py
--rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/locale/en-US/message.json
--rw-r--r--   0        0        0    15165 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/locale/ja-JP/message.json
--rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/locale/zh-TW/message.json
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/scripts/publish.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/tests/test_messages.py
--rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/tests/locale/en-US/message.json
--rw-r--r--   0        0        0    15165 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/tests/locale/ja-JP/message.json
--rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/tests/locale/zh-TW/message.json
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/LICENSE
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/README.md
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1270 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/py.typed
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/.github/workflows/checker.yml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/example/main.py
+-rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/example/locale/en-US/message.json
+-rw-r--r--   0        0        0    15165 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/example/locale/ja-JP/message.json
+-rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/example/locale/zh-TW/message.json
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/__init__.py
+-rw-r--r--   0        0        0     1377 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/_helpers.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/base.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/handler.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/middleware.py
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/translator.py
+-rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/locales/en-US/message.json
+-rw-r--r--   0        0        0    15166 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/locales/ja-JP/message.json
+-rw-r--r--   0        0        0    11216 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/locales/zh-TW/message.json
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/scripts/publish.py
+-rw-r--r--   0        0        0     4337 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/tests/test_messages.py
+-rw-r--r--   0        0        0    12482 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/tests/locale/en-US/message.json
+-rw-r--r--   0        0        0    15165 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/tests/locale/ja-JP/message.json
+-rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/tests/locale/zh-TW/message.json
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/README.md
+-rw-r--r--   0        0        0     2556 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 fastapi_validation_i18n-0.4.1/PKG-INFO
```

### Comparing `fastapi_validation_i18n-0.4.0/.pre-commit-config.yaml` & `fastapi_validation_i18n-0.4.1/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -21,24 +21,27 @@
         args:
           - -i
           - column_limit = 88
           - based_on_style = "google"
           - split_before_logical_operator = true
           - split_before_arithmetic_operator = true
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.7
+    rev: v0.3.4
     hooks:
       - id: ruff
         args:
           - --fix
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.7.1
+    rev: v1.9.0
     hooks:
       - id: mypy
+        additional_dependencies:
+          - "pydantic>=2"
         args:
+          - --explicit-package-bases
           - --strict-optional
           - --ignore-missing-imports
           - --warn-redundant-casts
           - --warn-unused-ignores
           - --disallow-any-generics
           - --check-untyped-defs
           - --disallow-untyped-defs
```

### Comparing `fastapi_validation_i18n-0.4.0/.github/workflows/checker.yml` & `fastapi_validation_i18n-0.4.1/.github/workflows/checker.yml`

 * *Files identical despite different names*

### Comparing `fastapi_validation_i18n-0.4.0/.github/workflows/publish.yml` & `fastapi_validation_i18n-0.4.1/.github/workflows/publish.yml`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,14 @@
           key: ${{ runner.os }}-python-${{ env.pythonLocation }}-${{ hashFiles('pyproject.toml') }}-publish
       - name: Install build dependencies
         if: steps.cache.outputs.cache-hit != 'true'
         run: pip install build
       - name: Build distribution
         run: python -m build
       - name: Publish
-        uses: pypa/gh-action-pypi-publish@v1.8.6
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           password: ${{ secrets.PYPI_API_TOKEN }}
       - name: Dump GitHub context
         env:
           GITHUB_CONTEXT: ${{ toJson(github) }}
         run: echo "$GITHUB_CONTEXT"
```

### Comparing `fastapi_validation_i18n-0.4.0/example/main.py` & `fastapi_validation_i18n-0.4.1/example/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 from enum import Enum
 from ipaddress import IPv4Address, IPv6Address
 from typing import Annotated, List, Literal, Union
 
 from fastapi import FastAPI
 from fastapi.exceptions import RequestValidationError
 from fastapi.responses import JSONResponse
-from pydantic import BaseModel, Field, field_validator, ValidationError
+from pydantic import BaseModel, Field, ValidationError
+from pydantic.functional_validators import field_validator
 from pydantic.networks import AnyHttpUrl
 from starlette.requests import Request
 
 from fastapi_validation_i18n import i18n_exception_handler, I18nMiddleware, Translator
+from fastapi_validation_i18n.base import setup
 
+# use this separately
 app = FastAPI(debug=True)
 
-app.add_middleware(I18nMiddleware, locale_path='example/locale')
 
-# for request validation error
-app.add_exception_handler(RequestValidationError, i18n_exception_handler)
+def setup_separately(app: FastAPI) -> None:
+    app.add_middleware(I18nMiddleware, locale_path='example/locale')
 
-# for pydantic validation error
-app.add_exception_handler(ValidationError, i18n_exception_handler)
+    # for request validation error
+    app.add_exception_handler(RequestValidationError, i18n_exception_handler)
+
+    # for pydantic validation error
+    app.add_exception_handler(ValidationError, i18n_exception_handler)
+
+
+def setup_with_single_function(app: FastAPI) -> None:
+    setup(app)
+
+
+# setup_separately(app)
+setup_with_single_function(app)
 
 
 class BlackCat(BaseModel):
     pet_type: Literal['cat']
     color: Literal['black']
     black_name: str
 
@@ -40,31 +53,31 @@
 class DeepBody(BaseModel):
     deep_body: str = Field(..., min_length=20)
     url: AnyHttpUrl
     ipv4: IPv4Address
 
     @field_validator('url')
     @classmethod
-    def validate_url(cls, v: AnyHttpUrl):
+    def validate_url(cls, v: AnyHttpUrl) -> str:
         return v.__str__()
 
     @field_validator('ipv4')
     @classmethod
-    def validate_ipv4(cls, v: IPv4Address):
+    def validate_ipv4(cls, v: IPv4Address) -> str:
         return v.__str__()
 
 
 class InnerNestedExample(BaseModel):
     inner_body: List[DeepBody] = Field(..., max_length=2)
     cat: Cat
     ipv6: IPv6Address
 
     @field_validator('ipv6')
     @classmethod
-    def validate_ipv6(cls, v: IPv6Address):
+    def validate_ipv6(cls, v: IPv6Address) -> str:
         return v.__str__()
 
 
 CustomType = Annotated[str | int, Field(..., min_length=2, max_length=5)]
 
 
 class NestedExample(BaseModel):
@@ -82,15 +95,15 @@
     string: str = Field(max_length=10)
     integer: int = Field(default=1)
     nested: NestedExample
     ipt_enum: MyEnum
 
 
 @app.get('/')
-async def root(r: Request):
+async def root(r: Request) -> dict[str, str]:
     return {
         'message':
             Translator('ja-JP',
                        locale_path='example/locale').t('message.field required'),
         'request_locale_message':
             Translator(r.state.locale,
                        locale_path='example/locale').t('message.field required'),
@@ -100,8 +113,8 @@
 @app.post('/')
 async def post_root(payload: Example) -> JSONResponse:
     return JSONResponse(content=payload.model_dump())
 
 
 @app.get('/examples')
 async def get_examples() -> Example:
-    return Example(**{'message': 'this will not show up'})
+    return Example(**{'message': 'this will not show up'})  # type: ignore
```

### Comparing `fastapi_validation_i18n-0.4.0/example/locale/en-US/message.json` & `fastapi_validation_i18n-0.4.1/example/locale/en-US/message.json`

 * *Files identical despite different names*

### Comparing `fastapi_validation_i18n-0.4.0/example/locale/ja-JP/message.json` & `fastapi_validation_i18n-0.4.1/example/locale/ja-JP/message.json`

 * *Files identical despite different names*

### Comparing `fastapi_validation_i18n-0.4.0/example/locale/zh-TW/message.json` & `fastapi_validation_i18n-0.4.1/example/locale/zh-TW/message.json`

 * *Files identical despite different names*

### Comparing `fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/handler.py` & `fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,7 +11,10 @@
         r: Request, e: RequestValidationError | ValidationError) -> JSONResponse:
     t = Translator(r.state.locale, locale_path=r.state.locale_path)
     errors = translate_errors(t, e.errors())
     return JSONResponse(
         {'errors': errors},
         status_code=422,
     )
+
+
+__all__ = ['i18n_exception_handler']
```

### Comparing `fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/middleware.py` & `fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/middleware.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from typing import Sequence
-
 from starlette.middleware.base import BaseHTTPMiddleware, RequestResponseEndpoint
 from starlette.requests import Request
 from starlette.types import ASGIApp
 
 
 class I18nMiddleware(BaseHTTPMiddleware):
 
     def __init__(self,
                  app: ASGIApp,
-                 locale_path: str = 'locale',
-                 locale_list: Sequence[str] = ('zh-TW'),
+                 locale_path: str = 'locales',
+                 locale_list: tuple[str, ...] = (
+                     'zh-TW',
+                     'en-US',
+                     'ja-JP',
+                 ),
                  fallback_locale: str = 'zh-TW'):
         super().__init__(app)
         self.locale_path = locale_path
         self.locale_list = locale_list
         self.fallback_locale = fallback_locale
 
     async def dispatch(  # type: ignore
@@ -26,7 +28,10 @@
         if locale not in self.locale_list:
             locale = self.fallback_locale
 
         request.state.locale = locale
         request.state.locale_path = self.locale_path
 
         return await call_next(request)
+
+
+__all__ = ['I18nMiddleware']
```

### Comparing `fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/translator.py` & `fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/translator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 import json
+import os
 from typing import Any, Dict
 
+from ._helpers import get_package_root
+
 
 class Translator:
     _instances: Dict[str, 'Translator'] = {}
 
     def __new__(cls, locale: str, **args: Any) -> 'Translator':
         if locale not in cls._instances:
             cls._instances[locale] = super().__new__(cls)
         return cls._instances[locale]
 
-    def __init__(self, locale: str, locale_path: str = 'locale'):
+    def __init__(self, locale: str, locale_path: str):
         self.locale = locale
         self.locale_path = locale_path.rstrip('/')
+        self.translations: Dict[str, Any] = {}
 
     def load_translation(self, file_key: str) -> Any | Dict[str, Any] | None:
+        if file_key in self.translations:
+            return self.translations[file_key]
         file_path = f'{self.locale_path}/{self.locale}/{file_key}.json'
+        if not os.path.isfile(file_path):
+            file_path = str(
+                get_package_root().joinpath(f'locales/{self.locale}/{file_key}.json'))
         try:
             with open(file_path, encoding='utf-8') as file:
                 translation = json.load(file)
+            self.translations[file_key] = translation
             return translation
         except FileNotFoundError:
             return None
 
     def t(self, key: str, **kwargs: Any) -> str:
         file_key, *translation_keys = key.split('.')
         translation = self.load_translation(file_key)
@@ -34,7 +44,10 @@
             if translation is None:
                 return f'Key {key} not found in {self.locale} locale'
 
         if kwargs:
             translation = translation.format(**kwargs)  # type: ignore
 
         return translation
+
+
+__all__ = ['Translator']
```

### Comparing `fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/locale/en-US/message.json` & `fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/locales/en-US/message.json`

 * *Files identical despite different names*

### Comparing `fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/locale/ja-JP/message.json` & `fastapi_validation_i18n-0.4.1/tests/locale/ja-JP/message.json`

 * *Files identical despite different names*

### Comparing `fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/locale/zh-TW/message.json` & `fastapi_validation_i18n-0.4.1/tests/locale/zh-TW/message.json`

 * *Files identical despite different names*

### Comparing `fastapi_validation_i18n-0.4.0/fastapi_validation_i18n/scripts/publish.py` & `fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/scripts/publish.py`

 * *Files identical despite different names*

### Comparing `fastapi_validation_i18n-0.4.0/tests/test_messages.py` & `fastapi_validation_i18n-0.4.1/tests/test_messages.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+# type: ignore
 from enum import Enum
 from ipaddress import IPv4Address, IPv6Address
 from pathlib import Path
 from typing import Annotated, List, Literal, Union
 
-import pytest
 from pydantic import BaseModel, field_validator
 from pydantic.fields import Field
 from pydantic.networks import AnyHttpUrl
 from pydantic_core import ValidationError
+import pytest
 
 from fastapi_validation_i18n._helpers import translate_errors
 from fastapi_validation_i18n.translator import Translator
 
 translator = Translator('zh-TW', locale_path=str(Path.cwd()) + '/tests/locale')
 
 
@@ -140,22 +141,22 @@
             "type": "literal_error",
             "loc": ("nested", "inner", "cat", "black", "pet_type"),
             "msg": "輸入應為 'cat'",
             "input": "dog",
             "ctx": {
                 "expected": "'cat'"
             },
-            "url": "https://errors.pydantic.dev/2.5/v/literal_error"
+            "url": "https://errors.pydantic.dev/2.6/v/literal_error"
         },
         {
             "type": "too_long",
             "loc": ("nested", "custom_input"),
             "msg": "Value 在驗證後最多應有 5 個項目,而不是 8",
             "input": "dddddddd",
             "ctx": {
                 "field_type": "Value",
                 "max_length": 5,
                 "actual_length": 8
             },
-            "url": "https://errors.pydantic.dev/2.5/v/too_long"
+            "url": "https://errors.pydantic.dev/2.6/v/too_long"
         }
     ]
```

### Comparing `fastapi_validation_i18n-0.4.0/tests/locale/en-US/message.json` & `fastapi_validation_i18n-0.4.1/tests/locale/en-US/message.json`

 * *Files identical despite different names*

### Comparing `fastapi_validation_i18n-0.4.0/tests/locale/ja-JP/message.json` & `fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/locales/ja-JP/message.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -941,8 +941,8 @@
 00003ac0: 222c 0a20 2022 7661 6c75 6520 6973 206e  ",.  "value is n
 00003ad0: 6f74 2061 2076 616c 6964 2049 5076 3420  ot a valid IPv4 
 00003ae0: 6f72 2049 5076 3620 6e65 7477 6f72 6b22  or IPv6 network"
 00003af0: 3a20 22e5 80a4 e381 afe6 9c89 e58a b9e3  : ".............
 00003b00: 81aa 4950 7634 e381 bee3 819f e381 af49  ..IPv4.........I
 00003b10: 5076 36e3 838d e383 83e3 8388 e383 afe3  Pv6.............
 00003b20: 83bc e382 afe3 81a7 e381 afe3 8182 e382  ................
-00003b30: 8ae3 81be e381 9be3 8293 220a 7d         ..........".}
+00003b30: 8ae3 81be e381 9be3 8293 220a 7d0a       ..........".}.
```

### Comparing `fastapi_validation_i18n-0.4.0/tests/locale/zh-TW/message.json` & `fastapi_validation_i18n-0.4.1/fastapi_validation_i18n/locales/zh-TW/message.json`

 * *Format-specific differences are supported for JSON files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JSON text data*

 * *Files 0% similar despite different names*

```diff
@@ -694,8 +694,8 @@
 00002b50: 8de6 98af e69c 89e6 9588 e79a 8420 4950  ............. IP
 00002b60: 7634 20e6 8896 2049 5076 3620 e68e a5e5  v4 ... IPv6 ....
 00002b70: 8fa3 222c 0a20 2022 7661 6c75 6520 6973  ..",.  "value is
 00002b80: 206e 6f74 2061 2076 616c 6964 2049 5076   not a valid IPv
 00002b90: 3420 6f72 2049 5076 3620 6e65 7477 6f72  4 or IPv6 networ
 00002ba0: 6b22 3a20 22e5 80bc e4b8 8de6 98af e69c  k": "...........
 00002bb0: 89e6 9588 e79a 8420 4950 7634 20e6 8896  ....... IPv4 ...
-00002bc0: 2049 5076 3620 e7b6 b2e7 b5a1 220a 7d     IPv6 ......".}
+00002bc0: 2049 5076 3620 e7b6 b2e7 b5a1 220a 7d0a   IPv6 ......".}.
```

### Comparing `fastapi_validation_i18n-0.4.0/LICENSE` & `fastapi_validation_i18n-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_validation_i18n-0.4.0/README.md` & `fastapi_validation_i18n-0.4.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -54,39 +54,48 @@
         "allowed_values": "'black', 'white'"
       }
     }
   ]
 }
 ```
 ## Attention
-- support pydantic v1 only now(2023/08/16)
+- For FastAPI >=0.100.0 and pydantic v2, please use **^0.4.0**
+- For FastAPI < 0.100.0 nad pydantic v1, please use **^0.3.0**
 - built-in locales are **zh-TW, en-US, ja-JP**, you can change the locales by yourself
 
 ## How to run
 1. publish locales to your app path
 ```bash
 # default to "locale" in your project path
 poetry run publish-locale <your-path> [--locale]
 ```
-1. add middleware and exception handler to your FastAPI app
+### Setup in FastAPI
+- use `setup`
+```py
+from fastapi_validation_i18n import setup
+from fastapi import FastAPI
+app = FastAPI()
+setup(app, locale_path=..., locale_list=...)
+
+```
+- use middleware and exception handler
 ```py
 from fastapi import FastAPI
 from fastapi_validation_i18n import I18nMiddleware, i18n_exception_handler
 from fastapi.exceptions import RequestValidationError
 
 app = FastAPI()
 
 app.add_middleware(I18nMiddleware, locale_path='your-publish-path')
 
 app.add_exception_handler(
     RequestValidationError,
     i18n_exception_handler
 )
 ```
-3. start use it
 
 there's 3 way to set locale
 
 1. set `accept-language` header to your request
 2. set an API with `locale` in path
 3. set `locale` query parameter to your request
```

### Comparing `fastapi_validation_i18n-0.4.0/pyproject.toml` & `fastapi_validation_i18n-0.4.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -40,23 +40,23 @@
 
 [tool.poetry.dependencies]
 python = "^3.8"
 fastapi = ">0.99"
 pydantic = "^2"
 typer = {extras = ["all"], version = "^0.9.0"}
 
-
 [tool.poetry.group.dev.dependencies]
-ruff = "^0.1"
-yapf = "^0.40.1"
-uvicorn = "^0.23.2"
-mypy = "^1.5.0"
-pytest = "^7.4.0"
+ruff = "^0.3.4"
+yapf = "^0.40.2"
+uvicorn = "^0.29.0"
+mypy = "^1.9.0"
+pytest = "^8.1.1"
 pre-commit = "^3.5.0"
-pydantic-core = "^2.14.5"
+pydantic-core = "^2.16.0"
+
 
 [tool.mypy]
 strict_optional = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 disallow_any_generics = true
 check_untyped_defs = true
@@ -65,23 +65,23 @@
 column_limit = 88
 based_on_style = "google"
 split_before_logical_operator = true
 split_before_arithmetic_operator = true # flake8 W504
 
 [tool.ruff]
 line-length = 88
-select = [
+lint.select = [
     "E", # pycodestyle errors
     "W", # pycodestyle warnings
     "F", # pyflakes
     "I", # isort
     "C", # flake8-comprehensions
     "B", # flake8-bugbear
 ]
-ignore = [
+lint.ignore = [
     "E501",
     "B008",
     "E402",
     "E226",
     "B904",
     "B030",
     "B006"
@@ -89,23 +89,23 @@
 extend-exclude = [
     ".venv",
     ".git",
     "__pycache__",
     "__init__.py",
     "frontend",
 ]
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-single-line = false
 force-sort-within-sections = true
 known-third-party = ["fastapi", "pydantic", "starlette"]
 single-line-exclusions = ["typing"]
 order-by-type = false
-[tool.ruff.mccabe]
+[tool.ruff.lint.mccabe]
 max-complexity = 10
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 inline-quotes = "single"
 
 [tool.pytest.ini_options]
 addopts = """
   -ra
   -q
   --strict-markers
@@ -117,7 +117,11 @@
 
 log_format = "%(asctime)s (%(filename)-16s:%(lineno)-3s) %(levelname)-8s %(message)s"
 log_date_format = "%Y-%M-%D %H:%M:%S"
 
 
 [tool.poetry.scripts]
 publish-locale = 'fastapi_validation_i18n.scripts.publish:main'
+
+[virtualenv]
+create = true
+in-project = true
```

### Comparing `fastapi_validation_i18n-0.4.0/PKG-INFO` & `fastapi_validation_i18n-0.4.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: fastapi_validation_i18n
-Version: 0.4.0
+Version: 0.4.1
 Summary: FastAPI request validation with i18n error message
 Project-URL: Repository, https://github.com/whchi/fastapi-validation-i18n
 Author-email: whchi <whccchi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: fastapi,i18n,pydantic,validation
 Requires-Python: >=3.8
@@ -68,39 +68,48 @@
         "allowed_values": "'black', 'white'"
       }
     }
   ]
 }
 ```
 ## Attention
-- support pydantic v1 only now(2023/08/16)
+- For FastAPI >=0.100.0 and pydantic v2, please use **^0.4.0**
+- For FastAPI < 0.100.0 nad pydantic v1, please use **^0.3.0**
 - built-in locales are **zh-TW, en-US, ja-JP**, you can change the locales by yourself
 
 ## How to run
 1. publish locales to your app path
 ```bash
 # default to "locale" in your project path
 poetry run publish-locale <your-path> [--locale]
 ```
-1. add middleware and exception handler to your FastAPI app
+### Setup in FastAPI
+- use `setup`
+```py
+from fastapi_validation_i18n import setup
+from fastapi import FastAPI
+app = FastAPI()
+setup(app, locale_path=..., locale_list=...)
+
+```
+- use middleware and exception handler
 ```py
 from fastapi import FastAPI
 from fastapi_validation_i18n import I18nMiddleware, i18n_exception_handler
 from fastapi.exceptions import RequestValidationError
 
 app = FastAPI()
 
 app.add_middleware(I18nMiddleware, locale_path='your-publish-path')
 
 app.add_exception_handler(
     RequestValidationError,
     i18n_exception_handler
 )
 ```
-3. start use it
 
 there's 3 way to set locale
 
 1. set `accept-language` header to your request
 2. set an API with `locale` in path
 3. set `locale` query parameter to your request
```

