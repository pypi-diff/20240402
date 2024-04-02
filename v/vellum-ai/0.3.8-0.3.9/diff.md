# Comparing `tmp/vellum_ai-0.3.8.tar.gz` & `tmp/vellum_ai-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vellum_ai-0.3.8.tar", max compression
+gzip compressed data, was "vellum_ai-0.3.9.tar", max compression
```

## Comparing `vellum_ai-0.3.8.tar` & `vellum_ai-0.3.9.tar`

### file list

```diff
@@ -1,304 +1,311 @@
--rw-r--r--   0        0        0     1073 2024-03-01 23:22:53.859043 vellum_ai-0.3.8/LICENSE
--rw-r--r--   0        0        0     2980 2024-03-01 23:22:53.859043 vellum_ai-0.3.8/README.md
--rw-r--r--   0        0        0      401 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/pyproject.toml
--rw-r--r--   0        0        0    26703 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/__init__.py
--rw-r--r--   0        0        0    61957 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/client.py
--rw-r--r--   0        0        0      519 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/core/__init__.py
--rw-r--r--   0        0        0      426 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/core/api_error.py
--rw-r--r--   0        0        0     1212 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/core/datetime_utils.py
--rw-r--r--   0        0        0     3799 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      498 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/environment.py
--rw-r--r--   0        0        0      402 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/errors/bad_request_error.py
--rw-r--r--   0        0        0      327 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/errors/conflict_error.py
--rw-r--r--   0        0        0      247 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/errors/not_found_error.py
--rw-r--r--   0        0        0        0 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/py.typed
--rw-r--r--   0        0        0      675 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/__init__.py
--rw-r--r--   0        0        0      157 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/deployments/__init__.py
--rw-r--r--   0        0        0    10752 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/deployments/client.py
--rw-r--r--   0        0        0      183 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/deployments/types/__init__.py
--rw-r--r--   0        0        0      518 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/deployments/types/deployments_list_request_status.py
--rw-r--r--   0        0        0       65 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/document_indexes/__init__.py
--rw-r--r--   0        0        0    10894 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/document_indexes/client.py
--rw-r--r--   0        0        0       65 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/documents/__init__.py
--rw-r--r--   0        0        0    17776 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/documents/client.py
--rw-r--r--   0        0        0       65 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/folder_entities/__init__.py
--rw-r--r--   0        0        0     3748 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/folder_entities/client.py
--rw-r--r--   0        0        0       65 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/model_versions/__init__.py
--rw-r--r--   0        0        0     3053 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/model_versions/client.py
--rw-r--r--   0        0        0       65 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/registered_prompts/__init__.py
--rw-r--r--   0        0        0    12451 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/registered_prompts/client.py
--rw-r--r--   0        0        0       65 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/sandboxes/__init__.py
--rw-r--r--   0        0        0     9182 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/sandboxes/client.py
--rw-r--r--   0        0        0       65 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/test_suites/__init__.py
--rw-r--r--   0        0        0     8693 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/test_suites/client.py
--rw-r--r--   0        0        0      173 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/workflow_deployments/__init__.py
--rw-r--r--   0        0        0     6711 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/workflow_deployments/client.py
--rw-r--r--   0        0        0      208 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/workflow_deployments/types/__init__.py
--rw-r--r--   0        0        0      542 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/resources/workflow_deployments/types/workflow_deployments_list_request_status.py
--rw-r--r--   0        0        0    35563 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/__init__.py
--rw-r--r--   0        0        0     1003 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/api_node_result.py
--rw-r--r--   0        0        0     1125 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/api_node_result_data.py
--rw-r--r--   0        0        0     1050 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/array_chat_message_content.py
--rw-r--r--   0        0        0     1221 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/array_chat_message_content_item.py
--rw-r--r--   0        0        0     1345 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/array_chat_message_content_item_request.py
--rw-r--r--   0        0        0     1079 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/array_chat_message_content_request.py
--rw-r--r--   0        0        0      138 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/array_enum.py
--rw-r--r--   0        0        0     2451 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/array_variable_value_item.py
--rw-r--r--   0        0        0     1051 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/block_type_enum.py
--rw-r--r--   0        0        0      151 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/chat_history_enum.py
--rw-r--r--   0        0        0     1130 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/chat_history_input_request.py
--rw-r--r--   0        0        0      958 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/chat_history_variable_value.py
--rw-r--r--   0        0        0     1060 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/chat_message.py
--rw-r--r--   0        0        0     1466 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/chat_message_content.py
--rw-r--r--   0        0        0     1630 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/chat_message_content_request.py
--rw-r--r--   0        0        0     1089 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/chat_message_request.py
--rw-r--r--   0        0        0      914 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/chat_message_role.py
--rw-r--r--   0        0        0      980 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/code_execution_node_chat_history_result.py
--rw-r--r--   0        0        0      961 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/code_execution_node_error_result.py
--rw-r--r--   0        0        0      939 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/code_execution_node_json_result.py
--rw-r--r--   0        0        0      918 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/code_execution_node_number_result.py
--rw-r--r--   0        0        0     1054 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/code_execution_node_result.py
--rw-r--r--   0        0        0      989 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/code_execution_node_result_data.py
--rw-r--r--   0        0        0     2386 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/code_execution_node_result_output.py
--rw-r--r--   0        0        0      985 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/code_execution_node_search_results_result.py
--rw-r--r--   0        0        0      916 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/code_execution_node_string_result.py
--rw-r--r--   0        0        0     1042 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/conditional_node_result.py
--rw-r--r--   0        0        0      911 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/conditional_node_result_data.py
--rw-r--r--   0        0        0      918 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/deployment_provider_payload_response.py
--rw-r--r--   0        0        0     2000 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/deployment_read.py
--rw-r--r--   0        0        0     1634 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/document_document_to_document_index.py
--rw-r--r--   0        0        0     1867 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/document_index_read.py
--rw-r--r--   0        0        0     2264 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/document_read.py
--rw-r--r--   0        0        0      144 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/document_status.py
--rw-r--r--   0        0        0     2135 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/enriched_normalized_completion.py
--rw-r--r--   0        0        0      539 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/entity_status.py
--rw-r--r--   0        0        0      799 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/environment_enum.py
--rw-r--r--   0        0        0      138 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/error_enum.py
--rw-r--r--   0        0        0      939 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/error_variable_value.py
--rw-r--r--   0        0        0      958 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/execute_prompt_api_error_response.py
--rw-r--r--   0        0        0     1523 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/execute_prompt_event.py
--rw-r--r--   0        0        0      871 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/execute_prompt_response.py
--rw-r--r--   0        0        0      957 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/execute_workflow_error_response.py
--rw-r--r--   0        0        0     1091 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/execute_workflow_response.py
--rw-r--r--   0        0        0      963 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/execute_workflow_stream_error_response.py
--rw-r--r--   0        0        0     1024 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0      726 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/finish_reason_enum.py
--rw-r--r--   0        0        0      146 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/fulfilled_enum.py
--rw-r--r--   0        0        0     1248 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/fulfilled_execute_prompt_event.py
--rw-r--r--   0        0        0     1450 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/fulfilled_execute_prompt_response.py
--rw-r--r--   0        0        0     1109 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0     1012 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/fulfilled_function_call.py
--rw-r--r--   0        0        0     1145 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/fulfilled_prompt_execution_meta.py
--rw-r--r--   0        0        0     1302 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/fulfilled_workflow_node_result_event.py
--rw-r--r--   0        0        0      770 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/function_call.py
--rw-r--r--   0        0        0     1085 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/function_call_chat_message_content.py
--rw-r--r--   0        0        0     1114 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/function_call_chat_message_content_request.py
--rw-r--r--   0        0        0     1026 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/function_call_chat_message_content_value.py
--rw-r--r--   0        0        0     1033 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/function_call_chat_message_content_value_request.py
--rw-r--r--   0        0        0      153 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/function_call_enum.py
--rw-r--r--   0        0        0      932 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/function_call_variable_value.py
--rw-r--r--   0        0        0      950 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/generate_error_response.py
--rw-r--r--   0        0        0     1117 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/generate_options_request.py
--rw-r--r--   0        0        0     1581 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/generate_request.py
--rw-r--r--   0        0        0     1342 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/generate_response.py
--rw-r--r--   0        0        0     1397 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/generate_result.py
--rw-r--r--   0        0        0     1111 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/generate_result_data.py
--rw-r--r--   0        0        0      959 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/generate_result_error.py
--rw-r--r--   0        0        0      954 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/generate_stream_response.py
--rw-r--r--   0        0        0     1107 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/generate_stream_result.py
--rw-r--r--   0        0        0     1011 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/generate_stream_result_data.py
--rw-r--r--   0        0        0      995 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/image_chat_message_content.py
--rw-r--r--   0        0        0     1024 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/image_chat_message_content_request.py
--rw-r--r--   0        0        0      138 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/image_enum.py
--rw-r--r--   0        0        0     1181 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/indexing_state_enum.py
--rw-r--r--   0        0        0      146 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/initiated_enum.py
--rw-r--r--   0        0        0     1147 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/initiated_execute_prompt_event.py
--rw-r--r--   0        0        0     1173 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/initiated_prompt_execution_meta.py
--rw-r--r--   0        0        0     1323 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/initiated_workflow_node_result_event.py
--rw-r--r--   0        0        0      136 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/json_enum.py
--rw-r--r--   0        0        0     1057 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/json_input_request.py
--rw-r--r--   0        0        0      917 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/json_variable_value.py
--rw-r--r--   0        0        0     4282 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/logical_operator.py
--rw-r--r--   0        0        0      490 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/logprobs_enum.py
--rw-r--r--   0        0        0     1333 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/metadata_filter_config_request.py
--rw-r--r--   0        0        0      528 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/metadata_filter_rule_combinator.py
--rw-r--r--   0        0        0     1349 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/metadata_filter_rule_request.py
--rw-r--r--   0        0        0     1356 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/model_version_build_config.py
--rw-r--r--   0        0        0     1632 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/model_version_exec_config.py
--rw-r--r--   0        0        0     1247 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/model_version_exec_config_parameters.py
--rw-r--r--   0        0        0     2575 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/model_version_read.py
--rw-r--r--   0        0        0     1032 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/model_version_read_status_enum.py
--rw-r--r--   0        0        0     1217 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/model_version_sandbox_snapshot.py
--rw-r--r--   0        0        0     1014 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/named_test_case_chat_history_variable_value_request.py
--rw-r--r--   0        0        0      995 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/named_test_case_error_variable_value_request.py
--rw-r--r--   0        0        0      951 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/named_test_case_json_variable_value_request.py
--rw-r--r--   0        0        0      930 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/named_test_case_number_variable_value_request.py
--rw-r--r--   0        0        0     1019 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/named_test_case_search_results_variable_value_request.py
--rw-r--r--   0        0        0      928 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/named_test_case_string_variable_value_request.py
--rw-r--r--   0        0        0     2630 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/named_test_case_variable_value_request.py
--rw-r--r--   0        0        0     1015 2024-03-01 23:22:53.863044 vellum_ai-0.3.8/src/vellum/types/node_input_compiled_array_value.py
--rw-r--r--   0        0        0     1003 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_input_compiled_chat_history_value.py
--rw-r--r--   0        0        0      984 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_input_compiled_error_value.py
--rw-r--r--   0        0        0      962 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_input_compiled_json_value.py
--rw-r--r--   0        0        0      941 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_input_compiled_number_value.py
--rw-r--r--   0        0        0     1008 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_input_compiled_search_results_value.py
--rw-r--r--   0        0        0      939 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_input_compiled_string_value.py
--rw-r--r--   0        0        0     2730 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_input_variable_compiled_value.py
--rw-r--r--   0        0        0     1004 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_output_compiled_array_value.py
--rw-r--r--   0        0        0      992 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_output_compiled_chat_history_value.py
--rw-r--r--   0        0        0      973 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_output_compiled_error_value.py
--rw-r--r--   0        0        0      979 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_output_compiled_function_value.py
--rw-r--r--   0        0        0      951 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_output_compiled_json_value.py
--rw-r--r--   0        0        0      930 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_output_compiled_number_value.py
--rw-r--r--   0        0        0      997 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_output_compiled_search_results_value.py
--rw-r--r--   0        0        0      928 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_output_compiled_string_value.py
--rw-r--r--   0        0        0     3015 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/node_output_compiled_value.py
--rw-r--r--   0        0        0     1013 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/normalized_log_probs.py
--rw-r--r--   0        0        0     1014 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/normalized_token_log_probs.py
--rw-r--r--   0        0        0      140 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/number_enum.py
--rw-r--r--   0        0        0      896 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/number_variable_value.py
--rw-r--r--   0        0        0     1087 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/paginated_slim_deployment_read_list.py
--rw-r--r--   0        0        0     1062 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/paginated_slim_document_list.py
--rw-r--r--   0        0        0     1103 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/paginated_slim_workflow_deployment_list.py
--rw-r--r--   0        0        0      752 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/processing_failure_reason_enum.py
--rw-r--r--   0        0        0      962 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/processing_state_enum.py
--rw-r--r--   0        0        0     1819 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/prompt_deployment_expand_meta_request_request.py
--rw-r--r--   0        0        0     1159 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/prompt_deployment_input_request.py
--rw-r--r--   0        0        0     1266 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/prompt_execution_meta.py
--rw-r--r--   0        0        0     1017 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/prompt_node_result.py
--rw-r--r--   0        0        0      987 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/prompt_node_result_data.py
--rw-r--r--   0        0        0     1336 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/prompt_output.py
--rw-r--r--   0        0        0     1164 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/prompt_template_block.py
--rw-r--r--   0        0        0      983 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/prompt_template_block_data.py
--rw-r--r--   0        0        0     1012 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/prompt_template_block_data_request.py
--rw-r--r--   0        0        0     1586 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/prompt_template_block_properties.py
--rw-r--r--   0        0        0     1622 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/prompt_template_block_properties_request.py
--rw-r--r--   0        0        0     1200 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/prompt_template_block_request.py
--rw-r--r--   0        0        0     2516 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/provider_enum.py
--rw-r--r--   0        0        0     1192 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/raw_prompt_execution_overrides_request.py
--rw-r--r--   0        0        0      956 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/register_prompt_error_response.py
--rw-r--r--   0        0        0     1215 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/register_prompt_model_parameters_request.py
--rw-r--r--   0        0        0     1035 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/register_prompt_prompt.py
--rw-r--r--   0        0        0     1269 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/register_prompt_prompt_info_request.py
--rw-r--r--   0        0        0     1926 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/register_prompt_response.py
--rw-r--r--   0        0        0     1149 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/registered_prompt_deployment.py
--rw-r--r--   0        0        0     1020 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/registered_prompt_input_variable_request.py
--rw-r--r--   0        0        0     1057 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/registered_prompt_model_version.py
--rw-r--r--   0        0        0     1040 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/registered_prompt_sandbox.py
--rw-r--r--   0        0        0      960 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/registered_prompt_sandbox_snapshot.py
--rw-r--r--   0        0        0      144 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/rejected_enum.py
--rw-r--r--   0        0        0     1172 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/rejected_execute_prompt_event.py
--rw-r--r--   0        0        0     1410 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/rejected_execute_prompt_response.py
--rw-r--r--   0        0        0     1123 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/rejected_execute_workflow_workflow_result_event.py
--rw-r--r--   0        0        0     1051 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/rejected_function_call.py
--rw-r--r--   0        0        0     1144 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/rejected_prompt_execution_meta.py
--rw-r--r--   0        0        0     1246 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/rejected_workflow_node_result_event.py
--rw-r--r--   0        0        0     1098 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/sandbox_scenario.py
--rw-r--r--   0        0        0     1108 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/scenario_input.py
--rw-r--r--   0        0        0     1137 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/scenario_input_request.py
--rw-r--r--   0        0        0      580 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/scenario_input_type_enum.py
--rw-r--r--   0        0        0      948 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_error_response.py
--rw-r--r--   0        0        0     1221 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_filters_request.py
--rw-r--r--   0        0        0     1017 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_node_result.py
--rw-r--r--   0        0        0     1159 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_node_result_data.py
--rw-r--r--   0        0        0     1579 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_request_options_request.py
--rw-r--r--   0        0        0     1071 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_response.py
--rw-r--r--   0        0        0     1306 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_result.py
--rw-r--r--   0        0        0     1418 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_result_document.py
--rw-r--r--   0        0        0     1357 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_result_document_request.py
--rw-r--r--   0        0        0      970 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_result_merging_request.py
--rw-r--r--   0        0        0     1335 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_result_request.py
--rw-r--r--   0        0        0      155 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_results_enum.py
--rw-r--r--   0        0        0      963 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_results_variable_value.py
--rw-r--r--   0        0        0     1117 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/search_weights_request.py
--rw-r--r--   0        0        0     1811 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/slim_deployment_read.py
--rw-r--r--   0        0        0     3074 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/slim_document.py
--rw-r--r--   0        0        0     2205 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/slim_workflow_deployment.py
--rw-r--r--   0        0        0      146 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/streaming_enum.py
--rw-r--r--   0        0        0     1393 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/streaming_execute_prompt_event.py
--rw-r--r--   0        0        0     1043 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/streaming_prompt_execution_meta.py
--rw-r--r--   0        0        0     1322 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/streaming_workflow_node_result_event.py
--rw-r--r--   0        0        0      950 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/string_chat_message_content.py
--rw-r--r--   0        0        0      957 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/string_chat_message_content_request.py
--rw-r--r--   0        0        0      140 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/string_enum.py
--rw-r--r--   0        0        0     1035 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/string_input_request.py
--rw-r--r--   0        0        0      894 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/string_variable_value.py
--rw-r--r--   0        0        0     1787 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/submit_completion_actual_request.py
--rw-r--r--   0        0        0      895 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/submit_completion_actuals_error_response.py
--rw-r--r--   0        0        0     1413 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/submit_workflow_execution_actual_request.py
--rw-r--r--   0        0        0      977 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/templating_node_chat_history_result.py
--rw-r--r--   0        0        0      958 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/templating_node_error_result.py
--rw-r--r--   0        0        0      936 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/templating_node_json_result.py
--rw-r--r--   0        0        0      915 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/templating_node_number_result.py
--rw-r--r--   0        0        0     1037 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/templating_node_result.py
--rw-r--r--   0        0        0      976 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/templating_node_result_data.py
--rw-r--r--   0        0        0     2287 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/templating_node_result_output.py
--rw-r--r--   0        0        0      982 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/templating_node_search_results_result.py
--rw-r--r--   0        0        0      913 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/templating_node_string_result.py
--rw-r--r--   0        0        0     1108 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/terminal_node_chat_history_result.py
--rw-r--r--   0        0        0     1089 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/terminal_node_error_result.py
--rw-r--r--   0        0        0     1067 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/terminal_node_json_result.py
--rw-r--r--   0        0        0     1046 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/terminal_node_number_result.py
--rw-r--r--   0        0        0     1027 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/terminal_node_result.py
--rw-r--r--   0        0        0      968 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/terminal_node_result_data.py
--rw-r--r--   0        0        0     2225 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/terminal_node_result_output.py
--rw-r--r--   0        0        0     1113 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/terminal_node_search_results_result.py
--rw-r--r--   0        0        0     1044 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/terminal_node_string_result.py
--rw-r--r--   0        0        0      987 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/test_case_chat_history_variable_value.py
--rw-r--r--   0        0        0      968 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/test_case_error_variable_value.py
--rw-r--r--   0        0        0      946 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/test_case_json_variable_value.py
--rw-r--r--   0        0        0      925 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/test_case_number_variable_value.py
--rw-r--r--   0        0        0      992 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/test_case_search_results_variable_value.py
--rw-r--r--   0        0        0      923 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/test_case_string_variable_value.py
--rw-r--r--   0        0        0     2246 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/test_case_variable_value.py
--rw-r--r--   0        0        0     1092 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/test_suite_test_case.py
--rw-r--r--   0        0        0      886 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/upload_document_error_response.py
--rw-r--r--   0        0        0      956 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/upload_document_response.py
--rw-r--r--   0        0        0      957 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/vellum_error.py
--rw-r--r--   0        0        0      969 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/vellum_error_code_enum.py
--rw-r--r--   0        0        0      964 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/vellum_error_request.py
--rw-r--r--   0        0        0      927 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/vellum_image.py
--rw-r--r--   0        0        0      934 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/vellum_image_request.py
--rw-r--r--   0        0        0      964 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/vellum_variable.py
--rw-r--r--   0        0        0     1855 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/vellum_variable_type.py
--rw-r--r--   0        0        0     2211 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_deployment_read.py
--rw-r--r--   0        0        0     1001 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_event_error.py
--rw-r--r--   0        0        0     2014 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_execution_actual_chat_history_request.py
--rw-r--r--   0        0        0     1951 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_execution_actual_json_request.py
--rw-r--r--   0        0        0     1928 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_execution_actual_string_request.py
--rw-r--r--   0        0        0     1921 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_execution_event_error_code.py
--rw-r--r--   0        0        0      567 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_execution_event_type.py
--rw-r--r--   0        0        0     1145 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_execution_node_result_event.py
--rw-r--r--   0        0        0     1140 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_execution_workflow_result_event.py
--rw-r--r--   0        0        0     2384 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_node_result_data.py
--rw-r--r--   0        0        0     1632 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_node_result_event.py
--rw-r--r--   0        0        0     1035 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_node_result_event_state.py
--rw-r--r--   0        0        0     2643 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_output.py
--rw-r--r--   0        0        0     1116 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_output_chat_history.py
--rw-r--r--   0        0        0     1091 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_output_error.py
--rw-r--r--   0        0        0     1108 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_output_function_call.py
--rw-r--r--   0        0        0     1091 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_output_image.py
--rw-r--r--   0        0        0     1067 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_output_json.py
--rw-r--r--   0        0        0     1048 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_output_number.py
--rw-r--r--   0        0        0     1123 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_output_search_results.py
--rw-r--r--   0        0        0     1046 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_output_string.py
--rw-r--r--   0        0        0     1146 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_request_chat_history_input_request.py
--rw-r--r--   0        0        0     1666 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_request_input_request.py
--rw-r--r--   0        0        0     1075 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_request_json_input_request.py
--rw-r--r--   0        0        0     1056 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_request_number_input_request.py
--rw-r--r--   0        0        0     1054 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_request_string_input_request.py
--rw-r--r--   0        0        0     1347 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_result_event.py
--rw-r--r--   0        0        0     2500 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data.py
--rw-r--r--   0        0        0     1397 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data_chat_history.py
--rw-r--r--   0        0        0     1372 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data_error.py
--rw-r--r--   0        0        0     1348 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data_json.py
--rw-r--r--   0        0        0     1329 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data_number.py
--rw-r--r--   0        0        0     1404 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data_search_results.py
--rw-r--r--   0        0        0     1478 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data_string.py
--rw-r--r--   0        0        0      873 2024-03-01 23:22:53.867044 vellum_ai-0.3.8/src/vellum/types/workflow_stream_event.py
--rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 vellum_ai-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/LICENSE
+-rw-r--r--   0        0        0     2980 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/README.md
+-rw-r--r--   0        0        0      401 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0    27647 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/__init__.py
+-rw-r--r--   0        0        0    61957 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/client.py
+-rw-r--r--   0        0        0      519 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/core/api_error.py
+-rw-r--r--   0        0        0     1212 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/core/datetime_utils.py
+-rw-r--r--   0        0        0     3799 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      498 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/environment.py
+-rw-r--r--   0        0        0      402 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/errors/bad_request_error.py
+-rw-r--r--   0        0        0      327 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/errors/conflict_error.py
+-rw-r--r--   0        0        0      247 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/errors/not_found_error.py
+-rw-r--r--   0        0        0        0 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/py.typed
+-rw-r--r--   0        0        0      675 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/__init__.py
+-rw-r--r--   0        0        0      157 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/deployments/__init__.py
+-rw-r--r--   0        0        0    10752 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/deployments/client.py
+-rw-r--r--   0        0        0      183 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/deployments/types/__init__.py
+-rw-r--r--   0        0        0      518 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/deployments/types/deployments_list_request_status.py
+-rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/document_indexes/__init__.py
+-rw-r--r--   0        0        0    10894 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/document_indexes/client.py
+-rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/documents/__init__.py
+-rw-r--r--   0        0        0    17776 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/folder_entities/__init__.py
+-rw-r--r--   0        0        0     3748 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/folder_entities/client.py
+-rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/model_versions/__init__.py
+-rw-r--r--   0        0        0     3053 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/model_versions/client.py
+-rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/registered_prompts/__init__.py
+-rw-r--r--   0        0        0    12451 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/registered_prompts/client.py
+-rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/sandboxes/__init__.py
+-rw-r--r--   0        0        0     9182 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/sandboxes/client.py
+-rw-r--r--   0        0        0       65 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/test_suites/__init__.py
+-rw-r--r--   0        0        0     8693 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/test_suites/client.py
+-rw-r--r--   0        0        0      173 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/workflow_deployments/__init__.py
+-rw-r--r--   0        0        0     6711 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/workflow_deployments/client.py
+-rw-r--r--   0        0        0      208 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/workflow_deployments/types/__init__.py
+-rw-r--r--   0        0        0      542 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/resources/workflow_deployments/types/workflow_deployments_list_request_status.py
+-rw-r--r--   0        0        0    36776 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/__init__.py
+-rw-r--r--   0        0        0     1003 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/api_node_result.py
+-rw-r--r--   0        0        0     1125 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/api_node_result_data.py
+-rw-r--r--   0        0        0     1050 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/array_chat_message_content.py
+-rw-r--r--   0        0        0     1221 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/array_chat_message_content_item.py
+-rw-r--r--   0        0        0     1345 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/array_chat_message_content_item_request.py
+-rw-r--r--   0        0        0     1079 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/array_chat_message_content_request.py
+-rw-r--r--   0        0        0      138 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/array_enum.py
+-rw-r--r--   0        0        0     2451 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/array_variable_value_item.py
+-rw-r--r--   0        0        0     1051 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/block_type_enum.py
+-rw-r--r--   0        0        0      151 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_history_enum.py
+-rw-r--r--   0        0        0     1130 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_history_input_request.py
+-rw-r--r--   0        0        0      958 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_history_variable_value.py
+-rw-r--r--   0        0        0     1060 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_message.py
+-rw-r--r--   0        0        0     1466 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_message_content.py
+-rw-r--r--   0        0        0     1630 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_message_content_request.py
+-rw-r--r--   0        0        0     1089 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_message_request.py
+-rw-r--r--   0        0        0      914 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/chat_message_role.py
+-rw-r--r--   0        0        0      980 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_chat_history_result.py
+-rw-r--r--   0        0        0      961 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_error_result.py
+-rw-r--r--   0        0        0      939 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_json_result.py
+-rw-r--r--   0        0        0      918 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_number_result.py
+-rw-r--r--   0        0        0     1054 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_result.py
+-rw-r--r--   0        0        0     1029 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_result_data.py
+-rw-r--r--   0        0        0     2386 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_result_output.py
+-rw-r--r--   0        0        0      985 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_search_results_result.py
+-rw-r--r--   0        0        0      916 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/code_execution_node_string_result.py
+-rw-r--r--   0        0        0     1042 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/conditional_node_result.py
+-rw-r--r--   0        0        0      911 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/conditional_node_result_data.py
+-rw-r--r--   0        0        0      918 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/deployment_provider_payload_response.py
+-rw-r--r--   0        0        0     2000 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/deployment_read.py
+-rw-r--r--   0        0        0     1634 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/document_document_to_document_index.py
+-rw-r--r--   0        0        0     1867 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/document_index_read.py
+-rw-r--r--   0        0        0     2264 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/document_read.py
+-rw-r--r--   0        0        0      144 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/document_status.py
+-rw-r--r--   0        0        0     2135 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/enriched_normalized_completion.py
+-rw-r--r--   0        0        0      539 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/entity_status.py
+-rw-r--r--   0        0        0      799 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/environment_enum.py
+-rw-r--r--   0        0        0      138 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/error_enum.py
+-rw-r--r--   0        0        0      939 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/error_variable_value.py
+-rw-r--r--   0        0        0      958 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_prompt_api_error_response.py
+-rw-r--r--   0        0        0     1523 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_prompt_event.py
+-rw-r--r--   0        0        0      871 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_prompt_response.py
+-rw-r--r--   0        0        0      957 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_workflow_error_response.py
+-rw-r--r--   0        0        0     1091 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_workflow_response.py
+-rw-r--r--   0        0        0      963 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_workflow_stream_error_response.py
+-rw-r--r--   0        0        0     1024 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0      726 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/finish_reason_enum.py
+-rw-r--r--   0        0        0      146 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_enum.py
+-rw-r--r--   0        0        0     1248 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_execute_prompt_event.py
+-rw-r--r--   0        0        0     1450 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_execute_prompt_response.py
+-rw-r--r--   0        0        0     1109 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0     1012 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_function_call.py
+-rw-r--r--   0        0        0     1145 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1302 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/fulfilled_workflow_node_result_event.py
+-rw-r--r--   0        0        0      770 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call.py
+-rw-r--r--   0        0        0     1085 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content.py
+-rw-r--r--   0        0        0     1114 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content_request.py
+-rw-r--r--   0        0        0     1026 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content_value.py
+-rw-r--r--   0        0        0     1033 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content_value_request.py
+-rw-r--r--   0        0        0      153 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call_enum.py
+-rw-r--r--   0        0        0      932 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/function_call_variable_value.py
+-rw-r--r--   0        0        0      950 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/generate_error_response.py
+-rw-r--r--   0        0        0     1117 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/generate_options_request.py
+-rw-r--r--   0        0        0     1581 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/generate_request.py
+-rw-r--r--   0        0        0     1342 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/generate_response.py
+-rw-r--r--   0        0        0     1397 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/generate_result.py
+-rw-r--r--   0        0        0     1111 2024-03-06 02:55:26.078354 vellum_ai-0.3.9/src/vellum/types/generate_result_data.py
+-rw-r--r--   0        0        0      959 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/generate_result_error.py
+-rw-r--r--   0        0        0      954 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/generate_stream_response.py
+-rw-r--r--   0        0        0     1107 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/generate_stream_result.py
+-rw-r--r--   0        0        0     1011 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/generate_stream_result_data.py
+-rw-r--r--   0        0        0      995 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/image_chat_message_content.py
+-rw-r--r--   0        0        0     1024 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/image_chat_message_content_request.py
+-rw-r--r--   0        0        0      138 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/image_enum.py
+-rw-r--r--   0        0        0     1181 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/indexing_state_enum.py
+-rw-r--r--   0        0        0      146 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/initiated_enum.py
+-rw-r--r--   0        0        0     1147 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/initiated_execute_prompt_event.py
+-rw-r--r--   0        0        0     1173 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/initiated_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1323 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/initiated_workflow_node_result_event.py
+-rw-r--r--   0        0        0      136 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/json_enum.py
+-rw-r--r--   0        0        0     1057 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/json_input_request.py
+-rw-r--r--   0        0        0      917 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/json_variable_value.py
+-rw-r--r--   0        0        0     4282 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/logical_operator.py
+-rw-r--r--   0        0        0      490 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/logprobs_enum.py
+-rw-r--r--   0        0        0     1333 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/metadata_filter_config_request.py
+-rw-r--r--   0        0        0      528 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/metadata_filter_rule_combinator.py
+-rw-r--r--   0        0        0     1349 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/metadata_filter_rule_request.py
+-rw-r--r--   0        0        0     1356 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/model_version_build_config.py
+-rw-r--r--   0        0        0     1632 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/model_version_exec_config.py
+-rw-r--r--   0        0        0     1247 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/model_version_exec_config_parameters.py
+-rw-r--r--   0        0        0     2575 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/model_version_read.py
+-rw-r--r--   0        0        0     1032 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/model_version_read_status_enum.py
+-rw-r--r--   0        0        0     1217 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/model_version_sandbox_snapshot.py
+-rw-r--r--   0        0        0     1014 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_chat_history_variable_value_request.py
+-rw-r--r--   0        0        0      995 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_error_variable_value_request.py
+-rw-r--r--   0        0        0      951 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_json_variable_value_request.py
+-rw-r--r--   0        0        0      930 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_number_variable_value_request.py
+-rw-r--r--   0        0        0     1019 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_search_results_variable_value_request.py
+-rw-r--r--   0        0        0      928 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_string_variable_value_request.py
+-rw-r--r--   0        0        0     2630 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/named_test_case_variable_value_request.py
+-rw-r--r--   0        0        0     1032 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_array_value.py
+-rw-r--r--   0        0        0     1003 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_chat_history_value.py
+-rw-r--r--   0        0        0      984 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_error_value.py
+-rw-r--r--   0        0        0      962 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_json_value.py
+-rw-r--r--   0        0        0      941 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_number_value.py
+-rw-r--r--   0        0        0     1008 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_search_results_value.py
+-rw-r--r--   0        0        0      939 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_compiled_string_value.py
+-rw-r--r--   0        0        0     2730 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_input_variable_compiled_value.py
+-rw-r--r--   0        0        0     1021 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_array_value.py
+-rw-r--r--   0        0        0      992 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_chat_history_value.py
+-rw-r--r--   0        0        0      973 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_error_value.py
+-rw-r--r--   0        0        0      979 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_function_value.py
+-rw-r--r--   0        0        0      951 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_json_value.py
+-rw-r--r--   0        0        0      930 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_number_value.py
+-rw-r--r--   0        0        0      997 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_search_results_value.py
+-rw-r--r--   0        0        0      928 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_string_value.py
+-rw-r--r--   0        0        0     3015 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/node_output_compiled_value.py
+-rw-r--r--   0        0        0     1013 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/normalized_log_probs.py
+-rw-r--r--   0        0        0     1014 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/normalized_token_log_probs.py
+-rw-r--r--   0        0        0      140 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/number_enum.py
+-rw-r--r--   0        0        0      896 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/number_variable_value.py
+-rw-r--r--   0        0        0     1087 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/paginated_slim_deployment_read_list.py
+-rw-r--r--   0        0        0     1062 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/paginated_slim_document_list.py
+-rw-r--r--   0        0        0     1103 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/paginated_slim_workflow_deployment_list.py
+-rw-r--r--   0        0        0      752 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/processing_failure_reason_enum.py
+-rw-r--r--   0        0        0      962 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/processing_state_enum.py
+-rw-r--r--   0        0        0     1819 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_deployment_expand_meta_request_request.py
+-rw-r--r--   0        0        0     1159 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_deployment_input_request.py
+-rw-r--r--   0        0        0     1266 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_execution_meta.py
+-rw-r--r--   0        0        0     1017 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_node_result.py
+-rw-r--r--   0        0        0      987 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_node_result_data.py
+-rw-r--r--   0        0        0     1336 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_output.py
+-rw-r--r--   0        0        0     1164 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_template_block.py
+-rw-r--r--   0        0        0      983 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_template_block_data.py
+-rw-r--r--   0        0        0     1012 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_template_block_data_request.py
+-rw-r--r--   0        0        0     1586 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_template_block_properties.py
+-rw-r--r--   0        0        0     1622 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_template_block_properties_request.py
+-rw-r--r--   0        0        0     1200 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/prompt_template_block_request.py
+-rw-r--r--   0        0        0     2516 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/provider_enum.py
+-rw-r--r--   0        0        0     1192 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/raw_prompt_execution_overrides_request.py
+-rw-r--r--   0        0        0      956 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/register_prompt_error_response.py
+-rw-r--r--   0        0        0     1215 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/register_prompt_model_parameters_request.py
+-rw-r--r--   0        0        0     1035 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/register_prompt_prompt.py
+-rw-r--r--   0        0        0     1269 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/register_prompt_prompt_info_request.py
+-rw-r--r--   0        0        0     1926 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/register_prompt_response.py
+-rw-r--r--   0        0        0     1149 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/registered_prompt_deployment.py
+-rw-r--r--   0        0        0     1020 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/registered_prompt_input_variable_request.py
+-rw-r--r--   0        0        0     1057 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/registered_prompt_model_version.py
+-rw-r--r--   0        0        0     1040 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/registered_prompt_sandbox.py
+-rw-r--r--   0        0        0      960 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/registered_prompt_sandbox_snapshot.py
+-rw-r--r--   0        0        0      144 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_enum.py
+-rw-r--r--   0        0        0     1172 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_execute_prompt_event.py
+-rw-r--r--   0        0        0     1410 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_execute_prompt_response.py
+-rw-r--r--   0        0        0     1123 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_execute_workflow_workflow_result_event.py
+-rw-r--r--   0        0        0     1051 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_function_call.py
+-rw-r--r--   0        0        0     1144 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1246 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/rejected_workflow_node_result_event.py
+-rw-r--r--   0        0        0     1098 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/sandbox_scenario.py
+-rw-r--r--   0        0        0     1108 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/scenario_input.py
+-rw-r--r--   0        0        0     1137 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/scenario_input_request.py
+-rw-r--r--   0        0        0      580 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/scenario_input_type_enum.py
+-rw-r--r--   0        0        0      948 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_error_response.py
+-rw-r--r--   0        0        0     1221 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_filters_request.py
+-rw-r--r--   0        0        0     1017 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_node_result.py
+-rw-r--r--   0        0        0     1159 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_node_result_data.py
+-rw-r--r--   0        0        0     1579 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_request_options_request.py
+-rw-r--r--   0        0        0     1071 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_response.py
+-rw-r--r--   0        0        0     1306 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_result.py
+-rw-r--r--   0        0        0     1418 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_result_document.py
+-rw-r--r--   0        0        0     1357 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_result_document_request.py
+-rw-r--r--   0        0        0      970 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_result_merging_request.py
+-rw-r--r--   0        0        0     1335 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_result_request.py
+-rw-r--r--   0        0        0      155 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_results_enum.py
+-rw-r--r--   0        0        0      963 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_results_variable_value.py
+-rw-r--r--   0        0        0     1117 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/search_weights_request.py
+-rw-r--r--   0        0        0     1811 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/slim_deployment_read.py
+-rw-r--r--   0        0        0     3074 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/slim_document.py
+-rw-r--r--   0        0        0     2205 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/slim_workflow_deployment.py
+-rw-r--r--   0        0        0      146 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/streaming_enum.py
+-rw-r--r--   0        0        0     1393 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/streaming_execute_prompt_event.py
+-rw-r--r--   0        0        0     1043 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/streaming_prompt_execution_meta.py
+-rw-r--r--   0        0        0     1322 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/streaming_workflow_node_result_event.py
+-rw-r--r--   0        0        0      950 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/string_chat_message_content.py
+-rw-r--r--   0        0        0      957 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/string_chat_message_content_request.py
+-rw-r--r--   0        0        0      140 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/string_enum.py
+-rw-r--r--   0        0        0     1035 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/string_input_request.py
+-rw-r--r--   0        0        0      894 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/string_variable_value.py
+-rw-r--r--   0        0        0     1787 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/submit_completion_actual_request.py
+-rw-r--r--   0        0        0      895 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/submit_completion_actuals_error_response.py
+-rw-r--r--   0        0        0     1413 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/submit_workflow_execution_actual_request.py
+-rw-r--r--   0        0        0      150 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/subworkflow_enum.py
+-rw-r--r--   0        0        0      937 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/subworkflow_node_result.py
+-rw-r--r--   0        0        0      977 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_chat_history_result.py
+-rw-r--r--   0        0        0      958 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_error_result.py
+-rw-r--r--   0        0        0      936 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_json_result.py
+-rw-r--r--   0        0        0      915 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_number_result.py
+-rw-r--r--   0        0        0     1037 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_result.py
+-rw-r--r--   0        0        0      976 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_result_data.py
+-rw-r--r--   0        0        0     2287 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_result_output.py
+-rw-r--r--   0        0        0      982 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_search_results_result.py
+-rw-r--r--   0        0        0      913 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/templating_node_string_result.py
+-rw-r--r--   0        0        0     1137 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_array_result.py
+-rw-r--r--   0        0        0     1108 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_chat_history_result.py
+-rw-r--r--   0        0        0     1089 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_error_result.py
+-rw-r--r--   0        0        0     1099 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_function_call_result.py
+-rw-r--r--   0        0        0     1067 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_json_result.py
+-rw-r--r--   0        0        0     1046 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_number_result.py
+-rw-r--r--   0        0        0     1027 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_result.py
+-rw-r--r--   0        0        0      968 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_result_data.py
+-rw-r--r--   0        0        0     2917 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_result_output.py
+-rw-r--r--   0        0        0     1113 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_search_results_result.py
+-rw-r--r--   0        0        0     1044 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/terminal_node_string_result.py
+-rw-r--r--   0        0        0      987 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_chat_history_variable_value.py
+-rw-r--r--   0        0        0      968 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_error_variable_value.py
+-rw-r--r--   0        0        0      946 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_json_variable_value.py
+-rw-r--r--   0        0        0      925 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_number_variable_value.py
+-rw-r--r--   0        0        0      992 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_search_results_variable_value.py
+-rw-r--r--   0        0        0      923 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_string_variable_value.py
+-rw-r--r--   0        0        0     2246 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_case_variable_value.py
+-rw-r--r--   0        0        0     1092 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/test_suite_test_case.py
+-rw-r--r--   0        0        0      886 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/upload_document_error_response.py
+-rw-r--r--   0        0        0      956 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/upload_document_response.py
+-rw-r--r--   0        0        0      957 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_error.py
+-rw-r--r--   0        0        0     1221 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_error_code_enum.py
+-rw-r--r--   0        0        0      964 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_error_request.py
+-rw-r--r--   0        0        0      927 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_image.py
+-rw-r--r--   0        0        0      934 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_image_request.py
+-rw-r--r--   0        0        0      964 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_variable.py
+-rw-r--r--   0        0        0     1855 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/vellum_variable_type.py
+-rw-r--r--   0        0        0     2211 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_deployment_read.py
+-rw-r--r--   0        0        0     1001 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_event_error.py
+-rw-r--r--   0        0        0     2014 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_actual_chat_history_request.py
+-rw-r--r--   0        0        0     1951 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_actual_json_request.py
+-rw-r--r--   0        0        0     1928 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_actual_string_request.py
+-rw-r--r--   0        0        0     2185 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_event_error_code.py
+-rw-r--r--   0        0        0      567 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_event_type.py
+-rw-r--r--   0        0        0     1145 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_node_result_event.py
+-rw-r--r--   0        0        0     1140 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_execution_workflow_result_event.py
+-rw-r--r--   0        0        0     2715 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_node_result_data.py
+-rw-r--r--   0        0        0     1632 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_node_result_event.py
+-rw-r--r--   0        0        0     1035 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_node_result_event_state.py
+-rw-r--r--   0        0        0     2934 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output.py
+-rw-r--r--   0        0        0     1139 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_array.py
+-rw-r--r--   0        0        0     1116 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_chat_history.py
+-rw-r--r--   0        0        0     1091 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_error.py
+-rw-r--r--   0        0        0     1108 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_function_call.py
+-rw-r--r--   0        0        0     1091 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_image.py
+-rw-r--r--   0        0        0     1067 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_json.py
+-rw-r--r--   0        0        0     1048 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_number.py
+-rw-r--r--   0        0        0     1123 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_search_results.py
+-rw-r--r--   0        0        0     1046 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_output_string.py
+-rw-r--r--   0        0        0     1146 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_request_chat_history_input_request.py
+-rw-r--r--   0        0        0     1666 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_request_input_request.py
+-rw-r--r--   0        0        0     1075 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_request_json_input_request.py
+-rw-r--r--   0        0        0     1056 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_request_number_input_request.py
+-rw-r--r--   0        0        0     1054 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_request_string_input_request.py
+-rw-r--r--   0        0        0     1347 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event.py
+-rw-r--r--   0        0        0     3282 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data.py
+-rw-r--r--   0        0        0     1420 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_array.py
+-rw-r--r--   0        0        0     1397 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_chat_history.py
+-rw-r--r--   0        0        0     1372 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_error.py
+-rw-r--r--   0        0        0     1389 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_function_call.py
+-rw-r--r--   0        0        0     1348 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_json.py
+-rw-r--r--   0        0        0     1329 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_number.py
+-rw-r--r--   0        0        0     1404 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_search_results.py
+-rw-r--r--   0        0        0     1478 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_string.py
+-rw-r--r--   0        0        0      873 2024-03-06 02:55:26.082354 vellum_ai-0.3.9/src/vellum/types/workflow_stream_event.py
+-rw-r--r--   0        0        0     3486 1970-01-01 00:00:00.000000 vellum_ai-0.3.9/PKG-INFO
```

### Comparing `vellum_ai-0.3.8/LICENSE` & `vellum_ai-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/README.md` & `vellum_ai-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/__init__.py` & `vellum_ai-0.3.9/src/vellum/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -255,14 +255,16 @@
     StringVariableValue,
     SubmitCompletionActualRequest,
     SubmitCompletionActualsErrorResponse,
     SubmitWorkflowExecutionActualRequest,
     SubmitWorkflowExecutionActualRequest_ChatHistory,
     SubmitWorkflowExecutionActualRequest_Json,
     SubmitWorkflowExecutionActualRequest_String,
