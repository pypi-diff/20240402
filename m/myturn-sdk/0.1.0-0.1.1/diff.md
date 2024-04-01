# Comparing `tmp/myturn-sdk-0.1.0.tar.gz` & `tmp/myturn-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myturn-sdk-0.1.0.tar", last modified: Tue Feb 27 11:20:04 2024, max compression
+gzip compressed data, was "myturn-sdk-0.1.1.tar", last modified: Mon Apr  1 23:10:59 2024, max compression
```

## Comparing `myturn-sdk-0.1.0.tar` & `myturn-sdk-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:20:04.949706 myturn-sdk-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:20:04.941706 myturn-sdk-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:20:04.945706 myturn-sdk-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:20:04.945706 myturn-sdk-0.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-02-27 11:20:04.949706 myturn-sdk-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-02-27 11:20:04.949706 myturn-sdk-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:20:04.941706 myturn-sdk-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:20:04.945706 myturn-sdk-0.1.0/src/myturn_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/browser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:20:04.949706 myturn-sdk-0.1.0/src/myturn_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/models/address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/models/login_result.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/models/opening_hours.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/models/opening_hours_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/models/opening_times.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/models/response_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/models/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/models/user_search_request.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/models/user_search_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/myturn_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/myturn_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/myturn_my_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/myturn_public_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/myturn_service_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/src/myturn_sdk/myturn_users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:20:04.949706 myturn-sdk-0.1.0/src/myturn_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-02-27 11:20:04.000000 myturn-sdk-0.1.0/src/myturn_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-02-27 11:20:04.000000 myturn-sdk-0.1.0/src/myturn_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 11:20:04.000000 myturn-sdk-0.1.0/src/myturn_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-27 11:20:04.000000 myturn-sdk-0.1.0/src/myturn_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-02-27 11:20:04.000000 myturn-sdk-0.1.0/src/myturn_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 11:20:04.949706 myturn-sdk-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/tests/browser_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/tests/myturn_my_account_unit_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4799 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/tests/myturn_public_info_integration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-02-27 11:19:58.000000 myturn-sdk-0.1.0/tests/myturn_users_integration_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:10:59.651938 myturn-sdk-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:10:59.643937 myturn-sdk-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:10:59.643937 myturn-sdk-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:10:59.643937 myturn-sdk-0.1.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-01 23:10:59.651938 myturn-sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-01 23:10:59.651938 myturn-sdk-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:10:59.643937 myturn-sdk-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:10:59.647938 myturn-sdk-0.1.1/src/myturn_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7948 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/browser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:10:59.647938 myturn-sdk-0.1.1/src/myturn_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/inventory_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/inventory_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/inventory_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/login_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/opening_hours.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/opening_hours_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/opening_times.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/response_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/user_search_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/models/user_search_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/myturn_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/myturn_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/myturn_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/myturn_my_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/myturn_public_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/myturn_service_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/src/myturn_sdk/myturn_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:10:59.651938 myturn-sdk-0.1.1/src/myturn_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-01 23:10:59.000000 myturn-sdk-0.1.1/src/myturn_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-01 23:10:59.000000 myturn-sdk-0.1.1/src/myturn_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 23:10:59.000000 myturn-sdk-0.1.1/src/myturn_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-01 23:10:59.000000 myturn-sdk-0.1.1/src/myturn_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-01 23:10:59.000000 myturn-sdk-0.1.1/src/myturn_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 23:10:59.651938 myturn-sdk-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/tests/browser_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/tests/myturn_inventory_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/tests/myturn_my_account_unit_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/tests/myturn_public_info_integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6207 2024-04-01 23:10:53.000000 myturn-sdk-0.1.1/tests/myturn_users_integration_test.py
```

### Comparing `myturn-sdk-0.1.0/.gitignore` & `myturn-sdk-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/LICENSE` & `myturn-sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/PKG-INFO` & `myturn-sdk-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myturn-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: An SDK for the MyTurn website.  Selenium based as there is no REST API.
 Home-page: https://github.com/aweddle2/myturn-sdk
 Project-URL: Bug Tracker, https://github.com/aweddle2/myturn-sdk/issues
 Project-URL: Changelog, https://github.com/aweddle2/myturn-sdk/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `myturn-sdk-0.1.0/README.md` & `myturn-sdk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/setup.cfg` & `myturn-sdk-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/src/myturn_sdk/browser.py` & `myturn-sdk-0.1.1/src/myturn_sdk/browser.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from selenium.webdriver.support.ui import WebDriverWait, Select
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.common.exceptions import NoSuchElementException
 import os
 import time
 import sys
 from seleniumrequests import Chrome
