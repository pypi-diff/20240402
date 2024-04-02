# Comparing `tmp/iec_api-0.2.7.tar.gz` & `tmp/iec_api-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iec_api-0.2.7.tar", max compression
+gzip compressed data, was "iec_api-0.2.8.tar", max compression
```

## Comparing `iec_api-0.2.7.tar` & `iec_api-0.2.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1071 2024-03-04 11:57:06.505138 iec_api-0.2.7/LICENSE
--rw-r--r--   0        0        0      599 2024-03-04 11:57:06.505138 iec_api-0.2.7/README.md
--rw-r--r--   0        0        0        0 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/__init__.py
--rw-r--r--   0        0        0     6580 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/commons.py
--rw-r--r--   0        0        0     2024 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/const.py
--rw-r--r--   0        0        0     7729 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/data.py
--rw-r--r--   0        0        0    15414 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/iec_client.py
--rw-r--r--   0        0        0     8500 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/login.py
--rw-r--r--   0        0        0     1287 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/account.py
--rw-r--r--   0        0        0     2724 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/contract.py
--rw-r--r--   0        0        0     2157 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/customer.py
--rw-r--r--   0        0        0     2941 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/device.py
--rw-r--r--   0        0        0     1994 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/device_type.py
--rw-r--r--   0        0        0     1768 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/electric_bill.py
--rw-r--r--   0        0        0      639 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/exceptions.py
--rw-r--r--   0        0        0     4123 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/invoice.py
--rw-r--r--   0        0        0      265 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/jwt.py
--rw-r--r--   0        0        0     2532 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/meter_reading.py
--rw-r--r--   0        0        0      658 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/okta_errors.py
--rw-r--r--   0        0        0     3600 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/remote_reading.py
--rw-r--r--   0        0        0      971 2024-03-04 11:57:06.505138 iec_api-0.2.7/iec_api/models/response_descriptor.py
--rw-r--r--   0        0        0     1068 2024-03-04 11:57:06.505138 iec_api-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 iec_api-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-03-05 13:13:52.455421 iec_api-0.2.8/LICENSE
+-rw-r--r--   0        0        0      599 2024-03-05 13:13:52.455421 iec_api-0.2.8/README.md
+-rw-r--r--   0        0        0        0 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/__init__.py
+-rw-r--r--   0        0        0     6580 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/commons.py
+-rw-r--r--   0        0        0     2024 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/const.py
+-rw-r--r--   0        0        0     7729 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/data.py
+-rw-r--r--   0        0        0    15414 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/iec_client.py
+-rw-r--r--   0        0        0     8500 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/login.py
+-rw-r--r--   0        0        0     1287 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/account.py
+-rw-r--r--   0        0        0     2724 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/contract.py
+-rw-r--r--   0        0        0     2157 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/customer.py
+-rw-r--r--   0        0        0     2951 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/device.py
+-rw-r--r--   0        0        0     1994 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/device_type.py
+-rw-r--r--   0        0        0     1768 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/electric_bill.py
+-rw-r--r--   0        0        0      639 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/exceptions.py
+-rw-r--r--   0        0        0     4153 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/invoice.py
+-rw-r--r--   0        0        0      265 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/jwt.py
+-rw-r--r--   0        0        0     2532 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/meter_reading.py
+-rw-r--r--   0        0        0      658 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/okta_errors.py
+-rw-r--r--   0        0        0     3600 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/remote_reading.py
+-rw-r--r--   0        0        0      971 2024-03-05 13:13:52.455421 iec_api-0.2.8/iec_api/models/response_descriptor.py
+-rw-r--r--   0        0        0     1068 2024-03-05 13:13:52.455421 iec_api-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     1596 1970-01-01 00:00:00.000000 iec_api-0.2.8/PKG-INFO
```

### Comparing `iec_api-0.2.7/LICENSE` & `iec_api-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/README.md` & `iec_api-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/commons.py` & `iec_api-0.2.8/iec_api/commons.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/const.py` & `iec_api-0.2.8/iec_api/const.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/data.py` & `iec_api-0.2.8/iec_api/data.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/iec_client.py` & `iec_api-0.2.8/iec_api/iec_client.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/login.py` & `iec_api-0.2.8/iec_api/login.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/models/account.py` & `iec_api-0.2.8/iec_api/models/account.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/models/contract.py` & `iec_api-0.2.8/iec_api/models/contract.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/models/customer.py` & `iec_api-0.2.8/iec_api/models/customer.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/models/device.py` & `iec_api-0.2.8/iec_api/models/device.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 @dataclass
 class CounterDevice(DataClassDictMixin):
     """Counter Device dataclass."""
 
     device: str = field(metadata=field_options(alias="device"))
     register: str = field(metadata=field_options(alias="register"))
     last_mr: str = field(metadata=field_options(alias="lastMR"))
