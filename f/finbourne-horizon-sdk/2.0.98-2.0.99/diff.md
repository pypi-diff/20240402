# Comparing `tmp/finbourne_horizon_sdk-2.0.98.tar.gz` & `tmp/finbourne_horizon_sdk-2.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_horizon_sdk-2.0.98.tar", max compression
+gzip compressed data, was "finbourne_horizon_sdk-2.0.99.tar", max compression
```

## Comparing `finbourne_horizon_sdk-2.0.98.tar` & `finbourne_horizon_sdk-2.0.99.tar`

### file list

```diff
@@ -1,73 +1,73 @@
--rw-r--r--   0        0        0    14292 2024-03-08 13:23:14.127003 finbourne_horizon_sdk-2.0.98/README.md
--rw-r--r--   0        0        0     4755 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/__init__.py
--rw-r--r--   0        0        0      305 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/api/__init__.py
--rw-r--r--   0        0        0    46616 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/api/instrument_api.py
--rw-r--r--   0        0        0    60678 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/api/integrations_api.py
--rw-r--r--   0        0        0    36418 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/api/process_history_api.py
--rw-r--r--   0        0        0    43381 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/api/vendor_api.py
--rw-r--r--   0        0        0    30805 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/api_client.py
--rw-r--r--   0        0        0      852 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/api_response.py
--rw-r--r--   0        0        0    14454 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/configuration.py
--rw-r--r--   0        0        0     5338 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/exceptions.py
--rw-r--r--   0        0        0      300 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/__init__.py
--rw-r--r--   0        0        0    30675 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/api_client.py
--rw-r--r--   0        0        0     9793 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8112 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/api_configuration.py
--rw-r--r--   0        0        0     6808 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12710 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/rest.py
--rw-r--r--   0        0        0    11576 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3889 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     3945 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/__init__.py
--rw-r--r--   0        0        0     1980 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/allowed_parameter_value.py
--rw-r--r--   0        0        0     4469 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_complete_request.py
--rw-r--r--   0        0        0     2024 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_complete_response.py
--rw-r--r--   0        0        0      745 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_complete_status.py
--rw-r--r--   0        0        0     2132 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_file_details.py
--rw-r--r--   0        0        0      707 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_file_type.py
--rw-r--r--   0        0        0     2646 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_update_request.py
--rw-r--r--   0        0        0     2010 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_update_response.py
--rw-r--r--   0        0        0     2887 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/create_instance_request.py
--rw-r--r--   0        0        0     2599 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/enrichment_response.py
--rw-r--r--   0        0        0     2036 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/execute_instance_response.py
--rw-r--r--   0        0        0     2282 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/file_details.py
--rw-r--r--   0        0        0     1936 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/identifiers.py
--rw-r--r--   0        0        0     1918 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/instance_identifier.py
--rw-r--r--   0        0        0     2504 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/integration_description.py
--rw-r--r--   0        0        0     3719 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/integration_instance.py
--rw-r--r--   0        0        0     2258 2024-03-08 13:23:14.121003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/link.py
--rw-r--r--   0        0        0     3208 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_entity.py
--rw-r--r--   0        0        0     3665 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_field.py
--rw-r--r--   0        0        0     3853 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_problem_details.py
--rw-r--r--   0        0        0     3533 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_property_definition.py
--rw-r--r--   0        0        0     2811 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_property_definition_overrides.py
--rw-r--r--   0        0        0     3938 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_property_definition_overrides_response.py
--rw-r--r--   0        0        0     3012 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_property_to_vendor_field_mapping.py
--rw-r--r--   0        0        0     4482 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3667 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/onboard_instrument_request.py
--rw-r--r--   0        0        0     2734 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/onboard_instrument_response.py
--rw-r--r--   0        0        0     8430 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/open_figi_data.py
--rw-r--r--   0        0        0      986 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/open_figi_parameter_option_name.py
--rw-r--r--   0        0        0     2780 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/open_figi_perm_id_result.py
--rw-r--r--   0        0        0     2887 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/open_figi_search_result.py
--rw-r--r--   0        0        0      768 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/optionality.py
--rw-r--r--   0        0        0     4224 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/paged_resource_list_of_process_information.py
--rw-r--r--   0        0        0     4237 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/paged_resource_list_of_process_update_result.py
--rw-r--r--   0        0        0     4164 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/paged_resource_list_of_vendor_product.py
--rw-r--r--   0        0        0     3037 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/perm_id_data.py
--rw-r--r--   0        0        0     3386 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/process_information.py
--rw-r--r--   0        0        0     3838 2024-03-08 13:23:14.122003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/process_summary.py
--rw-r--r--   0        0        0     2963 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/process_update_result.py
--rw-r--r--   0        0        0     2247 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/query_request.py
--rw-r--r--   0        0        0     2205 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/query_specification.py
--rw-r--r--   0        0        0     1865 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/resource_id.py
--rw-r--r--   0        0        0     3460 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/row_details.py
--rw-r--r--   0        0        0     2017 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/trigger.py
--rw-r--r--   0        0        0     2957 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/update_instance_request.py
--rw-r--r--   0        0        0     2707 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/vendor_product.py
--rw-r--r--   0        0        0        0 2024-03-08 13:23:14.123003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/py.typed
--rw-r--r--   0        0        0    10031 2024-03-08 13:23:14.124003 finbourne_horizon_sdk-2.0.98/finbourne_horizon/rest.py
--rw-r--r--   0        0        0      866 2024-03-08 13:23:14.127003 finbourne_horizon_sdk-2.0.98/pyproject.toml
--rw-r--r--   0        0        0    15341 1970-01-01 00:00:00.000000 finbourne_horizon_sdk-2.0.98/PKG-INFO
+-rw-r--r--   0        0        0    14292 2024-03-11 13:54:49.471807 finbourne_horizon_sdk-2.0.99/README.md
+-rw-r--r--   0        0        0     4755 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/__init__.py
+-rw-r--r--   0        0        0      305 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/__init__.py
+-rw-r--r--   0        0        0    46616 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/instrument_api.py
+-rw-r--r--   0        0        0    60678 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/integrations_api.py
+-rw-r--r--   0        0        0    36418 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/process_history_api.py
+-rw-r--r--   0        0        0    43381 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/vendor_api.py
+-rw-r--r--   0        0        0    30805 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api_client.py
+-rw-r--r--   0        0        0      852 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/api_response.py
+-rw-r--r--   0        0        0    14454 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/configuration.py
+-rw-r--r--   0        0        0     5338 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/exceptions.py
+-rw-r--r--   0        0        0      300 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/__init__.py
+-rw-r--r--   0        0        0    30675 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/api_client.py
+-rw-r--r--   0        0        0     9793 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8112 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6808 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12710 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/rest.py
+-rw-r--r--   0        0        0    11576 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3889 2024-03-11 13:54:49.468807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     3945 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/__init__.py
+-rw-r--r--   0        0        0     1980 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/allowed_parameter_value.py
+-rw-r--r--   0        0        0     4469 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_complete_request.py
+-rw-r--r--   0        0        0     2024 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_complete_response.py
+-rw-r--r--   0        0        0      745 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_complete_status.py
+-rw-r--r--   0        0        0     2132 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_file_details.py
+-rw-r--r--   0        0        0      707 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_file_type.py
+-rw-r--r--   0        0        0     2646 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_update_request.py
+-rw-r--r--   0        0        0     2010 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_update_response.py
+-rw-r--r--   0        0        0     2887 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/create_instance_request.py
+-rw-r--r--   0        0        0     2599 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/enrichment_response.py
+-rw-r--r--   0        0        0     2036 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/execute_instance_response.py
+-rw-r--r--   0        0        0     2282 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/file_details.py
+-rw-r--r--   0        0        0     1936 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/identifiers.py
+-rw-r--r--   0        0        0     1918 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/instance_identifier.py
+-rw-r--r--   0        0        0     2504 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/integration_description.py
+-rw-r--r--   0        0        0     3719 2024-03-11 13:54:49.464807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/integration_instance.py
+-rw-r--r--   0        0        0     2258 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/link.py
+-rw-r--r--   0        0        0     3208 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_entity.py
+-rw-r--r--   0        0        0     3665 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_field.py
+-rw-r--r--   0        0        0     3853 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     3533 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_definition.py
+-rw-r--r--   0        0        0     2811 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_definition_overrides.py
+-rw-r--r--   0        0        0     3938 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_definition_overrides_response.py
+-rw-r--r--   0        0        0     3012 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_to_vendor_field_mapping.py
+-rw-r--r--   0        0        0     4482 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3667 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/onboard_instrument_request.py
+-rw-r--r--   0        0        0     2734 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/onboard_instrument_response.py
+-rw-r--r--   0        0        0     8430 2024-03-11 13:54:49.465807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_data.py
+-rw-r--r--   0        0        0      986 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_parameter_option_name.py
+-rw-r--r--   0        0        0     2780 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_perm_id_result.py
+-rw-r--r--   0        0        0     2887 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_search_result.py
+-rw-r--r--   0        0        0      768 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/optionality.py
+-rw-r--r--   0        0        0     4224 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/paged_resource_list_of_process_information.py
+-rw-r--r--   0        0        0     4237 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/paged_resource_list_of_process_update_result.py
+-rw-r--r--   0        0        0     4164 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/paged_resource_list_of_vendor_product.py
+-rw-r--r--   0        0        0     3037 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/perm_id_data.py
+-rw-r--r--   0        0        0     3386 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/process_information.py
+-rw-r--r--   0        0        0     3838 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/process_summary.py
+-rw-r--r--   0        0        0     2963 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/process_update_result.py
+-rw-r--r--   0        0        0     2247 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/query_request.py
+-rw-r--r--   0        0        0     2205 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/query_specification.py
+-rw-r--r--   0        0        0     1865 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/resource_id.py
+-rw-r--r--   0        0        0     3460 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/row_details.py
+-rw-r--r--   0        0        0     2017 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/trigger.py
+-rw-r--r--   0        0        0     2957 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/update_instance_request.py
+-rw-r--r--   0        0        0     2707 2024-03-11 13:54:49.466807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/vendor_product.py
+-rw-r--r--   0        0        0        0 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/py.typed
+-rw-r--r--   0        0        0    10031 2024-03-11 13:54:49.467807 finbourne_horizon_sdk-2.0.99/finbourne_horizon/rest.py
+-rw-r--r--   0        0        0      866 2024-03-11 13:54:49.471807 finbourne_horizon_sdk-2.0.99/pyproject.toml
+-rw-r--r--   0        0        0    15341 1970-01-01 00:00:00.000000 finbourne_horizon_sdk-2.0.99/PKG-INFO
```

### Comparing `finbourne_horizon_sdk-2.0.98/README.md` & `finbourne_horizon_sdk-2.0.99/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-horizon-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.392
-- Package version: 2.0.98
+- API version: 0.1.393
+- Package version: 2.0.99
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/__init__.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/api/instrument_api.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/instrument_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/api/integrations_api.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/integrations_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/api/process_history_api.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/process_history_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/api/vendor_api.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/api/vendor_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/api_client.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/api_response.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/configuration.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_horizon-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.392\n"\
+               "Version of the API: 0.1.393\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/exceptions.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/api_client.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/api_client_factory.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/api_configuration.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/configuration_loaders.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/proxy_config.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/refreshing_token.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/rest.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/retry.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/socket_keep_alive.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/extensions/tcp_keep_alive_connector.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/__init__.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/allowed_parameter_value.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/allowed_parameter_value.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_complete_request.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_complete_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_complete_response.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_complete_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_complete_status.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_complete_status.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_file_details.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_file_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_file_type.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_file_type.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_update_request.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/audit_update_response.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/audit_update_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/create_instance_request.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/create_instance_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/enrichment_response.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/enrichment_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/execute_instance_response.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/execute_instance_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/file_details.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/file_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/identifiers.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/identifiers.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/instance_identifier.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/instance_identifier.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/integration_description.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/integration_description.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/integration_instance.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/integration_instance.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/link.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/link.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_entity.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_entity.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_field.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_field.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_problem_details.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_property_definition.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_property_definition_overrides.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_definition_overrides.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_property_definition_overrides_response.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_definition_overrides_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_property_to_vendor_field_mapping.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_property_to_vendor_field_mapping.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/lusid_validation_problem_details.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/onboard_instrument_request.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/onboard_instrument_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/onboard_instrument_response.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/onboard_instrument_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/open_figi_data.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_data.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/open_figi_parameter_option_name.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_parameter_option_name.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/open_figi_perm_id_result.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_perm_id_result.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/open_figi_search_result.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/open_figi_search_result.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/optionality.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/optionality.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/paged_resource_list_of_process_information.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/paged_resource_list_of_process_information.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/paged_resource_list_of_process_update_result.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/paged_resource_list_of_process_update_result.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/paged_resource_list_of_vendor_product.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/paged_resource_list_of_vendor_product.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/perm_id_data.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/perm_id_data.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/process_information.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/process_information.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/process_summary.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/process_summary.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/process_update_result.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/process_update_result.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/query_request.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/query_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/query_specification.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/query_specification.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/resource_id.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/row_details.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/row_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/trigger.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/trigger.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/update_instance_request.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/update_instance_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/models/vendor_product.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/models/vendor_product.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/finbourne_horizon/rest.py` & `finbourne_horizon_sdk-2.0.99/finbourne_horizon/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_horizon_sdk-2.0.98/pyproject.toml` & `finbourne_horizon_sdk-2.0.99/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-horizon-sdk"
-version = "2.0.98"
+version = "2.0.99"
 description = "FINBOURNE Horizon API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/horizon-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Horizon API", "finbourne-horizon-sdk"]
 packages = [
```

### Comparing `finbourne_horizon_sdk-2.0.98/PKG-INFO` & `finbourne_horizon_sdk-2.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-horizon-sdk
-Version: 2.0.98
+Version: 2.0.99
 Summary: FINBOURNE Horizon API
 Home-page: https://github.com/finbourne/horizon-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Horizon API,finbourne-horizon-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # finbourne-horizon-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.392
-- Package version: 2.0.98
+- API version: 0.1.393
+- Package version: 2.0.99
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