+    SubworkflowEnum,
+    SubworkflowNodeResult,
     TemplatingNodeChatHistoryResult,
     TemplatingNodeErrorResult,
     TemplatingNodeJsonResult,
     TemplatingNodeNumberResult,
     TemplatingNodeResult,
     TemplatingNodeResultData,
     TemplatingNodeResultOutput,
@@ -270,23 +272,27 @@
     TemplatingNodeResultOutput_Error,
     TemplatingNodeResultOutput_Json,
     TemplatingNodeResultOutput_Number,
     TemplatingNodeResultOutput_SearchResults,
     TemplatingNodeResultOutput_String,
     TemplatingNodeSearchResultsResult,
     TemplatingNodeStringResult,
+    TerminalNodeArrayResult,
     TerminalNodeChatHistoryResult,
     TerminalNodeErrorResult,
+    TerminalNodeFunctionCallResult,
     TerminalNodeJsonResult,
     TerminalNodeNumberResult,
     TerminalNodeResult,
     TerminalNodeResultData,
     TerminalNodeResultOutput,
+    TerminalNodeResultOutput_Array,
     TerminalNodeResultOutput_ChatHistory,
     TerminalNodeResultOutput_Error,
+    TerminalNodeResultOutput_FunctionCall,
     TerminalNodeResultOutput_Json,
     TerminalNodeResultOutput_Number,
     TerminalNodeResultOutput_SearchResults,
     TerminalNodeResultOutput_String,
     TerminalNodeSearchResultsResult,
     TerminalNodeStringResult,
     TestCaseChatHistoryVariableValue,
