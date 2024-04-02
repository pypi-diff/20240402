# Comparing `tmp/finbourne_access_sdk-2.0.98.tar.gz` & `tmp/finbourne_access_sdk-2.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finbourne_access_sdk-2.0.98.tar", max compression
+gzip compressed data, was "finbourne_access_sdk-2.0.99.tar", max compression
```

## Comparing `finbourne_access_sdk-2.0.98.tar` & `finbourne_access_sdk-2.0.99.tar`

### file list

```diff
@@ -1,107 +1,107 @@
--rw-r--r--   0        0        0    17797 2024-02-26 11:51:25.906048 finbourne_access_sdk-2.0.98/README.md
--rw-r--r--   0        0        0     7542 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/__init__.py
--rw-r--r--   0        0        0      373 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/api/__init__.py
--rw-r--r--   0        0        0     7548 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/api/application_metadata_api.py
--rw-r--r--   0        0        0   160681 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/api/policies_api.py
--rw-r--r--   0        0        0    55448 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/api/policy_templates_api.py
--rw-r--r--   0        0        0    68280 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/api/roles_api.py
--rw-r--r--   0        0        0    76095 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/api/user_roles_api.py
--rw-r--r--   0        0        0    30808 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/api_client.py
--rw-r--r--   0        0        0      852 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/api_response.py
--rw-r--r--   0        0        0    14461 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/configuration.py
--rw-r--r--   0        0        0     5348 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/exceptions.py
--rw-r--r--   0        0        0      298 2024-02-26 11:51:25.902048 finbourne_access_sdk-2.0.98/finbourne_access/extensions/__init__.py
--rw-r--r--   0        0        0    30677 2024-02-26 11:51:25.902048 finbourne_access_sdk-2.0.98/finbourne_access/extensions/api_client.py
--rw-r--r--   0        0        0     9783 2024-02-26 11:51:25.902048 finbourne_access_sdk-2.0.98/finbourne_access/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8107 2024-02-26 11:51:25.902048 finbourne_access_sdk-2.0.98/finbourne_access/extensions/api_configuration.py
--rw-r--r--   0        0        0     6804 2024-02-26 11:51:25.902048 finbourne_access_sdk-2.0.98/finbourne_access/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2187 2024-02-26 11:51:25.902048 finbourne_access_sdk-2.0.98/finbourne_access/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2024-02-26 11:51:25.902048 finbourne_access_sdk-2.0.98/finbourne_access/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12709 2024-02-26 11:51:25.902048 finbourne_access_sdk-2.0.98/finbourne_access/extensions/rest.py
--rw-r--r--   0        0        0    11575 2024-02-26 11:51:25.902048 finbourne_access_sdk-2.0.98/finbourne_access/extensions/retry.py
--rw-r--r--   0        0        0     1653 2024-02-26 11:51:25.902048 finbourne_access_sdk-2.0.98/finbourne_access/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3888 2024-02-26 11:51:25.902048 finbourne_access_sdk-2.0.98/finbourne_access/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     6672 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/models/__init__.py
--rw-r--r--   0        0        0     3915 2024-02-26 11:51:25.897048 finbourne_access_sdk-2.0.98/finbourne_access/models/access_controlled_action.py
--rw-r--r--   0        0        0     4858 2024-02-26 11:51:25.897048 finbourne_access_sdk-2.0.98/finbourne_access/models/access_controlled_resource.py
--rw-r--r--   0        0        0     2076 2024-02-26 11:51:25.897048 finbourne_access_sdk-2.0.98/finbourne_access/models/action_id.py
--rw-r--r--   0        0        0     2702 2024-02-26 11:51:25.897048 finbourne_access_sdk-2.0.98/finbourne_access/models/add_policy_collection_to_role_request.py
--rw-r--r--   0        0        0     2458 2024-02-26 11:51:25.897048 finbourne_access_sdk-2.0.98/finbourne_access/models/add_policy_to_role_request.py
--rw-r--r--   0        0        0     3820 2024-02-26 11:51:25.897048 finbourne_access_sdk-2.0.98/finbourne_access/models/add_to_policy_collection_request.py
--rw-r--r--   0        0        0     2560 2024-02-26 11:51:25.897048 finbourne_access_sdk-2.0.98/finbourne_access/models/as_at_predicate_contract.py
--rw-r--r--   0        0        0     2485 2024-02-26 11:51:25.897048 finbourne_access_sdk-2.0.98/finbourne_access/models/as_at_range_for_spec.py
--rw-r--r--   0        0        0     2463 2024-02-26 11:51:25.897048 finbourne_access_sdk-2.0.98/finbourne_access/models/as_at_relative.py
--rw-r--r--   0        0        0     6885 2024-02-26 11:51:25.897048 finbourne_access_sdk-2.0.98/finbourne_access/models/attached_policy_definition_response.py
--rw-r--r--   0        0        0     1096 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/date_quality.py
--rw-r--r--   0        0        0      781 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/date_unit.py
--rw-r--r--   0        0        0     1968 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/effective_date_has_quality.py
--rw-r--r--   0        0        0     2535 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/effective_date_relative.py
--rw-r--r--   0        0        0     2145 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/effective_range.py
--rw-r--r--   0        0        0     2384 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/entitlement_metadata.py
--rw-r--r--   0        0        0     2622 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/evaluation_request.py
--rw-r--r--   0        0        0     2470 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/evaluation_response.py
--rw-r--r--   0        0        0      766 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/evaluation_result.py
--rw-r--r--   0        0        0     4456 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/for_spec.py
--rw-r--r--   0        0        0     3646 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/generate_policy_from_template_request.py
--rw-r--r--   0        0        0     3728 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/generated_policy_components.py
--rw-r--r--   0        0        0      654 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/grant.py
--rw-r--r--   0        0        0     2864 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/how_spec.py
--rw-r--r--   0        0        0     3188 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/id_selector_definition.py
--rw-r--r--   0        0        0     3113 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/identifier_part_schema.py
--rw-r--r--   0        0        0     4380 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/if_expression.py
--rw-r--r--   0        0        0     2432 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/if_feature_chain_expression.py
--rw-r--r--   0        0        0     3648 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/if_identity_claim_expression.py
--rw-r--r--   0        0        0     2322 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/if_identity_scope_expression.py
--rw-r--r--   0        0        0     2493 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/if_request_header_expression.py
--rw-r--r--   0        0        0     2416 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/key_value_pair_of_string_to_string.py
--rw-r--r--   0        0        0     2268 2024-02-26 11:51:25.898048 finbourne_access_sdk-2.0.98/finbourne_access/models/link.py
--rw-r--r--   0        0        0     3863 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4699 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     3112 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/match_all_selector_definition.py
--rw-r--r--   0        0        0     2445 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/metadata_expression.py
--rw-r--r--   0        0        0     3744 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/metadata_selector_definition.py
--rw-r--r--   0        0        0     2045 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/non_transitive_supervisor_role_resource.py
--rw-r--r--   0        0        0      847 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/operator.py
--rw-r--r--   0        0        0      995 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/point_in_time_specification.py
--rw-r--r--   0        0        0     6046 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_collection_creation_request.py
--rw-r--r--   0        0        0     2942 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_collection_id.py
--rw-r--r--   0        0        0     5202 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_collection_response.py
--rw-r--r--   0        0        0     5464 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_collection_update_request.py
--rw-r--r--   0        0        0     6881 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_creation_request.py
--rw-r--r--   0        0        0     2862 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_id.py
--rw-r--r--   0        0        0     3543 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_id_role_resource.py
--rw-r--r--   0        0        0     7548 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_response.py
--rw-r--r--   0        0        0     4489 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_selector_definition.py
--rw-r--r--   0        0        0     3683 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_template_creation_request.py
--rw-r--r--   0        0        0     5273 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_template_response.py
--rw-r--r--   0        0        0     3150 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_template_update_request.py
--rw-r--r--   0        0        0     2644 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_templated_selector.py
--rw-r--r--   0        0        0      697 2024-02-26 11:51:25.899048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_type.py
--rw-r--r--   0        0        0     6361 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/policy_update_request.py
--rw-r--r--   0        0        0      829 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/relative_to_date_time.py
--rw-r--r--   0        0        0     3863 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/remove_from_policy_collection_request.py
--rw-r--r--   0        0        0     4248 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/request_details.py
--rw-r--r--   0        0        0     3116 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/requested_action_key.py
--rw-r--r--   0        0        0     3219 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/resource_details.py
--rw-r--r--   0        0        0     4265 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/resource_list_of_access_controlled_resource.py
--rw-r--r--   0        0        0     4265 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/resource_list_of_policy_collection_response.py
--rw-r--r--   0        0        0     4144 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/resource_list_of_policy_response.py
--rw-r--r--   0        0        0     4241 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/resource_list_of_policy_template_response.py
--rw-r--r--   0        0        0     4169 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/resource_list_of_user_role_response.py
--rw-r--r--   0        0        0     3483 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/role_creation_request.py
--rw-r--r--   0        0        0     2846 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/role_id.py
--rw-r--r--   0        0        0     3208 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/role_resource_request.py
--rw-r--r--   0        0        0     4779 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/role_response.py
--rw-r--r--   0        0        0     3021 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/role_update_request.py
--rw-r--r--   0        0        0     4280 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/selector_definition.py
--rw-r--r--   0        0        0     3120 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/template_metadata.py
--rw-r--r--   0        0        0     3412 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/template_selection.py
--rw-r--r--   0        0        0     1071 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/text_operator.py
--rw-r--r--   0        0        0     2813 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/user_role_creation_request.py
--rw-r--r--   0        0        0     3271 2024-02-26 11:51:25.900048 finbourne_access_sdk-2.0.98/finbourne_access/models/user_role_response.py
--rw-r--r--   0        0        0     2259 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/models/user_role_update_request.py
--rw-r--r--   0        0        0     2144 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/models/when_spec.py
--rw-r--r--   0        0        0        0 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/py.typed
--rw-r--r--   0        0        0    10040 2024-02-26 11:51:25.901048 finbourne_access_sdk-2.0.98/finbourne_access/rest.py
--rw-r--r--   0        0        0      891 2024-02-26 11:51:25.906048 finbourne_access_sdk-2.0.98/pyproject.toml
--rw-r--r--   0        0        0    18882 1970-01-01 00:00:00.000000 finbourne_access_sdk-2.0.98/PKG-INFO
+-rw-r--r--   0        0        0    17797 2024-02-27 14:29:40.902362 finbourne_access_sdk-2.0.99/README.md
+-rw-r--r--   0        0        0     7542 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/__init__.py
+-rw-r--r--   0        0        0      373 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api/__init__.py
+-rw-r--r--   0        0        0     7548 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api/application_metadata_api.py
+-rw-r--r--   0        0        0   160681 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api/policies_api.py
+-rw-r--r--   0        0        0    55448 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api/policy_templates_api.py
+-rw-r--r--   0        0        0    68280 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api/roles_api.py
+-rw-r--r--   0        0        0    76095 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api/user_roles_api.py
+-rw-r--r--   0        0        0    30808 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/api_client.py
+-rw-r--r--   0        0        0      852 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/api_response.py
+-rw-r--r--   0        0        0    14461 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/configuration.py
+-rw-r--r--   0        0        0     5348 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/exceptions.py
+-rw-r--r--   0        0        0      298 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/__init__.py
+-rw-r--r--   0        0        0    30677 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/api_client.py
+-rw-r--r--   0        0        0     9783 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8107 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6804 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2187 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12709 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/rest.py
+-rw-r--r--   0        0        0    11575 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3888 2024-02-27 14:29:40.897362 finbourne_access_sdk-2.0.99/finbourne_access/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     6672 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/__init__.py
+-rw-r--r--   0        0        0     3915 2024-02-27 14:29:40.891362 finbourne_access_sdk-2.0.99/finbourne_access/models/access_controlled_action.py
+-rw-r--r--   0        0        0     4858 2024-02-27 14:29:40.891362 finbourne_access_sdk-2.0.99/finbourne_access/models/access_controlled_resource.py
+-rw-r--r--   0        0        0     2076 2024-02-27 14:29:40.891362 finbourne_access_sdk-2.0.99/finbourne_access/models/action_id.py
+-rw-r--r--   0        0        0     2702 2024-02-27 14:29:40.891362 finbourne_access_sdk-2.0.99/finbourne_access/models/add_policy_collection_to_role_request.py
+-rw-r--r--   0        0        0     2458 2024-02-27 14:29:40.891362 finbourne_access_sdk-2.0.99/finbourne_access/models/add_policy_to_role_request.py
+-rw-r--r--   0        0        0     3820 2024-02-27 14:29:40.891362 finbourne_access_sdk-2.0.99/finbourne_access/models/add_to_policy_collection_request.py
+-rw-r--r--   0        0        0     2560 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/as_at_predicate_contract.py
+-rw-r--r--   0        0        0     2485 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/as_at_range_for_spec.py
+-rw-r--r--   0        0        0     2463 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/as_at_relative.py
+-rw-r--r--   0        0        0     6885 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/attached_policy_definition_response.py
+-rw-r--r--   0        0        0     1096 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/date_quality.py
+-rw-r--r--   0        0        0      781 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/date_unit.py
+-rw-r--r--   0        0        0     1968 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/effective_date_has_quality.py
+-rw-r--r--   0        0        0     2535 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/effective_date_relative.py
+-rw-r--r--   0        0        0     2145 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/effective_range.py
+-rw-r--r--   0        0        0     2384 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/entitlement_metadata.py
+-rw-r--r--   0        0        0     2622 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/evaluation_request.py
+-rw-r--r--   0        0        0     2470 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/evaluation_response.py
+-rw-r--r--   0        0        0      766 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/evaluation_result.py
+-rw-r--r--   0        0        0     4456 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/for_spec.py
+-rw-r--r--   0        0        0     3646 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/generate_policy_from_template_request.py
+-rw-r--r--   0        0        0     3728 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/generated_policy_components.py
+-rw-r--r--   0        0        0      654 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/grant.py
+-rw-r--r--   0        0        0     2864 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/how_spec.py
+-rw-r--r--   0        0        0     3188 2024-02-27 14:29:40.892362 finbourne_access_sdk-2.0.99/finbourne_access/models/id_selector_definition.py
+-rw-r--r--   0        0        0     3113 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/identifier_part_schema.py
+-rw-r--r--   0        0        0     4380 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/if_expression.py
+-rw-r--r--   0        0        0     2432 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/if_feature_chain_expression.py
+-rw-r--r--   0        0        0     3648 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/if_identity_claim_expression.py
+-rw-r--r--   0        0        0     2322 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/if_identity_scope_expression.py
+-rw-r--r--   0        0        0     2493 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/if_request_header_expression.py
+-rw-r--r--   0        0        0     2416 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/key_value_pair_of_string_to_string.py
+-rw-r--r--   0        0        0     2268 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/link.py
+-rw-r--r--   0        0        0     3863 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4699 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     3112 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/match_all_selector_definition.py
+-rw-r--r--   0        0        0     2445 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/metadata_expression.py
+-rw-r--r--   0        0        0     3744 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/metadata_selector_definition.py
+-rw-r--r--   0        0        0     2045 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/non_transitive_supervisor_role_resource.py
+-rw-r--r--   0        0        0      847 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/operator.py
+-rw-r--r--   0        0        0      995 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/point_in_time_specification.py
+-rw-r--r--   0        0        0     6046 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_creation_request.py
+-rw-r--r--   0        0        0     2942 2024-02-27 14:29:40.893362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_id.py
+-rw-r--r--   0        0        0     5202 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_response.py
+-rw-r--r--   0        0        0     5464 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_update_request.py
+-rw-r--r--   0        0        0     6881 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_creation_request.py
+-rw-r--r--   0        0        0     2862 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_id.py
+-rw-r--r--   0        0        0     3543 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_id_role_resource.py
+-rw-r--r--   0        0        0     7548 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_response.py
+-rw-r--r--   0        0        0     4489 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_selector_definition.py
+-rw-r--r--   0        0        0     3683 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_template_creation_request.py
+-rw-r--r--   0        0        0     5273 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_template_response.py
+-rw-r--r--   0        0        0     3150 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_template_update_request.py
+-rw-r--r--   0        0        0     2644 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_templated_selector.py
+-rw-r--r--   0        0        0      697 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_type.py
+-rw-r--r--   0        0        0     6361 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/policy_update_request.py
+-rw-r--r--   0        0        0      829 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/relative_to_date_time.py
+-rw-r--r--   0        0        0     3863 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/remove_from_policy_collection_request.py
+-rw-r--r--   0        0        0     4248 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/request_details.py
+-rw-r--r--   0        0        0     3116 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/requested_action_key.py
+-rw-r--r--   0        0        0     3219 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/resource_details.py
+-rw-r--r--   0        0        0     4265 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_access_controlled_resource.py
+-rw-r--r--   0        0        0     4265 2024-02-27 14:29:40.894362 finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_policy_collection_response.py
+-rw-r--r--   0        0        0     4144 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_policy_response.py
+-rw-r--r--   0        0        0     4241 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_policy_template_response.py
+-rw-r--r--   0        0        0     4169 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_user_role_response.py
+-rw-r--r--   0        0        0     3483 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/role_creation_request.py
+-rw-r--r--   0        0        0     2846 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/role_id.py
+-rw-r--r--   0        0        0     3208 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/role_resource_request.py
+-rw-r--r--   0        0        0     4779 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/role_response.py
+-rw-r--r--   0        0        0     3021 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/role_update_request.py
+-rw-r--r--   0        0        0     4280 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/selector_definition.py
+-rw-r--r--   0        0        0     3120 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/template_metadata.py
+-rw-r--r--   0        0        0     3412 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/template_selection.py
+-rw-r--r--   0        0        0     1071 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/text_operator.py
+-rw-r--r--   0        0        0     2813 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/user_role_creation_request.py
+-rw-r--r--   0        0        0     3271 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/user_role_response.py
+-rw-r--r--   0        0        0     2259 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/user_role_update_request.py
+-rw-r--r--   0        0        0     2144 2024-02-27 14:29:40.895362 finbourne_access_sdk-2.0.99/finbourne_access/models/when_spec.py
+-rw-r--r--   0        0        0        0 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/py.typed
+-rw-r--r--   0        0        0    10040 2024-02-27 14:29:40.896362 finbourne_access_sdk-2.0.99/finbourne_access/rest.py
+-rw-r--r--   0        0        0      891 2024-02-27 14:29:40.902362 finbourne_access_sdk-2.0.99/pyproject.toml
+-rw-r--r--   0        0        0    18882 1970-01-01 00:00:00.000000 finbourne_access_sdk-2.0.99/PKG-INFO
```

### Comparing `finbourne_access_sdk-2.0.98/README.md` & `finbourne_access_sdk-2.0.99/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # finbourne-access-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.3720
-- Package version: 2.0.98
+- API version: 0.0.3721
+- Package version: 2.0.99
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/__init__.py` & `finbourne_access_sdk-2.0.99/finbourne_access/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/api/application_metadata_api.py` & `finbourne_access_sdk-2.0.99/finbourne_access/api/application_metadata_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/api/policies_api.py` & `finbourne_access_sdk-2.0.99/finbourne_access/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/api/policy_templates_api.py` & `finbourne_access_sdk-2.0.99/finbourne_access/api/policy_templates_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/api/roles_api.py` & `finbourne_access_sdk-2.0.99/finbourne_access/api/roles_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/api/user_roles_api.py` & `finbourne_access_sdk-2.0.99/finbourne_access/api/user_roles_api.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/api_client.py` & `finbourne_access_sdk-2.0.99/finbourne_access/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/api_response.py` & `finbourne_access_sdk-2.0.99/finbourne_access/api_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/configuration.py` & `finbourne_access_sdk-2.0.99/finbourne_access/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("finbourne_access-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.0.3720\n"\
+               "Version of the API: 0.0.3721\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/exceptions.py` & `finbourne_access_sdk-2.0.99/finbourne_access/exceptions.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/extensions/api_client.py` & `finbourne_access_sdk-2.0.99/finbourne_access/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/extensions/api_client_factory.py` & `finbourne_access_sdk-2.0.99/finbourne_access/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/extensions/api_configuration.py` & `finbourne_access_sdk-2.0.99/finbourne_access/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/extensions/configuration_loaders.py` & `finbourne_access_sdk-2.0.99/finbourne_access/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/extensions/proxy_config.py` & `finbourne_access_sdk-2.0.99/finbourne_access/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/extensions/refreshing_token.py` & `finbourne_access_sdk-2.0.99/finbourne_access/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/extensions/rest.py` & `finbourne_access_sdk-2.0.99/finbourne_access/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/extensions/retry.py` & `finbourne_access_sdk-2.0.99/finbourne_access/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/extensions/socket_keep_alive.py` & `finbourne_access_sdk-2.0.99/finbourne_access/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/extensions/tcp_keep_alive_connector.py` & `finbourne_access_sdk-2.0.99/finbourne_access/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/__init__.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/__init__.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/access_controlled_action.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/access_controlled_action.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/access_controlled_resource.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/action_id.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/action_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/add_policy_collection_to_role_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/add_policy_collection_to_role_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/add_policy_to_role_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/add_policy_to_role_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/add_to_policy_collection_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/add_to_policy_collection_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/as_at_predicate_contract.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/as_at_predicate_contract.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/as_at_range_for_spec.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/as_at_range_for_spec.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/as_at_relative.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/as_at_relative.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/attached_policy_definition_response.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/attached_policy_definition_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/date_quality.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/date_quality.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/date_unit.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/date_unit.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/effective_date_has_quality.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/effective_date_has_quality.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/effective_date_relative.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/effective_date_relative.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/effective_range.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/effective_range.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/entitlement_metadata.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/entitlement_metadata.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/evaluation_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/evaluation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/evaluation_response.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/evaluation_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/evaluation_result.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/evaluation_result.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/for_spec.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/for_spec.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/generate_policy_from_template_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/generate_policy_from_template_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/generated_policy_components.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/generated_policy_components.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/grant.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/grant.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/how_spec.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/how_spec.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/id_selector_definition.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/id_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/identifier_part_schema.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/identifier_part_schema.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/if_expression.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/if_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/if_feature_chain_expression.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/if_feature_chain_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/if_identity_claim_expression.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/if_identity_claim_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/if_identity_scope_expression.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/if_identity_scope_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/if_request_header_expression.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/if_request_header_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/key_value_pair_of_string_to_string.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/key_value_pair_of_string_to_string.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/link.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/link.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/lusid_problem_details.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/lusid_validation_problem_details.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/match_all_selector_definition.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/match_all_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/metadata_expression.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/metadata_expression.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/metadata_selector_definition.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/metadata_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/non_transitive_supervisor_role_resource.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/non_transitive_supervisor_role_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/operator.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/operator.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/point_in_time_specification.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/point_in_time_specification.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_collection_creation_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_collection_id.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_collection_response.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_collection_update_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_collection_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_creation_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_id.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_id_role_resource.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_id_role_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_response.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_selector_definition.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_template_creation_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_template_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_template_response.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_template_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_template_update_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_template_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_templated_selector.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_templated_selector.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_type.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_type.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/policy_update_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/policy_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/relative_to_date_time.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/relative_to_date_time.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/remove_from_policy_collection_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/remove_from_policy_collection_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/request_details.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/request_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/requested_action_key.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/requested_action_key.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/resource_details.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/resource_details.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/resource_list_of_access_controlled_resource.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_access_controlled_resource.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/resource_list_of_policy_collection_response.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_policy_collection_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/resource_list_of_policy_response.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_policy_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/resource_list_of_policy_template_response.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_policy_template_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/resource_list_of_user_role_response.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/resource_list_of_user_role_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/role_creation_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/role_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/role_id.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/role_id.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/role_resource_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/role_resource_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/role_response.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/role_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/role_update_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/role_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/selector_definition.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/selector_definition.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/template_metadata.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/template_metadata.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/template_selection.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/template_selection.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/text_operator.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/text_operator.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/user_role_creation_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/user_role_creation_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/user_role_response.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/user_role_response.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/user_role_update_request.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/user_role_update_request.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/models/when_spec.py` & `finbourne_access_sdk-2.0.99/finbourne_access/models/when_spec.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/finbourne_access/rest.py` & `finbourne_access_sdk-2.0.99/finbourne_access/rest.py`

 * *Files identical despite different names*

### Comparing `finbourne_access_sdk-2.0.98/pyproject.toml` & `finbourne_access_sdk-2.0.99/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "finbourne-access-sdk"
-version = "2.0.98"
+version = "2.0.99"
 description = "FINBOURNE Access Management API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/finbourne-access-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Access Management API", "finbourne-access-sdk"]
 packages = [
```

### Comparing `finbourne_access_sdk-2.0.98/PKG-INFO` & `finbourne_access_sdk-2.0.99/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finbourne-access-sdk
-Version: 2.0.98
+Version: 2.0.99
 Summary: FINBOURNE Access Management API
 Home-page: https://github.com/finbourne/finbourne-access-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Access Management API,finbourne-access-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # finbourne-access-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.0.3720
-- Package version: 2.0.98
+- API version: 0.0.3721
+- Package version: 2.0.99
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

