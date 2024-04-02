# Comparing `tmp/ticketsdk-2.2.1.tar.gz` & `tmp/ticketsdk-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ticketsdk-2.2.1.tar", last modified: Fri Mar 29 01:08:58 2024, max compression
+gzip compressed data, was "ticketsdk-2.2.2.tar", last modified: Tue Apr  2 03:16:59 2024, max compression
```

## Comparing `ticketsdk-2.2.1.tar` & `ticketsdk-2.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-03-29 01:08:58.996895 ticketsdk-2.2.1/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-03-29 01:08:58.996715 ticketsdk-2.2.1/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)     1722 2024-03-29 01:05:58.000000 ticketsdk-2.2.1/README.md
--rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-03-29 01:08:58.996945 ticketsdk-2.2.1/setup.cfg
--rw-r--r--   0 phamchuong   (501) staff       (20)      873 2024-03-29 01:04:05.000000 ticketsdk-2.2.1/setup.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-03-29 01:08:58.995617 ticketsdk-2.2.1/ticketsdk/
--rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-03-29 01:08:44.000000 ticketsdk-2.2.1/ticketsdk/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.2.1/ticketsdk/client.py
--rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.2.1/ticketsdk/constants.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-03-29 01:08:58.996306 ticketsdk-2.2.1/ticketsdk/seller/
--rw-r--r--   0 phamchuong   (501) staff       (20)     1277 2024-03-28 02:40:55.000000 ticketsdk-2.2.1/ticketsdk/seller/__init__.py
--rw-r--r--   0 phamchuong   (501) staff       (20)     1314 2024-03-29 01:05:58.000000 ticketsdk-2.2.1/ticketsdk/validators.py
-drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-03-29 01:08:58.996481 ticketsdk-2.2.1/ticketsdk.egg-info/
--rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-03-29 01:08:58.000000 ticketsdk-2.2.1/ticketsdk.egg-info/PKG-INFO
--rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-03-29 01:08:58.000000 ticketsdk-2.2.1/ticketsdk.egg-info/SOURCES.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-03-29 01:08:58.000000 ticketsdk-2.2.1/ticketsdk.egg-info/dependency_links.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-03-29 01:08:58.000000 ticketsdk-2.2.1/ticketsdk.egg-info/requires.txt
--rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-03-29 01:08:58.000000 ticketsdk-2.2.1/ticketsdk.egg-info/top_level.txt
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-02 03:16:59.940857 ticketsdk-2.2.2/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-02 03:16:59.940661 ticketsdk-2.2.2/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1077 2024-04-02 03:15:39.000000 ticketsdk-2.2.2/README.md
+-rw-r--r--   0 phamchuong   (501) staff       (20)       38 2024-04-02 03:16:59.940898 ticketsdk-2.2.2/setup.cfg
+-rw-r--r--   0 phamchuong   (501) staff       (20)      873 2024-03-29 01:04:05.000000 ticketsdk-2.2.2/setup.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-02 03:16:59.939192 ticketsdk-2.2.2/ticketsdk/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      516 2024-04-02 03:10:03.000000 ticketsdk-2.2.2/ticketsdk/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     3995 2024-03-27 09:22:59.000000 ticketsdk-2.2.2/ticketsdk/client.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)      354 2024-03-27 10:12:08.000000 ticketsdk-2.2.2/ticketsdk/constants.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-02 03:16:59.939935 ticketsdk-2.2.2/ticketsdk/seller/
+-rw-r--r--   0 phamchuong   (501) staff       (20)     2180 2024-04-02 03:09:09.000000 ticketsdk-2.2.2/ticketsdk/seller/__init__.py
+-rw-r--r--   0 phamchuong   (501) staff       (20)     1973 2024-04-02 03:09:09.000000 ticketsdk-2.2.2/ticketsdk/validators.py
+drwxr-xr-x   0 phamchuong   (501) staff       (20)        0 2024-04-02 03:16:59.940465 ticketsdk-2.2.2/ticketsdk.egg-info/
+-rw-r--r--   0 phamchuong   (501) staff       (20)      503 2024-04-02 03:16:59.000000 ticketsdk-2.2.2/ticketsdk.egg-info/PKG-INFO
+-rw-r--r--   0 phamchuong   (501) staff       (20)      300 2024-04-02 03:16:59.000000 ticketsdk-2.2.2/ticketsdk.egg-info/SOURCES.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       33 2024-04-02 03:16:59.000000 ticketsdk-2.2.2/ticketsdk.egg-info/dependency_links.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       55 2024-04-02 03:16:59.000000 ticketsdk-2.2.2/ticketsdk.egg-info/requires.txt
+-rw-r--r--   0 phamchuong   (501) staff       (20)       10 2024-04-02 03:16:59.000000 ticketsdk-2.2.2/ticketsdk.egg-info/top_level.txt
```

### Comparing `ticketsdk-2.2.1/setup.py` & `ticketsdk-2.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.1/ticketsdk/__init__.py` & `ticketsdk-2.2.2/ticketsdk/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import platform
 import logging
 