@@ -323,31 +329,34 @@
     WorkflowExecutionWorkflowResultEvent,
     WorkflowNodeResultData,
     WorkflowNodeResultData_Api,
     WorkflowNodeResultData_CodeExecution,
     WorkflowNodeResultData_Conditional,
     WorkflowNodeResultData_Prompt,
     WorkflowNodeResultData_Search,
+    WorkflowNodeResultData_Subworkflow,
     WorkflowNodeResultData_Templating,
     WorkflowNodeResultData_Terminal,
     WorkflowNodeResultEvent,
     WorkflowNodeResultEventState,
     WorkflowNodeResultEvent_Fulfilled,
     WorkflowNodeResultEvent_Initiated,
     WorkflowNodeResultEvent_Rejected,
     WorkflowNodeResultEvent_Streaming,
     WorkflowOutput,
+    WorkflowOutputArray,
     WorkflowOutputChatHistory,
     WorkflowOutputError,
     WorkflowOutputFunctionCall,
     WorkflowOutputImage,
     WorkflowOutputJson,
     WorkflowOutputNumber,
     WorkflowOutputSearchResults,
     WorkflowOutputString,
+    WorkflowOutput_Array,
     WorkflowOutput_ChatHistory,
     WorkflowOutput_Error,
     WorkflowOutput_FunctionCall,
     WorkflowOutput_Image,
     WorkflowOutput_Json,
     WorkflowOutput_Number,
     WorkflowOutput_SearchResults,
