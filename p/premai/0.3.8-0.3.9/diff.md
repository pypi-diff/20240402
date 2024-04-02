# Comparing `tmp/premai-0.3.8.tar.gz` & `tmp/premai-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "premai-0.3.8.tar", max compression
+gzip compressed data, was "premai-0.3.9.tar", max compression
```

## Comparing `premai-0.3.8.tar` & `premai-0.3.9.tar`

### file list

```diff
@@ -1,296 +1,82 @@
--rw-r--r--   0        0        0     1241 2024-02-16 13:49:48.551050 premai-0.3.8/README.md
--rw-r--r--   0        0        0      682 2024-02-16 13:49:48.551050 premai-0.3.8/premai/__init__.py
--rw-r--r--   0        0        0     3079 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/__init__.py
--rw-r--r--   0        0        0        0 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/chat_completions/__init__.py
--rw-r--r--   0        0        0    12136 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/chat_completions/v1_chat_completions_create.py
--rw-r--r--   0        0        0        0 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/datapoints/__init__.py
--rw-r--r--   0        0        0     2466 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/datapoints/v1_data_points_create.py
--rw-r--r--   0        0        0     1747 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/datapoints/v1_data_points_destroy.py
--rw-r--r--   0        0        0     2140 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/datapoints/v1_data_points_list.py
--rw-r--r--   0        0        0     2663 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/datapoints/v1_data_points_partial_update.py
--rw-r--r--   0        0        0     2033 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/datapoints/v1_data_points_retrieve.py
--rw-r--r--   0        0        0     2537 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/datapoints/v1_data_points_update.py
--rw-r--r--   0        0        0        0 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/embeddings/__init__.py
--rw-r--r--   0        0        0     6388 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/embeddings/v1_embeddings_create.py
--rw-r--r--   0        0        0        0 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/finetuning/__init__.py
--rw-r--r--   0        0        0     6374 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/finetuning/v1_finetuning_create.py
--rw-r--r--   0        0        0     6207 2024-02-16 13:49:48.551050 premai-0.3.8/premai/api/finetuning/v1_finetuning_retrieve.py
--rw-r--r--   0        0        0    11035 2024-02-16 13:49:48.551050 premai-0.3.8/premai/client.py
--rw-r--r--   0        0        0      489 2024-02-16 13:49:48.551050 premai-0.3.8/premai/errors.py
--rw-r--r--   0        0        0    35790 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/__init__.py
--rw-r--r--   0        0        0     2090 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/api_response_validation_error.py
--rw-r--r--   0        0        0      197 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/api_response_validation_error_code.py
--rw-r--r--   0        0        0      201 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/api_response_validation_error_code_enum.py
--rw-r--r--   0        0        0     1984 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/authentication_error.py
--rw-r--r--   0        0        0      176 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/authentication_error_code.py
--rw-r--r--   0        0        0      180 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/authentication_error_code_enum.py
--rw-r--r--   0        0        0     1904 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/catch_all_error.py
--rw-r--r--   0        0        0      158 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/catch_all_error_code.py
--rw-r--r--   0        0        0      162 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/catch_all_error_code_enum.py
--rw-r--r--   0        0        0    14109 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/chat_completion_input.py
--rw-r--r--   0        0        0     1535 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/chat_completion_input_logit_bias_type_0.py
--rw-r--r--   0        0        0     2410 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/chat_completion_input_messages_item.py
--rw-r--r--   0        0        0     1614 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/chat_completion_input_messages_item_role.py
--rw-r--r--   0        0        0     1550 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/chat_completion_input_response_format_type_0.py
--rw-r--r--   0        0        0     1426 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/chat_completion_input_tools_item.py
--rw-r--r--   0        0        0     4622 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/chat_completion_response.py
--rw-r--r--   0        0        0     2087 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/chat_completion_response_choices_item.py
--rw-r--r--   0        0        0     2697 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/chat_completion_response_usage.py
--rw-r--r--   0        0        0     1900 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/conflict_error.py
--rw-r--r--   0        0        0      158 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/conflict_error_code.py
--rw-r--r--   0        0        0      162 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/conflict_error_code_enum.py
--rw-r--r--   0        0        0     4472 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/data_point.py
--rw-r--r--   0        0        0     1860 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/embedding.py
--rw-r--r--   0        0        0     5481 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/embeddings_input.py
--rw-r--r--   0        0        0     1429 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/embeddings_input_encoding_format.py
--rw-r--r--   0        0        0     3850 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/embeddings_response.py
--rw-r--r--   0        0        0     1971 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/embeddings_response_data_item.py
--rw-r--r--   0        0        0     2670 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/embeddings_response_usage.py
--rw-r--r--   0        0        0      165 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/encoding_format_enum.py
--rw-r--r--   0        0        0     4678 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/fine_tuning_input.py
--rw-r--r--   0        0        0     1901 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/fine_tuning_input_training_data_item.py
--rw-r--r--   0        0        0     1907 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/fine_tuning_input_validaton_data_item.py
--rw-r--r--   0        0        0     1635 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/fine_tuning_response.py
--rw-r--r--   0        0        0     1802 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/fine_tuning_sample.py
--rw-r--r--   0        0        0     4068 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/input_data_point.py
--rw-r--r--   0        0        0     2072 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/internal_server_error_type_0.py
--rw-r--r--   0        0        0      197 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/internal_server_error_type_0_code.py
--rw-r--r--   0        0        0     2070 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/internal_server_error_type_1.py
--rw-r--r--   0        0        0      195 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/internal_server_error_type_1_code.py
--rw-r--r--   0        0        0     2062 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/internal_server_error_type_2.py
--rw-r--r--   0        0        0      187 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/internal_server_error_type_2_code.py
--rw-r--r--   0        0        0     2064 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/internal_server_error_type_3.py
--rw-r--r--   0        0        0      189 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/internal_server_error_type_3_code.py
--rw-r--r--   0        0        0     2070 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/internal_server_error_type_4.py
--rw-r--r--   0        0        0      195 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/internal_server_error_type_4_code.py
--rw-r--r--   0        0        0     2044 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/internal_server_error_type_5.py
--rw-r--r--   0        0        0      169 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/internal_server_error_type_5_code.py
--rw-r--r--   0        0        0     2054 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/message.py
--rw-r--r--   0        0        0     1458 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/message_role.py
--rw-r--r--   0        0        0     1978 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/model_not_found_error.py
--rw-r--r--   0        0        0      173 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/model_not_found_error_code.py
--rw-r--r--   0        0        0      177 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/model_not_found_error_code_enum.py
--rw-r--r--   0        0        0     1988 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/not_found_error_type_0.py
--rw-r--r--   0        0        0      179 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/not_found_error_type_0_code.py
--rw-r--r--   0        0        0     1982 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/not_found_error_type_1.py
--rw-r--r--   0        0        0      173 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/not_found_error_type_1_code.py
--rw-r--r--   0        0        0     5486 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/patched_data_point.py
--rw-r--r--   0        0        0     2016 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/permission_denied_error.py
--rw-r--r--   0        0        0      182 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/permission_denied_error_code.py
--rw-r--r--   0        0        0      186 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/permission_denied_error_code_enum.py
--rw-r--r--   0        0        0     2090 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_api_connection_error.py
--rw-r--r--   0        0        0      197 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_api_connection_error_code.py
--rw-r--r--   0        0        0      201 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_api_connection_error_code_enum.py
--rw-r--r--   0        0        0     2034 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_api_status_error.py
--rw-r--r--   0        0        0      185 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_api_status_error_code.py
--rw-r--r--   0        0        0      189 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_api_status_error_code_enum.py
--rw-r--r--   0        0        0     2048 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_api_timeout_error.py
--rw-r--r--   0        0        0      188 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_api_timeout_error_code.py
--rw-r--r--   0        0        0      192 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_api_timeout_error_code_enum.py
--rw-r--r--   0        0        0     2104 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_internal_server_error.py
--rw-r--r--   0        0        0      200 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_internal_server_error_code.py
--rw-r--r--   0        0        0      204 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_internal_server_error_code_enum.py
--rw-r--r--   0        0        0     2020 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_not_found_error.py
--rw-r--r--   0        0        0      182 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_not_found_error_code.py
--rw-r--r--   0        0        0      186 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/provider_not_found_error_code_enum.py
--rw-r--r--   0        0        0     1918 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/rate_limit_error.py
--rw-r--r--   0        0        0      161 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/rate_limit_error_code.py
--rw-r--r--   0        0        0      165 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/rate_limit_error_code_enum.py
--rw-r--r--   0        0        0     1964 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/response_choice.py
--rw-r--r--   0        0        0     4143 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/retrieve_fine_tuning_response.py
--rw-r--r--   0        0        0      181 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/role_enum.py
--rw-r--r--   0        0        0     2058 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/unprocessable_entity_error.py
--rw-r--r--   0        0        0      191 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/unprocessable_entity_error_code.py
--rw-r--r--   0        0        0      195 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/unprocessable_entity_error_code_enum.py
--rw-r--r--   0        0        0     2515 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/usage.py
--rw-r--r--   0        0        0    14902 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_data_body.py
--rw-r--r--   0        0        0     1616 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_data_body_logit_bias_type_0.py
--rw-r--r--   0        0        0     2639 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_data_body_messages_item.py
--rw-r--r--   0        0        0     1695 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_data_body_messages_item_role.py
--rw-r--r--   0        0        0     1631 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_data_body_response_format_type_0.py
--rw-r--r--   0        0        0     1507 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_data_body_tools_item.py
--rw-r--r--   0        0        0    19841 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_files_body.py
--rw-r--r--   0        0        0     1622 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_files_body_logit_bias_type_0.py
--rw-r--r--   0        0        0     2653 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_files_body_messages_item.py
--rw-r--r--   0        0        0     1701 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_files_body_messages_item_role.py
--rw-r--r--   0        0        0     1637 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_files_body_response_format_type_0.py
--rw-r--r--   0        0        0     1513 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_files_body_tools_item.py
--rw-r--r--   0        0        0    14902 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_json_body.py
--rw-r--r--   0        0        0     1616 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_json_body_logit_bias_type_0.py
--rw-r--r--   0        0        0     2639 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_json_body_messages_item.py
--rw-r--r--   0        0        0     1695 2024-02-16 13:49:48.555050 premai-0.3.8/premai/models/v1_chat_completions_create_json_body_messages_item_role.py
--rw-r--r--   0        0        0     1631 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_json_body_response_format_type_0.py
--rw-r--r--   0        0        0     1507 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_json_body_tools_item.py
--rw-r--r--   0        0        0     4944 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_200.py
--rw-r--r--   0        0        0     2168 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_200_choices_item.py
--rw-r--r--   0        0        0     2778 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_200_usage.py
--rw-r--r--   0        0        0     2863 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_400.py
--rw-r--r--   0        0        0      183 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_400_code.py
--rw-r--r--   0        0        0     2438 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_400_details.py
--rw-r--r--   0        0        0     3184 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_400_details_additional_property.py
--rw-r--r--   0        0        0     1735 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_400_details_additional_property_error_messages_item.py
--rw-r--r--   0        0        0     2180 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_401.py
--rw-r--r--   0        0        0      191 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_401_code.py
--rw-r--r--   0        0        0     2184 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_403.py
--rw-r--r--   0        0        0      195 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_403_code.py
--rw-r--r--   0        0        0     2252 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_404_type_0.py
--rw-r--r--   0        0        0      200 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_404_type_0_code.py
--rw-r--r--   0        0        0     2246 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_404_type_1.py
--rw-r--r--   0        0        0      194 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_404_type_1_code.py
--rw-r--r--   0        0        0     2168 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_409.py
--rw-r--r--   0        0        0      179 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_409_code.py
--rw-r--r--   0        0        0     2190 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_422.py
--rw-r--r--   0        0        0      201 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_422_code.py
--rw-r--r--   0        0        0     2170 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_429.py
--rw-r--r--   0        0        0      181 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_429_code.py
--rw-r--r--   0        0        0     2276 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_500_type_0.py
--rw-r--r--   0        0        0      212 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_500_type_0_code.py
--rw-r--r--   0        0        0     2262 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_500_type_1.py
--rw-r--r--   0        0        0      210 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_500_type_1_code.py
--rw-r--r--   0        0        0     2254 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_500_type_2.py
--rw-r--r--   0        0        0      202 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_500_type_2_code.py
--rw-r--r--   0        0        0     2256 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_500_type_3.py
--rw-r--r--   0        0        0      204 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_500_type_3_code.py
--rw-r--r--   0        0        0     2262 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_500_type_4.py
--rw-r--r--   0        0        0      210 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_500_type_4_code.py
--rw-r--r--   0        0        0     2236 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_500_type_5.py
--rw-r--r--   0        0        0      184 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_chat_completions_create_response_500_type_5_code.py
--rw-r--r--   0        0        0     4149 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_create_data_body.py
--rw-r--r--   0        0        0     5643 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_create_files_body.py
--rw-r--r--   0        0        0     4149 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_create_json_body.py
--rw-r--r--   0        0        0     4167 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_create_response_201.py
--rw-r--r--   0        0        0     4619 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_list_response_200_item.py
--rw-r--r--   0        0        0     5600 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_partial_update_data_body.py
--rw-r--r--   0        0        0     7476 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_partial_update_files_body.py
--rw-r--r--   0        0        0     5600 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_partial_update_json_body.py
--rw-r--r--   0        0        0     4649 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_partial_update_response_200.py
--rw-r--r--   0        0        0     4616 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_retrieve_response_200.py
--rw-r--r--   0        0        0     4149 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_update_data_body.py
--rw-r--r--   0        0        0     5643 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_update_files_body.py
--rw-r--r--   0        0        0     4149 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_update_json_body.py
--rw-r--r--   0        0        0     4167 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_data_points_update_response_200.py
--rw-r--r--   0        0        0     5661 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_data_body.py
--rw-r--r--   0        0        0     1504 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_data_body_encoding_format.py
--rw-r--r--   0        0        0     7579 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_files_body.py
--rw-r--r--   0        0        0     1510 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_files_body_encoding_format.py
--rw-r--r--   0        0        0     5661 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_json_body.py
--rw-r--r--   0        0        0     1504 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_json_body_encoding_format.py
--rw-r--r--   0        0        0     4124 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_200.py
--rw-r--r--   0        0        0     2046 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_200_data_item.py
--rw-r--r--   0        0        0     2745 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_200_usage.py
--rw-r--r--   0        0        0     2757 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_400.py
--rw-r--r--   0        0        0      178 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_400_code.py
--rw-r--r--   0        0        0     2363 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_400_details.py
--rw-r--r--   0        0        0     3069 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_400_details_additional_property.py
--rw-r--r--   0        0        0     1702 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_400_details_additional_property_error_messages_item.py
--rw-r--r--   0        0        0     2116 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_401.py
--rw-r--r--   0        0        0      186 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_401_code.py
--rw-r--r--   0        0        0     2120 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_403.py
--rw-r--r--   0        0        0      190 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_403_code.py
--rw-r--r--   0        0        0     2188 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_404_type_0.py
--rw-r--r--   0        0        0      195 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_404_type_0_code.py
--rw-r--r--   0        0        0     2182 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_404_type_1.py
--rw-r--r--   0        0        0      189 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_404_type_1_code.py
--rw-r--r--   0        0        0     2104 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_409.py
--rw-r--r--   0        0        0      174 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_409_code.py
--rw-r--r--   0        0        0     2126 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_422.py
--rw-r--r--   0        0        0      196 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_422_code.py
--rw-r--r--   0        0        0     2106 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_429.py
--rw-r--r--   0        0        0      176 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_429_code.py
--rw-r--r--   0        0        0     2200 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_500_type_0.py
--rw-r--r--   0        0        0      207 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_500_type_0_code.py
--rw-r--r--   0        0        0     2198 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_500_type_1.py
--rw-r--r--   0        0        0      205 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_500_type_1_code.py
--rw-r--r--   0        0        0     2190 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_500_type_2.py
--rw-r--r--   0        0        0      197 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_500_type_2_code.py
--rw-r--r--   0        0        0     2192 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_500_type_3.py
--rw-r--r--   0        0        0      199 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_500_type_3_code.py
--rw-r--r--   0        0        0     2198 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_500_type_4.py
--rw-r--r--   0        0        0      205 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_500_type_4_code.py
--rw-r--r--   0        0        0     2172 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_500_type_5.py
--rw-r--r--   0        0        0      179 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_embeddings_create_response_500_type_5_code.py
--rw-r--r--   0        0        0     4984 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_data_body.py
--rw-r--r--   0        0        0     1973 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_data_body_training_data_item.py
--rw-r--r--   0        0        0     1979 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_data_body_validaton_data_item.py
--rw-r--r--   0        0        0     6953 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_files_body.py
--rw-r--r--   0        0        0     1979 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_files_body_training_data_item.py
--rw-r--r--   0        0        0     1985 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_files_body_validaton_data_item.py
--rw-r--r--   0        0        0     4984 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_json_body.py
--rw-r--r--   0        0        0     1973 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_json_body_training_data_item.py
--rw-r--r--   0        0        0     1979 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_json_body_validaton_data_item.py
--rw-r--r--   0        0        0     1707 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_response_200.py
--rw-r--r--   0        0        0     2757 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_response_400.py
--rw-r--r--   0        0        0      178 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_response_400_code.py
--rw-r--r--   0        0        0     2363 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_response_400_details.py
--rw-r--r--   0        0        0     3069 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_response_400_details_additional_property.py
--rw-r--r--   0        0        0     1702 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_response_400_details_additional_property_error_messages_item.py
--rw-r--r--   0        0        0     2116 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_response_401.py
--rw-r--r--   0        0        0      186 2024-02-16 13:49:48.559050 premai-0.3.8/premai/models/v1_finetuning_create_response_401_code.py
--rw-r--r--   0        0        0     2120 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_403.py
--rw-r--r--   0        0        0      190 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_403_code.py
--rw-r--r--   0        0        0     2188 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_404_type_0.py
--rw-r--r--   0        0        0      195 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_404_type_0_code.py
--rw-r--r--   0        0        0     2182 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_404_type_1.py
--rw-r--r--   0        0        0      189 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_404_type_1_code.py
--rw-r--r--   0        0        0     2104 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_409.py
--rw-r--r--   0        0        0      174 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_409_code.py
--rw-r--r--   0        0        0     2126 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_422.py
--rw-r--r--   0        0        0      196 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_422_code.py
--rw-r--r--   0        0        0     2106 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_429.py
--rw-r--r--   0        0        0      176 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_429_code.py
--rw-r--r--   0        0        0     2200 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_500_type_0.py
--rw-r--r--   0        0        0      207 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_500_type_0_code.py
--rw-r--r--   0        0        0     2198 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_500_type_1.py
--rw-r--r--   0        0        0      205 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_500_type_1_code.py
--rw-r--r--   0        0        0     2190 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_500_type_2.py
--rw-r--r--   0        0        0      197 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_500_type_2_code.py
--rw-r--r--   0        0        0     2192 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_500_type_3.py
--rw-r--r--   0        0        0      199 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_500_type_3_code.py
--rw-r--r--   0        0        0     2198 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_500_type_4.py
--rw-r--r--   0        0        0      205 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_500_type_4_code.py
--rw-r--r--   0        0        0     2172 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_500_type_5.py
--rw-r--r--   0        0        0      179 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_create_response_500_type_5_code.py
--rw-r--r--   0        0        0     4176 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_200.py
--rw-r--r--   0        0        0     2797 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_400.py
--rw-r--r--   0        0        0      180 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_400_code.py
--rw-r--r--   0        0        0     2391 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_400_details.py
--rw-r--r--   0        0        0     3097 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_400_details_additional_property.py
--rw-r--r--   0        0        0     1714 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_400_details_additional_property_error_messages_item.py
--rw-r--r--   0        0        0     2140 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_401.py
--rw-r--r--   0        0        0      188 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_401_code.py
--rw-r--r--   0        0        0     2144 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_403.py
--rw-r--r--   0        0        0      192 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_403_code.py
--rw-r--r--   0        0        0     2212 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_404_type_0.py
--rw-r--r--   0        0        0      197 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_404_type_0_code.py
--rw-r--r--   0        0        0     2206 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_404_type_1.py
--rw-r--r--   0        0        0      191 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_404_type_1_code.py
--rw-r--r--   0        0        0     2128 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_409.py
--rw-r--r--   0        0        0      176 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_409_code.py
--rw-r--r--   0        0        0     2150 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_422.py
--rw-r--r--   0        0        0      198 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_422_code.py
--rw-r--r--   0        0        0     2130 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_429.py
--rw-r--r--   0        0        0      178 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_429_code.py
--rw-r--r--   0        0        0     2224 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_500_type_0.py
--rw-r--r--   0        0        0      209 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_500_type_0_code.py
--rw-r--r--   0        0        0     2222 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_500_type_1.py
--rw-r--r--   0        0        0      207 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_500_type_1_code.py
--rw-r--r--   0        0        0     2214 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_500_type_2.py
--rw-r--r--   0        0        0      199 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_500_type_2_code.py
--rw-r--r--   0        0        0     2216 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_500_type_3.py
--rw-r--r--   0        0        0      201 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_500_type_3_code.py
--rw-r--r--   0        0        0     2222 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_500_type_4.py
--rw-r--r--   0        0        0      207 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_500_type_4_code.py
--rw-r--r--   0        0        0     2196 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_500_type_5.py
--rw-r--r--   0        0        0      181 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/v1_finetuning_retrieve_response_500_type_5_code.py
--rw-r--r--   0        0        0     2431 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/validation_detail.py
--rw-r--r--   0        0        0     1456 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/validation_detail_error_messages_item.py
--rw-r--r--   0        0        0     2459 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/validation_error.py
--rw-r--r--   0        0        0      164 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/validation_error_code.py
--rw-r--r--   0        0        0      168 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/validation_error_code_enum.py
--rw-r--r--   0        0        0     2118 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/validation_error_details.py
--rw-r--r--   0        0        0     2858 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/validation_error_details_additional_property.py
--rw-r--r--   0        0        0     1609 2024-02-16 13:49:48.563050 premai-0.3.8/premai/models/validation_error_details_additional_property_error_messages_item.py
--rw-r--r--   0        0        0       25 2024-02-16 13:49:48.563050 premai-0.3.8/premai/py.typed
--rw-r--r--   0        0        0     1016 2024-02-16 13:49:48.563050 premai-0.3.8/premai/types.py
--rw-r--r--   0        0        0      523 2024-02-16 13:49:48.563050 premai-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1875 1970-01-01 00:00:00.000000 premai-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1308 2024-02-20 13:46:53.873863 premai-0.3.9/README.md
+-rw-r--r--   0        0        0      768 2024-02-20 13:46:53.873863 premai-0.3.9/premai/__init__.py
+-rw-r--r--   0        0        0     3343 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/chat_completions/__init__.py
+-rw-r--r--   0        0        0    12136 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/chat_completions/v1_chat_completions_create.py
+-rw-r--r--   0        0        0        0 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/datapoints/__init__.py
+-rw-r--r--   0        0        0     2216 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/datapoints/v1_data_points_create.py
+-rw-r--r--   0        0        0     1747 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/datapoints/v1_data_points_destroy.py
+-rw-r--r--   0        0        0     1981 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/datapoints/v1_data_points_list.py
+-rw-r--r--   0        0        0     2345 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/datapoints/v1_data_points_partial_update.py
+-rw-r--r--   0        0        0     1875 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/datapoints/v1_data_points_retrieve.py
+-rw-r--r--   0        0        0     2287 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/datapoints/v1_data_points_update.py
+-rw-r--r--   0        0        0        0 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/embeddings/__init__.py
+-rw-r--r--   0        0        0     5203 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/embeddings/v1_embeddings_create.py
+-rw-r--r--   0        0        0        0 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/finetuning/__init__.py
+-rw-r--r--   0        0        0     5191 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/finetuning/v1_finetuning_create.py
+-rw-r--r--   0        0        0     4979 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/finetuning/v1_finetuning_retrieve.py
+-rw-r--r--   0        0        0        0 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/models/__init__.py
+-rw-r--r--   0        0        0     1939 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/models/v1_models_list.py
+-rw-r--r--   0        0        0     1833 2024-02-20 13:46:53.873863 premai-0.3.9/premai/api/models/v1_models_retrieve.py
+-rw-r--r--   0        0        0    11121 2024-02-20 13:46:53.873863 premai-0.3.9/premai/client.py
+-rw-r--r--   0        0        0      489 2024-02-20 13:46:53.873863 premai-0.3.9/premai/errors.py
+-rw-r--r--   0        0        0     5509 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/__init__.py
+-rw-r--r--   0        0        0     2115 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/api_response_validation_error.py
+-rw-r--r--   0        0        0      201 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/api_response_validation_error_code_enum.py
+-rw-r--r--   0        0        0     2009 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/authentication_error.py
+-rw-r--r--   0        0        0      180 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/authentication_error_code_enum.py
+-rw-r--r--   0        0        0      131 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/blank_enum.py
+-rw-r--r--   0        0        0     1929 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/catch_all_error.py
+-rw-r--r--   0        0        0      162 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/catch_all_error_code_enum.py
+-rw-r--r--   0        0        0    19461 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/chat_completion_input.py
+-rw-r--r--   0        0        0     1535 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/chat_completion_input_logit_bias_type_0.py
+-rw-r--r--   0        0        0     1550 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/chat_completion_input_response_format_type_0.py
+-rw-r--r--   0        0        0     1426 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/chat_completion_input_tools_item.py
+-rw-r--r--   0        0        0     4219 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/chat_completion_response.py
+-rw-r--r--   0        0        0     1925 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/conflict_error.py
+-rw-r--r--   0        0        0      162 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/conflict_error_code_enum.py
+-rw-r--r--   0        0        0     4472 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/data_point.py
+-rw-r--r--   0        0        0     1860 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/embedding.py
+-rw-r--r--   0        0        0     7274 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/embeddings_input.py
+-rw-r--r--   0        0        0     3501 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/embeddings_response.py
+-rw-r--r--   0        0        0      165 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/encoding_format_enum.py
+-rw-r--r--   0        0        0     6243 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/fine_tuning_input.py
+-rw-r--r--   0        0        0     1635 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/fine_tuning_response.py
+-rw-r--r--   0        0        0     1802 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/fine_tuning_sample.py
+-rw-r--r--   0        0        0     5556 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/input_data_point.py
+-rw-r--r--   0        0        0     1854 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/message.py
+-rw-r--r--   0        0        0     2003 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/model_not_found_error.py
+-rw-r--r--   0        0        0      177 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/model_not_found_error_code_enum.py
+-rw-r--r--   0        0        0      430 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/model_provider_enum.py
+-rw-r--r--   0        0        0      208 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/model_type_enum.py
+-rw-r--r--   0        0        0     4347 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/models.py
+-rw-r--r--   0        0        0     7356 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/patched_data_point.py
+-rw-r--r--   0        0        0     2041 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/permission_denied_error.py
+-rw-r--r--   0        0        0      186 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/permission_denied_error_code_enum.py
+-rw-r--r--   0        0        0     2115 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/provider_api_connection_error.py
+-rw-r--r--   0        0        0      201 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/provider_api_connection_error_code_enum.py
+-rw-r--r--   0        0        0     2059 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/provider_api_status_error.py
+-rw-r--r--   0        0        0      189 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/provider_api_status_error_code_enum.py
+-rw-r--r--   0        0        0     2073 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/provider_api_timeout_error.py
+-rw-r--r--   0        0        0      192 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/provider_api_timeout_error_code_enum.py
+-rw-r--r--   0        0        0     2129 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/provider_internal_server_error.py
+-rw-r--r--   0        0        0      204 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/provider_internal_server_error_code_enum.py
+-rw-r--r--   0        0        0     2045 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/provider_not_found_error.py
+-rw-r--r--   0        0        0      186 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/provider_not_found_error_code_enum.py
+-rw-r--r--   0        0        0     1943 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/rate_limit_error.py
+-rw-r--r--   0        0        0      165 2024-02-20 13:46:53.873863 premai-0.3.9/premai/models/rate_limit_error_code_enum.py
+-rw-r--r--   0        0        0     1964 2024-02-20 13:46:53.877863 premai-0.3.9/premai/models/response_choice.py
+-rw-r--r--   0        0        0     4143 2024-02-20 13:46:53.877863 premai-0.3.9/premai/models/retrieve_fine_tuning_response.py
+-rw-r--r--   0        0        0      159 2024-02-20 13:46:53.877863 premai-0.3.9/premai/models/role_enum.py
+-rw-r--r--   0        0        0     2083 2024-02-20 13:46:53.877863 premai-0.3.9/premai/models/unprocessable_entity_error.py
+-rw-r--r--   0        0        0      195 2024-02-20 13:46:53.877863 premai-0.3.9/premai/models/unprocessable_entity_error_code_enum.py
+-rw-r--r--   0        0        0     2515 2024-02-20 13:46:53.877863 premai-0.3.9/premai/models/usage.py
+-rw-r--r--   0        0        0     2431 2024-02-20 13:46:53.877863 premai-0.3.9/premai/models/validation_detail.py
+-rw-r--r--   0        0        0     1456 2024-02-20 13:46:53.877863 premai-0.3.9/premai/models/validation_detail_error_messages_item.py
+-rw-r--r--   0        0        0     2484 2024-02-20 13:46:53.877863 premai-0.3.9/premai/models/validation_error.py
+-rw-r--r--   0        0        0      168 2024-02-20 13:46:53.877863 premai-0.3.9/premai/models/validation_error_code_enum.py
+-rw-r--r--   0        0        0     1906 2024-02-20 13:46:53.877863 premai-0.3.9/premai/models/validation_error_details.py
+-rw-r--r--   0        0        0       25 2024-02-20 13:46:53.877863 premai-0.3.9/premai/py.typed
+-rw-r--r--   0        0        0     1016 2024-02-20 13:46:53.877863 premai-0.3.9/premai/types.py
+-rw-r--r--   0        0        0      523 2024-02-20 13:46:53.877863 premai-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1942 1970-01-01 00:00:00.000000 premai-0.3.9/PKG-INFO
```

### Comparing `premai-0.3.8/README.md` & `premai-0.3.9/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -15,43 +15,44 @@
 
 ```python
 from premai import Prem
 
 client = Prem(
     api_key=YOUR_API_KEY
 )
-
-project_id = YOUR_PROJECT_ID
 ```
 
 ### Chat completion
 The `chat.completions` module allows you to generate completions based on user input. Here's an example:
 
 ```python
 messages = [
-    {"role": "system", "content": "You are a helpful assistant."},
     {"role": "user", "content": "Who won the world series in 2020?"},
 ]
-model = "gpt-3.5-turbo"
+model = "gpt-3.5-turbo" # optional
+system_prompt = "You are a helpful assistant." # optional
+project_id = YOUR_PROJECT_ID
 
 # Create completion
 response = client.chat.completions.create(
     project_id=project_id,
     messages=messages,
     model=model,
+    system_prompt=system_prompt,
     stream=False
 )
 
 print(response.choices)
 
 # Create completion with stream
 response = client.chat.completions.create(
     project_id=project_id,
     messages=messages,
     model=model,
+    system_prompt=system_prompt,
     stream=True
 )
 
 for chunk in response:
     if chunk.choices[0].delta["content"]:
         print(chunk.choices[0].delta["content"], end="")
```

