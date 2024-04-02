# Comparing `tmp/reversinglabs-sdk-py3-2.5.0.tar.gz` & `tmp/reversinglabs-sdk-py3-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reversinglabs-sdk-py3-2.5.0.tar", last modified: Sat Mar 30 20:26:48 2024, max compression
+gzip compressed data, was "reversinglabs-sdk-py3-2.5.1.tar", last modified: Tue Apr  2 15:20:20 2024, max compression
```

## Comparing `reversinglabs-sdk-py3-2.5.0.tar` & `reversinglabs-sdk-py3-2.5.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:26:48.454088 reversinglabs-sdk-py3-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     9974 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    48151 2024-03-30 20:26:48.454088 reversinglabs-sdk-py3-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    46794 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:26:48.450088 reversinglabs-sdk-py3-2.5.0/ReversingLabs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:26:48.454088 reversinglabs-sdk-py3-2.5.0/ReversingLabs/SDK/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/ReversingLabs/SDK/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    95910 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/ReversingLabs/SDK/a1000.py
--rw-r--r--   0 runner    (1001) docker     (127)    19593 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/ReversingLabs/SDK/clouddeepscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/ReversingLabs/SDK/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)   250836 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/ReversingLabs/SDK/ticloud.py
--rw-r--r--   0 runner    (1001) docker     (127)    16840 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/ReversingLabs/SDK/tiscale.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/ReversingLabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:26:48.454088 reversinglabs-sdk-py3-2.5.0/reversinglabs_sdk_py3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    48151 2024-03-30 20:26:48.000000 reversinglabs-sdk-py3-2.5.0/reversinglabs_sdk_py3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-30 20:26:48.000000 reversinglabs-sdk-py3-2.5.0/reversinglabs_sdk_py3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 20:26:48.000000 reversinglabs-sdk-py3-2.5.0/reversinglabs_sdk_py3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-30 20:26:48.000000 reversinglabs-sdk-py3-2.5.0/reversinglabs_sdk_py3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-30 20:26:48.000000 reversinglabs-sdk-py3-2.5.0/reversinglabs_sdk_py3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-30 20:26:48.000000 reversinglabs-sdk-py3-2.5.0/reversinglabs_sdk_py3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-30 20:26:48.454088 reversinglabs-sdk-py3-2.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-30 20:26:48.454088 reversinglabs-sdk-py3-2.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/tests/test_a1000.py
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/tests/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/tests/test_ticloud.py
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-03-30 20:26:44.000000 reversinglabs-sdk-py3-2.5.0/tests/test_tiscale.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:20:20.624092 reversinglabs-sdk-py3-2.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    47425 2024-04-02 15:20:20.624092 reversinglabs-sdk-py3-2.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    46067 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:20:20.620092 reversinglabs-sdk-py3-2.5.1/ReversingLabs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:20:20.624092 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    95910 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/a1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19593 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/clouddeepscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)   250836 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/ticloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16866 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/tiscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/ReversingLabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:20:20.624092 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    47425 2024-04-02 15:20:20.000000 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-02 15:20:20.000000 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:20:20.000000 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 15:20:20.000000 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 15:20:20.000000 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 15:20:20.000000 reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-02 15:20:20.624092 reversinglabs-sdk-py3-2.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 15:20:20.624092 reversinglabs-sdk-py3-2.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/tests/test_a1000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/tests/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/tests/test_ticloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-02 15:20:15.000000 reversinglabs-sdk-py3-2.5.1/tests/test_tiscale.py
```

### Comparing `reversinglabs-sdk-py3-2.5.0/CHANGELOG.md` & `reversinglabs-sdk-py3-2.5.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -211,19 +211,26 @@
 
 #### Improvements
 - Python package dependencies are now set to the following values:
   - `requests>=2.28.2`
   - `urllib3>=1.26.14`
 
 