@@ -359,22 +368,26 @@
     WorkflowRequestInputRequest_Number,
     WorkflowRequestInputRequest_String,
     WorkflowRequestJsonInputRequest,
     WorkflowRequestNumberInputRequest,
     WorkflowRequestStringInputRequest,
     WorkflowResultEvent,
     WorkflowResultEventOutputData,
+    WorkflowResultEventOutputDataArray,
     WorkflowResultEventOutputDataChatHistory,
     WorkflowResultEventOutputDataError,
+    WorkflowResultEventOutputDataFunctionCall,
     WorkflowResultEventOutputDataJson,
     WorkflowResultEventOutputDataNumber,
     WorkflowResultEventOutputDataSearchResults,
     WorkflowResultEventOutputDataString,
+    WorkflowResultEventOutputData_Array,
     WorkflowResultEventOutputData_ChatHistory,
     WorkflowResultEventOutputData_Error,
+    WorkflowResultEventOutputData_FunctionCall,
     WorkflowResultEventOutputData_Json,
     WorkflowResultEventOutputData_Number,
     WorkflowResultEventOutputData_SearchResults,
     WorkflowResultEventOutputData_String,
     WorkflowStreamEvent,
     WorkflowStreamEvent_Node,
     WorkflowStreamEvent_Workflow,
@@ -656,14 +669,16 @@
     "StringVariableValue",
     "SubmitCompletionActualRequest",
     "SubmitCompletionActualsErrorResponse",
     "SubmitWorkflowExecutionActualRequest",
     "SubmitWorkflowExecutionActualRequest_ChatHistory",
     "SubmitWorkflowExecutionActualRequest_Json",
     "SubmitWorkflowExecutionActualRequest_String",
+    "SubworkflowEnum",
+    "SubworkflowNodeResult",
     "TemplatingNodeChatHistoryResult",
     "TemplatingNodeErrorResult",
     "TemplatingNodeJsonResult",
     "TemplatingNodeNumberResult",
     "TemplatingNodeResult",
     "TemplatingNodeResultData",
     "TemplatingNodeResultOutput",
@@ -671,23 +686,27 @@
     "TemplatingNodeResultOutput_Error",
     "TemplatingNodeResultOutput_Json",
     "TemplatingNodeResultOutput_Number",
     "TemplatingNodeResultOutput_SearchResults",
     "TemplatingNodeResultOutput_String",
     "TemplatingNodeSearchResultsResult",
     "TemplatingNodeStringResult",
+    "TerminalNodeArrayResult",
     "TerminalNodeChatHistoryResult",
     "TerminalNodeErrorResult",
+    "TerminalNodeFunctionCallResult",
     "TerminalNodeJsonResult",
     "TerminalNodeNumberResult",
     "TerminalNodeResult",
     "TerminalNodeResultData",
     "TerminalNodeResultOutput",
+    "TerminalNodeResultOutput_Array",
     "TerminalNodeResultOutput_ChatHistory",
     "TerminalNodeResultOutput_Error",