-    last_mr_date: date = field(metadata=field_options(alias="lastMRDate"))
+    last_mr_date: Optional[date] = field(metadata=field_options(alias="lastMRDate"))
     last_mr_type: str = field(metadata=field_options(alias="lastMRType"))
     last_mr_type_desc: str = field(metadata=field_options(alias="lastMRTypeDesc"))
     connection_size: ConnectionSize = field(metadata=field_options(alias="connectionSize"))
 
 
 @dataclass
 class Devices(DataClassDictMixin):
```

### Comparing `iec_api-0.2.7/iec_api/models/device_type.py` & `iec_api-0.2.8/iec_api/models/device_type.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/models/electric_bill.py` & `iec_api-0.2.8/iec_api/models/electric_bill.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/models/exceptions.py` & `iec_api-0.2.8/iec_api/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/models/invoice.py` & `iec_api-0.2.8/iec_api/models/invoice.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,24 +54,24 @@
 #         "description": "OK"
 #     }
 # }
 
 
 @dataclass
 class Invoice(DataClassDictMixin):
-    full_date: datetime = field(metadata=field_options(alias="fullDate"))
+    full_date: Optional[datetime] = field(metadata=field_options(alias="fullDate"))
     from_date: Optional[datetime] = field(metadata=field_options(alias="fromDate"))
-    to_date: datetime = field(metadata=field_options(alias="toDate"))
+    to_date: Optional[datetime] = field(metadata=field_options(alias="toDate"))
     amount_origin: float = field(metadata=field_options(alias="amountOrigin"))
     amount_to_pay: float = field(metadata=field_options(alias="amountToPay"))
     amount_paid: float = field(metadata=field_options(alias="amountPaid"))
     invoice_id: int = field(metadata=field_options(alias="invoiceId"))
     contract_number: int = field(metadata=field_options(alias="contractNumber"))
     order_number: int = field(metadata=field_options(alias="orderNumber"))
-    last_date: str = field(metadata=field_options(alias="lastDate"))
+    last_date: Optional[str] = field(metadata=field_options(alias="lastDate"))
     invoice_payment_status: int = field(metadata=field_options(alias="invoicePaymentStatus"))
     document_id: str = field(metadata=field_options(alias="documentID"))
     days_period: str = field(metadata=field_options(alias="daysPeriod"))
     has_direct_debit: bool = field(metadata=field_options(alias="hasDirectDebit"))
     invoice_type: int = field(metadata=field_options(alias="invoiceType"))
 
     reading_code: int = field(metadata=field_options(alias="readingCode"), default=0)
```

### Comparing `iec_api-0.2.7/iec_api/models/meter_reading.py` & `iec_api-0.2.8/iec_api/models/meter_reading.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/models/okta_errors.py` & `iec_api-0.2.8/iec_api/models/okta_errors.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/models/remote_reading.py` & `iec_api-0.2.8/iec_api/models/remote_reading.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/iec_api/models/response_descriptor.py` & `iec_api-0.2.8/iec_api/models/response_descriptor.py`

 * *Files identical despite different names*

### Comparing `iec_api-0.2.7/pyproject.toml` & `iec_api-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iec-api"
-version = "0.2.7"
+version = "0.2.8"
 description = "A Python wrapper for Israel Electric Company API"
 authors = ["GuyKh"]
 license = "MIT"
 readme = "README.md"
 maintainers = [
     "Guy Khmelnitsky <guykhmel@gmail.com>",
 ]
```

### Comparing `iec_api-0.2.7/PKG-INFO` & `iec_api-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iec-api
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Python wrapper for Israel Electric Company API
 Home-page: https://github.com/GuyKh/py-iec-api
 License: MIT
 Keywords: python,poetry,api,iec,israel,electric
 Author: GuyKh
 Maintainer: Guy Khmelnitsky
 Maintainer-email: guykhmel@gmail.com
```