+import glob
 
 # Fixed to Chrome just now, but there this could be refactored to support any Selenium Browser
 
 
 class Browser():
     _scriptdir = os.path.dirname(os.path.realpath(sys.argv[0])) + os.sep
     _webdriver: webdriver
@@ -60,14 +61,21 @@
         self.get(url)
         # wait for file to finish downloading
         while not os.path.exists(self._scriptdir+os.sep+filename) or os.path.exists(self._scriptdir+os.sep+filename+'.crdownload'):
             time.sleep(1)
         # return the open file
         return open(self._scriptdir+os.sep+filename, encoding="utf8")
 
+    def openLastDownloadedFile(self):
+        # get last filename
+        list_of_files = glob.glob(self._scriptdir+'*')
+        latest_file = max(list_of_files, key=os.path.getctime)
+        # return the open file
+        return open(latest_file, encoding="utf8")
+
     def deleteDownload(self, filename: str):
         if os.path.exists(self._scriptdir+os.sep+filename):
             os.remove(self._scriptdir+os.sep+filename)
 
     def get(self, url: str):
         return self._webdriver.get(url)
```

### Comparing `myturn-sdk-0.1.0/src/myturn_sdk/models/opening_hours.py` & `myturn-sdk-0.1.1/src/myturn_sdk/models/opening_hours.py`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/src/myturn_sdk/models/user.py` & `myturn-sdk-0.1.1/src/myturn_sdk/models/user.py`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/src/myturn_sdk/myturn_authenticator.py` & `myturn-sdk-0.1.1/src/myturn_sdk/myturn_authenticator.py`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/src/myturn_sdk/myturn_client.py` & `myturn-sdk-0.1.1/src/myturn_sdk/myturn_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from .browser import Browser
 from .myturn_users import MyTurnUsers
 from .myturn_my_account import MyTurnMyAccount
 from .myturn_public_info import MyTurnPublicInfo
 from .myturn_authenticator import MyTurnAuthenticator
+from .myturn_inventory import MyTurnInventory
 
 
 class MyTurnClient():
     users: MyTurnUsers
     myAccount: MyTurnMyAccount
     publicInfo: MyTurnPublicInfo
+    inventory: MyTurnInventory
 
     def __init__(self, myturnSubDomain: str, username: str, password: str, headless: bool = True):
         libraryUrl = 'https://'+myturnSubDomain+'.myturn.com/library/'
         browser = Browser(headless)
         authenticator = MyTurnAuthenticator(
             libraryUrl, browser, username, password)
 
         self.users = MyTurnUsers(libraryUrl, browser, authenticator)
         self.myAccount = MyTurnMyAccount(libraryUrl, browser, authenticator)
         self.publicInfo = MyTurnPublicInfo(libraryUrl, browser)
+        self.inventory = MyTurnInventory(libraryUrl, browser, authenticator)
```

### Comparing `myturn-sdk-0.1.0/src/myturn_sdk/myturn_my_account.py` & `myturn-sdk-0.1.1/src/myturn_sdk/myturn_my_account.py`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/src/myturn_sdk/myturn_public_info.py` & `myturn-sdk-0.1.1/src/myturn_sdk/myturn_public_info.py`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/src/myturn_sdk/myturn_service_base.py` & `myturn-sdk-0.1.1/src/myturn_sdk/myturn_service_base.py`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/src/myturn_sdk/myturn_users.py` & `myturn-sdk-0.1.1/src/myturn_sdk/myturn_users.py`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/src/myturn_sdk.egg-info/PKG-INFO` & `myturn-sdk-0.1.1/src/myturn_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myturn-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: An SDK for the MyTurn website.  Selenium based as there is no REST API.
 Home-page: https://github.com/aweddle2/myturn-sdk
 Project-URL: Bug Tracker, https://github.com/aweddle2/myturn-sdk/issues
 Project-URL: Changelog, https://github.com/aweddle2/myturn-sdk/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