+    "TerminalNodeResultOutput_FunctionCall",
     "TerminalNodeResultOutput_Json",
     "TerminalNodeResultOutput_Number",
     "TerminalNodeResultOutput_SearchResults",
     "TerminalNodeResultOutput_String",
     "TerminalNodeSearchResultsResult",
     "TerminalNodeStringResult",
     "TestCaseChatHistoryVariableValue",
@@ -726,31 +745,34 @@
     "WorkflowExecutionWorkflowResultEvent",
     "WorkflowNodeResultData",
     "WorkflowNodeResultData_Api",
     "WorkflowNodeResultData_CodeExecution",
     "WorkflowNodeResultData_Conditional",
     "WorkflowNodeResultData_Prompt",
     "WorkflowNodeResultData_Search",
+    "WorkflowNodeResultData_Subworkflow",
     "WorkflowNodeResultData_Templating",
     "WorkflowNodeResultData_Terminal",
     "WorkflowNodeResultEvent",
     "WorkflowNodeResultEventState",
     "WorkflowNodeResultEvent_Fulfilled",
     "WorkflowNodeResultEvent_Initiated",
     "WorkflowNodeResultEvent_Rejected",
     "WorkflowNodeResultEvent_Streaming",
     "WorkflowOutput",
+    "WorkflowOutputArray",
     "WorkflowOutputChatHistory",
     "WorkflowOutputError",
     "WorkflowOutputFunctionCall",
     "WorkflowOutputImage",
     "WorkflowOutputJson",
     "WorkflowOutputNumber",
     "WorkflowOutputSearchResults",
     "WorkflowOutputString",
+    "WorkflowOutput_Array",
     "WorkflowOutput_ChatHistory",
     "WorkflowOutput_Error",
     "WorkflowOutput_FunctionCall",
     "WorkflowOutput_Image",
     "WorkflowOutput_Json",
     "WorkflowOutput_Number",
     "WorkflowOutput_SearchResults",
@@ -762,22 +784,26 @@
     "WorkflowRequestInputRequest_Number",
     "WorkflowRequestInputRequest_String",
     "WorkflowRequestJsonInputRequest",
     "WorkflowRequestNumberInputRequest",
     "WorkflowRequestStringInputRequest",
     "WorkflowResultEvent",
     "WorkflowResultEventOutputData",
+    "WorkflowResultEventOutputDataArray",
     "WorkflowResultEventOutputDataChatHistory",
     "WorkflowResultEventOutputDataError",
+    "WorkflowResultEventOutputDataFunctionCall",
     "WorkflowResultEventOutputDataJson",
     "WorkflowResultEventOutputDataNumber",
     "WorkflowResultEventOutputDataSearchResults",
     "WorkflowResultEventOutputDataString",
+    "WorkflowResultEventOutputData_Array",
     "WorkflowResultEventOutputData_ChatHistory",
     "WorkflowResultEventOutputData_Error",
+    "WorkflowResultEventOutputData_FunctionCall",
     "WorkflowResultEventOutputData_Json",
     "WorkflowResultEventOutputData_Number",
     "WorkflowResultEventOutputData_SearchResults",
     "WorkflowResultEventOutputData_String",
     "WorkflowStreamEvent",
     "WorkflowStreamEvent_Node",
     "WorkflowStreamEvent_Workflow",
```

### Comparing `vellum_ai-0.3.8/src/vellum/client.py` & `vellum_ai-0.3.9/src/vellum/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/core/__init__.py` & `vellum_ai-0.3.9/src/vellum/core/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/core/client_wrapper.py` & `vellum_ai-0.3.9/src/vellum/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.api_key = api_key
         self._environment = environment
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "vellum-ai",
-            "X-Fern-SDK-Version": "0.3.8",
+            "X-Fern-SDK-Version": "0.3.9",
         }
         headers["X_API_KEY"] = self.api_key
         return headers
 
     def get_environment(self) -> VellumEnvironment:
         return self._environment
```

### Comparing `vellum_ai-0.3.8/src/vellum/core/datetime_utils.py` & `vellum_ai-0.3.9/src/vellum/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/core/jsonable_encoder.py` & `vellum_ai-0.3.9/src/vellum/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/resources/__init__.py` & `vellum_ai-0.3.9/src/vellum/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/resources/deployments/client.py` & `vellum_ai-0.3.9/src/vellum/resources/deployments/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/resources/deployments/types/deployments_list_request_status.py` & `vellum_ai-0.3.9/src/vellum/resources/deployments/types/deployments_list_request_status.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/resources/document_indexes/client.py` & `vellum_ai-0.3.9/src/vellum/resources/document_indexes/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/resources/documents/client.py` & `vellum_ai-0.3.9/src/vellum/resources/documents/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/resources/folder_entities/client.py` & `vellum_ai-0.3.9/src/vellum/resources/folder_entities/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/resources/model_versions/client.py` & `vellum_ai-0.3.9/src/vellum/resources/model_versions/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/resources/registered_prompts/client.py` & `vellum_ai-0.3.9/src/vellum/resources/registered_prompts/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/resources/sandboxes/client.py` & `vellum_ai-0.3.9/src/vellum/resources/sandboxes/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/resources/test_suites/client.py` & `vellum_ai-0.3.9/src/vellum/resources/test_suites/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/resources/workflow_deployments/client.py` & `vellum_ai-0.3.9/src/vellum/resources/workflow_deployments/client.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/resources/workflow_deployments/types/workflow_deployments_list_request_status.py` & `vellum_ai-0.3.9/src/vellum/resources/workflow_deployments/types/workflow_deployments_list_request_status.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/__init__.py` & `vellum_ai-0.3.9/src/vellum/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,14 +282,16 @@
 from .submit_completion_actuals_error_response import SubmitCompletionActualsErrorResponse
 from .submit_workflow_execution_actual_request import (
     SubmitWorkflowExecutionActualRequest,
     SubmitWorkflowExecutionActualRequest_ChatHistory,
     SubmitWorkflowExecutionActualRequest_Json,
     SubmitWorkflowExecutionActualRequest_String,
 )
+from .subworkflow_enum import SubworkflowEnum
+from .subworkflow_node_result import SubworkflowNodeResult
 from .templating_node_chat_history_result import TemplatingNodeChatHistoryResult
 from .templating_node_error_result import TemplatingNodeErrorResult
 from .templating_node_json_result import TemplatingNodeJsonResult
 from .templating_node_number_result import TemplatingNodeNumberResult
 from .templating_node_result import TemplatingNodeResult
 from .templating_node_result_data import TemplatingNodeResultData
 from .templating_node_result_output import (
@@ -299,24 +301,28 @@
     TemplatingNodeResultOutput_Json,
     TemplatingNodeResultOutput_Number,
     TemplatingNodeResultOutput_SearchResults,
     TemplatingNodeResultOutput_String,
 )
 from .templating_node_search_results_result import TemplatingNodeSearchResultsResult
 from .templating_node_string_result import TemplatingNodeStringResult
+from .terminal_node_array_result import TerminalNodeArrayResult
 from .terminal_node_chat_history_result import TerminalNodeChatHistoryResult
 from .terminal_node_error_result import TerminalNodeErrorResult
+from .terminal_node_function_call_result import TerminalNodeFunctionCallResult
 from .terminal_node_json_result import TerminalNodeJsonResult
 from .terminal_node_number_result import TerminalNodeNumberResult
 from .terminal_node_result import TerminalNodeResult
 from .terminal_node_result_data import TerminalNodeResultData
 from .terminal_node_result_output import (
     TerminalNodeResultOutput,
+    TerminalNodeResultOutput_Array,
     TerminalNodeResultOutput_ChatHistory,
     TerminalNodeResultOutput_Error,
+    TerminalNodeResultOutput_FunctionCall,
     TerminalNodeResultOutput_Json,
     TerminalNodeResultOutput_Number,
     TerminalNodeResultOutput_SearchResults,
     TerminalNodeResultOutput_String,
 )
 from .terminal_node_search_results_result import TerminalNodeSearchResultsResult
 from .terminal_node_string_result import TerminalNodeStringResult
@@ -357,36 +363,39 @@
 from .workflow_node_result_data import (
     WorkflowNodeResultData,
     WorkflowNodeResultData_Api,
     WorkflowNodeResultData_CodeExecution,
     WorkflowNodeResultData_Conditional,
     WorkflowNodeResultData_Prompt,
     WorkflowNodeResultData_Search,
+    WorkflowNodeResultData_Subworkflow,
     WorkflowNodeResultData_Templating,
     WorkflowNodeResultData_Terminal,
 )
 from .workflow_node_result_event import (
     WorkflowNodeResultEvent,
     WorkflowNodeResultEvent_Fulfilled,
     WorkflowNodeResultEvent_Initiated,
     WorkflowNodeResultEvent_Rejected,
     WorkflowNodeResultEvent_Streaming,
 )
 from .workflow_node_result_event_state import WorkflowNodeResultEventState
 from .workflow_output import (
     WorkflowOutput,
+    WorkflowOutput_Array,
     WorkflowOutput_ChatHistory,
     WorkflowOutput_Error,
     WorkflowOutput_FunctionCall,
     WorkflowOutput_Image,
     WorkflowOutput_Json,
     WorkflowOutput_Number,
     WorkflowOutput_SearchResults,
     WorkflowOutput_String,
 )
+from .workflow_output_array import WorkflowOutputArray
 from .workflow_output_chat_history import WorkflowOutputChatHistory
 from .workflow_output_error import WorkflowOutputError
 from .workflow_output_function_call import WorkflowOutputFunctionCall
 from .workflow_output_image import WorkflowOutputImage
 from .workflow_output_json import WorkflowOutputJson
 from .workflow_output_number import WorkflowOutputNumber
 from .workflow_output_search_results import WorkflowOutputSearchResults
@@ -401,23 +410,27 @@
 )
 from .workflow_request_json_input_request import WorkflowRequestJsonInputRequest
 from .workflow_request_number_input_request import WorkflowRequestNumberInputRequest
 from .workflow_request_string_input_request import WorkflowRequestStringInputRequest
 from .workflow_result_event import WorkflowResultEvent
 from .workflow_result_event_output_data import (
     WorkflowResultEventOutputData,
+    WorkflowResultEventOutputData_Array,
     WorkflowResultEventOutputData_ChatHistory,
     WorkflowResultEventOutputData_Error,
+    WorkflowResultEventOutputData_FunctionCall,
     WorkflowResultEventOutputData_Json,
     WorkflowResultEventOutputData_Number,
     WorkflowResultEventOutputData_SearchResults,
     WorkflowResultEventOutputData_String,
 )
+from .workflow_result_event_output_data_array import WorkflowResultEventOutputDataArray
 from .workflow_result_event_output_data_chat_history import WorkflowResultEventOutputDataChatHistory
 from .workflow_result_event_output_data_error import WorkflowResultEventOutputDataError
