# Comparing `tmp/ta_sites-0.4.8.tar.gz` & `tmp/ta_sites-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-1en9g_7n/ta_sites-0.4.8.tar", last modified: Tue Sep  5 15:32:42 2023, max compression
+gzip compressed data, was "/opt/atlassian/pipelines/agent/build/dist/.tmp-6jfo6w0z/ta_sites-0.4.9.tar", last modified: Wed Sep 27 16:39:57 2023, max compression
```

## Comparing `ta_sites-0.4.8.tar` & `ta_sites-0.4.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-05 15:32:42.882099 ta_sites-0.4.8/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-09-05 15:32:22.000000 ta_sites-0.4.8/AUTHORS.rst
--rw-rw-rw-   0 root         (0) root         (0)     1095 2023-09-05 15:32:22.000000 ta_sites-0.4.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-09-05 15:32:42.882099 ta_sites-0.4.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-09-05 15:32:22.000000 ta_sites-0.4.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      307 2023-09-05 15:32:42.882099 ta_sites-0.4.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1056 2023-09-05 15:32:22.000000 ta_sites-0.4.8/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-05 15:32:42.878099 ta_sites-0.4.8/ta_sites/
--rw-rw-rw-   0 root         (0) root         (0)      602 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-05 15:32:42.878099 ta_sites-0.4.8/ta_sites/always_care/
--rw-rw-rw-   0 root         (0) root         (0)      269 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/always_care/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      152 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/always_care/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     9569 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/always_care/requests_core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-05 15:32:42.878099 ta_sites-0.4.8/ta_sites/basic/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/basic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4304 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/basic/core.py
--rw-rw-rw-   0 root         (0) root         (0)      340 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/basic/exceptions.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-05 15:32:42.882099 ta_sites-0.4.8/ta_sites/central_reach/
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/central_reach/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17161 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/central_reach/core.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/central_reach/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10146 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/central_reach/requests_core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-05 15:32:42.882099 ta_sites-0.4.8/ta_sites/quickbooks/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/quickbooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25676 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/quickbooks/core.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/quickbooks/grouped_row.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-05 15:32:42.882099 ta_sites-0.4.8/ta_sites/salesforce/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/salesforce/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2656 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/salesforce/core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-05 15:32:42.882099 ta_sites-0.4.8/ta_sites/versant/
--rw-rw-rw-   0 root         (0) root         (0)      199 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/versant/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/versant/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)    10568 2023-09-05 15:32:22.000000 ta_sites-0.4.8/ta_sites/versant/requests_core.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-05 15:32:42.878099 ta_sites-0.4.8/ta_sites.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)      805 2023-09-05 15:32:42.000000 ta_sites-0.4.8/ta_sites.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-09-05 15:32:42.000000 ta_sites-0.4.8/ta_sites.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-09-05 15:32:42.000000 ta_sites-0.4.8/ta_sites.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-09-05 15:32:42.000000 ta_sites-0.4.8/ta_sites.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-09-05 15:32:42.000000 ta_sites-0.4.8/ta_sites.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-09-05 15:32:42.000000 ta_sites-0.4.8/ta_sites.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-27 16:39:57.282517 ta_sites-0.4.9/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-09-27 16:39:35.000000 ta_sites-0.4.9/AUTHORS.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1095 2023-09-27 16:39:35.000000 ta_sites-0.4.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      874 2023-09-27 16:39:57.282517 ta_sites-0.4.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-09-27 16:39:35.000000 ta_sites-0.4.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-09-27 16:39:57.282517 ta_sites-0.4.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2023-09-27 16:39:35.000000 ta_sites-0.4.9/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-27 16:39:57.278517 ta_sites-0.4.9/ta_sites/
+-rw-rw-rw-   0 root         (0) root         (0)      602 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-27 16:39:57.278517 ta_sites-0.4.9/ta_sites/always_care/
+-rw-rw-rw-   0 root         (0) root         (0)      269 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/always_care/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      152 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/always_care/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     9569 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/always_care/requests_core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-27 16:39:57.278517 ta_sites-0.4.9/ta_sites/basic/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/basic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4304 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/basic/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      340 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/basic/exceptions.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-27 16:39:57.278517 ta_sites-0.4.9/ta_sites/central_reach/
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/central_reach/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17104 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/central_reach/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/central_reach/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10188 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/central_reach/requests_core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-27 16:39:57.282517 ta_sites-0.4.9/ta_sites/quickbooks/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/quickbooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25676 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/quickbooks/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/quickbooks/grouped_row.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-27 16:39:57.282517 ta_sites-0.4.9/ta_sites/salesforce/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/salesforce/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/salesforce/core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-27 16:39:57.282517 ta_sites-0.4.9/ta_sites/versant/
+-rw-rw-rw-   0 root         (0) root         (0)      199 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/versant/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/versant/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)    10568 2023-09-27 16:39:35.000000 ta_sites-0.4.9/ta_sites/versant/requests_core.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-09-27 16:39:57.278517 ta_sites-0.4.9/ta_sites.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      874 2023-09-27 16:39:57.000000 ta_sites-0.4.9/ta_sites.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-09-27 16:39:57.000000 ta_sites-0.4.9/ta_sites.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-09-27 16:39:57.000000 ta_sites-0.4.9/ta_sites.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-09-27 16:39:57.000000 ta_sites-0.4.9/ta_sites.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-09-27 16:39:57.000000 ta_sites-0.4.9/ta_sites.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-09-27 16:39:57.000000 ta_sites-0.4.9/ta_sites.egg-info/top_level.txt
```

### Comparing `ta_sites-0.4.8/LICENSE` & `ta_sites-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.8/PKG-INFO` & `ta_sites-0.4.9/ta_sites.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
-Name: ta_sites
-Version: 0.4.8
+Name: ta-sites
+Version: 0.4.9
 Summary: TA Sites
 Home-page: https://www.thoughtfulautomation.com/
 Author: Serhii Romanets
 Author-email: serhii.romanets@thoughtful.ai
 Keywords: ta_sites
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: requests
+Requires-Dist: datetime
+Requires-Dist: retry
 
 # ta-sites
 [![pip version](https://img.shields.io/pypi/v/ta-sites.svg)](https://pypi.python.org/pypi/ta-sites)
 
 Thoughtful Automation sites package. This package contains the function required for Thoughtful Automation bots. Documentation may be closed and certain functions may not work outside the Thoughtful Automation environment.
 
 Example Usage
```

### Comparing `ta_sites-0.4.8/setup.py` & `ta_sites-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup_args = dict(
     name="ta_sites",
-    version="0.4.8",
+    version="0.4.9",
     packages=[
         "ta_sites",
         "ta_sites.central_reach",
         "ta_sites.basic",
         "ta_sites.quickbooks",
         "ta_sites.salesforce",
         "ta_sites.versant",
```

### Comparing `ta_sites-0.4.8/ta_sites/__init__.py` & `ta_sites-0.4.9/ta_sites/__init__.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.8/ta_sites/always_care/requests_core.py` & `ta_sites-0.4.9/ta_sites/always_care/requests_core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.8/ta_sites/basic/core.py` & `ta_sites-0.4.9/ta_sites/basic/core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.8/ta_sites/central_reach/__init__.py` & `ta_sites-0.4.9/ta_sites/central_reach/__init__.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.8/ta_sites/central_reach/core.py` & `ta_sites-0.4.9/ta_sites/central_reach/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
             os.mkdir(self.temp_folder)
             self.browser.set_download_directory(self.temp_folder, True)
 
         for i in range(1, 4):
             try:
                 self.browser.open_chrome_browser(self.url, headless=self._headless)
                 self.browser.set_window_size(1920, 1080)
-                # self.browser.maximize_browser_window()
 
                 self.wait_element('//input[@type="password"]', is_need_screenshot=False, timeout=10)
 
                 self.check_scheduled_maintenance()
 
                 self.wait_element('//input[@type="password"]')
                 self.browser.input_text_when_element_is_visible('//input[@type="text"]', self.login)
```

### Comparing `ta_sites-0.4.8/ta_sites/central_reach/exceptions.py` & `ta_sites-0.4.9/ta_sites/central_reach/exceptions.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.8/ta_sites/central_reach/requests_core.py` & `ta_sites-0.4.9/ta_sites/central_reach/requests_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
                     f"{exc_message}Status Code: {response.status_code}, " f"Headers: {response.headers}"
                 )
 
     @retry_if_bad_request
     def _login_to_central_reach(self, login: str, password: str) -> None:
         central_reach_core = CentralReachCore(login, password, headless=True)
         central_reach_core.login_to_site()
+        self.session = requests.session()
 
         # Check authorisation
         timeout_time = datetime.datetime.now() + datetime.timedelta(seconds=30)
         while datetime.datetime.now() < timeout_time:
             try:
                 # Set cookies
                 for name, value in central_reach_core.browser.get_cookies(as_dict=True).items():
```

### Comparing `ta_sites-0.4.8/ta_sites/quickbooks/core.py` & `ta_sites-0.4.9/ta_sites/quickbooks/core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.8/ta_sites/quickbooks/grouped_row.py` & `ta_sites-0.4.9/ta_sites/quickbooks/grouped_row.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.8/ta_sites/salesforce/core.py` & `ta_sites-0.4.9/ta_sites/salesforce/core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.8/ta_sites/versant/requests_core.py` & `ta_sites-0.4.9/ta_sites/versant/requests_core.py`

 * *Files identical despite different names*

### Comparing `ta_sites-0.4.8/ta_sites.egg-info/PKG-INFO` & `ta_sites-0.4.9/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
-Name: ta-sites
-Version: 0.4.8
+Name: ta_sites
+Version: 0.4.9
 Summary: TA Sites
 Home-page: https://www.thoughtfulautomation.com/
 Author: Serhii Romanets
 Author-email: serhii.romanets@thoughtful.ai
 Keywords: ta_sites
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
+Requires-Dist: requests
+Requires-Dist: datetime
+Requires-Dist: retry
 
 # ta-sites
 [![pip version](https://img.shields.io/pypi/v/ta-sites.svg)](https://pypi.python.org/pypi/ta-sites)
 
 Thoughtful Automation sites package. This package contains the function required for Thoughtful Automation bots. Documentation may be closed and certain functions may not work outside the Thoughtful Automation environment.
 
 Example Usage
```

### Comparing `ta_sites-0.4.8/ta_sites.egg-info/SOURCES.txt` & `ta_sites-0.4.9/ta_sites.egg-info/SOURCES.txt`

 * *Files identical despite different names*