### Comparing `myturn-sdk-0.1.0/src/myturn_sdk.egg-info/SOURCES.txt` & `myturn-sdk-0.1.1/src/myturn_sdk.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -6,30 +6,35 @@
 setup.cfg
 .github/workflows/publish.yml
 .vscode/settings.json
 src/myturn_sdk/__init__.py
 src/myturn_sdk/browser.py
 src/myturn_sdk/myturn_authenticator.py
 src/myturn_sdk/myturn_client.py
+src/myturn_sdk/myturn_inventory.py
 src/myturn_sdk/myturn_my_account.py
 src/myturn_sdk/myturn_public_info.py
 src/myturn_sdk/myturn_service_base.py
 src/myturn_sdk/myturn_users.py
 src/myturn_sdk.egg-info/PKG-INFO
 src/myturn_sdk.egg-info/SOURCES.txt
 src/myturn_sdk.egg-info/dependency_links.txt
 src/myturn_sdk.egg-info/entry_points.txt
 src/myturn_sdk.egg-info/top_level.txt
 src/myturn_sdk/models/__init__.py
 src/myturn_sdk/models/address_response.py
+src/myturn_sdk/models/inventory_item.py
+src/myturn_sdk/models/inventory_search_request.py
+src/myturn_sdk/models/inventory_search_response.py
 src/myturn_sdk/models/login_result.py
 src/myturn_sdk/models/opening_hours.py
 src/myturn_sdk/models/opening_hours_response.py
 src/myturn_sdk/models/opening_times.py
 src/myturn_sdk/models/response_base.py
 src/myturn_sdk/models/user.py
 src/myturn_sdk/models/user_search_request.py
 src/myturn_sdk/models/user_search_response.py
 tests/browser_integration_test.py
+tests/myturn_inventory_integration_test.py
 tests/myturn_my_account_unit_test.py
 tests/myturn_public_info_integration_test.py
 tests/myturn_users_integration_test.py
```

### Comparing `myturn-sdk-0.1.0/tests/browser_integration_test.py` & `myturn-sdk-0.1.1/tests/browser_integration_test.py`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/tests/myturn_my_account_unit_test.py` & `myturn-sdk-0.1.1/tests/myturn_my_account_unit_test.py`

 * *Files identical despite different names*

### Comparing `myturn-sdk-0.1.0/tests/myturn_public_info_integration_test.py` & `myturn-sdk-0.1.1/tests/myturn_public_info_integration_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,16 +32,16 @@
         self.assertEqual(result.thursday.dayName, 'Thursday')
         self.assertEqual(result.friday.openTime, None)
         self.assertEqual(result.friday.closeTime, None)
         self.assertEqual(result.friday.dayName, 'Friday')
         self.assertEqual(result.saturday.openTime.hour, 10)
         self.assertEqual(result.saturday.closeTime.hour, 14)
         self.assertEqual(result.saturday.dayName, 'Saturday')
-        self.assertEqual(result.sunday.openTime.hour, 11)
-        self.assertEqual(result.sunday.closeTime.hour, 13)
+        self.assertEqual(result.sunday.openTime, None)
+        self.assertEqual(result.sunday.closeTime, None)
         self.assertEqual(result.sunday.dayName, 'Sunday')
 
     def test_ballarat_opening_hours(self):
         # Arrange
         myTurnClient = MyTurnClient(
             "ballarattoollibrary", None, None)
```

### Comparing `myturn-sdk-0.1.0/tests/myturn_users_integration_test.py` & `myturn-sdk-0.1.1/tests/myturn_users_integration_test.py`

 * *Files identical despite different names*

