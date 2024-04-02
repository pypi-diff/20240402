# Comparing `tmp/finbourne_identity_sdk-2.0.8.tar.gz` & `tmp/finbourne_identity_sdk-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_identity_sdk-2.0.8.tar", max compression
+gzip compressed data, was "finbourne_identity_sdk-2.0.9.tar", max compression
```

## Comparing `finbourne_identity_sdk-2.0.8.tar` & `finbourne_identity_sdk-2.0.9.tar`

### file list

```diff
@@ -1,68 +1,73 @@
--rw-r--r--   0        0        0    12674 2023-12-14 15:49:27.415132 finbourne_identity_sdk-2.0.8/README.md
--rw-r--r--   0        0        0     4202 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/__init__.py
--rw-r--r--   0        0        0      662 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/api/__init__.py
--rw-r--r--   0        0        0     7555 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/api/application_metadata_api.py
--rw-r--r--   0        0        0    36608 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/api/applications_api.py
--rw-r--r--   0        0        0    37493 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/api/authentication_api.py
--rw-r--r--   0        0        0    15650 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/api/identity_provider_api.py
--rw-r--r--   0        0        0    14849 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/api/me_api.py
--rw-r--r--   0        0        0    21844 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/api/personal_authentication_tokens_api.py
--rw-r--r--   0        0        0    57676 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/api/roles_api.py
--rw-r--r--   0        0        0     6894 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/api/tokens_api.py
--rw-r--r--   0        0        0    95605 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/api/users_api.py
--rw-r--r--   0        0        0    30571 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/api_client.py
--rw-r--r--   0        0        0      852 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/api_response.py
--rw-r--r--   0        0        0    14468 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/configuration.py
--rw-r--r--   0        0        0     5347 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/exceptions.py
--rw-r--r--   0        0        0      302 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/__init__.py
--rw-r--r--   0        0        0    30528 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/api_client.py
--rw-r--r--   0        0        0     9684 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8028 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/api_configuration.py
--rw-r--r--   0        0        0     6884 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2055 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12711 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/rest.py
--rw-r--r--   0        0        0    11577 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/retry.py
--rw-r--r--   0        0        0     1653 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3890 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     3027 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/__init__.py
--rw-r--r--   0        0        0     3920 2023-12-14 15:49:27.408132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/access_controlled_action.py
--rw-r--r--   0        0        0     4863 2023-12-14 15:49:27.408132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2075 2023-12-14 15:49:27.408132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/action_id.py
--rw-r--r--   0        0        0     2433 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/add_scim_response.py
--rw-r--r--   0        0        0     3346 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/api_key.py
--rw-r--r--   0        0        0     5236 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/authentication_information.py
--rw-r--r--   0        0        0     2781 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/create_api_key.py
--rw-r--r--   0        0        0     4486 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/create_application_request.py
--rw-r--r--   0        0        0     3115 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/create_role_request.py
--rw-r--r--   0        0        0     5258 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/create_user_request.py
--rw-r--r--   0        0        0     3523 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/created_api_key.py
--rw-r--r--   0        0        0     3518 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/current_user_response.py
--rw-r--r--   0        0        0     2773 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/error_detail.py
--rw-r--r--   0        0        0     3189 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/id_selector_definition.py
--rw-r--r--   0        0        0     3114 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/identifier_part_schema.py
--rw-r--r--   0        0        0     2267 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/link.py
--rw-r--r--   0        0        0     4741 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/list_users_response.py
--rw-r--r--   0        0        0     3862 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4698 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     2987 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/o_auth_application.py
--rw-r--r--   0        0        0     4268 2023-12-14 15:49:27.409132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     1919 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/role_id.py
--rw-r--r--   0        0        0     2986 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/role_response.py
--rw-r--r--   0        0        0     1909 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/set_password.py
--rw-r--r--   0        0        0     2767 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/set_password_response.py
--rw-r--r--   0        0        0     1990 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/support_access_expiry.py
--rw-r--r--   0        0        0     2385 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/support_access_expiry_with_role.py
--rw-r--r--   0        0        0     3920 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/support_access_request.py
--rw-r--r--   0        0        0     5254 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/support_access_response.py
--rw-r--r--   0        0        0     3183 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/support_role.py
--rw-r--r--   0        0        0     2678 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/support_roles_response.py
--rw-r--r--   0        0        0     1930 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/temporary_password.py
--rw-r--r--   0        0        0     2554 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/update_role_request.py
--rw-r--r--   0        0        0     4749 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/update_user_request.py
--rw-r--r--   0        0        0     5145 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/user_response.py
--rw-r--r--   0        0        0     4917 2023-12-14 15:49:27.410132 finbourne_identity_sdk-2.0.8/finbourne_identity/models/user_summary.py
--rw-r--r--   0        0        0        0 2023-12-14 15:49:27.411132 finbourne_identity_sdk-2.0.8/finbourne_identity/py.typed
--rw-r--r--   0        0        0    10041 2023-12-14 15:49:27.412132 finbourne_identity_sdk-2.0.8/finbourne_identity/rest.py
--rw-r--r--   0        0        0      898 2023-12-14 15:49:27.415132 finbourne_identity_sdk-2.0.8/pyproject.toml
--rw-r--r--   0        0        0    13764 1970-01-01 00:00:00.000000 finbourne_identity_sdk-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0    13179 2023-12-15 17:30:01.092972 finbourne_identity_sdk-2.0.9/README.md
+-rw-r--r--   0        0        0     4611 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/__init__.py
+-rw-r--r--   0        0        0      662 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/__init__.py
+-rw-r--r--   0        0        0     7555 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/application_metadata_api.py
+-rw-r--r--   0        0        0    36608 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/applications_api.py
+-rw-r--r--   0        0        0    44723 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/authentication_api.py
+-rw-r--r--   0        0        0    15650 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/identity_provider_api.py
+-rw-r--r--   0        0        0    14849 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/me_api.py
+-rw-r--r--   0        0        0    21844 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/personal_authentication_tokens_api.py
+-rw-r--r--   0        0        0    57676 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/roles_api.py
+-rw-r--r--   0        0        0     6894 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/tokens_api.py
+-rw-r--r--   0        0        0    95605 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/api/users_api.py
+-rw-r--r--   0        0        0    30571 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/api_client.py
+-rw-r--r--   0        0        0      852 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/api_response.py
+-rw-r--r--   0        0        0    14468 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/configuration.py
+-rw-r--r--   0        0        0     5347 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/exceptions.py
+-rw-r--r--   0        0        0      302 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/__init__.py
+-rw-r--r--   0        0        0    30528 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/api_client.py
+-rw-r--r--   0        0        0     9684 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8028 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6884 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2055 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12711 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/rest.py
+-rw-r--r--   0        0        0    11577 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3890 2023-12-15 17:30:01.090972 finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     3436 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/__init__.py
+-rw-r--r--   0        0        0     3920 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4863 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2075 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/action_id.py
+-rw-r--r--   0        0        0     2433 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/add_scim_response.py
+-rw-r--r--   0        0        0     3346 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/api_key.py
+-rw-r--r--   0        0        0     5236 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/authentication_information.py
+-rw-r--r--   0        0        0     2781 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_api_key.py
+-rw-r--r--   0        0        0     4486 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_application_request.py
+-rw-r--r--   0        0        0     3115 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_role_request.py
+-rw-r--r--   0        0        0     5258 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_user_request.py
+-rw-r--r--   0        0        0     3523 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/created_api_key.py
+-rw-r--r--   0        0        0     3518 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/current_user_response.py
+-rw-r--r--   0        0        0     2773 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/error_detail.py
+-rw-r--r--   0        0        0     3189 2023-12-15 17:30:01.086972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3114 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     2267 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/link.py
+-rw-r--r--   0        0        0     4741 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/list_users_response.py
+-rw-r--r--   0        0        0     3862 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4698 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     2987 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/o_auth_application.py
+-rw-r--r--   0        0        0     2209 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy.py
+-rw-r--r--   0        0        0     2276 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy_age.py
+-rw-r--r--   0        0        0     2553 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy_complexity.py
+-rw-r--r--   0        0        0     3139 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy_conditions.py
+-rw-r--r--   0        0        0     2058 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/password_policy_lockout.py
+-rw-r--r--   0        0        0     4268 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     1919 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/role_id.py
+-rw-r--r--   0        0        0     2986 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/role_response.py
+-rw-r--r--   0        0        0     1909 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/set_password.py
+-rw-r--r--   0        0        0     2767 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/set_password_response.py
+-rw-r--r--   0        0        0     1990 2023-12-15 17:30:01.087972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_expiry.py
+-rw-r--r--   0        0        0     2385 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_expiry_with_role.py
+-rw-r--r--   0        0        0     3920 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_request.py
+-rw-r--r--   0        0        0     5254 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_response.py
+-rw-r--r--   0        0        0     3183 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_role.py
+-rw-r--r--   0        0        0     2678 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_roles_response.py
+-rw-r--r--   0        0        0     1930 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/temporary_password.py
+-rw-r--r--   0        0        0     2554 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/update_role_request.py
+-rw-r--r--   0        0        0     4749 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/update_user_request.py
+-rw-r--r--   0        0        0     5145 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/user_response.py
+-rw-r--r--   0        0        0     4917 2023-12-15 17:30:01.088972 finbourne_identity_sdk-2.0.9/finbourne_identity/models/user_summary.py
+-rw-r--r--   0        0        0        0 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/py.typed
+-rw-r--r--   0        0        0    10041 2023-12-15 17:30:01.089972 finbourne_identity_sdk-2.0.9/finbourne_identity/rest.py
+-rw-r--r--   0        0        0      898 2023-12-15 17:30:01.092972 finbourne_identity_sdk-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0    14269 1970-01-01 00:00:00.000000 finbourne_identity_sdk-2.0.9/PKG-INFO
```

### Comparing `finbourne_identity_sdk-2.0.8/README.md` & `finbourne_identity_sdk-2.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-identity-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.2723
-- Package version: 2.0.8
+- API version: 0.0.2725
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -115,14 +115,15 @@
 *ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
 *ApplicationsApi* | [**create_application**](docs/ApplicationsApi.md#create_application) | **POST** /api/applications | [EARLY ACCESS] CreateApplication: Create Application
 *ApplicationsApi* | [**delete_application**](docs/ApplicationsApi.md#delete_application) | **DELETE** /api/applications/{id} | [EARLY ACCESS] DeleteApplication: Delete Application
 *ApplicationsApi* | [**get_application**](docs/ApplicationsApi.md#get_application) | **GET** /api/applications/{id} | [EARLY ACCESS] GetApplication: Get Application
 *ApplicationsApi* | [**list_applications**](docs/ApplicationsApi.md#list_applications) | **GET** /api/applications | [EARLY ACCESS] ListApplications: List Applications
 *ApplicationsApi* | [**rotate_application_secrets**](docs/ApplicationsApi.md#rotate_application_secrets) | **POST** /api/applications/{id}/lifecycle/$newsecret | [EXPERIMENTAL] RotateApplicationSecrets: Rotate Application Secrets
 *AuthenticationApi* | [**get_authentication_information**](docs/AuthenticationApi.md#get_authentication_information) | **GET** /api/authentication/information | GetAuthenticationInformation: Gets AuthenticationInformation
+*AuthenticationApi* | [**get_password_policy**](docs/AuthenticationApi.md#get_password_policy) | **GET** /api/authentication/password-policy/{userType} | [EXPERIMENTAL] GetPasswordPolicy: Gets Password Policy for a user type
 *AuthenticationApi* | [**get_support_access_history**](docs/AuthenticationApi.md#get_support_access_history) | **GET** /api/authentication/support | [EARLY ACCESS] GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination
 *AuthenticationApi* | [**get_support_roles**](docs/AuthenticationApi.md#get_support_roles) | **GET** /api/authentication/support-roles | [EARLY ACCESS] GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation
 *AuthenticationApi* | [**grant_support_access**](docs/AuthenticationApi.md#grant_support_access) | **POST** /api/authentication/support | [EARLY ACCESS] GrantSupportAccess: Grants FINBOURNE support access to your account
 *AuthenticationApi* | [**invalidate_support_access**](docs/AuthenticationApi.md#invalidate_support_access) | **DELETE** /api/authentication/support | [EARLY ACCESS] InvalidateSupportAccess: Revoke any FINBOURNE support access to your account
 *IdentityProviderApi* | [**add_scim**](docs/IdentityProviderApi.md#add_scim) | **PUT** /api/identityprovider/scim | [EARLY ACCESS] AddScim: Add SCIM
 *IdentityProviderApi* | [**remove_scim**](docs/IdentityProviderApi.md#remove_scim) | **DELETE** /api/identityprovider/scim | [EARLY ACCESS] RemoveScim: Remove SCIM
 *MeApi* | [**get_user_info**](docs/MeApi.md#get_user_info) | **GET** /api/me | [EARLY ACCESS] GetUserInfo: Get User Info
@@ -172,14 +173,19 @@
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
  - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [Link](docs/Link.md)
  - [ListUsersResponse](docs/ListUsersResponse.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
  - [OAuthApplication](docs/OAuthApplication.md)
+ - [PasswordPolicy](docs/PasswordPolicy.md)
+ - [PasswordPolicyAge](docs/PasswordPolicyAge.md)
+ - [PasswordPolicyComplexity](docs/PasswordPolicyComplexity.md)
+ - [PasswordPolicyConditions](docs/PasswordPolicyConditions.md)
+ - [PasswordPolicyLockout](docs/PasswordPolicyLockout.md)
  - [ResourceListOfAccessControlledResource](docs/ResourceListOfAccessControlledResource.md)
  - [RoleId](docs/RoleId.md)
  - [RoleResponse](docs/RoleResponse.md)
  - [SetPassword](docs/SetPassword.md)
  - [SetPasswordResponse](docs/SetPasswordResponse.md)
  - [SupportAccessExpiry](docs/SupportAccessExpiry.md)
  - [SupportAccessExpiryWithRole](docs/SupportAccessExpiryWithRole.md)
```

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/__init__.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,14 +52,19 @@
 from finbourne_identity.models.id_selector_definition import IdSelectorDefinition
 from finbourne_identity.models.identifier_part_schema import IdentifierPartSchema
 from finbourne_identity.models.link import Link
 from finbourne_identity.models.list_users_response import ListUsersResponse
 from finbourne_identity.models.lusid_problem_details import LusidProblemDetails
 from finbourne_identity.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from finbourne_identity.models.o_auth_application import OAuthApplication
+from finbourne_identity.models.password_policy import PasswordPolicy
+from finbourne_identity.models.password_policy_age import PasswordPolicyAge
+from finbourne_identity.models.password_policy_complexity import PasswordPolicyComplexity
+from finbourne_identity.models.password_policy_conditions import PasswordPolicyConditions
+from finbourne_identity.models.password_policy_lockout import PasswordPolicyLockout
 from finbourne_identity.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 from finbourne_identity.models.role_id import RoleId
 from finbourne_identity.models.role_response import RoleResponse
 from finbourne_identity.models.set_password import SetPassword
 from finbourne_identity.models.set_password_response import SetPasswordResponse
 from finbourne_identity.models.support_access_expiry import SupportAccessExpiry
 from finbourne_identity.models.support_access_expiry_with_role import SupportAccessExpiryWithRole
```

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/api/__init__.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/api/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/api/application_metadata_api.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/api/applications_api.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/api/applications_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/api/authentication_api.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/api/authentication_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,19 +18,20 @@
 
 from pydantic import validate_arguments, ValidationError
 from typing import overload, Optional, Union, Awaitable
 
 from typing_extensions import Annotated
 from datetime import datetime
 
-from pydantic import Field
+from pydantic import Field, constr, validator
 
 from typing import List, Optional
 
 from finbourne_identity.models.authentication_information import AuthenticationInformation
+from finbourne_identity.models.password_policy import PasswordPolicy
 from finbourne_identity.models.support_access_request import SupportAccessRequest
 from finbourne_identity.models.support_access_response import SupportAccessResponse
 from finbourne_identity.models.support_roles_response import SupportRolesResponse
 
 from finbourne_identity.api_client import ApiClient
 from finbourne_identity.api_response import ApiResponse
 from finbourne_identity.exceptions import (  # noqa: F401
@@ -181,14 +182,165 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @overload
+    async def get_password_policy(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], **kwargs) -> PasswordPolicy:  # noqa: E501
+        ...
+
+    @overload
+    def get_password_policy(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], async_req: Optional[bool]=True, **kwargs) -> PasswordPolicy:  # noqa: E501
+        ...
+
+    @validate_arguments
+    def get_password_policy(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], async_req: Optional[bool]=None, **kwargs) -> Union[PasswordPolicy, Awaitable[PasswordPolicy]]:  # noqa: E501
+        """[EXPERIMENTAL] GetPasswordPolicy: Gets Password Policy for a user type  # noqa: E501
+
+        Get the password policy for a given user type  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_password_policy(user_type, async_req=True)
+        >>> result = thread.get()
+
+        :param user_type: The type of user (should only be personal or service) (required)
+        :type user_type: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _request_timeout: timeout setting for this request.
+               If one number provided, it will be total request
+               timeout. It can also be a pair (tuple) of
+               (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: PasswordPolicy
+        """
+        kwargs['_return_http_data_only'] = True
+        if '_preload_content' in kwargs:
+            message = "Error! Please call the get_password_policy_with_http_info method with `_preload_content` instead and obtain raw data from ApiResponse.raw_data"  # noqa: E501
+            raise ValueError(message)
+        if async_req is not None:
+            kwargs['async_req'] = async_req
+        return self.get_password_policy_with_http_info(user_type, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def get_password_policy_with_http_info(self, user_type : Annotated[constr(strict=True, max_length=20, min_length=1), Field(..., description="The type of user (should only be personal or service)")], **kwargs) -> ApiResponse:  # noqa: E501
+        """[EXPERIMENTAL] GetPasswordPolicy: Gets Password Policy for a user type  # noqa: E501
+
+        Get the password policy for a given user type  # noqa: E501
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.get_password_policy_with_http_info(user_type, async_req=True)
+        >>> result = thread.get()
+
+        :param user_type: The type of user (should only be personal or service) (required)
+        :type user_type: str
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the ApiResponse.data will
+                                 be set to none and raw_data will store the
+                                 HTTP response body without reading/decoding.
+                                 Default is True.
+        :type _preload_content: bool, optional
+        :param _return_http_data_only: response data instead of ApiResponse
+                                       object with status code, headers, etc
+        :type _return_http_data_only: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(PasswordPolicy, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'user_type'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method get_password_policy" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+        if _params['user_type']:
+            _path_params['userType'] = _params['user_type']
+
+
+        # process the query parameters
+        _query_params = []
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+        # process the form parameters
+        _form_params = []
+        _files = {}
+        # process the body parameter
+        _body_params = None
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # authentication setting
+        _auth_settings = ['oauth2']  # noqa: E501
+
+        _response_types_map = {
+            '200': "PasswordPolicy",
+            '400': "LusidValidationProblemDetails",
+        }
+
+        return self.api_client.call_api(
+            '/api/authentication/password-policy/{userType}', 'GET',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/api/identity_provider_api.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/api/identity_provider_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/api/me_api.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/api/me_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/api/personal_authentication_tokens_api.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/api/personal_authentication_tokens_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/api/roles_api.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/api/tokens_api.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/api/tokens_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/api/users_api.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/api/users_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/api_client.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/api_response.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/configuration.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_identity-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.2723\n"\
+               "Version of the API: 0.0.2725\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/exceptions.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/api_client.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/api_client_factory.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/api_configuration.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/configuration_loaders.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/proxy_config.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/refreshing_token.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/rest.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/retry.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/socket_keep_alive.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/extensions/tcp_keep_alive_connector.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/__init__.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,19 @@
 from finbourne_identity.models.id_selector_definition import IdSelectorDefinition
 from finbourne_identity.models.identifier_part_schema import IdentifierPartSchema
 from finbourne_identity.models.link import Link
 from finbourne_identity.models.list_users_response import ListUsersResponse
 from finbourne_identity.models.lusid_problem_details import LusidProblemDetails
 from finbourne_identity.models.lusid_validation_problem_details import LusidValidationProblemDetails
 from finbourne_identity.models.o_auth_application import OAuthApplication
+from finbourne_identity.models.password_policy import PasswordPolicy
+from finbourne_identity.models.password_policy_age import PasswordPolicyAge
+from finbourne_identity.models.password_policy_complexity import PasswordPolicyComplexity
+from finbourne_identity.models.password_policy_conditions import PasswordPolicyConditions
+from finbourne_identity.models.password_policy_lockout import PasswordPolicyLockout
 from finbourne_identity.models.resource_list_of_access_controlled_resource import ResourceListOfAccessControlledResource
 from finbourne_identity.models.role_id import RoleId
 from finbourne_identity.models.role_response import RoleResponse
 from finbourne_identity.models.set_password import SetPassword
 from finbourne_identity.models.set_password_response import SetPasswordResponse
 from finbourne_identity.models.support_access_expiry import SupportAccessExpiry
 from finbourne_identity.models.support_access_expiry_with_role import SupportAccessExpiryWithRole
```

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/access_controlled_action.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/access_controlled_resource.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/action_id.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/action_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/add_scim_response.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/add_scim_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/api_key.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/api_key.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/authentication_information.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/authentication_information.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/create_api_key.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_api_key.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/create_application_request.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_application_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/create_role_request.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_role_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/create_user_request.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/create_user_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/created_api_key.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/created_api_key.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/current_user_response.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/current_user_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/error_detail.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/error_detail.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/id_selector_definition.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/identifier_part_schema.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/link.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/link.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/list_users_response.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/list_users_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/lusid_problem_details.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/lusid_validation_problem_details.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/o_auth_application.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/o_auth_application.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/resource_list_of_access_controlled_resource.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/role_id.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/role_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/role_response.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/role_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/set_password.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/set_password.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/set_password_response.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/set_password_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/support_access_expiry.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_expiry.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/support_access_expiry_with_role.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_expiry_with_role.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/support_access_request.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/support_access_response.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_access_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/support_role.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_role.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/support_roles_response.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/support_roles_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/temporary_password.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/temporary_password.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/update_role_request.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/update_role_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/update_user_request.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/update_user_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/user_response.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/user_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/models/user_summary.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/models/user_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/finbourne_identity/rest.py` & `finbourne_identity_sdk-2.0.9/finbourne_identity/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_identity_sdk-2.0.8/pyproject.toml` & `finbourne_identity_sdk-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-identity-sdk"
-version = "2.0.8"
+version = "2.0.9"
 description = "FINBOURNE Identity Service API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/finbourne-identity-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Identity Service API", "finbourne-identity-sdk"]
 packages = [
```

### Comparing `finbourne_identity_sdk-2.0.8/PKG-INFO` & `finbourne_identity_sdk-2.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-identity-sdk
-Version: 2.0.8
+Version: 2.0.9
 Summary: FINBOURNE Identity Service API
 Home-page: https://github.com/finbourne/finbourne-identity-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Identity Service API,finbourne-identity-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # finbourne-identity-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.2723
-- Package version: 2.0.8
+- API version: 0.0.2725
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
 
@@ -141,14 +141,15 @@
 *ApplicationMetadataApi* | [**list_access_controlled_resources**](docs/ApplicationMetadataApi.md#list_access_controlled_resources) | **GET** /api/metadata/access/resources | [EARLY ACCESS] ListAccessControlledResources: Get resources available for access control
 *ApplicationsApi* | [**create_application**](docs/ApplicationsApi.md#create_application) | **POST** /api/applications | [EARLY ACCESS] CreateApplication: Create Application
 *ApplicationsApi* | [**delete_application**](docs/ApplicationsApi.md#delete_application) | **DELETE** /api/applications/{id} | [EARLY ACCESS] DeleteApplication: Delete Application
 *ApplicationsApi* | [**get_application**](docs/ApplicationsApi.md#get_application) | **GET** /api/applications/{id} | [EARLY ACCESS] GetApplication: Get Application
 *ApplicationsApi* | [**list_applications**](docs/ApplicationsApi.md#list_applications) | **GET** /api/applications | [EARLY ACCESS] ListApplications: List Applications
 *ApplicationsApi* | [**rotate_application_secrets**](docs/ApplicationsApi.md#rotate_application_secrets) | **POST** /api/applications/{id}/lifecycle/$newsecret | [EXPERIMENTAL] RotateApplicationSecrets: Rotate Application Secrets
 *AuthenticationApi* | [**get_authentication_information**](docs/AuthenticationApi.md#get_authentication_information) | **GET** /api/authentication/information | GetAuthenticationInformation: Gets AuthenticationInformation
+*AuthenticationApi* | [**get_password_policy**](docs/AuthenticationApi.md#get_password_policy) | **GET** /api/authentication/password-policy/{userType} | [EXPERIMENTAL] GetPasswordPolicy: Gets Password Policy for a user type
 *AuthenticationApi* | [**get_support_access_history**](docs/AuthenticationApi.md#get_support_access_history) | **GET** /api/authentication/support | [EARLY ACCESS] GetSupportAccessHistory: Get the history of all support access granted and any information pertaining to their termination
 *AuthenticationApi* | [**get_support_roles**](docs/AuthenticationApi.md#get_support_roles) | **GET** /api/authentication/support-roles | [EARLY ACCESS] GetSupportRoles: Get mapping of support roles, the internal representation to a human friendly representation
 *AuthenticationApi* | [**grant_support_access**](docs/AuthenticationApi.md#grant_support_access) | **POST** /api/authentication/support | [EARLY ACCESS] GrantSupportAccess: Grants FINBOURNE support access to your account
 *AuthenticationApi* | [**invalidate_support_access**](docs/AuthenticationApi.md#invalidate_support_access) | **DELETE** /api/authentication/support | [EARLY ACCESS] InvalidateSupportAccess: Revoke any FINBOURNE support access to your account
 *IdentityProviderApi* | [**add_scim**](docs/IdentityProviderApi.md#add_scim) | **PUT** /api/identityprovider/scim | [EARLY ACCESS] AddScim: Add SCIM
 *IdentityProviderApi* | [**remove_scim**](docs/IdentityProviderApi.md#remove_scim) | **DELETE** /api/identityprovider/scim | [EARLY ACCESS] RemoveScim: Remove SCIM
 *MeApi* | [**get_user_info**](docs/MeApi.md#get_user_info) | **GET** /api/me | [EARLY ACCESS] GetUserInfo: Get User Info
@@ -198,14 +199,19 @@
  - [IdSelectorDefinition](docs/IdSelectorDefinition.md)
  - [IdentifierPartSchema](docs/IdentifierPartSchema.md)
  - [Link](docs/Link.md)
  - [ListUsersResponse](docs/ListUsersResponse.md)
  - [LusidProblemDetails](docs/LusidProblemDetails.md)
  - [LusidValidationProblemDetails](docs/LusidValidationProblemDetails.md)
  - [OAuthApplication](docs/OAuthApplication.md)
+ - [PasswordPolicy](docs/PasswordPolicy.md)
+ - [PasswordPolicyAge](docs/PasswordPolicyAge.md)
+ - [PasswordPolicyComplexity](docs/PasswordPolicyComplexity.md)
+ - [PasswordPolicyConditions](docs/PasswordPolicyConditions.md)
+ - [PasswordPolicyLockout](docs/PasswordPolicyLockout.md)
  - [ResourceListOfAccessControlledResource](docs/ResourceListOfAccessControlledResource.md)
  - [RoleId](docs/RoleId.md)
  - [RoleResponse](docs/RoleResponse.md)
  - [SetPassword](docs/SetPassword.md)
  - [SetPasswordResponse](docs/SetPasswordResponse.md)
  - [SupportAccessExpiry](docs/SupportAccessExpiry.md)
  - [SupportAccessExpiryWithRole](docs/SupportAccessExpiryWithRole.md)
```

