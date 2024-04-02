# Comparing `tmp/lusid_drive_sdk-2.0.8.tar.gz` & `tmp/lusid_drive_sdk-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_drive_sdk-2.0.8.tar", max compression
+gzip compressed data, was "lusid_drive_sdk-2.0.9.tar", max compression
```

## Comparing `lusid_drive_sdk-2.0.8.tar` & `lusid_drive_sdk-2.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     7241 2023-12-14 14:50:46.001405 lusid_drive_sdk-2.0.8/README.md
--rw-r--r--   0        0        0     2077 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/__init__.py
--rw-r--r--   0        0        0      271 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/api/__init__.py
--rw-r--r--   0        0        0     7516 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/api/application_metadata_api.py
--rw-r--r--   0        0        0    46851 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/api/files_api.py
--rw-r--r--   0        0        0    65918 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/api/folders_api.py
--rw-r--r--   0        0        0    10285 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/api/search_api.py
--rw-r--r--   0        0        0    30511 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/api_client.py
--rw-r--r--   0        0        0      852 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/api_response.py
--rw-r--r--   0        0        0    14436 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/configuration.py
--rw-r--r--   0        0        0     5336 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/exceptions.py
--rw-r--r--   0        0        0      288 2023-12-14 14:50:46.000405 lusid_drive_sdk-2.0.8/lusid_drive/extensions/__init__.py
--rw-r--r--   0        0        0    30461 2023-12-14 14:50:46.000405 lusid_drive_sdk-2.0.8/lusid_drive/extensions/api_client.py
--rw-r--r--   0        0        0     9614 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8000 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/extensions/api_configuration.py
--rw-r--r--   0        0        0     6856 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2055 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2023-12-14 14:50:46.000405 lusid_drive_sdk-2.0.8/lusid_drive/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12704 2023-12-14 14:50:46.000405 lusid_drive_sdk-2.0.8/lusid_drive/extensions/rest.py
--rw-r--r--   0        0        0    11570 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/extensions/retry.py
--rw-r--r--   0        0        0     1653 2023-12-14 14:50:46.000405 lusid_drive_sdk-2.0.8/lusid_drive/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3883 2023-12-14 14:50:46.000405 lusid_drive_sdk-2.0.8/lusid_drive/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     1349 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/__init__.py
--rw-r--r--   0        0        0     3888 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/access_controlled_action.py
--rw-r--r--   0        0        0     4831 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2064 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/action_id.py
--rw-r--r--   0        0        0     2703 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/create_folder.py
--rw-r--r--   0        0        0     3171 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/id_selector_definition.py
--rw-r--r--   0        0        0     3096 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2256 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/link.py
--rw-r--r--   0        0        0     3851 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4687 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     4150 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/paged_resource_list_of_storage_object.py
--rw-r--r--   0        0        0     4243 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     3105 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/search_body.py
--rw-r--r--   0        0        0     6063 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/storage_object.py
--rw-r--r--   0        0        0     2714 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/update_file.py
--rw-r--r--   0        0        0     2719 2023-12-14 14:50:45.998405 lusid_drive_sdk-2.0.8/lusid_drive/models/update_folder.py
--rw-r--r--   0        0        0        0 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/py.typed
--rw-r--r--   0        0        0    10023 2023-12-14 14:50:45.999405 lusid_drive_sdk-2.0.8/lusid_drive/rest.py
--rw-r--r--   0        0        0      835 2023-12-14 14:50:46.001405 lusid_drive_sdk-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     8269 1970-01-01 00:00:00.000000 lusid_drive_sdk-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     7241 2023-12-19 14:51:15.304728 lusid_drive_sdk-2.0.9/README.md
+-rw-r--r--   0        0        0     2077 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/__init__.py
+-rw-r--r--   0        0        0      271 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/api/__init__.py
+-rw-r--r--   0        0        0     7516 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/api/application_metadata_api.py
+-rw-r--r--   0        0        0    46851 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/api/files_api.py
+-rw-r--r--   0        0        0    65918 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/api/folders_api.py
+-rw-r--r--   0        0        0    10285 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/api/search_api.py
+-rw-r--r--   0        0        0    30511 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/api_client.py
+-rw-r--r--   0        0        0      852 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/api_response.py
+-rw-r--r--   0        0        0    14436 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/configuration.py
+-rw-r--r--   0        0        0     5336 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/exceptions.py
+-rw-r--r--   0        0        0      288 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/__init__.py
+-rw-r--r--   0        0        0    30461 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/api_client.py
+-rw-r--r--   0        0        0     9614 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8000 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6856 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2055 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12704 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/rest.py
+-rw-r--r--   0        0        0    11570 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3883 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     1349 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/models/__init__.py
+-rw-r--r--   0        0        0     3888 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4831 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2064 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/action_id.py
+-rw-r--r--   0        0        0     2703 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/create_folder.py
+-rw-r--r--   0        0        0     3171 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3096 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2256 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/link.py
+-rw-r--r--   0        0        0     3851 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4687 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     4150 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/paged_resource_list_of_storage_object.py
+-rw-r--r--   0        0        0     4243 2023-12-19 14:51:15.301728 lusid_drive_sdk-2.0.9/lusid_drive/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     3105 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/models/search_body.py
+-rw-r--r--   0        0        0     6063 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/models/storage_object.py
+-rw-r--r--   0        0        0     2714 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/models/update_file.py
+-rw-r--r--   0        0        0     2719 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/models/update_folder.py
+-rw-r--r--   0        0        0        0 2023-12-19 14:51:15.302729 lusid_drive_sdk-2.0.9/lusid_drive/py.typed
+-rw-r--r--   0        0        0    10023 2023-12-19 14:51:15.303728 lusid_drive_sdk-2.0.9/lusid_drive/rest.py
+-rw-r--r--   0        0        0      835 2023-12-19 14:51:15.304728 lusid_drive_sdk-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8269 1970-01-01 00:00:00.000000 lusid_drive_sdk-2.0.9/PKG-INFO
```

### Comparing `lusid_drive_sdk-2.0.8/README.md` & `lusid_drive_sdk-2.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-drive-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.601
-- Package version: 2.0.8
+- API version: 0.1.602
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/__init__.py` & `lusid_drive_sdk-2.0.9/lusid_drive/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/api/application_metadata_api.py` & `lusid_drive_sdk-2.0.9/lusid_drive/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/api/files_api.py` & `lusid_drive_sdk-2.0.9/lusid_drive/api/files_api.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/api/folders_api.py` & `lusid_drive_sdk-2.0.9/lusid_drive/api/folders_api.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/api/search_api.py` & `lusid_drive_sdk-2.0.9/lusid_drive/api/search_api.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/api_client.py` & `lusid_drive_sdk-2.0.9/lusid_drive/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/api_response.py` & `lusid_drive_sdk-2.0.9/lusid_drive/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/configuration.py` & `lusid_drive_sdk-2.0.9/lusid_drive/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_drive-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.601\n"\
+               "Version of the API: 0.1.602\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/exceptions.py` & `lusid_drive_sdk-2.0.9/lusid_drive/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/extensions/api_client.py` & `lusid_drive_sdk-2.0.9/lusid_drive/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/extensions/api_client_factory.py` & `lusid_drive_sdk-2.0.9/lusid_drive/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/extensions/api_configuration.py` & `lusid_drive_sdk-2.0.9/lusid_drive/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/extensions/configuration_loaders.py` & `lusid_drive_sdk-2.0.9/lusid_drive/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/extensions/proxy_config.py` & `lusid_drive_sdk-2.0.9/lusid_drive/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/extensions/refreshing_token.py` & `lusid_drive_sdk-2.0.9/lusid_drive/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/extensions/rest.py` & `lusid_drive_sdk-2.0.9/lusid_drive/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/extensions/retry.py` & `lusid_drive_sdk-2.0.9/lusid_drive/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/extensions/socket_keep_alive.py` & `lusid_drive_sdk-2.0.9/lusid_drive/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/extensions/tcp_keep_alive_connector.py` & `lusid_drive_sdk-2.0.9/lusid_drive/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/__init__.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/access_controlled_action.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/access_controlled_resource.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/action_id.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/action_id.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/create_folder.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/create_folder.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/id_selector_definition.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/identifier_part_schema.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/link.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/link.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/lusid_problem_details.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/lusid_validation_problem_details.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/paged_resource_list_of_storage_object.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/paged_resource_list_of_storage_object.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/resource_list_of_access_controlled_resource.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/search_body.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/search_body.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/storage_object.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/storage_object.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/update_file.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/update_file.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/models/update_folder.py` & `lusid_drive_sdk-2.0.9/lusid_drive/models/update_folder.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/lusid_drive/rest.py` & `lusid_drive_sdk-2.0.9/lusid_drive/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_drive_sdk-2.0.8/pyproject.toml` & `lusid_drive_sdk-2.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-drive-sdk"
-version = "2.0.8"
+version = "2.0.9"
 description = "FINBOURNE Drive API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/drive-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Drive API", "lusid-drive-sdk"]
 packages = [
```

### Comparing `lusid_drive_sdk-2.0.8/PKG-INFO` & `lusid_drive_sdk-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-drive-sdk
-Version: 2.0.8
+Version: 2.0.9
 Summary: FINBOURNE Drive API
 Home-page: https://github.com/finbourne/drive-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Drive API,lusid-drive-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # lusid-drive-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.601
-- Package version: 2.0.8
+- API version: 0.1.602
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

