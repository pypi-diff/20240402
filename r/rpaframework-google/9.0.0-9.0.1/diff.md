# Comparing `tmp/rpaframework_google-9.0.0.tar.gz` & `tmp/rpaframework_google-9.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpaframework_google-9.0.0.tar", max compression
+gzip compressed data, was "rpaframework_google-9.0.1.tar", max compression
```

## Comparing `rpaframework_google-9.0.0.tar` & `rpaframework_google-9.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    11560 2023-12-05 08:21:31.327110 rpaframework_google-9.0.0/LICENSE
--rw-r--r--   0        0        0     2325 2024-03-14 19:01:43.253451 rpaframework_google-9.0.0/pyproject.toml
--rw-r--r--   0        0        0      209 2023-12-05 08:21:31.328097 rpaframework_google-9.0.0/README.rst
--rw-r--r--   0        0        0   149454 2024-03-14 19:03:28.661807 rpaframework_google-9.0.0/RPA_Cloud_Google.libspec
--rw-r--r--   0        0        0     5376 2024-03-14 19:01:43.254451 rpaframework_google-9.0.0/src/RPA/Cloud/Google/__init__.py
--rw-r--r--   0        0        0      858 2023-12-05 08:21:31.331605 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/__init__.py
--rw-r--r--   0        0        0     2742 2024-03-14 19:01:43.254451 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/apps_script.py
--rw-r--r--   0        0        0      931 2024-03-14 19:01:43.255451 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/base.py
--rw-r--r--   0        0        0    11076 2024-03-14 19:01:43.255451 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/context.py
--rw-r--r--   0        0        0    12028 2024-03-14 19:01:43.255451 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/document_ai.py
--rw-r--r--   0        0        0    41601 2024-03-14 19:01:43.256579 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/drive.py
--rw-r--r--   0        0        0     2830 2023-12-05 08:21:31.332610 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/enums.py
--rw-r--r--   0        0        0    13280 2024-03-14 19:01:43.256579 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/gmail.py
--rw-r--r--   0        0        0     4370 2024-03-14 19:01:43.256579 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/natural_language.py
--rw-r--r--   0        0        0    27128 2024-03-14 19:01:43.257594 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/sheets.py
--rw-r--r--   0        0        0     4071 2024-03-14 19:01:43.257594 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/speech_to_text.py
--rw-r--r--   0        0        0     8666 2024-03-14 19:01:43.257594 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/storage.py
--rw-r--r--   0        0        0     3522 2024-03-14 19:01:43.258593 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/text_to_speech.py
--rw-r--r--   0        0        0     2732 2024-03-14 19:01:43.258593 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/translation.py
--rw-r--r--   0        0        0     3887 2024-03-14 19:01:43.258593 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/video_intelligence.py
--rw-r--r--   0        0        0     5556 2024-03-14 19:01:43.258593 rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/vision.py
--rw-r--r--   0        0        0     3418 2023-12-05 08:21:31.335037 rpaframework_google-9.0.0/src/RPA/scripts/google_authenticate.py
--rw-r--r--   0        0        0     2210 1970-01-01 00:00:00.000000 rpaframework_google-9.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11560 2023-12-05 08:21:31.327110 rpaframework_google-9.0.1/LICENSE
+-rw-r--r--   0        0        0     2284 2024-04-02 11:26:45.812451 rpaframework_google-9.0.1/pyproject.toml
+-rw-r--r--   0        0        0      209 2023-12-05 08:21:31.328097 rpaframework_google-9.0.1/README.rst
+-rw-r--r--   0        0        0   149454 2024-04-02 11:28:24.254515 rpaframework_google-9.0.1/RPA_Cloud_Google.libspec
+-rw-r--r--   0        0        0     5376 2024-03-14 19:01:43.254451 rpaframework_google-9.0.1/src/RPA/Cloud/Google/__init__.py
+-rw-r--r--   0        0        0      858 2023-12-05 08:21:31.331605 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/__init__.py
+-rw-r--r--   0        0        0     2742 2024-03-14 19:01:43.254451 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/apps_script.py
+-rw-r--r--   0        0        0      931 2024-03-14 19:01:43.255451 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/base.py
+-rw-r--r--   0        0        0    11076 2024-03-14 19:01:43.255451 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/context.py
+-rw-r--r--   0        0        0    12028 2024-03-14 19:01:43.255451 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/document_ai.py
+-rw-r--r--   0        0        0    41601 2024-03-14 19:01:43.256579 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/drive.py
+-rw-r--r--   0        0        0     2830 2023-12-05 08:21:31.332610 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/enums.py
+-rw-r--r--   0        0        0    13280 2024-03-14 19:01:43.256579 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/gmail.py
+-rw-r--r--   0        0        0     4370 2024-03-14 19:01:43.256579 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/natural_language.py
+-rw-r--r--   0        0        0    27128 2024-03-14 19:01:43.257594 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/sheets.py
+-rw-r--r--   0        0        0     4071 2024-03-14 19:01:43.257594 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/speech_to_text.py
+-rw-r--r--   0        0        0     8666 2024-03-14 19:01:43.257594 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/storage.py
+-rw-r--r--   0        0        0     3522 2024-03-14 19:01:43.258593 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/text_to_speech.py
+-rw-r--r--   0        0        0     2732 2024-03-14 19:01:43.258593 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/translation.py
+-rw-r--r--   0        0        0     3887 2024-03-14 19:01:43.258593 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/video_intelligence.py
+-rw-r--r--   0        0        0     5556 2024-03-14 19:01:43.258593 rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/vision.py
+-rw-r--r--   0        0        0     3418 2023-12-05 08:21:31.335037 rpaframework_google-9.0.1/src/RPA/scripts/google_authenticate.py
+-rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 rpaframework_google-9.0.1/PKG-INFO
```

### Comparing `rpaframework_google-9.0.0/LICENSE` & `rpaframework_google-9.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/pyproject.toml` & `rpaframework_google-9.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpaframework-google"
-version = "9.0.0"
+version = "9.0.1"
 description = "Google library for RPA Framework"
 authors = ["RPA Framework <rpafw@robocorp.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 
 homepage = "https://rpaframework.org/"
 documentation = "https://rpaframework.org/"
@@ -27,17 +27,16 @@
 
 include = ["*.libspec"]
 
 packages = [{ include = "RPA", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-rpaframework-core = "^11.0.0"
+rpaframework-core = "^11.3.1"
 robotframework = ">=4.0.0,!=4.0.1,!=6.1.0,<7.0.0"
-robotframework-pythonlibcore = "^4.2.0"
 google-api-python-client = "^2.58.0"
 google-auth-httplib2 = "^0.1.0"
 google-auth-oauthlib = "^0.5.2"
 google-cloud-language = "^2.5.2"
 google-cloud-speech = "^2.15.1"
 google-cloud-storage = "^2.5.0"
 google-cloud-texttospeech = "^2.12.1"
```

### Comparing `rpaframework_google-9.0.0/RPA_Cloud_Google.libspec` & `rpaframework_google-9.0.1/RPA_Cloud_Google.libspec`

 * *Files 0% similar despite different names*

#### Comparing `rpaframework_google-9.0.0/RPA_Cloud_Google.libspec` & `rpaframework_google-9.0.1/RPA_Cloud_Google.libspec`

```diff
@@ -1,9 +1,9 @@
 <?xml version="1.0" encoding="utf-8"?>
-<keywordspec name="RPA.Cloud.Google" type="LIBRARY" format="REST" scope="GLOBAL" generated="2024-03-14T19:03:29+00:00" specversion="5" source="./RPA/Cloud/Google/__init__.py" lineno="33">
+<keywordspec name="RPA.Cloud.Google" type="LIBRARY" format="REST" scope="GLOBAL" generated="2024-04-02T11:28:24+00:00" specversion="5" source="./RPA/Cloud/Google/__init__.py" lineno="33">
   <version/>
   <doc>`Google` is a library for operating with Google API endpoints.
 
 **Installation**
 
 Usage requires the following steps:
```

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/__init__.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/__init__.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/__init__.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/__init__.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/apps_script.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/apps_script.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/base.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/base.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/context.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/context.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/document_ai.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/document_ai.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/drive.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/drive.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/enums.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/enums.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/gmail.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/gmail.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/natural_language.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/natural_language.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/sheets.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/sheets.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/speech_to_text.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/speech_to_text.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/storage.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/storage.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/text_to_speech.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/text_to_speech.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/translation.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/translation.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/video_intelligence.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/video_intelligence.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/Cloud/Google/keywords/vision.py` & `rpaframework_google-9.0.1/src/RPA/Cloud/Google/keywords/vision.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/src/RPA/scripts/google_authenticate.py` & `rpaframework_google-9.0.1/src/RPA/scripts/google_authenticate.py`

 * *Files identical despite different names*

### Comparing `rpaframework_google-9.0.0/PKG-INFO` & `rpaframework_google-9.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpaframework-google
-Version: 9.0.0
+Version: 9.0.1
 Summary: Google library for RPA Framework
 Home-page: https://rpaframework.org/
 License: Apache-2.0
 Keywords: robotframework,rpa,automation,google
 Author: RPA Framework
 Author-email: rpafw@robocorp.com
 Requires-Python: >=3.8,<4.0
@@ -31,16 +31,15 @@
 Requires-Dist: google-cloud-storage (>=2.5.0,<3.0.0)
 Requires-Dist: google-cloud-texttospeech (>=2.12.1,<3.0.0)
 Requires-Dist: google-cloud-translate (>=3.8.1,<4.0.0)
 Requires-Dist: google-cloud-videointelligence (>=2.8.1,<3.0.0)
 Requires-Dist: google-cloud-vision (>=3.1.1,<4.0.0)
 Requires-Dist: grpcio (>=1.48.1,<2.0.0)
 Requires-Dist: robotframework (>=4.0.0,!=4.0.1,!=6.1.0,<7.0.0)
-Requires-Dist: robotframework-pythonlibcore (>=4.2.0,<5.0.0)
-Requires-Dist: rpaframework-core (>=11.0.0,<12.0.0)
+Requires-Dist: rpaframework-core (>=11.3.1,<12.0.0)
 Project-URL: Documentation, https://rpaframework.org/
 Project-URL: Repository, https://github.com/robocorp/rpaframework
 Description-Content-Type: text/x-rst
 
 rpaframework-google
 ===================
```

