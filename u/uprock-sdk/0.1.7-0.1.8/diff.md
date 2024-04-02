# Comparing `tmp/uprock_sdk-0.1.7.tar.gz` & `tmp/uprock_sdk-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uprock_sdk-0.1.7.tar", max compression
+gzip compressed data, was "uprock_sdk-0.1.8.tar", max compression
```

## Comparing `uprock_sdk-0.1.7.tar` & `uprock_sdk-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       12 2024-03-22 08:27:02.972500 uprock_sdk-0.1.7/README.md
--rw-r--r--   0        0        0      468 2024-03-22 08:27:02.973500 uprock_sdk-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      337 2024-03-22 08:27:02.973500 uprock_sdk-0.1.7/uprock_sdk/__init__.py
--rw-r--r--   0        0        0     2872 2024-03-22 08:27:02.973500 uprock_sdk-0.1.7/uprock_sdk/customers.py
--rw-r--r--   0        0        0      566 2024-03-22 08:27:02.973500 uprock_sdk-0.1.7/uprock_sdk/settings.py
--rw-r--r--   0        0        0     2931 2024-03-22 08:27:02.973500 uprock_sdk-0.1.7/uprock_sdk/terms.py
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 uprock_sdk-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       12 2024-04-02 10:27:21.425401 uprock_sdk-0.1.8/README.md
+-rw-r--r--   0        0        0      468 2024-04-02 10:27:21.425401 uprock_sdk-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      337 2024-04-02 10:27:21.425401 uprock_sdk-0.1.8/uprock_sdk/__init__.py
+-rw-r--r--   0        0        0     3176 2024-04-02 10:27:21.425401 uprock_sdk-0.1.8/uprock_sdk/customers.py
+-rw-r--r--   0        0        0      566 2024-04-02 10:27:21.426401 uprock_sdk-0.1.8/uprock_sdk/settings.py
+-rw-r--r--   0        0        0     2931 2024-04-02 10:27:21.426401 uprock_sdk-0.1.8/uprock_sdk/terms.py
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 uprock_sdk-0.1.8/PKG-INFO
```

### Comparing `uprock_sdk-0.1.7/uprock_sdk/customers.py` & `uprock_sdk-0.1.8/uprock_sdk/customers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,45 @@
 import datetime
 import enum
 from typing import Optional, Set, List
 
 import httpx
-from pydantic import BaseModel, EmailStr, model_validator, Field
+from pydantic import BaseModel, EmailStr, model_validator, Field, field_validator
 
 from uprock_sdk import GLOBAL_SETTINGS
 
 CLIENT = httpx.AsyncClient(base_url=GLOBAL_SETTINGS.CORE_API_URL)
 
 
 class BaseCustomer(BaseModel):
     telegram_id: Optional[int] = None
     email: Optional[EmailStr] = None
     email_verified: Optional[bool] = None
     first_name: Optional[str] = None
     last_name: Optional[str] = None
     username: Optional[str] = None
+    created_at: Optional[datetime.datetime] = None
 
     labels: Optional[List["BaseLabel"]] = None
     namespaces: Optional[Set[int]] = None
 
     @model_validator(mode="after")
     def telegram_id_or_email_required(self):
         if not self.telegram_id and not self.email:
             raise ValueError("Either telegram_id or email is required")
         return self
 
+    @field_validator("created_at")
+    @classmethod
+    def dt_is_not_native(cls, v: datetime.datetime) -> datetime.datetime:
+        if v and v.tzinfo is None:
+            v = v.replace(tzinfo=datetime.timezone.utc)
+
+        return v
+
 
 class CustomerRead(BaseCustomer):
     id: int
 
     updated_at: datetime.datetime
     created_at: datetime.datetime
```

### Comparing `uprock_sdk-0.1.7/uprock_sdk/settings.py` & `uprock_sdk-0.1.8/uprock_sdk/settings.py`

 * *Files identical despite different names*

### Comparing `uprock_sdk-0.1.7/uprock_sdk/terms.py` & `uprock_sdk-0.1.8/uprock_sdk/terms.py`

 * *Files identical despite different names*

### Comparing `uprock_sdk-0.1.7/PKG-INFO` & `uprock_sdk-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uprock-sdk
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: Aleksey Dalekin
 Author-email: adalekin@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

