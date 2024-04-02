# Comparing `tmp/waifuvault-1.3.2.tar.gz` & `tmp/waifuvault-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waifuvault-1.3.2.tar", last modified: Sun Mar 24 18:38:20 2024, max compression
+gzip compressed data, was "waifuvault-1.3.3.tar", last modified: Tue Apr  2 16:35:30 2024, max compression
```

## Comparing `waifuvault-1.3.2.tar` & `waifuvault-1.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:38:20.721122 waifuvault-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-24 18:38:09.000000 waifuvault-1.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-03-24 18:38:20.721122 waifuvault-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7772 2024-03-24 18:38:09.000000 waifuvault-1.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-24 18:38:09.000000 waifuvault-1.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-24 18:38:20.721122 waifuvault-1.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:38:20.717122 waifuvault-1.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:38:20.717122 waifuvault-1.3.2/src/waifuvault/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-24 18:38:09.000000 waifuvault-1.3.2/src/waifuvault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-03-24 18:38:09.000000 waifuvault-1.3.2/src/waifuvault/waifumodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-03-24 18:38:09.000000 waifuvault-1.3.2/src/waifuvault/waifuvault.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:38:20.721122 waifuvault-1.3.2/src/waifuvault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8464 2024-03-24 18:38:20.000000 waifuvault-1.3.2/src/waifuvault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-03-24 18:38:20.000000 waifuvault-1.3.2/src/waifuvault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-24 18:38:20.000000 waifuvault-1.3.2/src/waifuvault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-24 18:38:20.000000 waifuvault-1.3.2/src/waifuvault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-24 18:38:20.000000 waifuvault-1.3.2/src/waifuvault.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-24 18:38:20.721122 waifuvault-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7320 2024-03-24 18:38:09.000000 waifuvault-1.3.2/tests/test_waifuvault.py
+drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:35:30.316700 waifuvault-1.3.3/
+-rw-r--r--   0 walker     (501) staff       (20)     1071 2024-03-11 13:55:18.000000 waifuvault-1.3.3/LICENSE
+-rw-r--r--   0 walker     (501) staff       (20)     8464 2024-04-02 16:35:30.315367 waifuvault-1.3.3/PKG-INFO
+-rw-r--r--   0 walker     (501) staff       (20)     7772 2024-03-24 14:27:53.000000 waifuvault-1.3.3/README.md
+-rw-r--r--   0 walker     (501) staff       (20)      741 2024-04-02 16:33:02.000000 waifuvault-1.3.3/pyproject.toml
+-rw-r--r--   0 walker     (501) staff       (20)       38 2024-04-02 16:35:30.316944 waifuvault-1.3.3/setup.cfg
+drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:35:30.304127 waifuvault-1.3.3/src/
+drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:35:30.308924 waifuvault-1.3.3/src/waifuvault/
+-rw-r--r--   0 walker     (501) staff       (20)      133 2024-03-20 19:19:23.000000 waifuvault-1.3.3/src/waifuvault/__init__.py
+-rw-r--r--   0 walker     (501) staff       (20)     1695 2024-04-02 16:24:50.000000 waifuvault-1.3.3/src/waifuvault/waifumodels.py
+-rw-r--r--   0 walker     (501) staff       (20)     3568 2024-04-02 16:29:36.000000 waifuvault-1.3.3/src/waifuvault/waifuvault.py
+drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:35:30.313810 waifuvault-1.3.3/src/waifuvault.egg-info/
+-rw-r--r--   0 walker     (501) staff       (20)     8464 2024-04-02 16:35:30.000000 waifuvault-1.3.3/src/waifuvault.egg-info/PKG-INFO
+-rw-r--r--   0 walker     (501) staff       (20)      332 2024-04-02 16:35:30.000000 waifuvault-1.3.3/src/waifuvault.egg-info/SOURCES.txt
+-rw-r--r--   0 walker     (501) staff       (20)        1 2024-04-02 16:35:30.000000 waifuvault-1.3.3/src/waifuvault.egg-info/dependency_links.txt
+-rw-r--r--   0 walker     (501) staff       (20)       53 2024-04-02 16:35:30.000000 waifuvault-1.3.3/src/waifuvault.egg-info/requires.txt
+-rw-r--r--   0 walker     (501) staff       (20)       11 2024-04-02 16:35:30.000000 waifuvault-1.3.3/src/waifuvault.egg-info/top_level.txt
+drwxr-xr-x   0 walker     (501) staff       (20)        0 2024-04-02 16:35:30.312978 waifuvault-1.3.3/tests/
+-rw-r--r--   0 walker     (501) staff       (20)     7852 2024-04-02 16:33:02.000000 waifuvault-1.3.3/tests/test_waifuvault.py
```

### Comparing `waifuvault-1.3.2/LICENSE` & `waifuvault-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `waifuvault-1.3.2/PKG-INFO` & `waifuvault-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waifuvault
-Version: 1.3.2
+Version: 1.3.3
 Summary: waifuVault Python API module
 Author-email: Walker Aldridge <walker@waifuvault.moe>
 Project-URL: Homepage, https://github.com/waifuvault/waifuVault-python-api
 Project-URL: Issues, https://github.com/waifuvault/waifuVault-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `waifuvault-1.3.2/README.md` & `waifuvault-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `waifuvault-1.3.2/pyproject.toml` & `waifuvault-1.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "waifuvault"
-version = "1.3.2"
+version = "1.3.3"
 authors = [
     { name="Walker Aldridge", email="walker@waifuvault.moe" },
 ]
 description = "waifuVault Python API module"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `waifuvault-1.3.2/src/waifuvault/waifumodels.py` & `waifuvault-1.3.3/src/waifuvault/waifumodels.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Models for waifuVault
 import io
 
 
 class FileUpload:
-    def __init__(self, target: any, target_name: str = "unknown", expires: str = None, password: str = None, hidefilename: bool = False):
+    def __init__(self, target: any, target_name: str = "unknown", expires: str = None, password: str = None, hidefilename: bool = False, oneTimeDownload: bool = False):
         self.target = target
         self.target_name = target_name
         self.hidefilename = hidefilename
+        self.one_time_download = oneTimeDownload
         self.expires = expires
         self.password = password
 
     def is_url(self):
         if isinstance(self.target, io.BytesIO):
             return False
         return self.target.lower().startswith("http://") or self.target.lower().startswith("https://")
@@ -21,17 +22,26 @@
     def build_parameters(self):
         parameters = {}
         if self.password:
             parameters['password'] = self.password
         if self.expires:
             parameters['expires'] = self.expires
         if self.hidefilename:
-            parameters['hide_filename'] = self.hidefilename
+            parameters['hide_filename'] = str(self.hidefilename).lower()
+        if self.one_time_download:
+            parameters['one_time_download'] = str(self.one_time_download).lower()
         return parameters
 
 
 class FileResponse:
-    def __init__(self, token: str = None, url: str = None, protected: bool = False, retention_period: any = None):
+    def __init__(self, token: str = None, url: str = None, retention_period: any = None, options: any = None):
         self.token = token
         self.url = url
-        self.protected = protected
         self.retentionPeriod = retention_period
+        self.options = options
+
+
+class FileOptions:
+    def __init__(self, hide_filename: bool = False, one_time_download: bool = False, protected: bool = False):
+        self.hideFilename = hide_filename
+        self.oneTimeDownload = one_time_download
+        self.protected = protected
```

### Comparing `waifuvault-1.3.2/src/waifuvault/waifuvault.py` & `waifuvault-1.3.3/src/waifuvault/waifuvault.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import os
 from io import BytesIO
 
 import requests
 from requests_toolbelt import MultipartEncoder
 
-from .waifumodels import FileResponse, FileUpload
+from .waifumodels import FileResponse, FileUpload, FileOptions
 
 
 # Upload File
 def upload_file(file_obj: FileUpload):
     if file_obj.is_buffer():
         multipart_data = MultipartEncoder(
             fields={'file': (file_obj.target_name, file_obj.target)}
@@ -103,9 +103,13 @@
     return
 
 
 def __dict_to_obj(dict_obj: any):
     return FileResponse(
         dict_obj["token"],
         dict_obj["url"],
-        dict_obj["protected"],
-        dict_obj["retentionPeriod"])
+        dict_obj["retentionPeriod"],
+        FileOptions(
+            dict_obj["options.hideFileName"],
+            dict_obj["options.oneTimeDownload"],
+            dict_obj["protected"]
+        ))
```

### Comparing `waifuvault-1.3.2/src/waifuvault.egg-info/PKG-INFO` & `waifuvault-1.3.3/src/waifuvault.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waifuvault
-Version: 1.3.2
+Version: 1.3.3
 Summary: waifuVault Python API module
 Author-email: Walker Aldridge <walker@waifuvault.moe>
 Project-URL: Homepage, https://github.com/waifuvault/waifuVault-python-api
 Project-URL: Issues, https://github.com/waifuvault/waifuVault-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `waifuvault-1.3.2/tests/test_waifuvault.py` & `waifuvault-1.3.3/tests/test_waifuvault.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,130 +23,192 @@
                                   '{"url":"https://waifuvault.moe/f/something", "token":"test-token", "protected":false, "retentionPeriod":"10 minutes"}')
 bad_request = response_mock(False,
                             '{"name": "BAD_REQUEST", "message": "Error Test", "status": 400}',code=400)
 
 
 # URL Upload Tests
 def test_upload_url(mocker):