### Comparing `premai-0.3.8/premai/__init__.py` & `premai-0.3.9/premai/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from .client import AuthenticatedClient
 
 from .api import (
     DatapointsModule,
     EmbeddingsModule,
     FinetuningModule,
+    ModelsModule,
     ChatModuleWrapper,
 )
 
 class Prem:
     datapoints: DatapointsModule
     embeddings: EmbeddingsModule
     finetuning: FinetuningModule
+    models: ModelsModule
     chat: ChatModuleWrapper
 
     def __init__(self, api_key: str, base_url='https://app.premai.io'):
         client = AuthenticatedClient(token=api_key, base_url=base_url)
         # Init modules
         self.datapoints = DatapointsModule(client)
         self.embeddings = EmbeddingsModule(client)
         self.finetuning = FinetuningModule(client)
+        self.models = ModelsModule(client)
         self.chat = ChatModuleWrapper(client)
 
 __all__ = [
     "Prem"
 ]
```

### Comparing `premai-0.3.8/premai/api/__init__.py` & `premai-0.3.9/premai/api/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,97 +1,116 @@
 """ Contains methods for accessing the API """
 
 
 from typing_extensions import Unpack
 
 from ..models import (
-    V1ChatCompletionsCreateJsonBodyDict,
-    V1DataPointsCreateJsonBodyDict,
-    V1DataPointsPartialUpdateJsonBodyDict,
-    V1DataPointsUpdateJsonBodyDict,
-    V1EmbeddingsCreateJsonBodyDict,
-    V1FinetuningCreateJsonBodyDict,
+    ChatCompletionInputDict,
+    EmbeddingsInputDict,
+    FineTuningInputDict,
+    InputDataPointDict,
+    PatchedDataPointDict,
 )
 from .chat_completions.v1_chat_completions_create import v1_chat_completions_create_wrapper
 from .datapoints.v1_data_points_create import v1_data_points_create_wrapper
 from .datapoints.v1_data_points_destroy import v1_data_points_destroy_wrapper
 from .datapoints.v1_data_points_list import v1_data_points_list_wrapper
 from .datapoints.v1_data_points_partial_update import v1_data_points_partial_update_wrapper
 from .datapoints.v1_data_points_retrieve import v1_data_points_retrieve_wrapper
 from .datapoints.v1_data_points_update import v1_data_points_update_wrapper
 from .embeddings.v1_embeddings_create import v1_embeddings_create_wrapper
 from .finetuning.v1_finetuning_create import v1_finetuning_create_wrapper
 from .finetuning.v1_finetuning_retrieve import v1_finetuning_retrieve_wrapper
