# Comparing `tmp/lusid_workflow_sdk-2.0.8.tar.gz` & `tmp/lusid_workflow_sdk-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_workflow_sdk-2.0.8.tar", max compression
+gzip compressed data, was "lusid_workflow_sdk-2.0.9.tar", max compression
```

## Comparing `lusid_workflow_sdk-2.0.8.tar` & `lusid_workflow_sdk-2.0.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
--rw-r--r--   0        0        0    11754 2023-12-15 15:53:05.268203 lusid_workflow_sdk-2.0.8/README.md
--rw-r--r--   0        0        0     5331 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/__init__.py
--rw-r--r--   0        0        0      223 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/api/__init__.py
--rw-r--r--   0        0        0    57591 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/api/task_definitions_api.py
--rw-r--r--   0        0        0    44649 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/api/tasks_api.py
--rw-r--r--   0        0        0    44961 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/api/workers_api.py
--rw-r--r--   0        0        0    30535 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/api_client.py
--rw-r--r--   0        0        0      852 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/api_response.py
--rw-r--r--   0        0        0    14451 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/configuration.py
--rw-r--r--   0        0        0     5339 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/exceptions.py
--rw-r--r--   0        0        0      294 2023-12-15 15:53:05.265203 lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/__init__.py
--rw-r--r--   0        0        0    30488 2023-12-15 15:53:05.265203 lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/api_client.py
--rw-r--r--   0        0        0     9644 2023-12-15 15:53:05.265203 lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/api_client_factory.py
--rw-r--r--   0        0        0     8012 2023-12-15 15:53:05.265203 lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/api_configuration.py
--rw-r--r--   0        0        0     6868 2023-12-15 15:53:05.265203 lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/configuration_loaders.py
--rw-r--r--   0        0        0     2055 2023-12-15 15:53:05.265203 lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/proxy_config.py
--rw-r--r--   0        0        0    11032 2023-12-15 15:53:05.265203 lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/refreshing_token.py
--rw-r--r--   0        0        0    12707 2023-12-15 15:53:05.265203 lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/rest.py
--rw-r--r--   0        0        0    11573 2023-12-15 15:53:05.265203 lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/retry.py
--rw-r--r--   0        0        0     1653 2023-12-15 15:53:05.265203 lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/socket_keep_alive.py
--rw-r--r--   0        0        0     3886 2023-12-15 15:53:05.265203 lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/tcp_keep_alive_connector.py
--rw-r--r--   0        0        0     4627 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/__init__.py
--rw-r--r--   0        0        0     2711 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/action_definition.py
--rw-r--r--   0        0        0     2708 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/action_definition_response.py
--rw-r--r--   0        0        0     6172 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/action_details.py
--rw-r--r--   0        0        0     6643 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/action_details_response.py
--rw-r--r--   0        0        0     5403 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/create_child_task_configuration.py
--rw-r--r--   0        0        0     3162 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/create_child_tasks_action.py
--rw-r--r--   0        0        0     3763 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/create_child_tasks_action_response.py
--rw-r--r--   0        0        0     7465 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/create_task_definition_request.py
--rw-r--r--   0        0        0     4142 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/create_task_request.py
--rw-r--r--   0        0        0     3969 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/create_worker_request.py
--rw-r--r--   0        0        0     3456 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/deleted_entity_response.py
--rw-r--r--   0        0        0     2158 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/fail.py
--rw-r--r--   0        0        0     2470 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/fail_response.py
--rw-r--r--   0        0        0     2875 2023-12-15 15:53:05.261203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/field_mapping.py
--rw-r--r--   0        0        0     2604 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/get_worker_result_response.py
--rw-r--r--   0        0        0     2338 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/health_check.py
--rw-r--r--   0        0        0     2811 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/health_check_response.py
--rw-r--r--   0        0        0     2720 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/initial_state.py
--rw-r--r--   0        0        0     2259 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/link.py
--rw-r--r--   0        0        0     2604 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/luminesce_view.py
--rw-r--r--   0        0        0     2808 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/luminesce_view_response.py
--rw-r--r--   0        0        0     3854 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/lusid_problem_details.py
--rw-r--r--   0        0        0     4690 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/lusid_validation_problem_details.py
--rw-r--r--   0        0        0     4050 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/paged_resource_list_of_task.py
--rw-r--r--   0        0        0     4171 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/paged_resource_list_of_task_definition.py
--rw-r--r--   0        0        0     4074 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/paged_resource_list_of_worker.py
--rw-r--r--   0        0        0     3314 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/parameter.py
--rw-r--r--   0        0        0     2580 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/parameter_value.py
--rw-r--r--   0        0        0     1866 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/resource_id.py
--rw-r--r--   0        0        0     4010 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/resource_list_of_task.py
--rw-r--r--   0        0        0     2790 2023-12-15 15:53:05.262204 lusid_workflow_sdk-2.0.8/lusid_workflow/models/result_field.py
--rw-r--r--   0        0        0     2290 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/result_matching_pattern.py
--rw-r--r--   0        0        0     5710 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/resultant_child_task_configuration.py
--rw-r--r--   0        0        0     5910 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/run_worker_action.py
--rw-r--r--   0        0        0     6224 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/run_worker_action_response.py
--rw-r--r--   0        0        0     2425 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/run_worker_request.py
--rw-r--r--   0        0        0     2357 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/run_worker_response.py
--rw-r--r--   0        0        0     2113 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/sleep.py
--rw-r--r--   0        0        0     2169 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/sleep_response.py
--rw-r--r--   0        0        0     4394 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/stack.py
--rw-r--r--   0        0        0     8350 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/task.py
--rw-r--r--   0        0        0     7861 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_definition.py
--rw-r--r--   0        0        0     2087 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_definition_version.py
--rw-r--r--   0        0        0     2480 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_field_definition.py
--rw-r--r--   0        0        0     2543 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_instance_field.py
--rw-r--r--   0        0        0     2276 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_state_definition.py
--rw-r--r--   0        0        0     3412 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_summary.py
--rw-r--r--   0        0        0     4803 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_transition_definition.py
--rw-r--r--   0        0        0     2725 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/transition_trigger_definition.py
--rw-r--r--   0        0        0     2713 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/trigger_parent_task_action.py
--rw-r--r--   0        0        0     2907 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/trigger_parent_task_action_response.py
--rw-r--r--   0        0        0     1948 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/trigger_schema.py
--rw-r--r--   0        0        0     7127 2023-12-15 15:53:05.263203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/update_task_definition_request.py
--rw-r--r--   0        0        0     3585 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/update_task_request.py
--rw-r--r--   0        0        0     5121 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/version_info.py
--rw-r--r--   0        0        0     6134 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/worker.py
--rw-r--r--   0        0        0     6354 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/worker_configuration.py
--rw-r--r--   0        0        0     6935 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/worker_configuration_response.py
--rw-r--r--   0        0        0     4201 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/models/worker_status_triggers.py
--rw-r--r--   0        0        0        0 2023-12-15 15:53:05.264203 lusid_workflow_sdk-2.0.8/lusid_workflow/py.typed
--rw-r--r--   0        0        0    10029 2023-12-15 15:53:05.265203 lusid_workflow_sdk-2.0.8/lusid_workflow/rest.py
--rw-r--r--   0        0        0      856 2023-12-15 15:53:05.268203 lusid_workflow_sdk-2.0.8/pyproject.toml
--rw-r--r--   0        0        0    12800 1970-01-01 00:00:00.000000 lusid_workflow_sdk-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11754 2023-12-18 10:59:03.578883 lusid_workflow_sdk-2.0.9/README.md
+-rw-r--r--   0        0        0     5331 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/__init__.py
+-rw-r--r--   0        0        0      223 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/api/__init__.py
+-rw-r--r--   0        0        0    57591 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/api/task_definitions_api.py
+-rw-r--r--   0        0        0    44649 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/api/tasks_api.py
+-rw-r--r--   0        0        0    44961 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/api/workers_api.py
+-rw-r--r--   0        0        0    30535 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/api_client.py
+-rw-r--r--   0        0        0      852 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/api_response.py
+-rw-r--r--   0        0        0    14451 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/configuration.py
+-rw-r--r--   0        0        0     5339 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/exceptions.py
+-rw-r--r--   0        0        0      294 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/__init__.py
+-rw-r--r--   0        0        0    30488 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/api_client.py
+-rw-r--r--   0        0        0     9644 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/api_client_factory.py
+-rw-r--r--   0        0        0     8012 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/api_configuration.py
+-rw-r--r--   0        0        0     6868 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/configuration_loaders.py
+-rw-r--r--   0        0        0     2055 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/proxy_config.py
+-rw-r--r--   0        0        0    11032 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/refreshing_token.py
+-rw-r--r--   0        0        0    12707 2023-12-18 10:59:03.575883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/rest.py
+-rw-r--r--   0        0        0    11573 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/retry.py
+-rw-r--r--   0        0        0     1653 2023-12-18 10:59:03.575883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/socket_keep_alive.py
+-rw-r--r--   0        0        0     3886 2023-12-18 10:59:03.575883 lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/tcp_keep_alive_connector.py
+-rw-r--r--   0        0        0     4627 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/__init__.py
+-rw-r--r--   0        0        0     2711 2023-12-18 10:59:03.570883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_definition.py
+-rw-r--r--   0        0        0     2708 2023-12-18 10:59:03.570883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_definition_response.py
+-rw-r--r--   0        0        0     6172 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_details.py
+-rw-r--r--   0        0        0     6643 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_details_response.py
+-rw-r--r--   0        0        0     5403 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_child_task_configuration.py
+-rw-r--r--   0        0        0     3162 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_child_tasks_action.py
+-rw-r--r--   0        0        0     3763 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_child_tasks_action_response.py
+-rw-r--r--   0        0        0     7465 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_task_definition_request.py
+-rw-r--r--   0        0        0     4142 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_task_request.py
+-rw-r--r--   0        0        0     3969 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_worker_request.py
+-rw-r--r--   0        0        0     3456 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/deleted_entity_response.py
+-rw-r--r--   0        0        0     2158 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/fail.py
+-rw-r--r--   0        0        0     2470 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/fail_response.py
+-rw-r--r--   0        0        0     2875 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/field_mapping.py
+-rw-r--r--   0        0        0     2604 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/get_worker_result_response.py
+-rw-r--r--   0        0        0     2338 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/health_check.py
+-rw-r--r--   0        0        0     2811 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/health_check_response.py
+-rw-r--r--   0        0        0     2720 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/initial_state.py
+-rw-r--r--   0        0        0     2259 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/link.py
+-rw-r--r--   0        0        0     2604 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/luminesce_view.py
+-rw-r--r--   0        0        0     2808 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/luminesce_view_response.py
+-rw-r--r--   0        0        0     3854 2023-12-18 10:59:03.571883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/lusid_problem_details.py
+-rw-r--r--   0        0        0     4690 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/lusid_validation_problem_details.py
+-rw-r--r--   0        0        0     4050 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/paged_resource_list_of_task.py
+-rw-r--r--   0        0        0     4171 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/paged_resource_list_of_task_definition.py
+-rw-r--r--   0        0        0     4074 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/paged_resource_list_of_worker.py
+-rw-r--r--   0        0        0     3314 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/parameter.py
+-rw-r--r--   0        0        0     2580 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/parameter_value.py
+-rw-r--r--   0        0        0     1866 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/resource_id.py
+-rw-r--r--   0        0        0     4010 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/resource_list_of_task.py
+-rw-r--r--   0        0        0     2790 2023-12-18 10:59:03.570883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/result_field.py
+-rw-r--r--   0        0        0     2290 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/result_matching_pattern.py
+-rw-r--r--   0        0        0     5710 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/resultant_child_task_configuration.py
+-rw-r--r--   0        0        0     5910 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_action.py
+-rw-r--r--   0        0        0     6224 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_action_response.py
+-rw-r--r--   0        0        0     2425 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_request.py
+-rw-r--r--   0        0        0     2357 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_response.py
+-rw-r--r--   0        0        0     2113 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/sleep.py
+-rw-r--r--   0        0        0     2169 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/sleep_response.py
+-rw-r--r--   0        0        0     4394 2023-12-18 10:59:03.572883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/stack.py
+-rw-r--r--   0        0        0     8350 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task.py
+-rw-r--r--   0        0        0     7861 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_definition.py
+-rw-r--r--   0        0        0     2087 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_definition_version.py
+-rw-r--r--   0        0        0     2480 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_field_definition.py
+-rw-r--r--   0        0        0     2543 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_instance_field.py
+-rw-r--r--   0        0        0     2276 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_state_definition.py
+-rw-r--r--   0        0        0     3412 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_summary.py
+-rw-r--r--   0        0        0     4803 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_transition_definition.py
+-rw-r--r--   0        0        0     2725 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/transition_trigger_definition.py
+-rw-r--r--   0        0        0     2713 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/trigger_parent_task_action.py
+-rw-r--r--   0        0        0     2907 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/trigger_parent_task_action_response.py
+-rw-r--r--   0        0        0     1948 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/trigger_schema.py
+-rw-r--r--   0        0        0     7127 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/update_task_definition_request.py
+-rw-r--r--   0        0        0     3585 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/update_task_request.py
+-rw-r--r--   0        0        0     5121 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/version_info.py
+-rw-r--r--   0        0        0     6134 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker.py
+-rw-r--r--   0        0        0     6354 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker_configuration.py
+-rw-r--r--   0        0        0     6935 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker_configuration_response.py
+-rw-r--r--   0        0        0     4201 2023-12-18 10:59:03.573883 lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker_status_triggers.py
+-rw-r--r--   0        0        0        0 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/py.typed
+-rw-r--r--   0        0        0    10029 2023-12-18 10:59:03.574883 lusid_workflow_sdk-2.0.9/lusid_workflow/rest.py
+-rw-r--r--   0        0        0      856 2023-12-18 10:59:03.578883 lusid_workflow_sdk-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0    12800 1970-01-01 00:00:00.000000 lusid_workflow_sdk-2.0.9/PKG-INFO
```

### Comparing `lusid_workflow_sdk-2.0.8/README.md` & `lusid_workflow_sdk-2.0.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.673
-- Package version: 2.0.8
+- API version: 0.1.674
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/__init__.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/api/task_definitions_api.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/api/task_definitions_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/api/tasks_api.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/api/tasks_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/api/workers_api.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/api/workers_api.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/api_client.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/api_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/api_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/configuration.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
         :return: The report for debugging.
         """
         package_version = version("lusid_workflow-sdk")
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.1.673\n"\
+               "Version of the API: 0.1.674\n"\
                "SDK Package Version: {package_version}".\
                format(env=sys.platform, pyversion=sys.version, package_version=package_version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/exceptions.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/exceptions.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/api_client.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/api_client.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/api_client_factory.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/api_client_factory.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/api_configuration.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/api_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/configuration_loaders.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/configuration_loaders.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/proxy_config.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/proxy_config.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/refreshing_token.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/refreshing_token.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/rest.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/retry.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/retry.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/socket_keep_alive.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/socket_keep_alive.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/extensions/tcp_keep_alive_connector.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/extensions/tcp_keep_alive_connector.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/__init__.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/action_definition.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/action_definition_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_definition_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/action_details.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_details.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/action_details_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/action_details_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/create_child_task_configuration.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_child_task_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/create_child_tasks_action.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_child_tasks_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/create_child_tasks_action_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_child_tasks_action_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/create_task_definition_request.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_task_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/create_task_request.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_task_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/create_worker_request.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/create_worker_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/deleted_entity_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/deleted_entity_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/fail.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/fail.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/fail_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/fail_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/field_mapping.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/field_mapping.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/get_worker_result_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/get_worker_result_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/health_check.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/health_check.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/health_check_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/health_check_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/initial_state.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/initial_state.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/link.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/link.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/luminesce_view.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/luminesce_view.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/luminesce_view_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/luminesce_view_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/lusid_problem_details.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/lusid_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/lusid_validation_problem_details.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/lusid_validation_problem_details.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/paged_resource_list_of_task.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/paged_resource_list_of_task.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/paged_resource_list_of_task_definition.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/paged_resource_list_of_task_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/paged_resource_list_of_worker.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/paged_resource_list_of_worker.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/parameter.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/parameter.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/parameter_value.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/parameter_value.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/resource_id.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/resource_id.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/resource_list_of_task.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/resource_list_of_task.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/result_field.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/result_field.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/result_matching_pattern.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/result_matching_pattern.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/resultant_child_task_configuration.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/resultant_child_task_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/run_worker_action.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/run_worker_action_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_action_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/run_worker_request.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/run_worker_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/run_worker_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/sleep.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/sleep.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/sleep_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/sleep_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/stack.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/stack.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/task.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_definition.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_definition_version.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_definition_version.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_field_definition.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_field_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_instance_field.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_instance_field.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_state_definition.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_state_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_summary.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_summary.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/task_transition_definition.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/task_transition_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/transition_trigger_definition.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/transition_trigger_definition.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/trigger_parent_task_action.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/trigger_parent_task_action.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/trigger_parent_task_action_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/trigger_parent_task_action_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/trigger_schema.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/trigger_schema.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/update_task_definition_request.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/update_task_definition_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/update_task_request.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/update_task_request.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/version_info.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/version_info.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/worker.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/worker_configuration.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker_configuration.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/worker_configuration_response.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker_configuration_response.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/models/worker_status_triggers.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/models/worker_status_triggers.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/lusid_workflow/rest.py` & `lusid_workflow_sdk-2.0.9/lusid_workflow/rest.py`

 * *Files identical despite different names*

### Comparing `lusid_workflow_sdk-2.0.8/pyproject.toml` & `lusid_workflow_sdk-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lusid-workflow-sdk"
-version = "2.0.8"
+version = "2.0.9"
 description = "FINBOURNE Workflow API"
 authors = ["FINBOURNE Technology <info@finbourne.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/finbourne/workflow-sdk-python"
 keywords = ["OpenAPI", "OpenAPI-Generator", "FINBOURNE Workflow API", "lusid-workflow-sdk"]
 packages = [
```

### Comparing `lusid_workflow_sdk-2.0.8/PKG-INFO` & `lusid_workflow_sdk-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-workflow-sdk
-Version: 2.0.8
+Version: 2.0.9
 Summary: FINBOURNE Workflow API
 Home-page: https://github.com/finbourne/workflow-sdk-python
 License: MIT
 Keywords: OpenAPI,OpenAPI-Generator,FINBOURNE Workflow API,lusid-workflow-sdk
 Author: FINBOURNE Technology
 Author-email: info@finbourne.com
 Requires-Python: >=3.8,<4.0
@@ -25,16 +25,16 @@
 Description-Content-Type: text/markdown
 
 # lusid-workflow-sdk
 FINBOURNE Technology
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.1.673
-- Package version: 2.0.8
+- API version: 0.1.674
+- Package version: 2.0.9
 - Build package: org.openapitools.codegen.languages.PythonClientCodegen
 For more information, please visit [https://www.finbourne.com](https://www.finbourne.com)
 
 ## Requirements.
 
 Python 3.7+
```