+    # Given
     mock_put = mocker.patch('requests.put', return_value = ok_response_numeric)
     upload_file = waifuvault.FileUpload("https://walker.moe/assets/sunflowers.png", expires="10m")
+
+    # When
     upload_res = waifuvault.upload_file(upload_file)
     mock_put.assert_called_once_with(
         'https://waifuvault.moe/rest',
         params={'expires': '10m'},
         data={'url': 'https://walker.moe/assets/sunflowers.png'},
         headers=None)
+
+    # Then
     assert (upload_res.url == "https://waifuvault.moe/f/something"), "URL does not match"
     assert (upload_res.token == "test-token"), "Token does not match"
-    assert (upload_res.protected is False), "Protected does not match"
-    assert (upload_res.retentionPeriod == 100), "Retention does not match"
+    assert (upload_res.options.protected is False), "Protected does not match"
+    assert (upload_res.options.retentionPeriod == 100), "Retention does not match"
 
 
 def test_upload_url_error(mocker):
+    # Given
     mock_put = mocker.patch('requests.put', return_value = bad_request)
+
+    # When
     upload_file = waifuvault.FileUpload("https://walker.moe/assets/sunflowers.png", expires="10m")
+
+    # Then
     with pytest.raises(Exception, match=re.escape('Error 400 (BAD_REQUEST): Error Test')):
         upload_res = waifuvault.upload_file(upload_file)
 
 
 def test_upload_file(mocker):
+    # Given
     mock_put = mocker.patch('requests.put', return_value = ok_response_numeric)
     upload_file = waifuvault.FileUpload("tests/testfile.png", expires="10m")
+
+    # When
     upload_res = waifuvault.upload_file(upload_file)
+
+    # Then
     mock_put.assert_called_once()
     assert (upload_res.url == "https://waifuvault.moe/f/something"), "URL does not match"
     assert (upload_res.token == "test-token"), "Token does not match"
-    assert (upload_res.protected is False), "Protected does not match"
-    assert (upload_res.retentionPeriod == 100), "Retention does not match"
+    assert (upload_res.options.protected is False), "Protected does not match"
+    assert (upload_res.options.retentionPeriod == 100), "Retention does not match"
 
 
 def test_upload_file_error(mocker):
+    # Given
     mock_put = mocker.patch('requests.put', return_value = bad_request)
+
+    # When
     upload_file = waifuvault.FileUpload("tests/testfile.png", expires="10m")
+
+    # Then
     with pytest.raises(Exception, match=re.escape('Error 400 (BAD_REQUEST): Error Test')):
         upload_res = waifuvault.upload_file(upload_file)
 
 
 def test_upload_buffer(mocker):
+    # Given
     mock_put = mocker.patch('requests.put', return_value = ok_response_numeric)
     with open("tests/testfile.png", "rb") as fh:
         buf = io.BytesIO(fh.read())
     upload_file = waifuvault.FileUpload(buf,"testfile_buf.png",expires="10m")
+
+    # When
     upload_res = waifuvault.upload_file(upload_file)
+
+    # Then
     mock_put.assert_called_once()
     assert (upload_res.url == "https://waifuvault.moe/f/something"), "URL does not match"
     assert (upload_res.token == "test-token"), "Token does not match"
-    assert (upload_res.protected is False), "Protected does not match"
-    assert (upload_res.retentionPeriod == 100), "Retention does not match"
+    assert (upload_res.options.protected is False), "Protected does not match"
+    assert (upload_res.options.retentionPeriod == 100), "Retention does not match"
 
 
 def test_upload_buffer_error(mocker):