+from .models.v1_models_list import v1_models_list_wrapper
+from .models.v1_models_retrieve import v1_models_retrieve_wrapper
 
 
 class ChatCompletionsModule:
     def __init__(self, client):
         self._client = client
 
-    def create(self, **kwargs: Unpack[V1ChatCompletionsCreateJsonBodyDict]):
+    def create(self, **kwargs: Unpack[ChatCompletionInputDict]):
         return v1_chat_completions_create_wrapper(self._client)(**kwargs)
 
 
 class DatapointsModule:
     def __init__(self, client):
         self._client = client
 
     def list(
         self,
     ):
         return v1_data_points_list_wrapper(self._client)()
 
-    def create(self, **kwargs: Unpack[V1DataPointsCreateJsonBodyDict]):
+    def create(self, **kwargs: Unpack[InputDataPointDict]):
         return v1_data_points_create_wrapper(self._client)(**kwargs)
 
     def retrieve(
         self,
         id: int,
     ):
         return v1_data_points_retrieve_wrapper(self._client)(
             id,
         )
 
-    def update(self, id: int, **kwargs: Unpack[V1DataPointsUpdateJsonBodyDict]):
+    def update(self, id: int, **kwargs: Unpack[InputDataPointDict]):
         return v1_data_points_update_wrapper(self._client)(id, **kwargs)
 
     def delete(
         self,
         id: int,
     ):
         return v1_data_points_destroy_wrapper(self._client)(
             id,
         )
 
-    def patch(self, id: int, **kwargs: Unpack[V1DataPointsPartialUpdateJsonBodyDict]):
+    def patch(self, id: int, **kwargs: Unpack[PatchedDataPointDict]):
         return v1_data_points_partial_update_wrapper(self._client)(id, **kwargs)
 
 
 class EmbeddingsModule:
     def __init__(self, client):
         self._client = client
 
-    def create(self, **kwargs: Unpack[V1EmbeddingsCreateJsonBodyDict]):
+    def create(self, **kwargs: Unpack[EmbeddingsInputDict]):
         return v1_embeddings_create_wrapper(self._client)(**kwargs)
 
 
 class FinetuningModule:
     def __init__(self, client):
         self._client = client
 
-    def create(self, **kwargs: Unpack[V1FinetuningCreateJsonBodyDict]):
+    def create(self, **kwargs: Unpack[FineTuningInputDict]):
         return v1_finetuning_create_wrapper(self._client)(**kwargs)
 
     def retrieve(
         self,
         job_id: str,
     ):
         return v1_finetuning_retrieve_wrapper(self._client)(
             job_id,
         )
 
 
+class ModelsModule:
+    def __init__(self, client):
+        self._client = client
+
+    def list(
+        self,
+    ):
+        return v1_models_list_wrapper(self._client)()
+
+    def retrieve(
+        self,
+        id: int,
+    ):
+        return v1_models_retrieve_wrapper(self._client)(
+            id,
+        )
+
+
 class ChatModuleWrapper:
     completions: ChatCompletionsModule
 
     def __init__(self, client):
         self.completions = ChatCompletionsModule(client)
```

### Comparing `premai-0.3.8/premai/api/chat_completions/v1_chat_completions_create.py` & `premai-0.3.9/premai/api/chat_completions/v1_chat_completions_create.py`

 * *Files identical despite different names*

### Comparing `premai-0.3.8/premai/api/datapoints/v1_data_points_create.py` & `premai-0.3.9/premai/api/datapoints/v1_data_points_list.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,84 +1,69 @@
 from http import HTTPStatus
-from typing import Dict, Optional
+from typing import Dict, List, Optional
 
 import httpx
-from typing_extensions import Any, Unpack
+from typing_extensions import Any
 
 from ... import errors
-from ...models.v1_data_points_create_json_body import V1DataPointsCreateJsonBody
-from ...models.v1_data_points_create_response_201 import V1DataPointsCreateResponse201
+from ...models.data_point import DataPoint
 
 # from ...client import AuthenticatedClient, Client
 from ...types import Response
 
 
-def _get_kwargs(
-    **body: Unpack[V1DataPointsCreateJsonBody],
-) -> Dict[str, Any]:
-    headers: Dict[str, Any] = {}
-
+def _get_kwargs() -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
-        "method": "post",
+        "method": "get",
         "url": "/v1/data-points/",
     }
 
-    _json_body = body
-
-    _kwargs["json"] = _json_body
-    headers["Content-Type"] = "application/json"
-
-    _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client, response: httpx.Response) -> Optional[V1DataPointsCreateResponse201]:
-    if response.status_code == HTTPStatus.CREATED:
-        response_201 = V1DataPointsCreateResponse201.from_dict(response.json())
+def _parse_response(*, client, response: httpx.Response) -> Optional[List["DataPoint"]]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in _response_200:
+            response_200_item = DataPoint.from_dict(response_200_item_data)
 
-        return response_201
+            response_200.append(response_200_item)
+
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client, response: httpx.Response) -> Response[V1DataPointsCreateResponse201]:
+def _build_response(*, client, response: httpx.Response) -> Response[List["DataPoint"]]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
-def v1_data_points_create_wrapper(client):
-    def v1_data_points_create_wrapped(
-        **body: Unpack[V1DataPointsCreateJsonBody],
-    ) -> V1DataPointsCreateResponse201:
+def v1_data_points_list_wrapper(client):
+    def v1_data_points_list_wrapped() -> List["DataPoint"]:
         """
-        Args:
-            body (V1DataPointsCreateJsonBody):
-            body (V1DataPointsCreateDataBody):
-            body (V1DataPointsCreateFilesBody):
-
         Raises:
             errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[V1DataPointsCreateResponse201]
+            Response[List['DataPoint']]
         """
 
-        kwargs = _get_kwargs(
-            **body,
-        )
+        kwargs = _get_kwargs()
 
         httpx_client = client.get_httpx_client()
 
         response = httpx_client.request(
             **kwargs,
         )
 
         return _build_response(client=client, response=response).parsed
 
-    return v1_data_points_create_wrapped
+    return v1_data_points_list_wrapped
```

### Comparing `premai-0.3.8/premai/api/datapoints/v1_data_points_destroy.py` & `premai-0.3.9/premai/api/datapoints/v1_data_points_destroy.py`

 * *Files identical despite different names*

### Comparing `premai-0.3.8/premai/api/datapoints/v1_data_points_list.py` & `premai-0.3.9/premai/api/datapoints/v1_data_points_retrieve.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,69 +1,73 @@
 from http import HTTPStatus
-from typing import Dict, List, Optional
+from typing import Dict, Optional
 
 import httpx
 from typing_extensions import Any
 
 from ... import errors
-from ...models.v1_data_points_list_response_200_item import V1DataPointsListResponse200Item
+from ...models.data_point import DataPoint
 
 # from ...client import AuthenticatedClient, Client
 from ...types import Response
 
 
-def _get_kwargs() -> Dict[str, Any]:
+def _get_kwargs(
+    id: int,
+) -> Dict[str, Any]:
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/v1/data-points/",
+        "url": f"/v1/data-points/{id}/",
     }
 
     return _kwargs
 
 
-def _parse_response(*, client, response: httpx.Response) -> Optional[List["V1DataPointsListResponse200Item"]]:
+def _parse_response(*, client, response: httpx.Response) -> Optional[DataPoint]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in _response_200:
-            response_200_item = V1DataPointsListResponse200Item.from_dict(response_200_item_data)
-
-            response_200.append(response_200_item)
+        response_200 = DataPoint.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client, response: httpx.Response) -> Response[List["V1DataPointsListResponse200Item"]]:
+def _build_response(*, client, response: httpx.Response) -> Response[DataPoint]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
-def v1_data_points_list_wrapper(client):
-    def v1_data_points_list_wrapped() -> List["V1DataPointsListResponse200Item"]:
+def v1_data_points_retrieve_wrapper(client):
+    def v1_data_points_retrieve_wrapped(
+        id: int,
+    ) -> DataPoint:
         """
+        Args:
+            id (int):
+
         Raises:
             errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[List['V1DataPointsListResponse200Item']]
+            Response[DataPoint]
         """
 
-        kwargs = _get_kwargs()
+        kwargs = _get_kwargs(
+            id=id,
+        )
 
         httpx_client = client.get_httpx_client()
 
         response = httpx_client.request(
             **kwargs,
         )
 
         return _build_response(client=client, response=response).parsed
 
