# Comparing `tmp/c12_callisto_clients-2.0.0-py2.py3-none-any.whl.zip` & `tmp/c12_callisto_clients-2.0.1-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 40806 bytes, number of entries: 36
+Zip file size: 40786 bytes, number of entries: 36
 -rw-r--r--  2.0 unx      238 b- defN 23-Sep-19 15:34 c12_callisto_clients/__init__.py
 -rw-r--r--  2.0 unx      110 b- defN 23-Sep-19 13:08 c12_callisto_clients/user_configs.py
 -rw-r--r--  2.0 unx       68 b- defN 23-Sep-19 13:08 c12_callisto_clients/api/__init__.py
 -rw-r--r--  2.0 unx     9719 b- defN 23-Sep-19 13:23 c12_callisto_clients/api/client.py
--rw-r--r--  2.0 unx      725 b- defN 23-Sep-19 16:08 c12_callisto_clients/api/configs.py
+-rw-r--r--  2.0 unx      691 b- defN 23-Sep-20 08:25 c12_callisto_clients/api/configs.py
 -rw-r--r--  2.0 unx      136 b- defN 23-Sep-19 13:08 c12_callisto_clients/api/exceptions.py
 -rw-r--r--  2.0 unx       67 b- defN 23-Sep-19 15:26 c12_callisto_clients/pytket/__init__.py
 -rw-r--r--  2.0 unx       56 b- defN 23-Sep-19 15:26 c12_callisto_clients/pytket/extensions/__init__.py
 -rw-r--r--  2.0 unx       47 b- defN 23-Sep-19 13:08 c12_callisto_clients/pytket/extensions/callisto/__init__.py
 -rw-r--r--  2.0 unx       38 b- defN 23-Sep-19 13:08 c12_callisto_clients/pytket/extensions/callisto/backends/__init__.py
 -rw-r--r--  2.0 unx    15848 b- defN 23-Sep-19 13:23 c12_callisto_clients/pytket/extensions/callisto/backends/callisto.py
 -rw-r--r--  2.0 unx       84 b- defN 23-Sep-19 13:08 c12_callisto_clients/qiskit/__init__.py
@@ -27,12 +27,12 @@
 -rw-r--r--  2.0 unx      573 b- defN 23-Apr-12 13:40 c12simulator_clients/api/configs.py
 -rw-r--r--  2.0 unx      136 b- defN 23-Mar-20 13:06 c12simulator_clients/api/exceptions.py
 -rw-r--r--  2.0 unx       84 b- defN 23-Mar-17 11:20 c12simulator_clients/qiskit_back/__init__.py
 -rw-r--r--  2.0 unx     9633 b- defN 23-Sep-19 13:23 c12simulator_clients/qiskit_back/c12sim_backend.py
 -rw-r--r--  2.0 unx     8334 b- defN 23-Sep-19 13:23 c12simulator_clients/qiskit_back/c12sim_job.py
 -rw-r--r--  2.0 unx     3010 b- defN 23-Sep-19 13:23 c12simulator_clients/qiskit_back/c12sim_provider.py
 -rw-r--r--  2.0 unx      200 b- defN 23-Mar-20 13:06 c12simulator_clients/qiskit_back/exceptions.py
--rw-r--r--  2.0 unx     3632 b- defN 23-Sep-20 08:12 c12_callisto_clients-2.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Sep-20 08:12 c12_callisto_clients-2.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-Sep-20 08:12 c12_callisto_clients-2.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3542 b- defN 23-Sep-20 08:12 c12_callisto_clients-2.0.0.dist-info/RECORD
-36 files, 117236 bytes uncompressed, 34904 bytes compressed:  70.2%
+-rw-r--r--  2.0 unx     3632 b- defN 23-Sep-20 08:26 c12_callisto_clients-2.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Sep-20 08:26 c12_callisto_clients-2.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Sep-20 08:26 c12_callisto_clients-2.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3542 b- defN 23-Sep-20 08:26 c12_callisto_clients-2.0.1.dist-info/RECORD
+36 files, 117202 bytes uncompressed, 34884 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -90,20 +90,20 @@
 
 Filename: c12simulator_clients/qiskit_back/c12sim_provider.py
 Comment: 
 
 Filename: c12simulator_clients/qiskit_back/exceptions.py
 Comment: 
 