+from .workflow_result_event_output_data_function_call import WorkflowResultEventOutputDataFunctionCall
 from .workflow_result_event_output_data_json import WorkflowResultEventOutputDataJson
 from .workflow_result_event_output_data_number import WorkflowResultEventOutputDataNumber
 from .workflow_result_event_output_data_search_results import WorkflowResultEventOutputDataSearchResults
 from .workflow_result_event_output_data_string import WorkflowResultEventOutputDataString
 from .workflow_stream_event import WorkflowStreamEvent, WorkflowStreamEvent_Node, WorkflowStreamEvent_Workflow
 
 __all__ = [
@@ -675,14 +688,16 @@
     "StringVariableValue",
     "SubmitCompletionActualRequest",
     "SubmitCompletionActualsErrorResponse",
     "SubmitWorkflowExecutionActualRequest",
     "SubmitWorkflowExecutionActualRequest_ChatHistory",
     "SubmitWorkflowExecutionActualRequest_Json",
     "SubmitWorkflowExecutionActualRequest_String",
+    "SubworkflowEnum",
+    "SubworkflowNodeResult",
     "TemplatingNodeChatHistoryResult",
     "TemplatingNodeErrorResult",
     "TemplatingNodeJsonResult",
     "TemplatingNodeNumberResult",
     "TemplatingNodeResult",
     "TemplatingNodeResultData",
     "TemplatingNodeResultOutput",
@@ -690,23 +705,27 @@
     "TemplatingNodeResultOutput_Error",
     "TemplatingNodeResultOutput_Json",
     "TemplatingNodeResultOutput_Number",
     "TemplatingNodeResultOutput_SearchResults",
     "TemplatingNodeResultOutput_String",
     "TemplatingNodeSearchResultsResult",
     "TemplatingNodeStringResult",
+    "TerminalNodeArrayResult",
     "TerminalNodeChatHistoryResult",
     "TerminalNodeErrorResult",
+    "TerminalNodeFunctionCallResult",
     "TerminalNodeJsonResult",
     "TerminalNodeNumberResult",
     "TerminalNodeResult",
     "TerminalNodeResultData",
     "TerminalNodeResultOutput",
+    "TerminalNodeResultOutput_Array",
     "TerminalNodeResultOutput_ChatHistory",
     "TerminalNodeResultOutput_Error",
+    "TerminalNodeResultOutput_FunctionCall",
     "TerminalNodeResultOutput_Json",
     "TerminalNodeResultOutput_Number",
     "TerminalNodeResultOutput_SearchResults",
     "TerminalNodeResultOutput_String",
     "TerminalNodeSearchResultsResult",
     "TerminalNodeStringResult",
     "TestCaseChatHistoryVariableValue",
@@ -743,31 +762,34 @@
     "WorkflowExecutionWorkflowResultEvent",
     "WorkflowNodeResultData",
     "WorkflowNodeResultData_Api",
     "WorkflowNodeResultData_CodeExecution",
     "WorkflowNodeResultData_Conditional",
     "WorkflowNodeResultData_Prompt",
     "WorkflowNodeResultData_Search",
+    "WorkflowNodeResultData_Subworkflow",
     "WorkflowNodeResultData_Templating",
     "WorkflowNodeResultData_Terminal",
     "WorkflowNodeResultEvent",
     "WorkflowNodeResultEventState",
     "WorkflowNodeResultEvent_Fulfilled",
     "WorkflowNodeResultEvent_Initiated",
     "WorkflowNodeResultEvent_Rejected",
     "WorkflowNodeResultEvent_Streaming",
     "WorkflowOutput",
+    "WorkflowOutputArray",
     "WorkflowOutputChatHistory",
     "WorkflowOutputError",
     "WorkflowOutputFunctionCall",
     "WorkflowOutputImage",
     "WorkflowOutputJson",
     "WorkflowOutputNumber",
     "WorkflowOutputSearchResults",
     "WorkflowOutputString",
+    "WorkflowOutput_Array",
     "WorkflowOutput_ChatHistory",
     "WorkflowOutput_Error",
     "WorkflowOutput_FunctionCall",
     "WorkflowOutput_Image",
     "WorkflowOutput_Json",
     "WorkflowOutput_Number",
     "WorkflowOutput_SearchResults",
@@ -779,22 +801,26 @@
     "WorkflowRequestInputRequest_Number",
     "WorkflowRequestInputRequest_String",
     "WorkflowRequestJsonInputRequest",
     "WorkflowRequestNumberInputRequest",
     "WorkflowRequestStringInputRequest",
     "WorkflowResultEvent",
     "WorkflowResultEventOutputData",
+    "WorkflowResultEventOutputDataArray",
     "WorkflowResultEventOutputDataChatHistory",
     "WorkflowResultEventOutputDataError",
+    "WorkflowResultEventOutputDataFunctionCall",
     "WorkflowResultEventOutputDataJson",
     "WorkflowResultEventOutputDataNumber",
     "WorkflowResultEventOutputDataSearchResults",
     "WorkflowResultEventOutputDataString",
+    "WorkflowResultEventOutputData_Array",
     "WorkflowResultEventOutputData_ChatHistory",
     "WorkflowResultEventOutputData_Error",
+    "WorkflowResultEventOutputData_FunctionCall",
     "WorkflowResultEventOutputData_Json",
     "WorkflowResultEventOutputData_Number",
     "WorkflowResultEventOutputData_SearchResults",
     "WorkflowResultEventOutputData_String",
     "WorkflowStreamEvent",
     "WorkflowStreamEvent_Node",
     "WorkflowStreamEvent_Workflow",
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/api_node_result.py` & `vellum_ai-0.3.9/src/vellum/types/api_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/api_node_result_data.py` & `vellum_ai-0.3.9/src/vellum/types/api_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/array_chat_message_content.py` & `vellum_ai-0.3.9/src/vellum/types/array_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/array_chat_message_content_item.py` & `vellum_ai-0.3.9/src/vellum/types/array_chat_message_content_item.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/array_chat_message_content_item_request.py` & `vellum_ai-0.3.9/src/vellum/types/array_chat_message_content_item_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/array_chat_message_content_request.py` & `vellum_ai-0.3.9/src/vellum/types/array_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/array_variable_value_item.py` & `vellum_ai-0.3.9/src/vellum/types/array_variable_value_item.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/block_type_enum.py` & `vellum_ai-0.3.9/src/vellum/types/block_type_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/chat_history_input_request.py` & `vellum_ai-0.3.9/src/vellum/types/chat_history_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/chat_history_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/chat_history_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/chat_message.py` & `vellum_ai-0.3.9/src/vellum/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/chat_message_content.py` & `vellum_ai-0.3.9/src/vellum/types/chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/chat_message_content_request.py` & `vellum_ai-0.3.9/src/vellum/types/chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/chat_message_request.py` & `vellum_ai-0.3.9/src/vellum/types/chat_message_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/chat_message_role.py` & `vellum_ai-0.3.9/src/vellum/types/chat_message_role.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/code_execution_node_chat_history_result.py` & `vellum_ai-0.3.9/src/vellum/types/code_execution_node_chat_history_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/code_execution_node_error_result.py` & `vellum_ai-0.3.9/src/vellum/types/code_execution_node_error_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/code_execution_node_json_result.py` & `vellum_ai-0.3.9/src/vellum/types/code_execution_node_json_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/code_execution_node_number_result.py` & `vellum_ai-0.3.9/src/vellum/types/code_execution_node_number_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/code_execution_node_result.py` & `vellum_ai-0.3.9/src/vellum/types/code_execution_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/code_execution_node_result_data.py` & `vellum_ai-0.3.9/src/vellum/types/code_execution_node_result_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
 class CodeExecutionNodeResultData(pydantic.BaseModel):
     output: CodeExecutionNodeResultOutput
+    log_output_id: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/code_execution_node_result_output.py` & `vellum_ai-0.3.9/src/vellum/types/code_execution_node_result_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/code_execution_node_search_results_result.py` & `vellum_ai-0.3.9/src/vellum/types/code_execution_node_search_results_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/code_execution_node_string_result.py` & `vellum_ai-0.3.9/src/vellum/types/code_execution_node_string_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/conditional_node_result.py` & `vellum_ai-0.3.9/src/vellum/types/conditional_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/conditional_node_result_data.py` & `vellum_ai-0.3.9/src/vellum/types/conditional_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/deployment_provider_payload_response.py` & `vellum_ai-0.3.9/src/vellum/types/deployment_provider_payload_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/deployment_read.py` & `vellum_ai-0.3.9/src/vellum/types/deployment_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/document_document_to_document_index.py` & `vellum_ai-0.3.9/src/vellum/types/document_document_to_document_index.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/document_index_read.py` & `vellum_ai-0.3.9/src/vellum/types/document_index_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/document_read.py` & `vellum_ai-0.3.9/src/vellum/types/document_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/enriched_normalized_completion.py` & `vellum_ai-0.3.9/src/vellum/types/enriched_normalized_completion.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/entity_status.py` & `vellum_ai-0.3.9/src/vellum/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/environment_enum.py` & `vellum_ai-0.3.9/src/vellum/types/environment_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/error_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/error_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/execute_prompt_api_error_response.py` & `vellum_ai-0.3.9/src/vellum/types/execute_prompt_api_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/execute_prompt_event.py` & `vellum_ai-0.3.9/src/vellum/types/execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/execute_prompt_response.py` & `vellum_ai-0.3.9/src/vellum/types/execute_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/execute_workflow_error_response.py` & `vellum_ai-0.3.9/src/vellum/types/execute_workflow_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/execute_workflow_response.py` & `vellum_ai-0.3.9/src/vellum/types/execute_workflow_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/execute_workflow_stream_error_response.py` & `vellum_ai-0.3.9/src/vellum/types/execute_workflow_stream_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/execute_workflow_workflow_result_event.py` & `vellum_ai-0.3.9/src/vellum/types/execute_workflow_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/finish_reason_enum.py` & `vellum_ai-0.3.9/src/vellum/types/finish_reason_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/fulfilled_execute_prompt_event.py` & `vellum_ai-0.3.9/src/vellum/types/fulfilled_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/fulfilled_execute_prompt_response.py` & `vellum_ai-0.3.9/src/vellum/types/fulfilled_execute_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py` & `vellum_ai-0.3.9/src/vellum/types/fulfilled_execute_workflow_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/fulfilled_function_call.py` & `vellum_ai-0.3.9/src/vellum/types/fulfilled_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/fulfilled_prompt_execution_meta.py` & `vellum_ai-0.3.9/src/vellum/types/fulfilled_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/fulfilled_workflow_node_result_event.py` & `vellum_ai-0.3.9/src/vellum/types/fulfilled_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/function_call.py` & `vellum_ai-0.3.9/src/vellum/types/function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/function_call_chat_message_content.py` & `vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/function_call_chat_message_content_request.py` & `vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/function_call_chat_message_content_value.py` & `vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/function_call_chat_message_content_value_request.py` & `vellum_ai-0.3.9/src/vellum/types/function_call_chat_message_content_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/function_call_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/function_call_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/generate_error_response.py` & `vellum_ai-0.3.9/src/vellum/types/generate_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/generate_options_request.py` & `vellum_ai-0.3.9/src/vellum/types/generate_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/generate_request.py` & `vellum_ai-0.3.9/src/vellum/types/generate_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/generate_response.py` & `vellum_ai-0.3.9/src/vellum/types/generate_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/generate_result.py` & `vellum_ai-0.3.9/src/vellum/types/generate_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/generate_result_data.py` & `vellum_ai-0.3.9/src/vellum/types/generate_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/generate_result_error.py` & `vellum_ai-0.3.9/src/vellum/types/generate_result_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/generate_stream_response.py` & `vellum_ai-0.3.9/src/vellum/types/generate_stream_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/generate_stream_result.py` & `vellum_ai-0.3.9/src/vellum/types/generate_stream_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/generate_stream_result_data.py` & `vellum_ai-0.3.9/src/vellum/types/generate_stream_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/image_chat_message_content.py` & `vellum_ai-0.3.9/src/vellum/types/image_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/image_chat_message_content_request.py` & `vellum_ai-0.3.9/src/vellum/types/image_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/indexing_state_enum.py` & `vellum_ai-0.3.9/src/vellum/types/indexing_state_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/initiated_execute_prompt_event.py` & `vellum_ai-0.3.9/src/vellum/types/initiated_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/initiated_prompt_execution_meta.py` & `vellum_ai-0.3.9/src/vellum/types/initiated_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/initiated_workflow_node_result_event.py` & `vellum_ai-0.3.9/src/vellum/types/initiated_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/json_input_request.py` & `vellum_ai-0.3.9/src/vellum/types/json_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/json_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/json_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/logical_operator.py` & `vellum_ai-0.3.9/src/vellum/types/logical_operator.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/metadata_filter_config_request.py` & `vellum_ai-0.3.9/src/vellum/types/metadata_filter_config_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/metadata_filter_rule_combinator.py` & `vellum_ai-0.3.9/src/vellum/types/metadata_filter_rule_combinator.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/metadata_filter_rule_request.py` & `vellum_ai-0.3.9/src/vellum/types/metadata_filter_rule_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/model_version_build_config.py` & `vellum_ai-0.3.9/src/vellum/types/model_version_build_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/model_version_exec_config.py` & `vellum_ai-0.3.9/src/vellum/types/model_version_exec_config.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/model_version_exec_config_parameters.py` & `vellum_ai-0.3.9/src/vellum/types/model_version_exec_config_parameters.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/model_version_read.py` & `vellum_ai-0.3.9/src/vellum/types/model_version_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/model_version_read_status_enum.py` & `vellum_ai-0.3.9/src/vellum/types/model_version_read_status_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/model_version_sandbox_snapshot.py` & `vellum_ai-0.3.9/src/vellum/types/model_version_sandbox_snapshot.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/named_test_case_chat_history_variable_value_request.py` & `vellum_ai-0.3.9/src/vellum/types/named_test_case_chat_history_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/named_test_case_error_variable_value_request.py` & `vellum_ai-0.3.9/src/vellum/types/named_test_case_error_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/named_test_case_json_variable_value_request.py` & `vellum_ai-0.3.9/src/vellum/types/named_test_case_json_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/named_test_case_number_variable_value_request.py` & `vellum_ai-0.3.9/src/vellum/types/named_test_case_number_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/named_test_case_search_results_variable_value_request.py` & `vellum_ai-0.3.9/src/vellum/types/named_test_case_search_results_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/named_test_case_string_variable_value_request.py` & `vellum_ai-0.3.9/src/vellum/types/named_test_case_string_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/named_test_case_variable_value_request.py` & `vellum_ai-0.3.9/src/vellum/types/named_test_case_variable_value_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_input_compiled_array_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_array_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 except ImportError:
     import pydantic  # type: ignore
 
 
 class NodeInputCompiledArrayValue(pydantic.BaseModel):
     node_input_id: str
     key: str
-    value: typing.List[ArrayVariableValueItem]
+    value: typing.Optional[typing.List[ArrayVariableValueItem]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_input_compiled_chat_history_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_chat_history_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_input_compiled_error_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_error_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_input_compiled_json_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_json_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_input_compiled_number_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_number_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_input_compiled_search_results_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_search_results_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_input_compiled_string_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_input_compiled_string_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_input_variable_compiled_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_input_variable_compiled_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_output_compiled_array_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_search_results_value.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .array_variable_value_item import ArrayVariableValueItem
+from .search_result import SearchResult
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class NodeOutputCompiledArrayValue(pydantic.BaseModel):
+class NodeOutputCompiledSearchResultsValue(pydantic.BaseModel):
     node_output_id: str
-    value: typing.List[ArrayVariableValueItem]
+    value: typing.Optional[typing.List[SearchResult]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_output_compiled_chat_history_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_chat_history_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_output_compiled_error_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_error_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_output_compiled_function_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_function_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_output_compiled_json_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_json_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_output_compiled_number_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_number_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_output_compiled_search_results_value.py` & `vellum_ai-0.3.9/src/vellum/types/upload_document_error_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from .search_result import SearchResult
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class NodeOutputCompiledSearchResultsValue(pydantic.BaseModel):
-    node_output_id: str
-    value: typing.Optional[typing.List[SearchResult]]
+class UploadDocumentErrorResponse(pydantic.BaseModel):
+    detail: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_output_compiled_string_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_string_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/node_output_compiled_value.py` & `vellum_ai-0.3.9/src/vellum/types/node_output_compiled_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/normalized_log_probs.py` & `vellum_ai-0.3.9/src/vellum/types/normalized_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/normalized_token_log_probs.py` & `vellum_ai-0.3.9/src/vellum/types/normalized_token_log_probs.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/number_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/number_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/paginated_slim_deployment_read_list.py` & `vellum_ai-0.3.9/src/vellum/types/paginated_slim_deployment_read_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/paginated_slim_document_list.py` & `vellum_ai-0.3.9/src/vellum/types/paginated_slim_document_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/paginated_slim_workflow_deployment_list.py` & `vellum_ai-0.3.9/src/vellum/types/paginated_slim_workflow_deployment_list.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/processing_failure_reason_enum.py` & `vellum_ai-0.3.9/src/vellum/types/processing_failure_reason_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/processing_state_enum.py` & `vellum_ai-0.3.9/src/vellum/types/processing_state_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/prompt_deployment_expand_meta_request_request.py` & `vellum_ai-0.3.9/src/vellum/types/prompt_deployment_expand_meta_request_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/prompt_deployment_input_request.py` & `vellum_ai-0.3.9/src/vellum/types/prompt_deployment_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/prompt_execution_meta.py` & `vellum_ai-0.3.9/src/vellum/types/prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/prompt_node_result.py` & `vellum_ai-0.3.9/src/vellum/types/prompt_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/prompt_node_result_data.py` & `vellum_ai-0.3.9/src/vellum/types/prompt_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/prompt_output.py` & `vellum_ai-0.3.9/src/vellum/types/prompt_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/prompt_template_block.py` & `vellum_ai-0.3.9/src/vellum/types/prompt_template_block.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/prompt_template_block_data.py` & `vellum_ai-0.3.9/src/vellum/types/prompt_template_block_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/prompt_template_block_data_request.py` & `vellum_ai-0.3.9/src/vellum/types/prompt_template_block_data_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/prompt_template_block_properties.py` & `vellum_ai-0.3.9/src/vellum/types/prompt_template_block_properties.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/prompt_template_block_properties_request.py` & `vellum_ai-0.3.9/src/vellum/types/prompt_template_block_properties_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/prompt_template_block_request.py` & `vellum_ai-0.3.9/src/vellum/types/prompt_template_block_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/provider_enum.py` & `vellum_ai-0.3.9/src/vellum/types/provider_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/raw_prompt_execution_overrides_request.py` & `vellum_ai-0.3.9/src/vellum/types/raw_prompt_execution_overrides_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/register_prompt_error_response.py` & `vellum_ai-0.3.9/src/vellum/types/register_prompt_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/register_prompt_model_parameters_request.py` & `vellum_ai-0.3.9/src/vellum/types/register_prompt_model_parameters_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/register_prompt_prompt.py` & `vellum_ai-0.3.9/src/vellum/types/register_prompt_prompt.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/register_prompt_prompt_info_request.py` & `vellum_ai-0.3.9/src/vellum/types/register_prompt_prompt_info_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/register_prompt_response.py` & `vellum_ai-0.3.9/src/vellum/types/register_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/registered_prompt_deployment.py` & `vellum_ai-0.3.9/src/vellum/types/registered_prompt_deployment.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/registered_prompt_input_variable_request.py` & `vellum_ai-0.3.9/src/vellum/types/registered_prompt_input_variable_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/registered_prompt_model_version.py` & `vellum_ai-0.3.9/src/vellum/types/registered_prompt_model_version.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/registered_prompt_sandbox.py` & `vellum_ai-0.3.9/src/vellum/types/registered_prompt_sandbox.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/registered_prompt_sandbox_snapshot.py` & `vellum_ai-0.3.9/src/vellum/types/registered_prompt_sandbox_snapshot.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/rejected_execute_prompt_event.py` & `vellum_ai-0.3.9/src/vellum/types/rejected_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/rejected_execute_prompt_response.py` & `vellum_ai-0.3.9/src/vellum/types/rejected_execute_prompt_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/rejected_execute_workflow_workflow_result_event.py` & `vellum_ai-0.3.9/src/vellum/types/rejected_execute_workflow_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/rejected_function_call.py` & `vellum_ai-0.3.9/src/vellum/types/rejected_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/rejected_prompt_execution_meta.py` & `vellum_ai-0.3.9/src/vellum/types/rejected_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/rejected_workflow_node_result_event.py` & `vellum_ai-0.3.9/src/vellum/types/rejected_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/sandbox_scenario.py` & `vellum_ai-0.3.9/src/vellum/types/sandbox_scenario.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/scenario_input.py` & `vellum_ai-0.3.9/src/vellum/types/scenario_input.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/scenario_input_request.py` & `vellum_ai-0.3.9/src/vellum/types/scenario_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/scenario_input_type_enum.py` & `vellum_ai-0.3.9/src/vellum/types/scenario_input_type_enum.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_error_response.py` & `vellum_ai-0.3.9/src/vellum/types/search_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_filters_request.py` & `vellum_ai-0.3.9/src/vellum/types/search_filters_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_node_result.py` & `vellum_ai-0.3.9/src/vellum/types/search_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_node_result_data.py` & `vellum_ai-0.3.9/src/vellum/types/search_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_request_options_request.py` & `vellum_ai-0.3.9/src/vellum/types/search_request_options_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_response.py` & `vellum_ai-0.3.9/src/vellum/types/search_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_result.py` & `vellum_ai-0.3.9/src/vellum/types/search_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_result_document.py` & `vellum_ai-0.3.9/src/vellum/types/search_result_document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_result_document_request.py` & `vellum_ai-0.3.9/src/vellum/types/search_result_document_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_result_merging_request.py` & `vellum_ai-0.3.9/src/vellum/types/search_result_merging_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_result_request.py` & `vellum_ai-0.3.9/src/vellum/types/search_result_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_results_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/search_results_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/search_weights_request.py` & `vellum_ai-0.3.9/src/vellum/types/search_weights_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/slim_deployment_read.py` & `vellum_ai-0.3.9/src/vellum/types/slim_deployment_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/slim_document.py` & `vellum_ai-0.3.9/src/vellum/types/slim_document.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/slim_workflow_deployment.py` & `vellum_ai-0.3.9/src/vellum/types/slim_workflow_deployment.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/streaming_execute_prompt_event.py` & `vellum_ai-0.3.9/src/vellum/types/streaming_execute_prompt_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/streaming_prompt_execution_meta.py` & `vellum_ai-0.3.9/src/vellum/types/streaming_prompt_execution_meta.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/streaming_workflow_node_result_event.py` & `vellum_ai-0.3.9/src/vellum/types/streaming_workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/string_chat_message_content.py` & `vellum_ai-0.3.9/src/vellum/types/string_chat_message_content.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/string_chat_message_content_request.py` & `vellum_ai-0.3.9/src/vellum/types/string_chat_message_content_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/string_input_request.py` & `vellum_ai-0.3.9/src/vellum/types/string_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/string_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/submit_completion_actual_request.py` & `vellum_ai-0.3.9/src/vellum/types/submit_completion_actual_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/submit_completion_actuals_error_response.py` & `vellum_ai-0.3.9/src/vellum/types/submit_completion_actuals_error_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/submit_workflow_execution_actual_request.py` & `vellum_ai-0.3.9/src/vellum/types/submit_workflow_execution_actual_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/templating_node_chat_history_result.py` & `vellum_ai-0.3.9/src/vellum/types/templating_node_chat_history_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/templating_node_error_result.py` & `vellum_ai-0.3.9/src/vellum/types/templating_node_error_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/templating_node_json_result.py` & `vellum_ai-0.3.9/src/vellum/types/templating_node_json_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/templating_node_number_result.py` & `vellum_ai-0.3.9/src/vellum/types/templating_node_number_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/templating_node_result.py` & `vellum_ai-0.3.9/src/vellum/types/templating_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/templating_node_result_data.py` & `vellum_ai-0.3.9/src/vellum/types/templating_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/templating_node_result_output.py` & `vellum_ai-0.3.9/src/vellum/types/templating_node_result_output.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/templating_node_search_results_result.py` & `vellum_ai-0.3.9/src/vellum/types/templating_node_search_results_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/templating_node_string_result.py` & `vellum_ai-0.3.9/src/vellum/types/templating_node_string_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/terminal_node_chat_history_result.py` & `vellum_ai-0.3.9/src/vellum/types/terminal_node_chat_history_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/terminal_node_error_result.py` & `vellum_ai-0.3.9/src/vellum/types/terminal_node_error_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/terminal_node_json_result.py` & `vellum_ai-0.3.9/src/vellum/types/terminal_node_json_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/terminal_node_number_result.py` & `vellum_ai-0.3.9/src/vellum/types/terminal_node_number_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/terminal_node_result.py` & `vellum_ai-0.3.9/src/vellum/types/terminal_node_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/terminal_node_result_data.py` & `vellum_ai-0.3.9/src/vellum/types/terminal_node_result_data.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/terminal_node_result_output.py` & `vellum_ai-0.3.9/src/vellum/types/terminal_node_result_output.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 from __future__ import annotations
 
 import typing
 
 import typing_extensions
 
+from .terminal_node_array_result import TerminalNodeArrayResult
 from .terminal_node_chat_history_result import TerminalNodeChatHistoryResult
 from .terminal_node_error_result import TerminalNodeErrorResult
+from .terminal_node_function_call_result import TerminalNodeFunctionCallResult
 from .terminal_node_json_result import TerminalNodeJsonResult
 from .terminal_node_number_result import TerminalNodeNumberResult
 from .terminal_node_search_results_result import TerminalNodeSearchResultsResult
 from .terminal_node_string_result import TerminalNodeStringResult
 
 
 class TerminalNodeResultOutput_String(TerminalNodeStringResult):
@@ -55,14 +57,32 @@
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
+class TerminalNodeResultOutput_Array(TerminalNodeArrayResult):
+    type: typing_extensions.Literal["ARRAY"]
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+
+
+class TerminalNodeResultOutput_FunctionCall(TerminalNodeFunctionCallResult):
+    type: typing_extensions.Literal["FUNCTION_CALL"]
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+
+
 class TerminalNodeResultOutput_Error(TerminalNodeErrorResult):
     type: typing_extensions.Literal["ERROR"]
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
@@ -70,9 +90,11 @@
 
 TerminalNodeResultOutput = typing.Union[
     TerminalNodeResultOutput_String,
     TerminalNodeResultOutput_Number,
     TerminalNodeResultOutput_Json,
     TerminalNodeResultOutput_ChatHistory,
     TerminalNodeResultOutput_SearchResults,
+    TerminalNodeResultOutput_Array,
+    TerminalNodeResultOutput_FunctionCall,
     TerminalNodeResultOutput_Error,
 ]
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/terminal_node_search_results_result.py` & `vellum_ai-0.3.9/src/vellum/types/terminal_node_search_results_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/terminal_node_string_result.py` & `vellum_ai-0.3.9/src/vellum/types/terminal_node_string_result.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/test_case_chat_history_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/test_case_chat_history_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/test_case_error_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/test_case_error_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/test_case_json_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/test_case_json_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/test_case_number_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/test_case_number_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/test_case_search_results_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/test_case_search_results_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/test_case_string_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/test_case_string_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/test_case_variable_value.py` & `vellum_ai-0.3.9/src/vellum/types/test_case_variable_value.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/test_suite_test_case.py` & `vellum_ai-0.3.9/src/vellum/types/test_suite_test_case.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/upload_document_error_response.py` & `vellum_ai-0.3.9/src/vellum/types/vellum_image.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class UploadDocumentErrorResponse(pydantic.BaseModel):
-    detail: str
+class VellumImage(pydantic.BaseModel):
+    src: str
+    metadata: typing.Optional[typing.Dict[str, typing.Any]]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/upload_document_response.py` & `vellum_ai-0.3.9/src/vellum/types/upload_document_response.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/vellum_error.py` & `vellum_ai-0.3.9/src/vellum/types/vellum_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/vellum_error_code_enum.py` & `vellum_ai-0.3.9/src/vellum/types/vellum_error_code_enum.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,25 +7,30 @@
 
 
 class VellumErrorCodeEnum(str, enum.Enum):
     """
     - `INVALID_REQUEST` - INVALID_REQUEST
     - `PROVIDER_ERROR` - PROVIDER_ERROR
     - `INTERNAL_SERVER_ERROR` - INTERNAL_SERVER_ERROR
+    - `USER_DEFINED_ERROR` - USER_DEFINED_ERROR
     """
 
     INVALID_REQUEST = "INVALID_REQUEST"
     PROVIDER_ERROR = "PROVIDER_ERROR"
     INTERNAL_SERVER_ERROR = "INTERNAL_SERVER_ERROR"
+    USER_DEFINED_ERROR = "USER_DEFINED_ERROR"
 
     def visit(
         self,
         invalid_request: typing.Callable[[], T_Result],
         provider_error: typing.Callable[[], T_Result],
         internal_server_error: typing.Callable[[], T_Result],
+        user_defined_error: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is VellumErrorCodeEnum.INVALID_REQUEST:
             return invalid_request()
         if self is VellumErrorCodeEnum.PROVIDER_ERROR:
             return provider_error()
         if self is VellumErrorCodeEnum.INTERNAL_SERVER_ERROR:
             return internal_server_error()
+        if self is VellumErrorCodeEnum.USER_DEFINED_ERROR:
+            return user_defined_error()
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/vellum_error_request.py` & `vellum_ai-0.3.9/src/vellum/types/vellum_error_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/vellum_image.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_output_number.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,17 +7,22 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class VellumImage(pydantic.BaseModel):
-    src: str
-    metadata: typing.Optional[typing.Dict[str, typing.Any]]
+class WorkflowOutputNumber(pydantic.BaseModel):
+    """
+    A number output from a Workflow execution.
+    """
+
+    id: str
+    name: str = pydantic.Field(description="The output's name, as defined in the workflow")
+    value: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/vellum_image_request.py` & `vellum_ai-0.3.9/src/vellum/types/vellum_image_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/vellum_variable.py` & `vellum_ai-0.3.9/src/vellum/types/vellum_variable.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/vellum_variable_type.py` & `vellum_ai-0.3.9/src/vellum/types/vellum_variable_type.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_deployment_read.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_deployment_read.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_event_error.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_event_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_execution_actual_chat_history_request.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_execution_actual_chat_history_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_execution_actual_json_request.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_execution_actual_json_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_execution_actual_string_request.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_execution_actual_string_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_execution_event_error_code.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_execution_event_error_code.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,37 +10,42 @@
     """
     - `WORKFLOW_INITIALIZATION` - WORKFLOW_INITIALIZATION
     - `NODE_EXECUTION_COUNT_LIMIT_REACHED` - NODE_EXECUTION_COUNT_LIMIT_REACHED
     - `INTERNAL_SERVER_ERROR` - INTERNAL_SERVER_ERROR
     - `NODE_EXECUTION` - NODE_EXECUTION
     - `LLM_PROVIDER` - LLM_PROVIDER
     - `INVALID_TEMPLATE` - INVALID_TEMPLATE
+    - `USER_DEFINED_ERROR` - USER_DEFINED_ERROR
     """
 
     WORKFLOW_INITIALIZATION = "WORKFLOW_INITIALIZATION"
     NODE_EXECUTION_COUNT_LIMIT_REACHED = "NODE_EXECUTION_COUNT_LIMIT_REACHED"
     INTERNAL_SERVER_ERROR = "INTERNAL_SERVER_ERROR"
     NODE_EXECUTION = "NODE_EXECUTION"
     LLM_PROVIDER = "LLM_PROVIDER"
     INVALID_TEMPLATE = "INVALID_TEMPLATE"
+    USER_DEFINED_ERROR = "USER_DEFINED_ERROR"
 
     def visit(
         self,
         workflow_initialization: typing.Callable[[], T_Result],
         node_execution_count_limit_reached: typing.Callable[[], T_Result],
         internal_server_error: typing.Callable[[], T_Result],
         node_execution: typing.Callable[[], T_Result],
         llm_provider: typing.Callable[[], T_Result],
         invalid_template: typing.Callable[[], T_Result],
+        user_defined_error: typing.Callable[[], T_Result],
     ) -> T_Result:
         if self is WorkflowExecutionEventErrorCode.WORKFLOW_INITIALIZATION:
             return workflow_initialization()
         if self is WorkflowExecutionEventErrorCode.NODE_EXECUTION_COUNT_LIMIT_REACHED:
             return node_execution_count_limit_reached()
         if self is WorkflowExecutionEventErrorCode.INTERNAL_SERVER_ERROR:
             return internal_server_error()
         if self is WorkflowExecutionEventErrorCode.NODE_EXECUTION:
             return node_execution()
         if self is WorkflowExecutionEventErrorCode.LLM_PROVIDER:
             return llm_provider()
         if self is WorkflowExecutionEventErrorCode.INVALID_TEMPLATE:
             return invalid_template()
+        if self is WorkflowExecutionEventErrorCode.USER_DEFINED_ERROR:
+            return user_defined_error()
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_execution_event_type.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_execution_event_type.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_execution_node_result_event.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_execution_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_execution_workflow_result_event.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_execution_workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_node_result_data.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_node_result_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import typing_extensions
 
 from .api_node_result import ApiNodeResult
 from .code_execution_node_result import CodeExecutionNodeResult
 from .conditional_node_result import ConditionalNodeResult
 from .prompt_node_result import PromptNodeResult
 from .search_node_result import SearchNodeResult
+from .subworkflow_node_result import SubworkflowNodeResult
 from .templating_node_result import TemplatingNodeResult
 from .terminal_node_result import TerminalNodeResult
 
 
 class WorkflowNodeResultData_Prompt(PromptNodeResult):
     type: typing_extensions.Literal["PROMPT"]
 
@@ -74,16 +75,26 @@
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
+class WorkflowNodeResultData_Subworkflow(SubworkflowNodeResult):
+    type: typing_extensions.Literal["SUBWORKFLOW"]
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+
+
 WorkflowNodeResultData = typing.Union[
     WorkflowNodeResultData_Prompt,
     WorkflowNodeResultData_Search,
     WorkflowNodeResultData_Templating,
     WorkflowNodeResultData_CodeExecution,
     WorkflowNodeResultData_Conditional,
     WorkflowNodeResultData_Api,
     WorkflowNodeResultData_Terminal,
+    WorkflowNodeResultData_Subworkflow,
 ]
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_node_result_event.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_node_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_node_result_event_state.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_node_result_event_state.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_output.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 import typing
 
 import typing_extensions
 
+from .workflow_output_array import WorkflowOutputArray
 from .workflow_output_chat_history import WorkflowOutputChatHistory
 from .workflow_output_error import WorkflowOutputError
 from .workflow_output_function_call import WorkflowOutputFunctionCall
 from .workflow_output_image import WorkflowOutputImage
 from .workflow_output_json import WorkflowOutputJson
 from .workflow_output_number import WorkflowOutputNumber
 from .workflow_output_search_results import WorkflowOutputSearchResults
@@ -57,14 +58,23 @@
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
+class WorkflowOutput_Array(WorkflowOutputArray):
+    type: typing_extensions.Literal["ARRAY"]
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+
+
 class WorkflowOutput_Error(WorkflowOutputError):
     type: typing_extensions.Literal["ERROR"]
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
@@ -90,11 +100,12 @@
 
 WorkflowOutput = typing.Union[
     WorkflowOutput_String,
     WorkflowOutput_Number,
     WorkflowOutput_Json,
     WorkflowOutput_ChatHistory,
     WorkflowOutput_SearchResults,
+    WorkflowOutput_Array,
     WorkflowOutput_Error,
     WorkflowOutput_FunctionCall,
     WorkflowOutput_Image,
 ]
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_output_chat_history.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_output_chat_history.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_output_error.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_output_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_output_function_call.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_output_function_call.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_output_image.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_output_image.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_output_json.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_output_json.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_output_number.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_request_json_input_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class WorkflowOutputNumber(pydantic.BaseModel):
+class WorkflowRequestJsonInputRequest(pydantic.BaseModel):
     """
-    A number output from a Workflow execution.
+    The input for a JSON variable in a Workflow.
     """
 
-    id: str
-    name: str = pydantic.Field(description="The output's name, as defined in the workflow")
-    value: float
+    name: str = pydantic.Field(description="The variable's name, as defined in the Workflow.")
+    value: typing.Dict[str, typing.Any]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_output_search_results.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_output_search_results.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_output_string.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_output_string.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_request_chat_history_input_request.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_request_chat_history_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_request_input_request.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_request_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_request_json_input_request.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_request_string_input_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class WorkflowRequestJsonInputRequest(pydantic.BaseModel):
+class WorkflowRequestStringInputRequest(pydantic.BaseModel):
     """
-    The input for a JSON variable in a Workflow.
+    The input for a string variable in a Workflow.
     """
 
     name: str = pydantic.Field(description="The variable's name, as defined in the Workflow.")
-    value: typing.Dict[str, typing.Any]
+    value: str
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_request_number_input_request.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_request_number_input_request.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_request_string_input_request.py` & `vellum_ai-0.3.9/src/vellum/types/subworkflow_node_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,22 +7,19 @@
 
 try:
     import pydantic.v1 as pydantic  # type: ignore
 except ImportError:
     import pydantic  # type: ignore
 
 
-class WorkflowRequestStringInputRequest(pydantic.BaseModel):
+class SubworkflowNodeResult(pydantic.BaseModel):
     """
-    The input for a string variable in a Workflow.
+    A Node Result Event emitted from a Subworkflow Node.
     """
 
-    name: str = pydantic.Field(description="The variable's name, as defined in the Workflow.")
-    value: str
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_result_event.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_result_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 
 from __future__ import annotations
 
 import typing
 
 import typing_extensions
 
+from .workflow_result_event_output_data_array import WorkflowResultEventOutputDataArray
 from .workflow_result_event_output_data_chat_history import WorkflowResultEventOutputDataChatHistory
 from .workflow_result_event_output_data_error import WorkflowResultEventOutputDataError
+from .workflow_result_event_output_data_function_call import WorkflowResultEventOutputDataFunctionCall
 from .workflow_result_event_output_data_json import WorkflowResultEventOutputDataJson
 from .workflow_result_event_output_data_number import WorkflowResultEventOutputDataNumber
 from .workflow_result_event_output_data_search_results import WorkflowResultEventOutputDataSearchResults
 from .workflow_result_event_output_data_string import WorkflowResultEventOutputDataString
 
 
 class WorkflowResultEventOutputData_String(WorkflowResultEventOutputDataString):
@@ -55,14 +57,32 @@
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
 
 
+class WorkflowResultEventOutputData_Array(WorkflowResultEventOutputDataArray):
+    type: typing_extensions.Literal["ARRAY"]
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+
+
+class WorkflowResultEventOutputData_FunctionCall(WorkflowResultEventOutputDataFunctionCall):
+    type: typing_extensions.Literal["FUNCTION_CALL"]
+
+    class Config:
+        frozen = True
+        smart_union = True
+        allow_population_by_field_name = True
+
+
 class WorkflowResultEventOutputData_Error(WorkflowResultEventOutputDataError):
     type: typing_extensions.Literal["ERROR"]
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
@@ -70,9 +90,11 @@
 
 WorkflowResultEventOutputData = typing.Union[
     WorkflowResultEventOutputData_String,
     WorkflowResultEventOutputData_Number,
     WorkflowResultEventOutputData_Json,
     WorkflowResultEventOutputData_ChatHistory,
     WorkflowResultEventOutputData_SearchResults,
+    WorkflowResultEventOutputData_Array,
+    WorkflowResultEventOutputData_FunctionCall,
     WorkflowResultEventOutputData_Error,
 ]
```

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data_chat_history.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_chat_history.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data_error.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_error.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data_json.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_json.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data_number.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_number.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data_search_results.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_search_results.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_result_event_output_data_string.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_result_event_output_data_string.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/src/vellum/types/workflow_stream_event.py` & `vellum_ai-0.3.9/src/vellum/types/workflow_stream_event.py`

 * *Files identical despite different names*

### Comparing `vellum_ai-0.3.8/PKG-INFO` & `vellum_ai-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vellum-ai
-Version: 0.3.8
+Version: 0.3.9
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