-    return v1_data_points_list_wrapped
+    return v1_data_points_retrieve_wrapped
```

### Comparing `premai-0.3.8/premai/api/datapoints/v1_data_points_partial_update.py` & `premai-0.3.9/premai/api/datapoints/v1_data_points_partial_update.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from http import HTTPStatus
 from typing import Dict, Optional
 
 import httpx
 from typing_extensions import Any, Unpack
 
 from ... import errors
-from ...models.v1_data_points_partial_update_json_body import V1DataPointsPartialUpdateJsonBody
-from ...models.v1_data_points_partial_update_response_200 import V1DataPointsPartialUpdateResponse200
+from ...models.data_point import DataPoint
+from ...models.patched_data_point import PatchedDataPoint
 
 # from ...client import AuthenticatedClient, Client
 from ...types import Response
 
 
 def _get_kwargs(
     id: int,
-    **body: Unpack[V1DataPointsPartialUpdateJsonBody],
+    **body: Unpack[PatchedDataPoint],
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "patch",
         "url": f"/v1/data-points/{id}/",
     }
@@ -28,52 +28,52 @@
     _kwargs["json"] = _json_body
     headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client, response: httpx.Response) -> Optional[V1DataPointsPartialUpdateResponse200]:
+def _parse_response(*, client, response: httpx.Response) -> Optional[DataPoint]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = V1DataPointsPartialUpdateResponse200.from_dict(response.json())
+        response_200 = DataPoint.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client, response: httpx.Response) -> Response[V1DataPointsPartialUpdateResponse200]:
+def _build_response(*, client, response: httpx.Response) -> Response[DataPoint]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def v1_data_points_partial_update_wrapper(client):
     def v1_data_points_partial_update_wrapped(
         id: int,
-        **body: Unpack[V1DataPointsPartialUpdateJsonBody],
-    ) -> V1DataPointsPartialUpdateResponse200:
+        **body: Unpack[PatchedDataPoint],
+    ) -> DataPoint:
         """
         Args:
             id (int):
-            body (V1DataPointsPartialUpdateJsonBody):
-            body (V1DataPointsPartialUpdateDataBody):
-            body (V1DataPointsPartialUpdateFilesBody):
+            body (PatchedDataPoint):
+            body (PatchedDataPoint):
+            body (PatchedDataPoint):
 
         Raises:
             errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[V1DataPointsPartialUpdateResponse200]
+            Response[DataPoint]
         """
 
         kwargs = _get_kwargs(
             id=id,
             **body,
         )
```

### Comparing `premai-0.3.8/premai/api/datapoints/v1_data_points_retrieve.py` & `premai-0.3.9/premai/api/datapoints/v1_data_points_create.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,73 +1,83 @@
 from http import HTTPStatus
 from typing import Dict, Optional
 
 import httpx
-from typing_extensions import Any
+from typing_extensions import Any, Unpack
 
 from ... import errors
-from ...models.v1_data_points_retrieve_response_200 import V1DataPointsRetrieveResponse200
+from ...models.input_data_point import InputDataPoint
 
 # from ...client import AuthenticatedClient, Client
 from ...types import Response
 
 
 def _get_kwargs(
-    id: int,
+    **body: Unpack[InputDataPoint],
 ) -> Dict[str, Any]:
+    headers: Dict[str, Any] = {}
+
     _kwargs: Dict[str, Any] = {
-        "method": "get",
-        "url": f"/v1/data-points/{id}/",
+        "method": "post",
+        "url": "/v1/data-points/",
     }
 
+    _json_body = body
+
+    _kwargs["json"] = _json_body
+    headers["Content-Type"] = "application/json"
+
+    _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client, response: httpx.Response) -> Optional[V1DataPointsRetrieveResponse200]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = V1DataPointsRetrieveResponse200.from_dict(response.json())
+def _parse_response(*, client, response: httpx.Response) -> Optional[InputDataPoint]:
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = InputDataPoint.from_dict(response.json())
 
-        return response_200
+        return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client, response: httpx.Response) -> Response[V1DataPointsRetrieveResponse200]:
+def _build_response(*, client, response: httpx.Response) -> Response[InputDataPoint]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
-def v1_data_points_retrieve_wrapper(client):
-    def v1_data_points_retrieve_wrapped(
-        id: int,
-    ) -> V1DataPointsRetrieveResponse200:
+def v1_data_points_create_wrapper(client):
+    def v1_data_points_create_wrapped(
+        **body: Unpack[InputDataPoint],
+    ) -> InputDataPoint:
         """
         Args:
-            id (int):
+            body (InputDataPoint):
+            body (InputDataPoint):
+            body (InputDataPoint):
 
         Raises:
             errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[V1DataPointsRetrieveResponse200]
+            Response[InputDataPoint]
         """
 
         kwargs = _get_kwargs(
-            id=id,
+            **body,
         )
 
         httpx_client = client.get_httpx_client()
 
         response = httpx_client.request(
             **kwargs,
         )
 
         return _build_response(client=client, response=response).parsed
 
-    return v1_data_points_retrieve_wrapped
+    return v1_data_points_create_wrapped
```

### Comparing `premai-0.3.8/premai/api/datapoints/v1_data_points_update.py` & `premai-0.3.9/premai/api/datapoints/v1_data_points_update.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 from http import HTTPStatus
 from typing import Dict, Optional
 
 import httpx
 from typing_extensions import Any, Unpack
 
 from ... import errors
-from ...models.v1_data_points_update_json_body import V1DataPointsUpdateJsonBody
-from ...models.v1_data_points_update_response_200 import V1DataPointsUpdateResponse200
+from ...models.input_data_point import InputDataPoint
 
 # from ...client import AuthenticatedClient, Client
 from ...types import Response
 
 
 def _get_kwargs(
     id: int,
-    **body: Unpack[V1DataPointsUpdateJsonBody],
+    **body: Unpack[InputDataPoint],
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
     _kwargs: Dict[str, Any] = {
         "method": "put",
         "url": f"/v1/data-points/{id}/",
     }
@@ -28,52 +27,52 @@
     _kwargs["json"] = _json_body
     headers["Content-Type"] = "application/json"
 
     _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client, response: httpx.Response) -> Optional[V1DataPointsUpdateResponse200]:
+def _parse_response(*, client, response: httpx.Response) -> Optional[InputDataPoint]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = V1DataPointsUpdateResponse200.from_dict(response.json())
+        response_200 = InputDataPoint.from_dict(response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client, response: httpx.Response) -> Response[V1DataPointsUpdateResponse200]:
+def _build_response(*, client, response: httpx.Response) -> Response[InputDataPoint]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def v1_data_points_update_wrapper(client):
     def v1_data_points_update_wrapped(
         id: int,
-        **body: Unpack[V1DataPointsUpdateJsonBody],
-    ) -> V1DataPointsUpdateResponse200:
+        **body: Unpack[InputDataPoint],
+    ) -> InputDataPoint:
         """
         Args:
             id (int):
-            body (V1DataPointsUpdateJsonBody):
-            body (V1DataPointsUpdateDataBody):
-            body (V1DataPointsUpdateFilesBody):
+            body (InputDataPoint):
+            body (InputDataPoint):
+            body (InputDataPoint):
 
         Raises:
             errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
             httpx.TimeoutException: If the request takes longer than Client.timeout.
 
         Returns:
-            Response[V1DataPointsUpdateResponse200]
+            Response[InputDataPoint]
         """
 
         kwargs = _get_kwargs(
             id=id,
             **body,
         )
```

### Comparing `premai-0.3.8/premai/client.py` & `premai-0.3.9/premai/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing_extensions import Any
 
 from .api import (
     ChatCompletionsModule,
     DatapointsModule,
     EmbeddingsModule,
     FinetuningModule,
+    ModelsModule,
 )
 
 
 @define
 class Client:
     """A class for keeping track of data related to the API
 
@@ -243,15 +244,17 @@
 
 
 class Prem:
     chat_completions: ChatCompletionsModule
     datapoints: DatapointsModule
     embeddings: EmbeddingsModule
     finetuning: FinetuningModule
+    models: ModelsModule
 
     def __init__(self, api_key: str = "", base_url="https://app.premai.io"):
         client = AuthenticatedClient(token=api_key, base_url=base_url)
         # Init modules
         self.chat_completions = ChatCompletionsModule(client)
         self.datapoints = DatapointsModule(client)
         self.embeddings = EmbeddingsModule(client)
         self.finetuning = FinetuningModule(client)
+        self.models = ModelsModule(client)
```

### Comparing `premai-0.3.8/premai/models/api_response_validation_error.py` & `premai-0.3.9/premai/models/api_response_validation_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.api_response_validation_error_code import APIResponseValidationErrorCode
+from ..models.api_response_validation_error_code_enum import APIResponseValidationErrorCodeEnum
 
 T = TypeVar("T", bound="APIResponseValidationError")
 
 
 class APIResponseValidationErrorDict(TypedDict):
     message: str
-    code: APIResponseValidationErrorCode
+    code: APIResponseValidationErrorCodeEnum
     pass
 
 
 @_attrs_define
 class APIResponseValidationError:
     """
     Attributes:
         message (str):
-        code (APIResponseValidationErrorCode): * `APIResponseValidationError` - APIResponseValidationError
+        code (APIResponseValidationErrorCodeEnum): * `APIResponseValidationError` - APIResponseValidationError
     """
 
     message: str
-    code: APIResponseValidationErrorCode
+    code: APIResponseValidationErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         message = self.message
 
         code = self.code.value
@@ -45,15 +45,15 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         message = d.pop("message")
 
-        code = APIResponseValidationErrorCode(d.pop("code"))
+        code = APIResponseValidationErrorCodeEnum(d.pop("code"))
 
         api_response_validation_error = cls(
             message=message,
             code=code,
         )
 
         api_response_validation_error.additional_properties = d
```

### Comparing `premai-0.3.8/premai/models/authentication_error.py` & `premai-0.3.9/premai/models/authentication_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.authentication_error_code import AuthenticationErrorCode
+from ..models.authentication_error_code_enum import AuthenticationErrorCodeEnum
 
 T = TypeVar("T", bound="AuthenticationError")
 
 
 class AuthenticationErrorDict(TypedDict):
     message: str
-    code: AuthenticationErrorCode
+    code: AuthenticationErrorCodeEnum
     pass
 
 
 @_attrs_define
 class AuthenticationError:
     """
     Attributes:
         message (str):
-        code (AuthenticationErrorCode): * `AuthenticationError` - AuthenticationError
+        code (AuthenticationErrorCodeEnum): * `AuthenticationError` - AuthenticationError
     """
 
     message: str
-    code: AuthenticationErrorCode
+    code: AuthenticationErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         message = self.message
 
         code = self.code.value
@@ -45,15 +45,15 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         message = d.pop("message")
 
-        code = AuthenticationErrorCode(d.pop("code"))
+        code = AuthenticationErrorCodeEnum(d.pop("code"))
 
         authentication_error = cls(
             message=message,
             code=code,
         )
 
         authentication_error.additional_properties = d
```

### Comparing `premai-0.3.8/premai/models/catch_all_error.py` & `premai-0.3.9/premai/models/catch_all_error.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.catch_all_error_code import CatchAllErrorCode
+from ..models.catch_all_error_code_enum import CatchAllErrorCodeEnum
 
 T = TypeVar("T", bound="CatchAllError")
 
 
 class CatchAllErrorDict(TypedDict):
     message: str
-    code: CatchAllErrorCode
+    code: CatchAllErrorCodeEnum
     pass
 
 
 @_attrs_define
 class CatchAllError:
     """
     Attributes:
         message (str):
-        code (CatchAllErrorCode): * `CatchAllError` - CatchAllError
+        code (CatchAllErrorCodeEnum): * `CatchAllError` - CatchAllError
     """
 
     message: str
-    code: CatchAllErrorCode
+    code: CatchAllErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         message = self.message
 
         code = self.code.value
@@ -45,15 +45,15 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         message = d.pop("message")
 
-        code = CatchAllErrorCode(d.pop("code"))
+        code = CatchAllErrorCodeEnum(d.pop("code"))
 
         catch_all_error = cls(
             message=message,
             code=code,
         )
 
         catch_all_error.additional_properties = d
```

### Comparing `premai-0.3.8/premai/models/chat_completion_input.py` & `premai-0.3.9/premai/models/chat_completion_input.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-from typing import Dict, List, Type, Union, cast
+import json
+from typing import Dict, List, Tuple, Type, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, NotRequired, TypedDict, TypeVar
 
 from ..models.chat_completion_input_logit_bias_type_0 import ChatCompletionInputLogitBiasType0
-from ..models.chat_completion_input_messages_item import ChatCompletionInputMessagesItem
 from ..models.chat_completion_input_response_format_type_0 import ChatCompletionInputResponseFormatType0
 from ..models.chat_completion_input_tools_item import ChatCompletionInputToolsItem
+from ..models.message import Message
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="ChatCompletionInput")
 
 
 class ChatCompletionInputDict(TypedDict):
     project_id: int
-    messages: List["ChatCompletionInputMessagesItem"]
+    messages: List["Message"]
     model: NotRequired[Union[Unset, str]]
+    system_prompt: NotRequired[Union[Unset, str]]
     frequency_penalty: NotRequired[Union[Unset, float]]
     logit_bias: NotRequired[Union["ChatCompletionInputLogitBiasType0", None, Unset]]
     max_tokens: NotRequired[Union[None, Unset, int]]
     n: NotRequired[Union[Unset, int]]
     presence_penalty: NotRequired[Union[Unset, float]]
     response_format: NotRequired[Union["ChatCompletionInputResponseFormatType0", None, Unset]]
     seed: NotRequired[Union[None, Unset, int]]
@@ -34,16 +36,17 @@
 
 
 @_attrs_define
 class ChatCompletionInput:
     """
     Attributes:
         project_id (int): The ID of the project to use.
-        messages (List['ChatCompletionInputMessagesItem']): A list of messages comprising the conversation so far.
+        messages (List['Message']): A list of messages comprising the conversation so far.
         model (Union[Unset, str]): ID of the model to use. See the model endpoint compatibility table for details.