+    # Given
     mock_put = mocker.patch('requests.put', return_value = bad_request)
     with open("tests/testfile.png", "rb") as fh:
         buf = io.BytesIO(fh.read())
+
+    # When
     upload_file = waifuvault.FileUpload(buf, "testfile_buf.png", expires="10m")
+
+    # Then
     with pytest.raises(Exception, match=re.escape('Error 400 (BAD_REQUEST): Error Test')):
         upload_res = waifuvault.upload_file(upload_file)
 
 
 def test_file_info(mocker):
+    # Given
     mock_get = mocker.patch('requests.get', return_value = ok_response_human)
+
+    # When
     upload_info = waifuvault.file_info("test-token",True)
+
+    # Then
     mock_get.assert_called_once_with(
         'https://waifuvault.moe/rest/test-token',
         params={'formatted': 'true'})
     assert (upload_info.url == "https://waifuvault.moe/f/something"), "URL does not match"
     assert (upload_info.token == "test-token"), "Token does not match"
-    assert (upload_info.protected is False), "Protected does not match"
-    assert (upload_info.retentionPeriod == "10 minutes"), "Retention does not match"
+    assert (upload_info.options.protected is False), "Protected does not match"
+    assert (upload_info.options.retentionPeriod == "10 minutes"), "Retention does not match"
 
 
 def test_file_info_error(mocker):
+    # When
     mock_get = mocker.patch('requests.get', return_value = bad_request)
+
+    # Then
     with pytest.raises(Exception, match=re.escape('Error 400 (BAD_REQUEST): Error Test')):
         upload_info = waifuvault.file_info("bad-token",True)
 
 
 def test_update_info(mocker):
+    # Given
     mock_patch = mocker.patch('requests.patch', return_value = ok_response_numeric_protected)
+
+    # When
     update_info = waifuvault.file_update("test-token","dangerWaifu")
+
+    # Then
     mock_patch.assert_called_once_with(
         'https://waifuvault.moe/rest/test-token',
         data={'password': 'dangerWaifu','hideFilename': 'false'})
     assert (update_info.url == "https://waifuvault.moe/f/something"), "URL does not match"
     assert (update_info.token == "test-token"), "Token does not match"
-    assert (update_info.protected is True), "Protected does not match"
-    assert (update_info.retentionPeriod == 100), "Retention does not match"
+    assert (update_info.options.protected is True), "Protected does not match"
+    assert (update_info.options.retentionPeriod == 100), "Retention does not match"
 
 
 def test_update_info_error(mocker):
+    # When
     mock_patch = mocker.patch('requests.patch', return_value = bad_request)
+
+    # Then
     with pytest.raises(Exception, match=re.escape('Error 400 (BAD_REQUEST): Error Test')):
         update_info = waifuvault.file_update("test-token","dangerWaifu")
 
 
 def test_delete(mocker):
+    # Given
     mock_del = mocker.patch('requests.delete',
         return_value=response_mock(True,
             'true'))
+
+    # When
     del_file = waifuvault.delete_file("test-token")
+
+    # Then
     mock_del.assert_called_once_with('https://waifuvault.moe/rest/test-token')
     assert (del_file is True), "Delete did not return true"
 
 
 def test_delete_error(mocker):
+    # When
     mock_del = mocker.patch('requests.delete', return_value = bad_request)
+
+    # Then
     with pytest.raises(Exception, match=re.escape('Error 400 (BAD_REQUEST): Error Test')):
         del_file = waifuvault.delete_file("test-token")
 
 
 def test_download(mocker):
+    # Given
     mock_get = mocker.patch('requests.get',return_value = response_mock(True,'', bytes("someval","utf8")))
+
+    # When
     file_down = waifuvault.get_file(waifuvault.FileResponse(url="https://waifuvault.moe/f/something"), "dangerWaifu")
+
+    # Then
     mock_get.assert_called_once_with('https://waifuvault.moe/f/something', headers={'x-password': 'dangerWaifu'})
     assert (isinstance(file_down, io.BytesIO)), "Download did not return a buffer"
 
 
 def test_download_error(mocker):
+    # When
     mock_get = mocker.patch('requests.get', return_value=bad_request)
+
+    # Then
     with pytest.raises(Exception, match=re.escape('Error 400 (BAD_REQUEST): Error Test')):
         file_down = waifuvault.get_file(waifuvault.FileResponse(url="https://waifuvault.moe/f/something"), "dangerWaifu")
```

