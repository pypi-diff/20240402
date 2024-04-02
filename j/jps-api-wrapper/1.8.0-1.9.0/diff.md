# Comparing `tmp/jps_api_wrapper-1.8.0.tar.gz` & `tmp/jps_api_wrapper-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jps_api_wrapper-1.8.0.tar", last modified: Tue Aug  8 15:05:31 2023, max compression
+gzip compressed data, was "jps_api_wrapper-1.9.0.tar", last modified: Wed Sep  6 00:05:53 2023, max compression
```

## Comparing `jps_api_wrapper-1.8.0.tar` & `jps_api_wrapper-1.9.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:05:31.481794 jps_api_wrapper-1.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-07-20 17:34:54.000000 jps_api_wrapper-1.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8112 2023-08-08 15:05:31.481794 jps_api_wrapper-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6635 2023-07-20 17:34:54.000000 jps_api_wrapper-1.8.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-20 17:34:54.000000 jps_api_wrapper-1.8.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-08-08 15:05:31.482794 jps_api_wrapper-1.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:05:31.477794 jps_api_wrapper-1.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:05:31.479794 jps_api_wrapper-1.8.0/src/jps_api_wrapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-08 15:05:04.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   262861 2023-07-20 17:34:54.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper/classic.py
--rw-rw-rw-   0 root         (0) root         (0)   324202 2023-08-08 14:46:46.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper/pro.py
--rw-rw-rw-   0 root         (0) root         (0)    13172 2023-07-20 17:34:54.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper/request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     6752 2023-08-08 14:53:58.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:05:31.480794 jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8112 2023-08-08 15:05:31.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      454 2023-08-08 15:05:31.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-08 15:05:31.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-08-08 15:05:31.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-08-08 15:05:31.000000 jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-08 15:05:31.481794 jps_api_wrapper-1.8.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)   290397 2023-07-20 17:34:54.000000 jps_api_wrapper-1.8.0/tests/test_classic.py
--rw-rw-rw-   0 root         (0) root         (0)   216898 2023-08-08 14:46:46.000000 jps_api_wrapper-1.8.0/tests/test_pro.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 00:05:53.692927 jps_api_wrapper-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-09-05 23:56:49.000000 jps_api_wrapper-1.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8908 2023-09-06 00:05:53.692927 jps_api_wrapper-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     7431 2023-09-05 23:56:49.000000 jps_api_wrapper-1.9.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-09-05 23:56:49.000000 jps_api_wrapper-1.9.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-09-06 00:05:53.694927 jps_api_wrapper-1.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 00:05:53.688927 jps_api_wrapper-1.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 00:05:53.690927 jps_api_wrapper-1.9.0/src/jps_api_wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-06 00:05:26.000000 jps_api_wrapper-1.9.0/src/jps_api_wrapper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   262883 2023-09-05 23:56:49.000000 jps_api_wrapper-1.9.0/src/jps_api_wrapper/classic.py
+-rw-rw-rw-   0 root         (0) root         (0)   327347 2023-09-05 23:56:49.000000 jps_api_wrapper-1.9.0/src/jps_api_wrapper/pro.py
+-rw-rw-rw-   0 root         (0) root         (0)    13288 2023-09-05 23:56:49.000000 jps_api_wrapper-1.9.0/src/jps_api_wrapper/request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     6752 2023-09-05 23:56:49.000000 jps_api_wrapper-1.9.0/src/jps_api_wrapper/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 00:05:53.691927 jps_api_wrapper-1.9.0/src/jps_api_wrapper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8908 2023-09-06 00:05:53.000000 jps_api_wrapper-1.9.0/src/jps_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      454 2023-09-06 00:05:53.000000 jps_api_wrapper-1.9.0/src/jps_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-09-06 00:05:53.000000 jps_api_wrapper-1.9.0/src/jps_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-09-06 00:05:53.000000 jps_api_wrapper-1.9.0/src/jps_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-09-06 00:05:53.000000 jps_api_wrapper-1.9.0/src/jps_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-06 00:05:53.692927 jps_api_wrapper-1.9.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   290397 2023-09-05 23:56:49.000000 jps_api_wrapper-1.9.0/tests/test_classic.py
+-rw-rw-rw-   0 root         (0) root         (0)   218918 2023-09-05 23:56:49.000000 jps_api_wrapper-1.9.0/tests/test_pro.py
```

### Comparing `jps_api_wrapper-1.8.0/LICENSE` & `jps_api_wrapper-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.8.0/PKG-INFO` & `jps_api_wrapper-1.9.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jps_api_wrapper
-Version: 1.8.0
+Version: 1.9.0
 Summary: Jamf Pro Server API Python wrapper
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
@@ -24,14 +24,15 @@
 ## Table of Contents
 
 - [JPS (Jamf Pro Server) API Wrapper](#jps-jamf-pro-server-api-wrapper)
   - [Table of Contents](#table-of-contents)
   - [Background](#background)
   - [Install](#install)
   - [Usage](#usage)
+  - [API Client Authentication](#api-client-authentication)
   - [Method Documentation](#method-documentation)
   - [Other Notes](#other-notes)
   - [Contributing](#contributing)
   - [License](#license)
 
 ## Background
 
@@ -81,14 +82,37 @@
 classic.session.auth.invalidate()
 ```
 
 Any methods that require the data param will have a link to Jamf's documentation in the docstring and the method documentation for the syntax of the data that the request expects.
 
 For some examples of jps-api-wrapper usage in real projects feel free to check out my other projects in our [GitLab](https://gitlab.com/cvtc/appleatcvtc).
 
+## API Client Authentication
+
+To authenticate using an API Client added with JPS 10.49 use the new client parameter when initializing a Classic or Pro method. This new parameter is set to False be default to not affect current deployments of the wrapper.
+
+
+```
+from jps_api_wrapper.classic import Classic
+from jps_api_wrapper.pro import Pro
+from os import environ
+
+JPS_URL = "https://example.jamfcloud.com"
+CLIENT_ID = environ["CLIENT_ID"]
+CLIENT_SECRET = environ["CLIENT_SECRET"]
+
+with Classic(JPS_URL, CLIENT_ID, CLIENT_SECRET, client=True) as classic:
+    print(classic.get_computers())
+    print(classic.get_computer(1001))
+
+with Pro(JPS_URL, CLIENT_ID, CLIENT_SECRET, client=True) as pro:
+    print(pro.get_mobile_devices())
+```
+
+
 ## Method Documentation
 
 View the [ReadTheDocs](https://jps-api-wrapper.readthedocs.io/en/stable/)
 
 The method documentation is meant to match [Jamf's API Reference](https://developer.jamf.com/jamf-pro/reference/classic-api) for easy navigation of functionality.
 
 ## Other Notes
```

### Comparing `jps_api_wrapper-1.8.0/README.md` & `jps_api_wrapper-1.9.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ## Table of Contents
 
 - [JPS (Jamf Pro Server) API Wrapper](#jps-jamf-pro-server-api-wrapper)
   - [Table of Contents](#table-of-contents)
   - [Background](#background)
   - [Install](#install)
   - [Usage](#usage)
+  - [API Client Authentication](#api-client-authentication)
   - [Method Documentation](#method-documentation)
   - [Other Notes](#other-notes)
   - [Contributing](#contributing)
   - [License](#license)
 
 ## Background
 
@@ -68,14 +69,37 @@
 classic.session.auth.invalidate()
 ```
 
 Any methods that require the data param will have a link to Jamf's documentation in the docstring and the method documentation for the syntax of the data that the request expects.
 
 For some examples of jps-api-wrapper usage in real projects feel free to check out my other projects in our [GitLab](https://gitlab.com/cvtc/appleatcvtc).
 
+## API Client Authentication
+
+To authenticate using an API Client added with JPS 10.49 use the new client parameter when initializing a Classic or Pro method. This new parameter is set to False be default to not affect current deployments of the wrapper.
+
+
+```
+from jps_api_wrapper.classic import Classic
+from jps_api_wrapper.pro import Pro
+from os import environ
+
+JPS_URL = "https://example.jamfcloud.com"
+CLIENT_ID = environ["CLIENT_ID"]
+CLIENT_SECRET = environ["CLIENT_SECRET"]
+
+with Classic(JPS_URL, CLIENT_ID, CLIENT_SECRET, client=True) as classic:
+    print(classic.get_computers())
+    print(classic.get_computer(1001))
+
+with Pro(JPS_URL, CLIENT_ID, CLIENT_SECRET, client=True) as pro:
+    print(pro.get_mobile_devices())
+```
+
+
 ## Method Documentation
 
 View the [ReadTheDocs](https://jps-api-wrapper.readthedocs.io/en/stable/)
 
 The method documentation is meant to match [Jamf's API Reference](https://developer.jamf.com/jamf-pro/reference/classic-api) for easy navigation of functionality.
 
 ## Other Notes
```

### Comparing `jps_api_wrapper-1.8.0/setup.cfg` & `jps_api_wrapper-1.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jps_api_wrapper
-version = 1.8.0
+version = 1.9.0
 description = Jamf Pro Server API Python wrapper
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 readme = README.md
 license = MIT
 classifiers = 
 	License :: OSI Approved :: MIT License
```

### Comparing `jps_api_wrapper-1.8.0/src/jps_api_wrapper/classic.py` & `jps_api_wrapper-1.9.0/src/jps_api_wrapper/classic.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,16 @@
     valid_param_options,
     valid_subsets,
     validate_date,
 )
 
 
 class Classic(RequestBuilder):
-    def __init__(self, base_url, username, password):
-        super().__init__(base_url, username, password)  # pragma: no cover
+    def __init__(self, base_url, username, password, client=False):
+        super().__init__(base_url, username, password, client)  # pragma: no cover
 
     """
     /accounts
     """
 
     def get_accounts(self, data_type: str = "json") -> Union[dict, str]:
         """
```

### Comparing `jps_api_wrapper-1.8.0/src/jps_api_wrapper/pro.py` & `jps_api_wrapper-1.9.0/src/jps_api_wrapper/pro.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,16 @@
     remove_empty_params,
 )
 
 warnings.simplefilter("always", DeprecationWarning)
 
 
 class Pro(RequestBuilder):
-    def __init__(self, base_url, username, password):
-        super().__init__(base_url, username, password)  # pragma: no cover
+    def __init__(self, base_url, username, password, client=False):
+        super().__init__(base_url, username, password, client)  # pragma: no cover
 
     """
     advanced-mobile-device-searches
     """
 
     def get_advanced_mobile_device_searches(self) -> dict:
         """
@@ -1350,69 +1350,14 @@
         :returns:
             Cloud azure identity provider configuration information in JSON
         """
         endpoint = f"/api/v1/cloud-azure/{id}"
 
         return self._get(endpoint)
 
-    def get_cloud_azure_report(self, id: Union[int, str]):
-        """
-        Returns excel file of generated cloud azure report
-
-        :param id: Existing report ID
-
-        :returns: Cloud azure report excel file
-        """
-        headers = {
-            "accept": "application/vnd.openxmlformats-officedocument"
-            ".spreadsheetml.sheet",
-            "Content-type": "application/json",
-        }
-        endpoint = f"/api/v1/azure-ad-migration/reports/{id}/download"
-
-        return self._get(endpoint, headers=headers)
-
-    def get_cloud_azure_report_status(self, id: Union[int, str]) -> dict:
-        """
-        Returns status of Azure AD migration report
-
-        :param id: Existing report ID
-
-        :returns: Cloud azure report status information in JSON
-        """
-        endpoint = f"/api/v1/azure-ad-migration/reports/{id}"
-
-        return self._get(endpoint)
-
-    def get_cloud_azure_pending_report(self):
-        """
-        Returns info about pending report
-
-        :returns: Cloud azure pending report information in JSON
-        """
-        endpoint = "/api/v1/azure-ad-migration/reports/pending"
-
-        return self._get(endpoint)
-
-    def create_cloud_azure_report(self, data: dict) -> dict:
-        """
-        Starts a new process in background that will generate Excel report
-        with JSON data
-
-        :param data:
-            JSON data to create the report with. For syntax information view
-            `Jamf's documentation.
-            <https://developer.jamf.com/jamf-pro/reference/post_v1-azure-ad-migration-reports>`__
-
-        :returns: New cloud azure report information in JSON
-        """
-        endpoint = "/api/v1/azure-ad-migration/reports"
-
-        return self._post(endpoint, data)
-
     def create_cloud_azure_identity_provider_configuration(self, data: dict) -> dict:
         """
         Create new Azure Cloud Identity Provider configuration with unique
         display name
 
         :param data:
             JSON data to create the azure cloud identity provider configuration
@@ -5536,14 +5481,104 @@
         :returns: Managed software update statuses information in JSON
         """
         params = remove_empty_params({"filter": filter})
         endpoint = "/api/v1/managed-software-updates/update-statuses"
 
         return self._get(endpoint, params=params)
 
+    def get_managed_software_updates_plans(
+        self,
+        page: Union[int, str] = None,
+        page_size: int = None,
+        sort: List[str] = ["planUuid:asc"],
+        filter: str = None,
+    ) -> dict:
+        """
+        Returns managed software update plans
+
+        :param page: Page to return, default page is 0.
+        :param page_size: Page size to return, default page-size is 100.
+        :param sort:
+            Sorting criteria in the format: property:asc/desc. Default sort is
+            ["planUuid:asc"]. Multiple sort criteria are supported and must be
+            separated with a comma.
+
+            Example: ["planUuid:desc", "maxDeferrals:asc"]
+
+        :param filter:
+            Query in the RSQL format, allowing to filter Managed Software
+            Updates collection. Default filter is empty query - returning all
+            results for the requested page.
+
+            Options:
+            planUuid, device.deviceId, device.objectType, updateAction,
+            versionType, specificVersion, maxDeferrals.
+
+            Example: 'maxDeferrals >= 1 and versionType == "LATEST_ANY"'
+
+        :returns: Managed software update plans in JSON
+        """
+        params = remove_empty_params(
+            {
+                "page": page,
+                "page-size": page_size,
+                "sort": sort,
+                "filter": filter,
+            }
+        )
+        endpoint = "/api/v1/managed-software-updates/plans"
+
+        return self._get(endpoint, params=params)
+
+    def get_managed_software_updates_feature_toggle(self) -> dict:
+        """
+        Returns status of the managed software updates feature toggle
+
+        :returns: Status of the managed software updates feature toggle in JSON
+        """
+        endpoint = "/api/v1/managed-software-updates/plans/feature-toggle"
+
+        return self._get(endpoint)
+
+    def get_managed_software_updates_group_plans(
+        self,
+        id: Union[int, str],
+        group_type: str,
+    ) -> dict:
+        """
+        Returns managed software update plans for a group by ID
+
+        :param id: Managed software update group ID
+        :param group_type:
+            Managed software update group type
+
+            Options:
+            COMPUTER_GROUP, MOBILE_DEVICE_GROUP
+
+            Example: "COMPUTER_GROUP"
+
+        :returns: Managed software update plans for a group in JSON
+        """
+        params = {"group-type": group_type}
+        endpoint = f"/api/v1/managed-software-updates/plans/group/{id}"
+
+        return self._get(endpoint, params=params)
+
+    def get_managed_software_updates_plan(self, id: str) -> dict:
+        """
+        Returns a managed software update plan by UUID
+
+        :param id: Managed software update plan UUID
+
+        :returns: Managed software update plan in JSON
+        """
+        endpoint = f"/api/v1/managed-software-updates/plans/{id}"
+
+        return self._get(endpoint)
+
     def get_managed_software_updates_computer_group(self, id: Union[int, str]) -> dict:
         """
         Returns managed software update statuses for computer group by ID
 
         :param id: Computer group ID
 
         :returns:
@@ -5600,14 +5635,62 @@
         """
         endpoint = (
             f"/api/v1/managed-software-updates/update-statuses/mobile-devices/{id}"
         )
 
         return self._get(endpoint)
 
+    def create_managed_software_updates_plan(self, data: dict) -> dict:
+        """
+        Creates a managed software update plan with JSON data
+
+        :param data:
+            JSON data to create managed software update plan with. For syntax
+            information view `Jamf's documentation.
+            <https://developer.jamf.com/jamf-pro/reference/post_v1-managed-software-updates-plans>`__
+
+        :returns: New managed software update plan in JSON
+        """
+        endpoint = "/api/v1/managed-software-updates/plans"
+
+        return self._post(endpoint, data)
+
+    def create_managed_software_updates_group_plan(self, data: dict) -> dict:
+        """
+        Creates a managed software update plans for a group with JSON data
+
+        :param data:
+            JSON data to create managed software update plans for a group with.
+            For syntax information view `Jamf's documentation.
+            <https://developer.jamf.com/jamf-pro/reference/post_v1-managed-software-updates-plans-group>`__
+
+        :returns: New managed software update plans for the group in JSON
+        """
+        endpoint = "/api/v1/managed-software-updates/plans/group"
+
+        return self._post(endpoint, data)
+
+    def update_managed_software_updates_feature_toggle(self, data: dict) -> dict:
+        """
+        Updates the value of the feature toggle for managed software updates,
+        turning the feature on or off
+
+        :param data:
+            JSON data to update the managed software updates feature toggle
+            with. For syntax information view `Jamf's documentation.
+            <https://developer.jamf.com/jamf-pro/reference/put_v1-managed-software-updates-plans-feature-toggle>`__
+
+        :returns:
+            Updated status of the managed software update feature toggle status
+            in JSON
+        """
+        endpoint = "/api/v1/managed-software-updates/plans/feature-toggle"
+
+        return self._put(endpoint, data)
+
     """
     mdm
     """
 
     def get_mdm_commands(
         self,
         page: int = None,
```

### Comparing `jps_api_wrapper-1.8.0/src/jps_api_wrapper/request_builder.py` & `jps_api_wrapper-1.9.0/src/jps_api_wrapper/request_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,27 @@
     :param base_url:
         Base URL of the JPS server
         e.g. https://example.jamfcloud.com
     :param username:
         Username for the JPS instance
     :param password:
         Password for the JPS instance
+    :param client:
+        Whether or not the credentials are for an API client
 
     :raises InvalidDataType:
         data_type is not json or xml
     """
 
-    def __init__(self, base_url: str, username: str, password: str):  # pragma: no cover
+    def __init__(
+        self, base_url: str, username: str, password: str, client: bool
+    ):  # pragma: no cover
         self.base_url = base_url
         self.session = requests.Session()
-        self.session.auth = JamfAuth(self.base_url, username, password)
+        self.session.auth = JamfAuth(self.base_url, username, password, client)
 
     def __enter__(self):  # pragma: no cover
         self.session.auth.refresh_auth_if_needed()
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):  # pragma: no cover
         self.session.auth.invalidate()
```

### Comparing `jps_api_wrapper-1.8.0/src/jps_api_wrapper/utils.py` & `jps_api_wrapper-1.9.0/src/jps_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.8.0/src/jps_api_wrapper.egg-info/PKG-INFO` & `jps_api_wrapper-1.9.0/src/jps_api_wrapper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jps-api-wrapper
-Version: 1.8.0
+Version: 1.9.0
 Summary: Jamf Pro Server API Python wrapper
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
@@ -24,14 +24,15 @@
 ## Table of Contents
 
 - [JPS (Jamf Pro Server) API Wrapper](#jps-jamf-pro-server-api-wrapper)
   - [Table of Contents](#table-of-contents)
   - [Background](#background)
   - [Install](#install)
   - [Usage](#usage)
+  - [API Client Authentication](#api-client-authentication)
   - [Method Documentation](#method-documentation)
   - [Other Notes](#other-notes)
   - [Contributing](#contributing)
   - [License](#license)
 
 ## Background
 
@@ -81,14 +82,37 @@
 classic.session.auth.invalidate()
 ```
 
 Any methods that require the data param will have a link to Jamf's documentation in the docstring and the method documentation for the syntax of the data that the request expects.
 
 For some examples of jps-api-wrapper usage in real projects feel free to check out my other projects in our [GitLab](https://gitlab.com/cvtc/appleatcvtc).
 
+## API Client Authentication
+
+To authenticate using an API Client added with JPS 10.49 use the new client parameter when initializing a Classic or Pro method. This new parameter is set to False be default to not affect current deployments of the wrapper.
+
+
+```
+from jps_api_wrapper.classic import Classic
+from jps_api_wrapper.pro import Pro
+from os import environ
+
+JPS_URL = "https://example.jamfcloud.com"
+CLIENT_ID = environ["CLIENT_ID"]
+CLIENT_SECRET = environ["CLIENT_SECRET"]
+
+with Classic(JPS_URL, CLIENT_ID, CLIENT_SECRET, client=True) as classic:
+    print(classic.get_computers())
+    print(classic.get_computer(1001))
+
+with Pro(JPS_URL, CLIENT_ID, CLIENT_SECRET, client=True) as pro:
+    print(pro.get_mobile_devices())
+```
+
+
 ## Method Documentation
 
 View the [ReadTheDocs](https://jps-api-wrapper.readthedocs.io/en/stable/)
 
 The method documentation is meant to match [Jamf's API Reference](https://developer.jamf.com/jamf-pro/reference/classic-api) for easy navigation of functionality.
 
 ## Other Notes
```

### Comparing `jps_api_wrapper-1.8.0/tests/test_classic.py` & `jps_api_wrapper-1.9.0/tests/test_classic.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.8.0/tests/test_pro.py` & `jps_api_wrapper-1.9.0/tests/test_pro.py`

 * *Files 1% similar despite different names*

```diff
@@ -1123,64 +1123,14 @@
     when used with required params
     """
     responses.add(response_builder("GET", jps_url("/api/v1/cloud-azure/1001")))
     assert pro.get_cloud_azure_identity_provider_configuration(1001) == EXPECTED_JSON
 
 
 @responses.activate
-def test_get_cloud_azure_report(pro):
-    """
-    Ensures that get_cloud_azure_report completes successfully when run with
-    required params
-    """
-    responses.add(
-        response_builder(
-            "GET", jps_url("/api/v1/azure-ad-migration/reports/1001/download")
-        )
-    )
-    assert pro.get_cloud_azure_report(1001) == EXPECTED_JSON
-
-
-@responses.activate
-def test_get_cloud_azure_report_status(pro):
-    """
-    Ensures that get_cloud_azure_report_status completes successfully when
-    run with required params
-    """
-    responses.add(
-        response_builder("GET", jps_url("/api/v1/azure-ad-migration/reports/1001"))
-    )
-    assert pro.get_cloud_azure_report_status(1001) == EXPECTED_JSON
-
-
-@responses.activate
-def test_get_cloud_azure_pending_report(pro):
-    """
-    Ensures that get_cloud_azure_pending_report completes successfully when
-    run with required params
-    """
-    responses.add(
-        response_builder("GET", jps_url("/api/v1/azure-ad-migration/reports/pending"))
-    )
-    assert pro.get_cloud_azure_pending_report() == EXPECTED_JSON
-
-
-@responses.activate
-def test_create_cloud_azure_report(pro):
-    """
-    Ensures that create_cloud_azure_report completes successfully when run with
-    required params
-    """
-    responses.add(
-        response_builder("POST", jps_url("/api/v1/azure-ad-migration/reports"))
-    )
-    assert pro.create_cloud_azure_report(EXPECTED_JSON) == EXPECTED_JSON
-
-
-@responses.activate
 def test_create_cloud_azure_identity_provider_configuration(pro):
     """
     Ensures that create_cloud_azure_identity_provider_configuration completes
     successfully when run with required params
     """
     responses.add(response_builder("POST", jps_url("/api/v1/cloud-azure")))
     assert (
@@ -4400,14 +4350,89 @@
     assert (
         pro.get_managed_software_updates_statuses(filter="downloaded==True")
         == EXPECTED_JSON
     )
 
 
 @responses.activate
+def test_get_managed_software_updates_plans(pro):
+    """
+    Ensures that get_managed_software_updates_plans returns JSON when used
+    without optional params
+    """
+    responses.add(
+        response_builder("GET", jps_url("/api/v1/managed-software-updates/plans"))
+    )
+    assert pro.get_managed_software_updates_plans() == EXPECTED_JSON
+
+
+@responses.activate
+def test_get_managed_software_updates_plans_optional_params(pro):
+    """
+    Ensures that get_managed_software_updates_plans returns JSON when used with
+    all optional params
+    """
+    responses.add(
+        response_builder("GET", jps_url("/api/v1/managed-software-updates/plans"))
+    )
+    assert (
+        pro.get_managed_software_updates_plans(
+            0,
+            100,
+            ["planUuid:desc", "maxDeferrals:asc"],
+            'maxDeferrals >= 1 and versionType == "LATEST_ANY"',
+        )
+        == EXPECTED_JSON
+    )
+
+
+@responses.activate
+def test_get_managed_software_updates_feature_toggle(pro):
+    """
+    Ensures that get_managed_software_updates_feature_toggle returns JSON when
+    used
+    """
+    responses.add(
+        response_builder(
+            "GET", jps_url("/api/v1/managed-software-updates/plans/feature-toggle")
+        )
+    )
+    assert pro.get_managed_software_updates_feature_toggle() == EXPECTED_JSON
+
+
+@responses.activate
+def test_get_managed_software_updates_group_plans(pro):
+    """
+    Ensures that get_managed_software_updates_group_plans return JSON when
+    used with required params
+    """
+    responses.add(
+        response_builder(
+            "GET", jps_url("/api/v1/managed-software-updates/plans/group/1001")
+        )
+    )
+    assert (
+        pro.get_managed_software_updates_group_plans(1001, "COMPUTER_GROUP")
+        == EXPECTED_JSON
+    )
+
+
+@responses.activate
+def test_get_managed_software_updates_plan(pro):
+    """
+    Ensures that get_managed_software_updates_plan returns JSON when used with
+    required params
+    """
+    responses.add(
+        response_builder("GET", jps_url("/api/v1/managed-software-updates/plans/1001"))
+    )
+    assert pro.get_managed_software_updates_plan(1001) == EXPECTED_JSON
+
+
+@responses.activate
 def test_get_managed_software_updates_computer_group(pro):
     """
     Ensures that get_managed_software_updates_computer_group returns JSON when
     used with required params
     """
     responses.add(
         response_builder(
@@ -4466,14 +4491,59 @@
                 "/api/v1/managed-software-updates/update-statuses/mobile-devices/1001"
             ),
         )
     )
     assert pro.get_managed_software_updates_mobile_device(1001) == EXPECTED_JSON
 
 
+@responses.activate
+def test_create_managed_software_updates_plan(pro):
+    """
+    Ensures that create_managed_software_updates_plan returns JSON when used
+    with required params
+    """
+    responses.add(
+        response_builder("POST", jps_url("/api/v1/managed-software-updates/plans"))
+    )
+    assert pro.create_managed_software_updates_plan(EXPECTED_JSON) == EXPECTED_JSON
+
+
+@responses.activate
+def test_create_managed_software_updates_group_plan(pro):
+    """
+    Ensures that create_managed_software_updates_group_plan returns JSON when
+    used with required params
+    """
+    responses.add(
+        response_builder(
+            "POST", jps_url("/api/v1/managed-software-updates/plans/group")
+        )
+    )
+    assert (
+        pro.create_managed_software_updates_group_plan(EXPECTED_JSON) == EXPECTED_JSON
+    )
+
+
+@responses.activate
+def test_update_managed_software_updates_feature_toggle(pro):
+    """
+    Ensures that update_managed_software_updates_feature_toggle returns JSON
+    when used with required params
+    """
+    responses.add(
+        response_builder(
+            "PUT", jps_url("/api/v1/managed-software-updates/plans/feature-toggle")
+        )
+    )
+    assert (
+        pro.update_managed_software_updates_feature_toggle(EXPECTED_JSON)
+        == EXPECTED_JSON
+    )
+
+
 """
 mdm
 """
 
 
 @responses.activate
 def test_get_mdm_commands(pro):
```