+        system_prompt (Union[Unset, str]): The system prompt to use.
         frequency_penalty (Union[Unset, float]): Number between -2.0 and 2.0. Positive values penalize new tokens based
             on their existing frequency.
         logit_bias (Union['ChatCompletionInputLogitBiasType0', None, Unset]): JSON object that maps tokens to an
             associated bias value from -100 to 100.
         max_tokens (Union[None, Unset, int]): The maximum number of tokens to generate in the chat completion.
         n (Union[Unset, int]): How many chat completion choices to generate for each input message.
         presence_penalty (Union[Unset, float]): Number between -2.0 and 2.0. Positive values penalize new tokens based
@@ -58,16 +61,17 @@
         top_p (Union[None, Unset, float]): An alternative to sampling with temperature, called nucleus sampling.
         tools (Union[Unset, List['ChatCompletionInputToolsItem']]): A list of tools the model may call. Currently, only
             functions are supported as a tool.
         user (Union[None, Unset, str]): A unique identifier representing your end-user.
     """
 
     project_id: int
-    messages: List["ChatCompletionInputMessagesItem"]
+    messages: List["Message"]
     model: Union[Unset, str] = UNSET
+    system_prompt: Union[Unset, str] = UNSET
     frequency_penalty: Union[Unset, float] = UNSET
     logit_bias: Union["ChatCompletionInputLogitBiasType0", None, Unset] = UNSET
     max_tokens: Union[None, Unset, int] = UNSET
     n: Union[Unset, int] = UNSET
     presence_penalty: Union[Unset, float] = UNSET
     response_format: Union["ChatCompletionInputResponseFormatType0", None, Unset] = UNSET
     seed: Union[None, Unset, int] = UNSET
@@ -89,14 +93,16 @@
         messages = []
         for messages_item_data in self.messages:
             messages_item = messages_item_data.to_dict()
             messages.append(messages_item)
 
         model = self.model
 
+        system_prompt = self.system_prompt
+
         frequency_penalty = self.frequency_penalty
 
         logit_bias: Union[Dict[str, Any], None, Unset]
         if isinstance(self.logit_bias, Unset):
             logit_bias = UNSET
         elif isinstance(self.logit_bias, ChatCompletionInputLogitBiasType0):
             logit_bias = self.logit_bias.to_dict()
@@ -166,14 +172,156 @@
             {
                 "project_id": project_id,
                 "messages": messages,
             }
         )
         if model is not UNSET:
             field_dict["model"] = model
+        if system_prompt is not UNSET:
+            field_dict["system_prompt"] = system_prompt
+        if frequency_penalty is not UNSET:
+            field_dict["frequency_penalty"] = frequency_penalty
+        if logit_bias is not UNSET:
+            field_dict["logit_bias"] = logit_bias
+        if max_tokens is not UNSET:
+            field_dict["max_tokens"] = max_tokens
+        if n is not UNSET:
+            field_dict["n"] = n
+        if presence_penalty is not UNSET:
+            field_dict["presence_penalty"] = presence_penalty
+        if response_format is not UNSET:
+            field_dict["response_format"] = response_format
+        if seed is not UNSET:
+            field_dict["seed"] = seed
+        if stop is not UNSET:
+            field_dict["stop"] = stop
+        if stream is not UNSET:
+            field_dict["stream"] = stream
+        if temperature is not UNSET:
+            field_dict["temperature"] = temperature
+        if top_p is not UNSET:
+            field_dict["top_p"] = top_p
+        if tools is not UNSET:
+            field_dict["tools"] = tools
+        if user is not UNSET:
+            field_dict["user"] = user
+
+        return field_dict
+
+    def to_multipart(self) -> Dict[str, Any]:
+        project_id = (
+            self.project_id
+            if isinstance(self.project_id, Unset)
+            else (None, str(self.project_id).encode(), "text/plain")
+        )
+
+        _temp_messages = []
+        for messages_item_data in self.messages:
+            messages_item = messages_item_data.to_dict()
+            _temp_messages.append(messages_item)
+        messages = (None, json.dumps(_temp_messages).encode(), "application/json")
+
+        model = self.model if isinstance(self.model, Unset) else (None, str(self.model).encode(), "text/plain")
+
+        system_prompt = (
+            self.system_prompt
+            if isinstance(self.system_prompt, Unset)
+            else (None, str(self.system_prompt).encode(), "text/plain")
+        )
+
+        frequency_penalty = (
+            self.frequency_penalty
+            if isinstance(self.frequency_penalty, Unset)
+            else (None, str(self.frequency_penalty).encode(), "text/plain")
+        )
+
+        logit_bias: Union[None, Tuple[None, bytes, str], Unset]
+        if isinstance(self.logit_bias, Unset):
+            logit_bias = UNSET
+        elif isinstance(self.logit_bias, ChatCompletionInputLogitBiasType0):
+            logit_bias = (None, json.dumps(self.logit_bias.to_dict()).encode(), "application/json")
+        else:
+            logit_bias = self.logit_bias
+
+        max_tokens: Union[None, Unset, int]
+        if isinstance(self.max_tokens, Unset):
+            max_tokens = UNSET
+        else:
+            max_tokens = self.max_tokens
+
+        n = self.n if isinstance(self.n, Unset) else (None, str(self.n).encode(), "text/plain")
+
+        presence_penalty = (
+            self.presence_penalty
+            if isinstance(self.presence_penalty, Unset)
+            else (None, str(self.presence_penalty).encode(), "text/plain")
+        )
+
+        response_format: Union[None, Tuple[None, bytes, str], Unset]
+        if isinstance(self.response_format, Unset):
+            response_format = UNSET
+        elif isinstance(self.response_format, ChatCompletionInputResponseFormatType0):
+            response_format = (None, json.dumps(self.response_format.to_dict()).encode(), "application/json")
+        else:
+            response_format = self.response_format
+
+        seed: Union[None, Unset, int]
+        if isinstance(self.seed, Unset):
+            seed = UNSET
+        else:
+            seed = self.seed
+
+        stop: Union[None, Unset, str]
+        if isinstance(self.stop, Unset):
+            stop = UNSET
+        else:
+            stop = self.stop
+
+        stream = self.stream if isinstance(self.stream, Unset) else (None, str(self.stream).encode(), "text/plain")
+
+        temperature: Union[None, Unset, float]
+        if isinstance(self.temperature, Unset):
+            temperature = UNSET
+        else:
+            temperature = self.temperature
+
+        top_p: Union[None, Unset, float]
+        if isinstance(self.top_p, Unset):
+            top_p = UNSET
+        else:
+            top_p = self.top_p
+
+        tools: Union[Unset, Tuple[None, bytes, str]] = UNSET
+        if not isinstance(self.tools, Unset):
+            _temp_tools = []
+            for tools_item_data in self.tools:
+                tools_item = tools_item_data.to_dict()
+                _temp_tools.append(tools_item)
+            tools = (None, json.dumps(_temp_tools).encode(), "application/json")
+
+        user: Union[None, Unset, str]
+        if isinstance(self.user, Unset):
+            user = UNSET
+        else:
+            user = self.user
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(
+            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
+        )
+        field_dict.update(
+            {
+                "project_id": project_id,
+                "messages": messages,
+            }
+        )
+        if model is not UNSET:
+            field_dict["model"] = model
+        if system_prompt is not UNSET:
+            field_dict["system_prompt"] = system_prompt
         if frequency_penalty is not UNSET:
             field_dict["frequency_penalty"] = frequency_penalty
         if logit_bias is not UNSET:
             field_dict["logit_bias"] = logit_bias
         if max_tokens is not UNSET:
             field_dict["max_tokens"] = max_tokens
         if n is not UNSET:
@@ -198,30 +346,32 @@
             field_dict["user"] = user
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         from ..models.chat_completion_input_logit_bias_type_0 import ChatCompletionInputLogitBiasType0
-        from ..models.chat_completion_input_messages_item import ChatCompletionInputMessagesItem
         from ..models.chat_completion_input_response_format_type_0 import ChatCompletionInputResponseFormatType0
         from ..models.chat_completion_input_tools_item import ChatCompletionInputToolsItem
+        from ..models.message import Message
 
         d = src_dict.copy() if src_dict else {}
         project_id = d.pop("project_id")
 
         messages = []
         _messages = d.pop("messages")
         for messages_item_data in _messages:
-            messages_item = ChatCompletionInputMessagesItem.from_dict(messages_item_data)
+            messages_item = Message.from_dict(messages_item_data)
 
             messages.append(messages_item)
 
         model = d.pop("model", UNSET)
 
+        system_prompt = d.pop("system_prompt", UNSET)
+
         frequency_penalty = d.pop("frequency_penalty", UNSET)
 
         def _parse_logit_bias(data: object) -> Union["ChatCompletionInputLogitBiasType0", None, Unset]:
             if data is None:
                 return data
             if isinstance(data, Unset):
                 return data
@@ -321,14 +471,15 @@
 
         user = _parse_user(d.pop("user", UNSET))
 
         chat_completion_input = cls(
             project_id=project_id,
             messages=messages,
             model=model,
+            system_prompt=system_prompt,
             frequency_penalty=frequency_penalty,
             logit_bias=logit_bias,
             max_tokens=max_tokens,
             n=n,
             presence_penalty=presence_penalty,
             response_format=response_format,
             seed=seed,
```

### Comparing `premai-0.3.8/premai/models/chat_completion_input_logit_bias_type_0.py` & `premai-0.3.9/premai/models/chat_completion_input_logit_bias_type_0.py`

 * *Files identical despite different names*

### Comparing `premai-0.3.8/premai/models/chat_completion_input_messages_item.py` & `premai-0.3.9/premai/models/message.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,40 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.chat_completion_input_messages_item_role import ChatCompletionInputMessagesItemRole
+from ..models.role_enum import RoleEnum
 
-T = TypeVar("T", bound="ChatCompletionInputMessagesItem")
+T = TypeVar("T", bound="Message")
 
 
-class ChatCompletionInputMessagesItemDict(TypedDict):
-    role: "ChatCompletionInputMessagesItemRole"
+class MessageDict(TypedDict):
+    role: RoleEnum
     content: str
     pass
 
 
 @_attrs_define
-class ChatCompletionInputMessagesItem:
+class Message:
     """
     Attributes:
-        role (ChatCompletionInputMessagesItemRole): The role of the sender (e.g., 'user', 'assistant' or 'system').
-
-            * `user` - user
-            * `system` - system
+        role (RoleEnum): * `user` - user
             * `assistant` - assistant
         content (str): The content of the message.
     """
 
-    role: "ChatCompletionInputMessagesItemRole"
+    role: RoleEnum
     content: str
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        role = self.role.to_dict()
+        role = self.role.value
 
         content = self.content
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
@@ -46,28 +43,26 @@
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.chat_completion_input_messages_item_role import ChatCompletionInputMessagesItemRole
-
         d = src_dict.copy() if src_dict else {}
-        role = ChatCompletionInputMessagesItemRole.from_dict(d.pop("role"))
+        role = RoleEnum(d.pop("role"))
 
         content = d.pop("content")
 
-        chat_completion_input_messages_item = cls(
+        message = cls(
             role=role,
             content=content,
         )
 
-        chat_completion_input_messages_item.additional_properties = d
-        return chat_completion_input_messages_item
+        message.additional_properties = d
+        return message
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/chat_completion_input_messages_item_role.py` & `premai-0.3.9/premai/models/fine_tuning_sample.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,65 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-T = TypeVar("T", bound="ChatCompletionInputMessagesItemRole")
+T = TypeVar("T", bound="FineTuningSample")
 
 
-class ChatCompletionInputMessagesItemRoleDict(TypedDict):
+class FineTuningSampleDict(TypedDict):
+    input_: str
+    output: str
     pass
 
 
 @_attrs_define
-class ChatCompletionInputMessagesItemRole:
-    """The role of the sender (e.g., 'user', 'assistant' or 'system').
-
-    * `user` - user
-    * `system` - system
-    * `assistant` - assistant
-
+class FineTuningSample:
     """
+    Attributes:
+        input_ (str): The input text.
+        output (str): The output text.
+    """
+
+    input_: str
+    output: str
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
+        input_ = self.input_
+
+        output = self.output
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
-        field_dict.update({})
+        field_dict.update(
+            {
+                "input": input_,
+                "output": output,
+            }
+        )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
-        chat_completion_input_messages_item_role = cls()
+        input_ = d.pop("input")
+
+        output = d.pop("output")
+
+        fine_tuning_sample = cls(
+            input_=input_,
+            output=output,
+        )
 
-        chat_completion_input_messages_item_role.additional_properties = d
-        return chat_completion_input_messages_item_role
+        fine_tuning_sample.additional_properties = d
+        return fine_tuning_sample
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/chat_completion_input_response_format_type_0.py` & `premai-0.3.9/premai/models/chat_completion_input_response_format_type_0.py`

 * *Files identical despite different names*

### Comparing `premai-0.3.8/premai/models/chat_completion_input_tools_item.py` & `premai-0.3.9/premai/models/chat_completion_input_tools_item.py`

 * *Files identical despite different names*

### Comparing `premai-0.3.8/premai/models/chat_completion_response.py` & `premai-0.3.9/premai/models/chat_completion_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,53 @@
 from typing import Dict, List, Type, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, NotRequired, TypedDict, TypeVar
 
-from ..models.chat_completion_response_choices_item import ChatCompletionResponseChoicesItem
-from ..models.chat_completion_response_usage import ChatCompletionResponseUsage
+from ..models.response_choice import ResponseChoice
+from ..models.usage import Usage
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="ChatCompletionResponse")
 
 
 class ChatCompletionResponseDict(TypedDict):
     id: str
-    choices: List["ChatCompletionResponseChoicesItem"]
+    choices: List["ResponseChoice"]
     created: int
     model: str
     provider_name: str
     provider_id: str
-    usage: NotRequired[Union[Unset, ChatCompletionResponseUsage]]
+    usage: NotRequired[Union[Unset, Usage]]
     pass
 
 
 @_attrs_define
 class ChatCompletionResponse:
     """
     Attributes:
         id (str): A unique identifier for the chat completion. Each chunk has the same ID.
-        choices (List['ChatCompletionResponseChoicesItem']): A list of chat completion choices. Can be more than one if
-            n is greater than 1.
+        choices (List['ResponseChoice']): A list of chat completion choices. Can be more than one if n is greater than
+            1.
         created (int): The Unix timestamp (in seconds) of when the chat completion was created. Each chunk has the same
             timestamp.
         model (str): The model to generate the completion.
         provider_name (str): The name of the provider that generated the completion.
         provider_id (str): The ID of the provider that generated the completion.
-        usage (Union[Unset, ChatCompletionResponseUsage]): The usage statistics for the completion.
+        usage (Union[Unset, Usage]):
     """
 
     id: str