-v2.5.0 (2024-03-29)
+v2.5.0 (2024-03-30)
 -------------------
 
 #### Removals
 - **a1000** module:
   - Removed the `a1000.A1000.advanced_search_v2` method.
 
 #### Improvements
 - Added unit tests.
 - Added CI/CD (Actions) workflows for running unit tests and publishing the package to PyPI.
 - **ticloud** module:
   - `md5` and `sha256` can now be used in `DynamicAnalysis.get_dynamic_analysis_results` for fetching sample analysis results.
+
+
+v2.5.1 (2024-04-02)
+-------------------
+
+#### Improvements
+- Updated the README with an example of error handling.
```

### Comparing `reversinglabs-sdk-py3-2.5.0/LICENSE` & `reversinglabs-sdk-py3-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.0/PKG-INFO` & `reversinglabs-sdk-py3-2.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.5.0
+Version: 2.5.1
 Summary: Python SDK for using ReversingLabs services.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
@@ -1110,48 +1110,30 @@
 
 results = titanium_scale.upload_sample_and_get_results(
     file_source=open("/path/to/file.exe", "rb"),
     full_report=True
 )
 ```
 
-
-#### CloudDeepScan
-```python
-from ReversingLabs.SDK.clouddeepscan import CloudDeepScan, CloudDeepScanException
+#### Error handling
+Each module raises corresponding custom exceptions according to the error status code returned in the response. 
+Custom exception classes that correspond to error status codes also carry the original response object in its entirety. 
+To learn how to fetch and use the response object out of the exception object, see the following examples.
+```python
+from ReversingLabs.SDK.ticloud import FileReputation
 
 
-cloud_deep_scan = CloudDeepScan(
-    token_endpoint="https://exampletokenendpoint.reversinglabs.com/oauth2/token",
-    rest_hostname="https://example.clouddeepscan.com",
-    client_id="exampleclientid",
-    client_secret="exampleclientsecret"
+file_rep = FileReputation(
+    host="https://data.reversinglabs.com",
+    username="u/username",
+    password="password"
 )
-try:
-    submission_id = cloud_deep_scan.upload_sample(sample_path="/path/to/file/suspicious_file.exe")
-except CloudDeepScanException:
-    pass
-
-try:
-    status_data = cloud_deep_scan.fetch_submission(submission_id=submission_id)  # Returns CloudDeepScanSubmissionStatus instance
-    print(status_data.id)  # submission id
-    print(str(status_data.created_at))  # datetime instance
-    print(status_data.status)  # status
-    print(status_data.report)  # URI path to the report file
-except CloudDeepScanException:
-    pass
-
-try:
-    submission_history = cloud_deep_scan.fetch_submission_history(sample_hash="0f5de47158e40b5d791cb3698b7dc599be21cf95")
-    for submission_status in submission_history:
-        print(submission_status.id)  # submission id
-        print(str(submission_status.created_at))  # datetime instance
-        print(submission_status.status)  # status
-        print(submission_status.report)  # URI path to the report file
-except CloudDeepScanException:
-    pass
 
 try:
-    cloud_deep_scan.download_report(sample_hash="0f5de47158e40b5d791cb3698b7dc599be21cf95", report_output_path="reports/report1.json")  # report parent directory must exist
-except CloudDeepScanException:
-    pass
+    resp = file_rep.get_file_reputation(hash_input="cf23df2207d99a74fbe169e3eba035e633b65d94")
+except Exception as e:
+    if hasattr(e, "response_object"):
+        print(e.response_object.content)
+    else:
+        raise 
 ```
+Same approach can also be used for A1000 and TitaniumScale.
```

### Comparing `reversinglabs-sdk-py3-2.5.0/README.md` & `reversinglabs-sdk-py3-2.5.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1078,48 +1078,30 @@
 
 results = titanium_scale.upload_sample_and_get_results(
     file_source=open("/path/to/file.exe", "rb"),
     full_report=True
 )
 ```
 
-
-#### CloudDeepScan
+#### Error handling
+Each module raises corresponding custom exceptions according to the error status code returned in the response. 
+Custom exception classes that correspond to error status codes also carry the original response object in its entirety. 
+To learn how to fetch and use the response object out of the exception object, see the following examples.
 ```python