-Filename: c12_callisto_clients-2.0.0.dist-info/METADATA
+Filename: c12_callisto_clients-2.0.1.dist-info/METADATA
 Comment: 
 
-Filename: c12_callisto_clients-2.0.0.dist-info/WHEEL
+Filename: c12_callisto_clients-2.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: c12_callisto_clients-2.0.0.dist-info/top_level.txt
+Filename: c12_callisto_clients-2.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: c12_callisto_clients-2.0.0.dist-info/RECORD
+Filename: c12_callisto_clients-2.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## c12_callisto_clients/api/configs.py

```diff
@@ -1,15 +1,15 @@
 """
   Basic URLs to the C12 sim APIs.
 """
 
 import os
 
-HOST_URL = os.getenv("C12_HOST_URL", "api.dev-simulator.c12qe.net")
-PORT = os.getenv("C12_PORT")  # Used for testing purposes
+HOST_URL = os.getenv("C12_HOST_URL", "57.128.103.232")
+PORT = os.getenv("C12_PORT", "8080")
 PROTOCOL = os.getenv("C12_PROTOCOL", "http")
 
 API_BASE_URL = f"{PROTOCOL}://{HOST_URL}{'' if PORT is None else ':'+str(PORT)}/api"
 
 API_SIMULATOR_URL = API_BASE_URL + "/c12sim"
 API_HEALTH_URL = API_BASE_URL + "/health"
```

## Comparing `c12_callisto_clients-2.0.0.dist-info/METADATA` & `c12_callisto_clients-2.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c12-callisto-clients
-Version: 2.0.0
+Version: 2.0.1
 Summary: Different clients for access to the C12 simulator
 Home-page: https://github.com/c12qe/c12simulator-clients
 Author: C12 Quantum Electronics
 Author-email: viktor@c12qe.com
 License: MIT
 Project-URL: Homepage, https://www.c12qe.com
 Project-URL: Source code, https://github.com/c12qe/c12simulator-clients
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: c12-callisto-clients Version: 2.0.0 Summary:
+Metadata-Version: 2.1 Name: c12-callisto-clients Version: 2.0.1 Summary:
 Different clients for access to the C12 simulator Home-page: https://
 github.com/c12qe/c12simulator-clients Author: C12 Quantum Electronics Author-
 email: viktor@c12qe.com License: MIT Project-URL: Homepage, https://
 www.c12qe.com Project-URL: Source code, https://github.com/c12qe/c12simulator-
 clients Project-URL: Issues, https://github.com/c12qe/c12simulator-clients/
 issues Project-URL: Documentation, https://github.com/c12qe/c12simulator-
 clients/tree/master/docs Keywords: qiskit quantum c12 simulator Classifier:
```

## Comparing `c12_callisto_clients-2.0.0.dist-info/RECORD` & `c12_callisto_clients-2.0.1.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 c12_callisto_clients/__init__.py,sha256=kcNwNPjY5F1mqXH9GsAbqluax1mCdYOP2xS2kLjqKhY,238
 c12_callisto_clients/user_configs.py,sha256=DAyfYH5OHHNVQRmV_c8uut4bGAI5DZgs0VHdMRtshuQ,110
 c12_callisto_clients/api/__init__.py,sha256=RGQhfLIZT1rIbTyTUlBnP8pivcXs4-XIsLfJh3JEvW0,68
 c12_callisto_clients/api/client.py,sha256=5BAgb2V8Ege0JgHTLsPZC3eIYfmI6IQVs1Mldw5V37Q,9719