-__version__ = "2.2.1"
+__version__ = "2.2.2"
 Version = __version__
 
 try:
     from logging import NullHandler
 except ImportError:
 
     class NullHandler(logging.Handler):
```

### Comparing `ticketsdk-2.2.1/ticketsdk/client.py` & `ticketsdk-2.2.2/ticketsdk/client.py`

 * *Files identical despite different names*

### Comparing `ticketsdk-2.2.1/ticketsdk/seller/__init__.py` & `ticketsdk-2.2.2/ticketsdk/seller/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from marshmallow import ValidationError
 
 from ticketsdk.constants import LAMBDA_URI, LAMBDA_ENDPOINT_FOR_TICKET, LAMBDA_AUTHEN
 from ticketsdk.client import ServiceHttpClient
-from ticketsdk.validators import NewTicketSchema, NewSellerSchema
+from ticketsdk.validators import (
+    NewTicketSchema,
+    NewSellerSchema,
+    ListTicketSchema,
+    DetailTicketSchema,
+)
 
 headers = {
     "Authorization": LAMBDA_AUTHEN,
     "Content-Type": "application/json",
 }
 
 
@@ -33,9 +38,35 @@
         except ValidationError as err:
             raise ValueError(err.messages)
         response = ServiceHttpClient(LAMBDA_URI).execute(
             method="post",
             uri=LAMBDA_ENDPOINT_FOR_TICKET,
             body=self.body,
             headers=headers,
+        )
+        return response.get("response").get("result")
+
+    def list_ticket(self):
+        try:
+            ListTicketSchema().load(self.body)
+        except ValidationError as err:
+            raise ValueError(err.messages)
+        response = ServiceHttpClient(LAMBDA_URI).execute(
+            method="post",
+            uri=LAMBDA_ENDPOINT_FOR_TICKET,
+            body=self.body,
+            headers=headers,
+        )
+        return response.get("response").get("result")
+
+    def detail_ticket(self):
+        try:
+            DetailTicketSchema().load(self.body)
+        except ValidationError as err:
+            raise ValueError(err.messages)
+        response = ServiceHttpClient(LAMBDA_URI).execute(
+            method="post",
+            uri=LAMBDA_ENDPOINT_FOR_TICKET,
+            body=self.body,
+            headers=headers,
         )
         return response.get("response").get("result")
```

### Comparing `ticketsdk-2.2.1/ticketsdk/validators.py` & `ticketsdk-2.2.2/ticketsdk/validators.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,24 @@
 
 
 def validate_from_system(val):
     if val not in list_from_system:
         raise ValidationError(f"from_system in : {list_from_system}")
 
 
+def validate_type_list(val):
+    if val not in ["list"]:
+        raise ValidationError(f"lambda_type not exists")
+
+
+def validate_type_detail(val):
+    if val not in ["detail"]:
+        raise ValidationError(f"lambda_type not exists")
+
+
 class NewTicketSchema(Schema):
     issue_code = fields.Str(required=True, validate=validate_issue_code)
     from_system = fields.Str(required=True, validate=validate_from_system)
     ref_code = fields.Str(required=True)
     partner_code = fields.Str(required=True)
     ticket_name = fields.Str(required=True)
     requested_email = fields.Str(required=True)
@@ -36,7 +46,25 @@
     email = fields.Str(required=True)
     cs_email = fields.Str(required=True)
     lambda_type = fields.Str(required=True)
 
     class Meta:
         strict = True
         unknown = RAISE
+
+
+class ListTicketSchema(Schema):
+    lambda_type = fields.Str(required=True, validate=validate_type_list)
+    page = fields.Int(required=True)
+
+    class Meta:
+        strict = True
+        unknown = RAISE
+
+
+class DetailTicketSchema(Schema):
+    lambda_type = fields.Str(required=True, validate=validate_type_detail)
+    ticket_id = fields.Int(required=True)
+
+    class Meta:
+        strict = True
+        unknown = RAISE
```

