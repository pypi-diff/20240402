# Comparing `tmp/dapla_statbank_client-1.1.1.tar.gz` & `tmp/dapla_statbank_client-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_statbank_client-1.1.1.tar", max compression
+gzip compressed data, was "dapla_statbank_client-1.1.2.tar", max compression
```

## Comparing `dapla_statbank_client-1.1.1.tar` & `dapla_statbank_client-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2024-03-22 13:48:44.490588 dapla_statbank_client-1.1.1/LICENSE
--rw-r--r--   0        0        0    13544 2024-03-22 13:48:44.490588 dapla_statbank_client-1.1.1/README.md
--rw-r--r--   0        0        0     4224 2024-03-22 13:48:58.902563 dapla_statbank_client-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1581 2024-03-22 13:48:44.494588 dapla_statbank_client-1.1.1/src/statbank/__init__.py
--rw-r--r--   0        0        0     4105 2024-03-22 13:48:44.494588 dapla_statbank_client-1.1.1/src/statbank/api_types.py
--rw-r--r--   0        0        0     5776 2024-03-22 13:48:44.494588 dapla_statbank_client-1.1.1/src/statbank/apidata.py
--rw-r--r--   0        0        0     3993 2024-03-22 13:48:44.494588 dapla_statbank_client-1.1.1/src/statbank/auth.py
--rw-r--r--   0        0        0    19130 2024-03-22 13:48:58.902563 dapla_statbank_client-1.1.1/src/statbank/client.py
--rw-r--r--   0        0        0     1136 2024-03-22 13:48:58.902563 dapla_statbank_client-1.1.1/src/statbank/globals.py
--rw-r--r--   0        0        0        0 2024-03-22 13:48:44.494588 dapla_statbank_client-1.1.1/src/statbank/py.typed
--rw-r--r--   0        0        0     1304 2024-03-22 13:48:44.494588 dapla_statbank_client-1.1.1/src/statbank/statbank_logger.py
--rw-r--r--   0        0        0    14430 2024-03-22 13:48:58.902563 dapla_statbank_client-1.1.1/src/statbank/transfer.py
--rw-r--r--   0        0        0    17741 2024-03-22 13:48:44.494588 dapla_statbank_client-1.1.1/src/statbank/uttrekk.py
--rw-r--r--   0        0        0    26391 2024-03-22 13:48:44.494588 dapla_statbank_client-1.1.1/src/statbank/uttrekk_validations.py
--rw-r--r--   0        0        0    14932 1970-01-01 00:00:00.000000 dapla_statbank_client-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-02 07:35:33.336023 dapla_statbank_client-1.1.2/LICENSE
+-rw-r--r--   0        0        0    13544 2024-04-02 07:35:33.336023 dapla_statbank_client-1.1.2/README.md
+-rw-r--r--   0        0        0     4224 2024-04-02 07:35:43.240079 dapla_statbank_client-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1581 2024-04-02 07:35:33.340023 dapla_statbank_client-1.1.2/src/statbank/__init__.py
+-rw-r--r--   0        0        0     4105 2024-04-02 07:35:33.340023 dapla_statbank_client-1.1.2/src/statbank/api_types.py
+-rw-r--r--   0        0        0     5776 2024-04-02 07:35:33.340023 dapla_statbank_client-1.1.2/src/statbank/apidata.py
+-rw-r--r--   0        0        0     3993 2024-04-02 07:35:33.340023 dapla_statbank_client-1.1.2/src/statbank/auth.py
+-rw-r--r--   0        0        0    19221 2024-04-02 07:35:43.240079 dapla_statbank_client-1.1.2/src/statbank/client.py
+-rw-r--r--   0        0        0     1136 2024-04-02 07:35:33.340023 dapla_statbank_client-1.1.2/src/statbank/globals.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:35:33.340023 dapla_statbank_client-1.1.2/src/statbank/py.typed
+-rw-r--r--   0        0        0     1304 2024-04-02 07:35:33.340023 dapla_statbank_client-1.1.2/src/statbank/statbank_logger.py
+-rw-r--r--   0        0        0    14529 2024-04-02 07:35:43.240079 dapla_statbank_client-1.1.2/src/statbank/transfer.py
+-rw-r--r--   0        0        0    17741 2024-04-02 07:35:33.340023 dapla_statbank_client-1.1.2/src/statbank/uttrekk.py
+-rw-r--r--   0        0        0    26391 2024-04-02 07:35:33.340023 dapla_statbank_client-1.1.2/src/statbank/uttrekk_validations.py
+-rw-r--r--   0        0        0    14932 1970-01-01 00:00:00.000000 dapla_statbank_client-1.1.2/PKG-INFO
```

### Comparing `dapla_statbank_client-1.1.1/LICENSE` & `dapla_statbank_client-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.1.1/README.md` & `dapla_statbank_client-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.1.1/pyproject.toml` & `dapla_statbank_client-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-statbank-client"
-version = "1.1.1"
+version = "1.1.2"
 description = "Handles data transfer Statbank <-> Dapla for Statistics Norway"
 authors = ["Statistics Norway", "Carl F. Corneil <cfc@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-statbank-client"
 repository = "https://github.com/statisticsnorway/dapla-statbank-client"
 documentation = "https://statisticsnorway.github.io/dapla-statbank-client"
```

### Comparing `dapla_statbank_client-1.1.1/src/statbank/__init__.py` & `dapla_statbank_client-1.1.2/src/statbank/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.1.1/src/statbank/api_types.py` & `dapla_statbank_client-1.1.2/src/statbank/api_types.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.1.1/src/statbank/apidata.py` & `dapla_statbank_client-1.1.2/src/statbank/apidata.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.1.1/src/statbank/auth.py` & `dapla_statbank_client-1.1.2/src/statbank/auth.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.1.1/src/statbank/client.py` & `dapla_statbank_client-1.1.2/src/statbank/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,17 +99,20 @@
                 hours=1,
             )  # Compensate for setting the timezone, stop publishing date from moving
         else:
             self.date = date
         self._validate_date()
         self.date = self.date.replace(hour=8, minute=0, second=0, microsecond=0)
         if self.check_username_password:
+            logger.info(
+                "Checking filbeskrivelse of random tableid 05300 to double-check username & password early.",
+            )
             self.get_description(
                 "05300",
-            )  # Random tableid to double check username&password early
+            )
         logger.info("Publishing date set to %s", self.date.isoformat("T", "seconds"))
 
     # Representation
     def __str__(self) -> str:
         """Print a human readable text of the clients attributes."""
         return f"""StatbankClient for user {self.loaduser}
         Publishing at {self.date}
```

### Comparing `dapla_statbank_client-1.1.1/src/statbank/globals.py` & `dapla_statbank_client-1.1.2/src/statbank/globals.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.1.1/src/statbank/statbank_logger.py` & `dapla_statbank_client-1.1.2/src/statbank/statbank_logger.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.1.1/src/statbank/transfer.py` & `dapla_statbank_client-1.1.2/src/statbank/transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
             self.headers = headers
         try:
             self.params = self._build_params()
             self._validate_datatype()
             self.body = self._body_from_data()
 
             url_load_params = self.urls["loader"] + urllib.parse.urlencode(self.params)
+            urllib.parse.urlparse(url_load_params)  # Test to see if url is valid format
             self.response = self._make_transfer_request(url_load_params)
             self._cleanup_response()
         finally:
             del self.headers  # Cleaning up auth-storing
             self.__delay = False
         self._handle_response()
 
@@ -285,15 +286,15 @@
         return {
             "initialier": self.shortuser,
             "hovedtabell": self.tableid,
             "publiseringsdato": date,
             "fagansvarlig1": self.cc,
             "fagansvarlig2": self.bcc,
             "auto_overskriv_data": str(int(self.overwrite)),
-            "auto_godkjenn_data": self.approve,
+            "auto_godkjenn_data": str(int(self.approve)),
         }
 
     def _make_transfer_request(
         self,
         url_params: str,
     ) -> r.Response:
         result = r.post(url_params, headers=self.headers, data=self.body, timeout=15)
```

### Comparing `dapla_statbank_client-1.1.1/src/statbank/uttrekk.py` & `dapla_statbank_client-1.1.2/src/statbank/uttrekk.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.1.1/src/statbank/uttrekk_validations.py` & `dapla_statbank_client-1.1.2/src/statbank/uttrekk_validations.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.1.1/PKG-INFO` & `dapla_statbank_client-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-statbank-client
-Version: 1.1.1
+Version: 1.1.2
 Summary: Handles data transfer Statbank <-> Dapla for Statistics Norway
 Home-page: https://github.com/statisticsnorway/dapla-statbank-client
 License: MIT
 Author: Statistics Norway
 Requires-Python: >=3.10,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