-    choices: List["ChatCompletionResponseChoicesItem"]
+    choices: List["ResponseChoice"]
     created: int
     model: str
     provider_name: str
     provider_id: str
-    usage: Union[Unset, "ChatCompletionResponseUsage"] = UNSET
+    usage: Union[Unset, "Usage"] = UNSET
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
         choices = []
@@ -82,41 +82,41 @@
         if usage is not UNSET:
             field_dict["usage"] = usage
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.chat_completion_response_choices_item import ChatCompletionResponseChoicesItem
-        from ..models.chat_completion_response_usage import ChatCompletionResponseUsage
+        from ..models.response_choice import ResponseChoice
+        from ..models.usage import Usage
 
         d = src_dict.copy() if src_dict else {}
         id = d.pop("id")
 
         choices = []
         _choices = d.pop("choices")
         for choices_item_data in _choices:
-            choices_item = ChatCompletionResponseChoicesItem.from_dict(choices_item_data)
+            choices_item = ResponseChoice.from_dict(choices_item_data)
 
             choices.append(choices_item)
 
         created = d.pop("created")
 
         model = d.pop("model")
 
         provider_name = d.pop("provider_name")
 
         provider_id = d.pop("provider_id")
 
         _usage = d.pop("usage", UNSET)
-        usage: Union[Unset, ChatCompletionResponseUsage]
+        usage: Union[Unset, Usage]
         if isinstance(_usage, Unset):
             usage = UNSET
         else:
-            usage = ChatCompletionResponseUsage.from_dict(_usage)
+            usage = Usage.from_dict(_usage)
 
         chat_completion_response = cls(
             id=id,
             choices=choices,
             created=created,
             model=model,
             provider_name=provider_name,
```

### Comparing `premai-0.3.8/premai/models/chat_completion_response_choices_item.py` & `premai-0.3.9/premai/models/response_choice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-T = TypeVar("T", bound="ChatCompletionResponseChoicesItem")
+T = TypeVar("T", bound="ResponseChoice")
 
 
-class ChatCompletionResponseChoicesItemDict(TypedDict):
+class ResponseChoiceDict(TypedDict):
     message: str
     finish_reason: str
     pass
 
 
 @_attrs_define
-class ChatCompletionResponseChoicesItem:
+class ResponseChoice:
     """
     Attributes:
         message (str): The generated message in the chat completion choice.
         finish_reason (str): The reason the chat completion finished, e.g., 'stop' or 'length'.
     """
 
     message: str
@@ -45,21 +45,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         message = d.pop("message")
 
         finish_reason = d.pop("finish_reason")
 
-        chat_completion_response_choices_item = cls(
+        response_choice = cls(
             message=message,
             finish_reason=finish_reason,
         )
 
-        chat_completion_response_choices_item.additional_properties = d
-        return chat_completion_response_choices_item
+        response_choice.additional_properties = d
+        return response_choice
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/chat_completion_response_usage.py` & `premai-0.3.9/premai/models/usage.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, NotRequired, TypedDict, TypeVar
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ChatCompletionResponseUsage")
+T = TypeVar("T", bound="Usage")
 
 
-class ChatCompletionResponseUsageDict(TypedDict):
+class UsageDict(TypedDict):
     completion_tokens: NotRequired[Union[Unset, int]]
     prompt_tokens: NotRequired[Union[Unset, int]]
     total_tokens: NotRequired[Union[Unset, int]]
     pass
 
 
 @_attrs_define
-class ChatCompletionResponseUsage:
-    """The usage statistics for the completion.
-
+class Usage:
+    """
     Attributes:
         completion_tokens (Union[Unset, int]):
         prompt_tokens (Union[Unset, int]):
         total_tokens (Union[Unset, int]):
     """
 
     completion_tokens: Union[Unset, int] = UNSET
@@ -56,22 +55,22 @@
         d = src_dict.copy() if src_dict else {}
         completion_tokens = d.pop("completion_tokens", UNSET)
 
         prompt_tokens = d.pop("prompt_tokens", UNSET)
 
         total_tokens = d.pop("total_tokens", UNSET)
 
-        chat_completion_response_usage = cls(
+        usage = cls(
             completion_tokens=completion_tokens,
             prompt_tokens=prompt_tokens,
             total_tokens=total_tokens,
         )
 
-        chat_completion_response_usage.additional_properties = d
-        return chat_completion_response_usage
+        usage.additional_properties = d
+        return usage
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/conflict_error.py` & `premai-0.3.9/premai/models/conflict_error.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.conflict_error_code import ConflictErrorCode
+from ..models.conflict_error_code_enum import ConflictErrorCodeEnum
 
 T = TypeVar("T", bound="ConflictError")
 
 
 class ConflictErrorDict(TypedDict):
     message: str
-    code: ConflictErrorCode
+    code: ConflictErrorCodeEnum
     pass
 
 
 @_attrs_define
 class ConflictError:
     """
     Attributes:
         message (str):
-        code (ConflictErrorCode): * `ConflictError` - ConflictError
+        code (ConflictErrorCodeEnum): * `ConflictError` - ConflictError
     """
 
     message: str
-    code: ConflictErrorCode
+    code: ConflictErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         message = self.message
 
         code = self.code.value
@@ -45,15 +45,15 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         message = d.pop("message")
 
-        code = ConflictErrorCode(d.pop("code"))
+        code = ConflictErrorCodeEnum(d.pop("code"))
 
         conflict_error = cls(
             message=message,
             code=code,
         )
 
         conflict_error.additional_properties = d
```

### Comparing `premai-0.3.8/premai/models/data_point.py` & `premai-0.3.9/premai/models/data_point.py`

 * *Files identical despite different names*

### Comparing `premai-0.3.8/premai/models/embedding.py` & `premai-0.3.9/premai/models/embedding.py`

 * *Files identical despite different names*

### Comparing `premai-0.3.8/premai/models/embeddings_input.py` & `premai-0.3.9/premai/models/embeddings_input.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,43 @@
-from typing import Dict, List, Type, Union, cast
+import json
+from typing import Dict, List, Tuple, Type, Union, cast
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
-from typing_extensions import Any, NotRequired, TypedDict, TypeVar
+from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.embeddings_input_encoding_format import EmbeddingsInputEncodingFormat
+from ..models.encoding_format_enum import EncodingFormatEnum
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="EmbeddingsInput")
 
 
 class EmbeddingsInputDict(TypedDict):
     project_id: int
     model: str
     input_: List[Union[List[List[int]], List[int], List[str], str]]
-    encoding_format: NotRequired[Union[Unset, EmbeddingsInputEncodingFormat]]
+    encoding_format: Union[Unset, EncodingFormatEnum] = EncodingFormatEnum.FLOAT
     pass
 
 
 @_attrs_define
 class EmbeddingsInput:
     """
     Attributes:
         project_id (int): The ID of the project to use.
         model (str): The model to generate the embeddings.
         input_ (List[Union[List[List[int]], List[int], List[str], str]]): Embedding Input
-        encoding_format (Union[Unset, EmbeddingsInputEncodingFormat]):
+        encoding_format (Union[Unset, EncodingFormatEnum]): * `float` - float
+            * `base64` - base64 Default: EncodingFormatEnum.FLOAT.
     """
 
     project_id: int
     model: str
     input_: List[Union[List[List[int]], List[int], List[str], str]]
-    encoding_format: Union[Unset, "EmbeddingsInputEncodingFormat"] = UNSET
+    encoding_format: Union[Unset, EncodingFormatEnum] = EncodingFormatEnum.FLOAT
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         project_id = self.project_id
 
         model = self.model
@@ -56,17 +58,17 @@
 
                     input_item.append(input_item_type_3_item)
 
             else:
                 input_item = input_item_data
             input_.append(input_item)
 
-        encoding_format: Union[Unset, Dict[str, Any]] = UNSET
+        encoding_format: Union[Unset, str] = UNSET
         if not isinstance(self.encoding_format, Unset):
-            encoding_format = self.encoding_format.to_dict()
+            encoding_format = self.encoding_format.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "project_id": project_id,
                 "model": model,
@@ -74,18 +76,66 @@
             }
         )
         if encoding_format is not UNSET:
             field_dict["encoding_format"] = encoding_format
 
         return field_dict
 
+    def to_multipart(self) -> Dict[str, Any]:
+        project_id = (
+            self.project_id
+            if isinstance(self.project_id, Unset)
+            else (None, str(self.project_id).encode(), "text/plain")
+        )
+
+        model = self.model if isinstance(self.model, Unset) else (None, str(self.model).encode(), "text/plain")
+
+        _temp_input_ = []
+        for input_item_data in self.input_:
+            input_item: Union[List[List[int]], List[int], List[str], str]
+            if isinstance(input_item_data, list):
+                input_item = input_item_data
+
+            elif isinstance(input_item_data, list):
+                input_item = input_item_data
+
+            elif isinstance(input_item_data, list):
+                input_item = []
+                for input_item_type_3_item_data in input_item_data:
+                    input_item_type_3_item = input_item_type_3_item_data
+
+                    input_item.append(input_item_type_3_item)
+
+            else:
+                input_item = input_item_data
+            _temp_input_.append(input_item)
+        input_ = (None, json.dumps(_temp_input_).encode(), "application/json")
+
+        encoding_format: Union[Unset, Tuple[None, bytes, str]] = UNSET
+        if not isinstance(self.encoding_format, Unset):
+            encoding_format = (None, str(self.encoding_format.value).encode(), "text/plain")
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(
+            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
+        )
+        field_dict.update(
+            {
+                "project_id": project_id,
+                "model": model,
+                "input": input_,
+            }
+        )
+        if encoding_format is not UNSET:
+            field_dict["encoding_format"] = encoding_format
+
+        return field_dict
+
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.embeddings_input_encoding_format import EmbeddingsInputEncodingFormat
-
         d = src_dict.copy() if src_dict else {}
         project_id = d.pop("project_id")
 
         model = d.pop("model")
 
         input_ = []
         _input_ = d.pop("input")
@@ -124,19 +174,19 @@
                 return cast(Union[List[List[int]], List[int], List[str], str], data)
 
             input_item = _parse_input_item(input_item_data)
 
             input_.append(input_item)
 
         _encoding_format = d.pop("encoding_format", UNSET)
-        encoding_format: Union[Unset, EmbeddingsInputEncodingFormat]
+        encoding_format: Union[Unset, EncodingFormatEnum]
         if isinstance(_encoding_format, Unset):
             encoding_format = UNSET
         else:
-            encoding_format = EmbeddingsInputEncodingFormat.from_dict(_encoding_format)
+            encoding_format = EncodingFormatEnum(_encoding_format)
 
         embeddings_input = cls(
             project_id=project_id,
             model=model,
             input_=input_,
             encoding_format=encoding_format,
         )
```

### Comparing `premai-0.3.8/premai/models/embeddings_input_encoding_format.py` & `premai-0.3.9/premai/models/validation_detail_error_messages_item.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-T = TypeVar("T", bound="EmbeddingsInputEncodingFormat")
+T = TypeVar("T", bound="ValidationDetailErrorMessagesItem")
 
 
-class EmbeddingsInputEncodingFormatDict(TypedDict):
+class ValidationDetailErrorMessagesItemDict(TypedDict):
     pass
 
 
 @_attrs_define
-class EmbeddingsInputEncodingFormat:
+class ValidationDetailErrorMessagesItem:
     """ """
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
-        embeddings_input_encoding_format = cls()
+        validation_detail_error_messages_item = cls()
 
-        embeddings_input_encoding_format.additional_properties = d
-        return embeddings_input_encoding_format
+        validation_detail_error_messages_item.additional_properties = d
+        return validation_detail_error_messages_item
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/embeddings_response.py` & `premai-0.3.9/premai/models/embeddings_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 from typing import Dict, List, Type, Union
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, NotRequired, TypedDict, TypeVar
 
-from ..models.embeddings_response_data_item import EmbeddingsResponseDataItem
-from ..models.embeddings_response_usage import EmbeddingsResponseUsage
+from ..models.embedding import Embedding
+from ..models.usage import Usage
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="EmbeddingsResponse")
 
 
 class EmbeddingsResponseDict(TypedDict):
-    data: List["EmbeddingsResponseDataItem"]
+    data: List["Embedding"]
     model: str
     provider_name: str
     provider_id: str
-    usage: NotRequired[Union[Unset, EmbeddingsResponseUsage]]
+    usage: NotRequired[Union[Unset, Usage]]
     pass
 
 
 @_attrs_define
 class EmbeddingsResponse:
     """
     Attributes:
-        data (List['EmbeddingsResponseDataItem']): The embeddings for the input.
+        data (List['Embedding']): The embeddings for the input.
         model (str): The model to generate the embeddings.
         provider_name (str): The name of the provider that generated the completion.
         provider_id (str): The ID of the provider that generated the completion.
-        usage (Union[Unset, EmbeddingsResponseUsage]): The usage statistics for the completion.
+        usage (Union[Unset, Usage]):
     """
 
-    data: List["EmbeddingsResponseDataItem"]
+    data: List["Embedding"]
     model: str
     provider_name: str
     provider_id: str
-    usage: Union[Unset, "EmbeddingsResponseUsage"] = UNSET
+    usage: Union[Unset, "Usage"] = UNSET
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         data = []
         for data_item_data in self.data:
             data_item = data_item_data.to_dict()
@@ -68,37 +68,37 @@
         if usage is not UNSET:
             field_dict["usage"] = usage
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.embeddings_response_data_item import EmbeddingsResponseDataItem
-        from ..models.embeddings_response_usage import EmbeddingsResponseUsage
+        from ..models.embedding import Embedding
+        from ..models.usage import Usage
 
         d = src_dict.copy() if src_dict else {}
         data = []
         _data = d.pop("data")
         for data_item_data in _data:
-            data_item = EmbeddingsResponseDataItem.from_dict(data_item_data)
+            data_item = Embedding.from_dict(data_item_data)
 
             data.append(data_item)
 
         model = d.pop("model")
 
         provider_name = d.pop("provider_name")
 
         provider_id = d.pop("provider_id")
 
         _usage = d.pop("usage", UNSET)
-        usage: Union[Unset, EmbeddingsResponseUsage]
+        usage: Union[Unset, Usage]
         if isinstance(_usage, Unset):
             usage = UNSET
         else:
-            usage = EmbeddingsResponseUsage.from_dict(_usage)
+            usage = Usage.from_dict(_usage)
 
         embeddings_response = cls(
             data=data,
             model=model,
             provider_name=provider_name,
             provider_id=provider_id,
             usage=usage,
```

### Comparing `premai-0.3.8/premai/models/embeddings_response_data_item.py` & `premai-0.3.9/premai/models/validation_error_details.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,74 +1,60 @@
-from typing import Dict, List, Type, cast
+from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-T = TypeVar("T", bound="EmbeddingsResponseDataItem")
+from ..models.validation_detail import ValidationDetail
 
+T = TypeVar("T", bound="ValidationErrorDetails")
 
-class EmbeddingsResponseDataItemDict(TypedDict):
-    index: int
-    embedding: List[float]
+
+class ValidationErrorDetailsDict(TypedDict):
     pass
 
 
 @_attrs_define
-class EmbeddingsResponseDataItem:
-    """
-    Attributes:
-        index (int): The index of the token in the input.
-        embedding (List[float]): The embedding for the input.
-    """
-
-    index: int
-    embedding: List[float]
+class ValidationErrorDetails:
+    """Detailed information about the validation errors."""
 
-    additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
+    additional_properties: Dict[str, "ValidationDetail"] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        index = self.index
-
-        embedding = self.embedding
-
         field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "index": index,
-                "embedding": embedding,
-            }
-        )
+        for prop_name, prop in self.additional_properties.items():
+            field_dict[prop_name] = prop.to_dict()
+        field_dict.update({})
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.validation_detail import ValidationDetail
+
         d = src_dict.copy() if src_dict else {}
-        index = d.pop("index")
+        validation_error_details = cls()
 
-        embedding = cast(List[float], d.pop("embedding"))
+        additional_properties = {}
+        for prop_name, prop_dict in d.items():
+            additional_property = ValidationDetail.from_dict(prop_dict)
 
-        embeddings_response_data_item = cls(
-            index=index,
-            embedding=embedding,
-        )
+            additional_properties[prop_name] = additional_property
 
-        embeddings_response_data_item.additional_properties = d
-        return embeddings_response_data_item
+        validation_error_details.additional_properties = additional_properties
+        return validation_error_details
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> Any:
+    def __getitem__(self, key: str) -> "ValidationDetail":
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: Any) -> None:
+    def __setitem__(self, key: str, value: "ValidationDetail") -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `premai-0.3.8/premai/models/fine_tuning_input_training_data_item.py` & `premai-0.3.9/premai/models/rate_limit_error.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-T = TypeVar("T", bound="FineTuningInputTrainingDataItem")
+from ..models.rate_limit_error_code_enum import RateLimitErrorCodeEnum
 
+T = TypeVar("T", bound="RateLimitError")
 
-class FineTuningInputTrainingDataItemDict(TypedDict):
-    input_: str
-    output: str
+
+class RateLimitErrorDict(TypedDict):
+    message: str
+    code: RateLimitErrorCodeEnum
     pass
 
 
 @_attrs_define
-class FineTuningInputTrainingDataItem:
+class RateLimitError:
     """
     Attributes:
-        input_ (str): The input text.
-        output (str): The output text.
+        message (str):
+        code (RateLimitErrorCodeEnum): * `RateLimitError` - RateLimitError
     """
 
-    input_: str
-    output: str
+    message: str
+    code: RateLimitErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        input_ = self.input_
+        message = self.message
 
-        output = self.output
+        code = self.code.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "input": input_,
-                "output": output,
+                "message": message,
+                "code": code,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
-        input_ = d.pop("input")
+        message = d.pop("message")
 
-        output = d.pop("output")
+        code = RateLimitErrorCodeEnum(d.pop("code"))
 
-        fine_tuning_input_training_data_item = cls(
-            input_=input_,
-            output=output,
+        rate_limit_error = cls(
+            message=message,
+            code=code,
         )
 
-        fine_tuning_input_training_data_item.additional_properties = d
-        return fine_tuning_input_training_data_item
+        rate_limit_error.additional_properties = d
+        return rate_limit_error
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/fine_tuning_input_validaton_data_item.py` & `premai-0.3.9/premai/models/provider_api_timeout_error.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-T = TypeVar("T", bound="FineTuningInputValidatonDataItem")
+from ..models.provider_api_timeout_error_code_enum import ProviderAPITimeoutErrorCodeEnum
 
+T = TypeVar("T", bound="ProviderAPITimeoutError")
 
-class FineTuningInputValidatonDataItemDict(TypedDict):
-    input_: str
-    output: str
+
+class ProviderAPITimeoutErrorDict(TypedDict):
+    message: str
+    code: ProviderAPITimeoutErrorCodeEnum
     pass
 
 
 @_attrs_define
-class FineTuningInputValidatonDataItem:
+class ProviderAPITimeoutError:
     """
     Attributes:
-        input_ (str): The input text.
-        output (str): The output text.
+        message (str):
+        code (ProviderAPITimeoutErrorCodeEnum): * `ProviderAPITimeoutError` - ProviderAPITimeoutError
     """
 
-    input_: str
-    output: str
+    message: str
+    code: ProviderAPITimeoutErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        input_ = self.input_
+        message = self.message
 
-        output = self.output
+        code = self.code.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "input": input_,
-                "output": output,
+                "message": message,
+                "code": code,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
-        input_ = d.pop("input")
+        message = d.pop("message")
 
-        output = d.pop("output")
+        code = ProviderAPITimeoutErrorCodeEnum(d.pop("code"))
 
-        fine_tuning_input_validaton_data_item = cls(
-            input_=input_,
-            output=output,
+        provider_api_timeout_error = cls(
+            message=message,
+            code=code,
         )
 
-        fine_tuning_input_validaton_data_item.additional_properties = d
-        return fine_tuning_input_validaton_data_item
+        provider_api_timeout_error.additional_properties = d
+        return provider_api_timeout_error
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/fine_tuning_response.py` & `premai-0.3.9/premai/models/fine_tuning_response.py`

 * *Files identical despite different names*

### Comparing `premai-0.3.8/premai/models/fine_tuning_sample.py` & `premai-0.3.9/premai/models/model_not_found_error.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,65 +1,67 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-T = TypeVar("T", bound="FineTuningSample")
+from ..models.model_not_found_error_code_enum import ModelNotFoundErrorCodeEnum
 
+T = TypeVar("T", bound="ModelNotFoundError")
 
-class FineTuningSampleDict(TypedDict):
-    input_: str
-    output: str
+
+class ModelNotFoundErrorDict(TypedDict):
+    message: str
+    code: ModelNotFoundErrorCodeEnum
     pass
 
 
 @_attrs_define
-class FineTuningSample:
+class ModelNotFoundError:
     """
     Attributes:
-        input_ (str): The input text.
-        output (str): The output text.
+        message (str):
+        code (ModelNotFoundErrorCodeEnum): * `ModelNotFoundError` - ModelNotFoundError
     """
 
-    input_: str
-    output: str
+    message: str
+    code: ModelNotFoundErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        input_ = self.input_
+        message = self.message
 
-        output = self.output
+        code = self.code.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "input": input_,
-                "output": output,
+                "message": message,
+                "code": code,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
-        input_ = d.pop("input")
+        message = d.pop("message")
 
-        output = d.pop("output")
+        code = ModelNotFoundErrorCodeEnum(d.pop("code"))
 
-        fine_tuning_sample = cls(
-            input_=input_,
-            output=output,
+        model_not_found_error = cls(
+            message=message,
+            code=code,
         )
 
-        fine_tuning_sample.additional_properties = d
-        return fine_tuning_sample
+        model_not_found_error.additional_properties = d
+        return model_not_found_error
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/input_data_point.py` & `premai-0.3.9/premai/models/input_data_point.py`

 * *Files 23% similar despite different names*

```diff
@@ -79,14 +79,61 @@
         if output is not UNSET:
             field_dict["output"] = output
         if trace is not UNSET:
             field_dict["trace"] = trace
 
         return field_dict
 
+    def to_multipart(self) -> Dict[str, Any]:
+        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
+
+        positive = (
+            self.positive if isinstance(self.positive, Unset) else (None, str(self.positive).encode(), "text/plain")
+        )
+
+        project = self.project if isinstance(self.project, Unset) else (None, str(self.project).encode(), "text/plain")
+
+        input_: Union[None, Unset, str]
+        if isinstance(self.input_, Unset):
+            input_ = UNSET
+        else:
+            input_ = self.input_
+
+        output: Union[None, Unset, str]
+        if isinstance(self.output, Unset):
+            output = UNSET
+        else:
+            output = self.output
+
+        trace: Union[None, Unset, str]
+        if isinstance(self.trace, Unset):
+            trace = UNSET
+        else:
+            trace = self.trace
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(
+            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
+        )
+        field_dict.update(
+            {
+                "id": id,
+                "positive": positive,
+                "project": project,
+            }
+        )
+        if input_ is not UNSET:
+            field_dict["input"] = input_
+        if output is not UNSET:
+            field_dict["output"] = output
+        if trace is not UNSET:
+            field_dict["trace"] = trace
+
+        return field_dict
+
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         id = d.pop("id")
 
         positive = d.pop("positive")
```

### Comparing `premai-0.3.8/premai/models/internal_server_error_type_0.py` & `premai-0.3.9/premai/models/permission_denied_error.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.internal_server_error_type_0_code import InternalServerErrorType0Code
+from ..models.permission_denied_error_code_enum import PermissionDeniedErrorCodeEnum
 
-T = TypeVar("T", bound="InternalServerErrorType0")
+T = TypeVar("T", bound="PermissionDeniedError")
 
 
-class InternalServerErrorType0Dict(TypedDict):
+class PermissionDeniedErrorDict(TypedDict):
     message: str
-    code: InternalServerErrorType0Code
+    code: PermissionDeniedErrorCodeEnum
     pass
 
 
 @_attrs_define
-class InternalServerErrorType0:
+class PermissionDeniedError:
     """
     Attributes:
         message (str):
-        code (InternalServerErrorType0Code): * `ProviderInternalServerError` - ProviderInternalServerError
+        code (PermissionDeniedErrorCodeEnum): * `PermissionDeniedError` - PermissionDeniedError
     """
 
     message: str
-    code: InternalServerErrorType0Code
+    code: PermissionDeniedErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         message = self.message
 
         code = self.code.value
@@ -45,23 +45,23 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         message = d.pop("message")
 
-        code = InternalServerErrorType0Code(d.pop("code"))
+        code = PermissionDeniedErrorCodeEnum(d.pop("code"))
 
-        internal_server_error_type_0 = cls(
+        permission_denied_error = cls(
             message=message,
             code=code,
         )
 
-        internal_server_error_type_0.additional_properties = d
-        return internal_server_error_type_0
+        permission_denied_error.additional_properties = d
+        return permission_denied_error
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/internal_server_error_type_2.py` & `premai-0.3.9/premai/models/provider_not_found_error.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.internal_server_error_type_2_code import InternalServerErrorType2Code
+from ..models.provider_not_found_error_code_enum import ProviderNotFoundErrorCodeEnum
 
-T = TypeVar("T", bound="InternalServerErrorType2")
+T = TypeVar("T", bound="ProviderNotFoundError")
 
 
-class InternalServerErrorType2Dict(TypedDict):
+class ProviderNotFoundErrorDict(TypedDict):
     message: str
-    code: InternalServerErrorType2Code
+    code: ProviderNotFoundErrorCodeEnum
     pass
 
 
 @_attrs_define
-class InternalServerErrorType2:
+class ProviderNotFoundError:
     """
     Attributes:
         message (str):
-        code (InternalServerErrorType2Code): * `ProviderAPIStatusError` - ProviderAPIStatusError
+        code (ProviderNotFoundErrorCodeEnum): * `ProviderNotFoundError` - ProviderNotFoundError
     """
 
     message: str
-    code: InternalServerErrorType2Code
+    code: ProviderNotFoundErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         message = self.message
 
         code = self.code.value
@@ -45,23 +45,23 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         message = d.pop("message")
 
-        code = InternalServerErrorType2Code(d.pop("code"))
+        code = ProviderNotFoundErrorCodeEnum(d.pop("code"))
 
-        internal_server_error_type_2 = cls(
+        provider_not_found_error = cls(
             message=message,
             code=code,
         )
 
-        internal_server_error_type_2.additional_properties = d
-        return internal_server_error_type_2
+        provider_not_found_error.additional_properties = d
+        return provider_not_found_error
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/internal_server_error_type_4.py` & `premai-0.3.9/premai/models/provider_api_connection_error.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.internal_server_error_type_4_code import InternalServerErrorType4Code
+from ..models.provider_api_connection_error_code_enum import ProviderAPIConnectionErrorCodeEnum
 
-T = TypeVar("T", bound="InternalServerErrorType4")
+T = TypeVar("T", bound="ProviderAPIConnectionError")
 
 
-class InternalServerErrorType4Dict(TypedDict):
+class ProviderAPIConnectionErrorDict(TypedDict):
     message: str
-    code: InternalServerErrorType4Code
+    code: ProviderAPIConnectionErrorCodeEnum
     pass
 
 
 @_attrs_define
-class InternalServerErrorType4:
+class ProviderAPIConnectionError:
     """
     Attributes:
         message (str):
-        code (InternalServerErrorType4Code): * `ProviderAPIConnectionError` - ProviderAPIConnectionError
+        code (ProviderAPIConnectionErrorCodeEnum): * `ProviderAPIConnectionError` - ProviderAPIConnectionError
     """
 
     message: str
-    code: InternalServerErrorType4Code
+    code: ProviderAPIConnectionErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         message = self.message
 
         code = self.code.value
@@ -45,23 +45,23 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         message = d.pop("message")
 
-        code = InternalServerErrorType4Code(d.pop("code"))
+        code = ProviderAPIConnectionErrorCodeEnum(d.pop("code"))
 
-        internal_server_error_type_4 = cls(
+        provider_api_connection_error = cls(
             message=message,
             code=code,
         )
 
-        internal_server_error_type_4.additional_properties = d
-        return internal_server_error_type_4
+        provider_api_connection_error.additional_properties = d
+        return provider_api_connection_error
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/model_not_found_error.py` & `premai-0.3.9/premai/models/provider_api_status_error.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.model_not_found_error_code import ModelNotFoundErrorCode
+from ..models.provider_api_status_error_code_enum import ProviderAPIStatusErrorCodeEnum
 
-T = TypeVar("T", bound="ModelNotFoundError")
+T = TypeVar("T", bound="ProviderAPIStatusError")
 
 
-class ModelNotFoundErrorDict(TypedDict):
+class ProviderAPIStatusErrorDict(TypedDict):
     message: str
-    code: ModelNotFoundErrorCode
+    code: ProviderAPIStatusErrorCodeEnum
     pass
 
 
 @_attrs_define
-class ModelNotFoundError:
+class ProviderAPIStatusError:
     """
     Attributes:
         message (str):
-        code (ModelNotFoundErrorCode): * `ModelNotFoundError` - ModelNotFoundError
+        code (ProviderAPIStatusErrorCodeEnum): * `ProviderAPIStatusError` - ProviderAPIStatusError
     """
 
     message: str
-    code: ModelNotFoundErrorCode
+    code: ProviderAPIStatusErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         message = self.message
 
         code = self.code.value
@@ -45,23 +45,23 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         message = d.pop("message")
 
-        code = ModelNotFoundErrorCode(d.pop("code"))
+        code = ProviderAPIStatusErrorCodeEnum(d.pop("code"))
 
-        model_not_found_error = cls(
+        provider_api_status_error = cls(
             message=message,
             code=code,
         )
 
-        model_not_found_error.additional_properties = d
-        return model_not_found_error
+        provider_api_status_error.additional_properties = d
+        return provider_api_status_error
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/patched_data_point.py` & `premai-0.3.9/premai/models/patched_data_point.py`

 * *Files 14% similar despite different names*

```diff
@@ -92,14 +92,69 @@
         if positive is not UNSET:
             field_dict["positive"] = positive
         if trace is not UNSET:
             field_dict["trace"] = trace
 
         return field_dict
 
+    def to_multipart(self) -> Dict[str, Any]:
+        id = self.id if isinstance(self.id, Unset) else (None, str(self.id).encode(), "text/plain")
+
+        created_at: Union[Unset, bytes] = UNSET
+        if not isinstance(self.created_at, Unset):
+            created_at = self.created_at.isoformat().encode()
+
+        updated_at: Union[Unset, bytes] = UNSET
+        if not isinstance(self.updated_at, Unset):
+            updated_at = self.updated_at.isoformat().encode()
+
+        input_: Union[None, Unset, str]
+        if isinstance(self.input_, Unset):
+            input_ = UNSET
+        else:
+            input_ = self.input_
+
+        output: Union[None, Unset, str]
+        if isinstance(self.output, Unset):
+            output = UNSET
+        else:
+            output = self.output
+
+        positive = (
+            self.positive if isinstance(self.positive, Unset) else (None, str(self.positive).encode(), "text/plain")
+        )
+
+        trace: Union[None, Unset, str]
+        if isinstance(self.trace, Unset):
+            trace = UNSET
+        else:
+            trace = self.trace
+
+        field_dict: Dict[str, Any] = {}
+        field_dict.update(
+            {key: (None, str(value).encode(), "text/plain") for key, value in self.additional_properties.items()}
+        )
+        field_dict.update({})
+        if id is not UNSET:
+            field_dict["id"] = id
+        if created_at is not UNSET:
+            field_dict["created_at"] = created_at
+        if updated_at is not UNSET:
+            field_dict["updated_at"] = updated_at
+        if input_ is not UNSET:
+            field_dict["input"] = input_
+        if output is not UNSET:
+            field_dict["output"] = output
+        if positive is not UNSET:
+            field_dict["positive"] = positive
+        if trace is not UNSET:
+            field_dict["trace"] = trace
+
+        return field_dict
+
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         id = d.pop("id", UNSET)
 
         _created_at = d.pop("created_at", UNSET)
         created_at: Union[Unset, datetime.datetime]
```

### Comparing `premai-0.3.8/premai/models/permission_denied_error.py` & `premai-0.3.9/premai/models/unprocessable_entity_error.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.permission_denied_error_code import PermissionDeniedErrorCode
+from ..models.unprocessable_entity_error_code_enum import UnprocessableEntityErrorCodeEnum
 
-T = TypeVar("T", bound="PermissionDeniedError")
+T = TypeVar("T", bound="UnprocessableEntityError")
 
 
-class PermissionDeniedErrorDict(TypedDict):
+class UnprocessableEntityErrorDict(TypedDict):
     message: str
-    code: PermissionDeniedErrorCode
+    code: UnprocessableEntityErrorCodeEnum
     pass
 
 
 @_attrs_define
-class PermissionDeniedError:
+class UnprocessableEntityError:
     """
     Attributes:
         message (str):
-        code (PermissionDeniedErrorCode): * `PermissionDeniedError` - PermissionDeniedError
+        code (UnprocessableEntityErrorCodeEnum): * `UnprocessableEntityError` - UnprocessableEntityError
     """
 
     message: str
-    code: PermissionDeniedErrorCode
+    code: UnprocessableEntityErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         message = self.message
 
         code = self.code.value
@@ -45,23 +45,23 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         message = d.pop("message")
 
-        code = PermissionDeniedErrorCode(d.pop("code"))
+        code = UnprocessableEntityErrorCodeEnum(d.pop("code"))
 
-        permission_denied_error = cls(
+        unprocessable_entity_error = cls(
             message=message,
             code=code,
         )
 
-        permission_denied_error.additional_properties = d
-        return permission_denied_error
+        unprocessable_entity_error.additional_properties = d
+        return unprocessable_entity_error
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/provider_api_connection_error.py` & `premai-0.3.9/premai/models/validation_detail.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.provider_api_connection_error_code import ProviderAPIConnectionErrorCode
+from ..models.validation_detail_error_messages_item import ValidationDetailErrorMessagesItem
 
-T = TypeVar("T", bound="ProviderAPIConnectionError")
+T = TypeVar("T", bound="ValidationDetail")
 
 
-class ProviderAPIConnectionErrorDict(TypedDict):
-    message: str
-    code: ProviderAPIConnectionErrorCode
+class ValidationDetailDict(TypedDict):
+    error_messages: List["ValidationDetailErrorMessagesItem"]
     pass
 
 
 @_attrs_define
-class ProviderAPIConnectionError:
+class ValidationDetail:
     """
     Attributes:
-        message (str):
-        code (ProviderAPIConnectionErrorCode): * `ProviderAPIConnectionError` - ProviderAPIConnectionError
+        error_messages (List['ValidationDetailErrorMessagesItem']): Error messages for the field.
     """
 
-    message: str
-    code: ProviderAPIConnectionErrorCode
+    error_messages: List["ValidationDetailErrorMessagesItem"]
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
-        message = self.message
-
-        code = self.code.value
+        error_messages = []
+        for error_messages_item_data in self.error_messages:
+            error_messages_item = error_messages_item_data.to_dict()
+            error_messages.append(error_messages_item)
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
-                "message": message,
-                "code": code,
+                "error_messages": error_messages,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.validation_detail_error_messages_item import ValidationDetailErrorMessagesItem
+
         d = src_dict.copy() if src_dict else {}
-        message = d.pop("message")
+        error_messages = []
+        _error_messages = d.pop("error_messages")
+        for error_messages_item_data in _error_messages:
+            error_messages_item = ValidationDetailErrorMessagesItem.from_dict(error_messages_item_data)
 
-        code = ProviderAPIConnectionErrorCode(d.pop("code"))
+            error_messages.append(error_messages_item)
 
-        provider_api_connection_error = cls(
-            message=message,
-            code=code,
+        validation_detail = cls(
+            error_messages=error_messages,
         )
 
-        provider_api_connection_error.additional_properties = d
-        return provider_api_connection_error
+        validation_detail.additional_properties = d
+        return validation_detail
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/provider_api_status_error.py` & `premai-0.3.9/premai/models/validation_error.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,79 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.provider_api_status_error_code import ProviderAPIStatusErrorCode
+from ..models.validation_error_code_enum import ValidationErrorCodeEnum
+from ..models.validation_error_details import ValidationErrorDetails
 
-T = TypeVar("T", bound="ProviderAPIStatusError")
+T = TypeVar("T", bound="ValidationError")
 
 
-class ProviderAPIStatusErrorDict(TypedDict):
+class ValidationErrorDict(TypedDict):
     message: str
-    code: ProviderAPIStatusErrorCode
+    details: "ValidationErrorDetails"
+    code: ValidationErrorCodeEnum
     pass
 
 
 @_attrs_define
-class ProviderAPIStatusError:
+class ValidationError:
     """
     Attributes:
-        message (str):
-        code (ProviderAPIStatusErrorCode): * `ProviderAPIStatusError` - ProviderAPIStatusError
+        message (str): A description of the validation error.
+        details (ValidationErrorDetails): Detailed information about the validation errors.
+        code (ValidationErrorCodeEnum): * `ValidationError` - ValidationError
     """
 
     message: str
-    code: ProviderAPIStatusErrorCode
+    details: "ValidationErrorDetails"
+    code: ValidationErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         message = self.message
 
+        details = self.details.to_dict()
+
         code = self.code.value
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update(
             {
                 "message": message,
+                "details": details,
                 "code": code,
             }
         )
 
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
+        from ..models.validation_error_details import ValidationErrorDetails
+
         d = src_dict.copy() if src_dict else {}
         message = d.pop("message")
 
-        code = ProviderAPIStatusErrorCode(d.pop("code"))
+        details = ValidationErrorDetails.from_dict(d.pop("details"))
+
+        code = ValidationErrorCodeEnum(d.pop("code"))
 
-        provider_api_status_error = cls(
+        validation_error = cls(
             message=message,
+            details=details,
             code=code,
         )
 
-        provider_api_status_error.additional_properties = d
-        return provider_api_status_error
+        validation_error.additional_properties = d
+        return validation_error
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `premai-0.3.8/premai/models/provider_internal_server_error.py` & `premai-0.3.9/premai/models/provider_internal_server_error.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from typing import Dict, List, Type
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 from typing_extensions import Any, TypedDict, TypeVar
 
-from ..models.provider_internal_server_error_code import ProviderInternalServerErrorCode
+from ..models.provider_internal_server_error_code_enum import ProviderInternalServerErrorCodeEnum
 
 T = TypeVar("T", bound="ProviderInternalServerError")
 
 
 class ProviderInternalServerErrorDict(TypedDict):
     message: str
-    code: ProviderInternalServerErrorCode
+    code: ProviderInternalServerErrorCodeEnum
     pass
 
 
 @_attrs_define
 class ProviderInternalServerError:
     """
     Attributes:
         message (str):
-        code (ProviderInternalServerErrorCode): * `ProviderInternalServerError` - ProviderInternalServerError
+        code (ProviderInternalServerErrorCodeEnum): * `ProviderInternalServerError` - ProviderInternalServerError
     """
 
     message: str
-    code: ProviderInternalServerErrorCode
+    code: ProviderInternalServerErrorCodeEnum
 
     additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
     def to_dict(self) -> Dict[str, Any]:
         message = self.message
 
         code = self.code.value
@@ -45,15 +45,15 @@
         return field_dict
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy() if src_dict else {}
         message = d.pop("message")
 
-        code = ProviderInternalServerErrorCode(d.pop("code"))
+        code = ProviderInternalServerErrorCodeEnum(d.pop("code"))
 
         provider_internal_server_error = cls(
             message=message,
             code=code,
         )
 
         provider_internal_server_error.additional_properties = d
```

### Comparing `premai-0.3.8/premai/models/retrieve_fine_tuning_response.py` & `premai-0.3.9/premai/models/retrieve_fine_tuning_response.py`

 * *Files identical despite different names*

### Comparing `premai-0.3.8/premai/types.py` & `premai-0.3.9/premai/types.py`

 * *Files identical despite different names*

### Comparing `premai-0.3.8/pyproject.toml` & `premai-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "premai"
-version = "0.3.8"
+version = "0.3.9"
 description = "A client library for accessing Prem APIs"
 authors = []
 readme = "README.md"
 packages = [
     {include = "premai"},
 ]
 include = ["CHANGELOG.md", "premai/py.typed"]
```

### Comparing `premai-0.3.8/PKG-INFO` & `premai-0.3.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: premai
-Version: 0.3.8
+Version: 0.3.9
 Summary: A client library for accessing Prem APIs
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -32,43 +32,44 @@
 
 ```python
 from premai import Prem
 
 client = Prem(
     api_key=YOUR_API_KEY
 )
-
-project_id = YOUR_PROJECT_ID
 ```
 
 ### Chat completion
 The `chat.completions` module allows you to generate completions based on user input. Here's an example:
 
 ```python
 messages = [
-    {"role": "system", "content": "You are a helpful assistant."},
     {"role": "user", "content": "Who won the world series in 2020?"},
 ]
-model = "gpt-3.5-turbo"
+model = "gpt-3.5-turbo" # optional
+system_prompt = "You are a helpful assistant." # optional
+project_id = YOUR_PROJECT_ID
 
 # Create completion
 response = client.chat.completions.create(
     project_id=project_id,
     messages=messages,
     model=model,
+    system_prompt=system_prompt,
     stream=False
 )
 
 print(response.choices)
 
 # Create completion with stream
 response = client.chat.completions.create(
     project_id=project_id,
     messages=messages,
     model=model,
+    system_prompt=system_prompt,
     stream=True
 )
 
 for chunk in response:
     if chunk.choices[0].delta["content"]:
         print(chunk.choices[0].delta["content"], end="")
```