-c12_callisto_clients/api/configs.py,sha256=9KE7ULet7C1d9xykpKjoq5ajNRUCdH_rpuTf8Lzq3uU,725
+c12_callisto_clients/api/configs.py,sha256=YXrHOy8MTeA8Req5wgMFPgkjnPc0ce5zSeIS1CVTxFk,691
 c12_callisto_clients/api/exceptions.py,sha256=PNU6_IwyfejUnvkACbJ9cUbI1VZbLrsmX4jL6EKcPGY,136
 c12_callisto_clients/pytket/__init__.py,sha256=ZzClkZB-qgATJRd6M5IAh5fep_LDM73Z92sffNAHoFM,67
 c12_callisto_clients/pytket/extensions/__init__.py,sha256=1rzZdjbx7wKRF6rqMkzMUHy2GgtmMmLuomJ_lvpRKqw,56
 c12_callisto_clients/pytket/extensions/callisto/__init__.py,sha256=Hyp0ACY90J-jXOPEKWZSxzJ6s31Bim4PBAn2xjpFBUQ,47
 c12_callisto_clients/pytket/extensions/callisto/backends/__init__.py,sha256=ts3xIJOo7v7iBarOVxyRzkkY9IHPyD3Cxahz0suyR54,38
 c12_callisto_clients/pytket/extensions/callisto/backends/callisto.py,sha256=oj0eVXyiiKa8dMoqkBW0rA8xUxzIhWWhjD24Ru2JE4I,15848
 c12_callisto_clients/qiskit/__init__.py,sha256=bHsGQK1gWaDK6yyTa1aIhtxXd8eqPOKr6fi9lKzil8U,84
@@ -26,11 +26,11 @@
 c12simulator_clients/api/configs.py,sha256=pmNNdH6Lou1fyZzWGdKimCE10Dc9AN46E_xXnm9AgcU,573
 c12simulator_clients/api/exceptions.py,sha256=PNU6_IwyfejUnvkACbJ9cUbI1VZbLrsmX4jL6EKcPGY,136
 c12simulator_clients/qiskit_back/__init__.py,sha256=bHsGQK1gWaDK6yyTa1aIhtxXd8eqPOKr6fi9lKzil8U,84
 c12simulator_clients/qiskit_back/c12sim_backend.py,sha256=fqAu43WwNA9B8VajG29Ds_3rvwUyCG3DZVaGwiKRNAI,9633
 c12simulator_clients/qiskit_back/c12sim_job.py,sha256=npfcfDoDUdi26zYgQZwfIf3_B9eY24AuKLlTSaeh0rk,8334
 c12simulator_clients/qiskit_back/c12sim_provider.py,sha256=ENZBrSZjStKzhb2PvLsdS6XrrF0DFPCOMZmdnBPRa2I,3010
 c12simulator_clients/qiskit_back/exceptions.py,sha256=TUqWV4IJfgF6ajTvHHuhX5GYiZ5pomCBLFUy6RAF0lI,200
-c12_callisto_clients-2.0.0.dist-info/METADATA,sha256=Mihk3DsBiwAnIL6RDAqW5q2_cg5l4kuUa3cu1vMZkjk,3632
-c12_callisto_clients-2.0.0.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
-c12_callisto_clients-2.0.0.dist-info/top_level.txt,sha256=TE8IYcO_ALxDoe7ZXDM4t2pclpMHMfCi_yM2IRctzyU,21
-c12_callisto_clients-2.0.0.dist-info/RECORD,,
+c12_callisto_clients-2.0.1.dist-info/METADATA,sha256=J4xttkgmqUBvJHPvKdkipS8YfucFFsFQJKXfXkoFWzE,3632
+c12_callisto_clients-2.0.1.dist-info/WHEEL,sha256=bb2Ot9scclHKMOLDEHY6B2sicWOgugjFKaJsT7vwMQo,110
+c12_callisto_clients-2.0.1.dist-info/top_level.txt,sha256=TE8IYcO_ALxDoe7ZXDM4t2pclpMHMfCi_yM2IRctzyU,21
+c12_callisto_clients-2.0.1.dist-info/RECORD,,
```