-from ReversingLabs.SDK.clouddeepscan import CloudDeepScan, CloudDeepScanException
+from ReversingLabs.SDK.ticloud import FileReputation
 
 
-cloud_deep_scan = CloudDeepScan(
-    token_endpoint="https://exampletokenendpoint.reversinglabs.com/oauth2/token",
-    rest_hostname="https://example.clouddeepscan.com",
-    client_id="exampleclientid",
-    client_secret="exampleclientsecret"
+file_rep = FileReputation(
+    host="https://data.reversinglabs.com",
+    username="u/username",
+    password="password"
 )
-try:
-    submission_id = cloud_deep_scan.upload_sample(sample_path="/path/to/file/suspicious_file.exe")
-except CloudDeepScanException:
-    pass
-
-try:
-    status_data = cloud_deep_scan.fetch_submission(submission_id=submission_id)  # Returns CloudDeepScanSubmissionStatus instance
-    print(status_data.id)  # submission id
-    print(str(status_data.created_at))  # datetime instance
-    print(status_data.status)  # status
-    print(status_data.report)  # URI path to the report file
-except CloudDeepScanException:
-    pass
-
-try:
-    submission_history = cloud_deep_scan.fetch_submission_history(sample_hash="0f5de47158e40b5d791cb3698b7dc599be21cf95")
-    for submission_status in submission_history:
-        print(submission_status.id)  # submission id
-        print(str(submission_status.created_at))  # datetime instance
-        print(submission_status.status)  # status
-        print(submission_status.report)  # URI path to the report file
-except CloudDeepScanException:
-    pass
 
 try:
-    cloud_deep_scan.download_report(sample_hash="0f5de47158e40b5d791cb3698b7dc599be21cf95", report_output_path="reports/report1.json")  # report parent directory must exist
-except CloudDeepScanException:
-    pass
+    resp = file_rep.get_file_reputation(hash_input="cf23df2207d99a74fbe169e3eba035e633b65d94")
+except Exception as e:
+    if hasattr(e, "response_object"):
+        print(e.response_object.content)
+    else:
+        raise 
 ```
+Same approach can also be used for A1000 and TitaniumScale.
```

### Comparing `reversinglabs-sdk-py3-2.5.0/ReversingLabs/SDK/a1000.py` & `reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/a1000.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.0/ReversingLabs/SDK/clouddeepscan.py` & `reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/clouddeepscan.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.0/ReversingLabs/SDK/helper.py` & `reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/helper.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.0/ReversingLabs/SDK/ticloud.py` & `reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/ticloud.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.0/ReversingLabs/SDK/tiscale.py` & `reversinglabs-sdk-py3-2.5.1/ReversingLabs/SDK/tiscale.py`

 * *Files 1% similar despite different names*

```diff
@@ -456,8 +456,8 @@
         """Accepts a response object for validation and raises an exception if an error status code is received.
             :return: response
             :rtype: requests.Response
         """
         exception = RESPONSE_CODE_ERROR_MAP.get(response.status_code, None)
         if not exception:
             return
-        raise exception
+        raise exception(response_object=response)
```

### Comparing `reversinglabs-sdk-py3-2.5.0/logo.png` & `reversinglabs-sdk-py3-2.5.1/logo.png`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.0/reversinglabs_sdk_py3.egg-info/PKG-INFO` & `reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reversinglabs-sdk-py3
-Version: 2.5.0
+Version: 2.5.1
 Summary: Python SDK for using ReversingLabs services.
 Home-page: https://github.com/reversinglabs/reversinglabs-sdk-py3
 Author: ReversingLabs
 Author-email: support@reversinglabs.com
 License: MIT
 Project-URL: Documentation, https://github.com/reversinglabs/reversinglabs-sdk-py3/blob/main/README.md
 Project-URL: Source, https://github.com/reversinglabs/reversinglabs-sdk-py3
@@ -1110,48 +1110,30 @@
 
 results = titanium_scale.upload_sample_and_get_results(
     file_source=open("/path/to/file.exe", "rb"),
     full_report=True
 )
 ```
 
-
-#### CloudDeepScan
-```python
-from ReversingLabs.SDK.clouddeepscan import CloudDeepScan, CloudDeepScanException
+#### Error handling
+Each module raises corresponding custom exceptions according to the error status code returned in the response. 
+Custom exception classes that correspond to error status codes also carry the original response object in its entirety. 
+To learn how to fetch and use the response object out of the exception object, see the following examples.
+```python
+from ReversingLabs.SDK.ticloud import FileReputation
 
 
-cloud_deep_scan = CloudDeepScan(
-    token_endpoint="https://exampletokenendpoint.reversinglabs.com/oauth2/token",
-    rest_hostname="https://example.clouddeepscan.com",
-    client_id="exampleclientid",
-    client_secret="exampleclientsecret"
+file_rep = FileReputation(
+    host="https://data.reversinglabs.com",
+    username="u/username",
+    password="password"
 )
-try:
-    submission_id = cloud_deep_scan.upload_sample(sample_path="/path/to/file/suspicious_file.exe")
-except CloudDeepScanException:
-    pass
-
-try:
-    status_data = cloud_deep_scan.fetch_submission(submission_id=submission_id)  # Returns CloudDeepScanSubmissionStatus instance
-    print(status_data.id)  # submission id
-    print(str(status_data.created_at))  # datetime instance
-    print(status_data.status)  # status
-    print(status_data.report)  # URI path to the report file
-except CloudDeepScanException:
-    pass
-
-try:
-    submission_history = cloud_deep_scan.fetch_submission_history(sample_hash="0f5de47158e40b5d791cb3698b7dc599be21cf95")
-    for submission_status in submission_history:
-        print(submission_status.id)  # submission id
-        print(str(submission_status.created_at))  # datetime instance
-        print(submission_status.status)  # status
-        print(submission_status.report)  # URI path to the report file
-except CloudDeepScanException:
-    pass
 
 try:
-    cloud_deep_scan.download_report(sample_hash="0f5de47158e40b5d791cb3698b7dc599be21cf95", report_output_path="reports/report1.json")  # report parent directory must exist
-except CloudDeepScanException:
-    pass
+    resp = file_rep.get_file_reputation(hash_input="cf23df2207d99a74fbe169e3eba035e633b65d94")
+except Exception as e:
+    if hasattr(e, "response_object"):
+        print(e.response_object.content)
+    else:
+        raise 
 ```
+Same approach can also be used for A1000 and TitaniumScale.
```

### Comparing `reversinglabs-sdk-py3-2.5.0/reversinglabs_sdk_py3.egg-info/SOURCES.txt` & `reversinglabs-sdk-py3-2.5.1/reversinglabs_sdk_py3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.0/setup.py` & `reversinglabs-sdk-py3-2.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.0/tests/test_a1000.py` & `reversinglabs-sdk-py3-2.5.1/tests/test_a1000.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.0/tests/test_helper.py` & `reversinglabs-sdk-py3-2.5.1/tests/test_helper.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.0/tests/test_ticloud.py` & `reversinglabs-sdk-py3-2.5.1/tests/test_ticloud.py`

 * *Files identical despite different names*

### Comparing `reversinglabs-sdk-py3-2.5.0/tests/test_tiscale.py` & `reversinglabs-sdk-py3-2.5.1/tests/test_tiscale.py`

 * *Files identical despite different names*

