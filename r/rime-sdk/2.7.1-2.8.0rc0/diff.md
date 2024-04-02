# Comparing `tmp/rime_sdk-2.7.1.tar.gz` & `tmp/rime_sdk-2.8.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rime_sdk-2.7.1.tar", last modified: Sun Mar 31 01:04:26 2024, max compression
+gzip compressed data, was "rime_sdk-2.8.0rc0.tar", last modified: Sat Mar 30 17:18:25 2024, max compression
```

## Comparing `rime_sdk-2.7.1.tar` & `rime_sdk-2.8.0rc0.tar`

### file list

```diff
@@ -1,584 +1,584 @@
-drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-31 01:04:26.340152 rime_sdk-2.7.1/
--rw-rw-r--   0 runner    (1001) runner    (1001)      566 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/LICENSE
--rw-rw-r--   0 runner    (1001) runner    (1001)     1272 2024-03-31 01:04:26.340152 rime_sdk-2.7.1/PKG-INFO
--rw-rw-r--   0 runner    (1001) runner    (1001)      984 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/README.md
-drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-31 01:04:26.316152 rime_sdk-2.7.1/rime_sdk/
--rw-rw-r--   0 runner    (1001) runner    (1001)     1490 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/__init__.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2268 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/authenticator.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    70820 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/client.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    23353 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/continuous_test.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    12282 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/data_collector.py
--rw-rw-r--   0 runner    (1001) runner    (1001)      883 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/detection_event.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    24996 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/generative_firewall.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3453 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/generative_model.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4892 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/image_builder.py
-drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-31 01:04:26.316152 rime_sdk-2.7.1/rime_sdk/internal/
--rw-rw-r--   0 runner    (1001) runner    (1001)        0 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/internal/__init__.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    18350 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/internal/config_parser.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     1004 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/internal/constants.py
--rw-rw-r--   0 runner    (1001) runner    (1001)      667 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/internal/decorators.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     9740 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/internal/file_upload.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     1973 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/internal/rest_error_handler.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     9376 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/internal/swagger_parser.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2577 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/internal/swagger_utils.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     1081 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/internal/test_helpers.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2681 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/internal/throttle_queue.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3570 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/internal/utils.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    18764 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/job.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5042 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/monitor.py
--rw-rw-r--   0 runner    (1001) runner    (1001)   107184 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/project.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    38328 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/registry.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4396 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/schedule.py
-drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-31 01:04:26.316152 rime_sdk-2.7.1/rime_sdk/swagger/
--rw-rw-r--   0 runner    (1001) runner    (1001)        0 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/__init__.py
-drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-31 01:04:26.316152 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/
--rw-rw-r--   0 runner    (1001) runner    (1001)    59228 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/__init__.py
-drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-31 01:04:26.316152 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/
--rw-rw-r--   0 runner    (1001) runner    (1001)     2411 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/__init__.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    46640 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5851 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/config_validator_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    18207 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    25430 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/data_collector_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    11733 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/detection_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    23108 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    17931 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    27750 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/file_upload_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    19109 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/firewall_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    23787 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    22695 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    10262 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    28916 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/image_registry_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    27170 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/integration_service_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    27728 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/job_reader_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    21865 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    14474 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/model_testing_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    35026 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    19932 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    74338 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/project_service_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    57883 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/registry_service_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    77856 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/results_reader_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4167 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/rime_info_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    18249 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/schedule_service_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    40655 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/user_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    25780 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/validation_service_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    46472 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    25179 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api_client.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8845 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/configuration.py
-drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-31 01:04:26.340152 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/
--rw-rw-r--   0 runner    (1001) runner    (1001)    56718 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/__init__.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4210 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4369 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4328 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6669 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5483 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5103 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3706 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3725 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3435 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8968 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3552 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4503 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3582 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2551 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6687 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    17329 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3362 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8011 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4630 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2674 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2695 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7390 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4396 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3292 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6273 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    13500 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8080 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4925 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5748 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2705 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5806 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    14085 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8545 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3410 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    15539 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4273 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2728 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/detection_event_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2587 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4205 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/detection_resolution.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7745 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2744 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2719 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2670 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4176 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    10779 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    10808 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7556 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7459 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3304 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3285 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2555 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3294 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3310 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3232 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     9982 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5075 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3149 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    10070 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5158 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6961 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2822 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4455 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3382 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generative_testing_result_standard_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4502 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3679 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5387 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4675 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2722 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6459 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2844 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5781 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3291 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2896 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6773 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3517 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3686 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    11464 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4144 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3934 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3740 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_list_firewall_instances_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8681 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3784 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4877 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3752 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3712 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3487 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     9562 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2808 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3447 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5128 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3869 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5046 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4841 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    12694 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2667 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5869 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7850 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_model_connection_spec.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4012 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3664 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3408 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4422 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4103 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2821 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2770 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3403 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3161 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2808 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4550 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5064 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3344 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3915 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/job_data_scan.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4710 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4752 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4794 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4426 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4187 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4033 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6007 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5102 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5050 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4570 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3633 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2543 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6549 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4842 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4373 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3722 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5728 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5076 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3993 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4508 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2674 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    13205 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/model_model.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3523 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4142 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2745 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2515 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6262 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4125 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3518 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4963 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    12705 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2665 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4511 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2667 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3520 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_transform.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2728 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4020 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5602 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2543 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3275 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     9399 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_notification.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2774 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2644 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_object_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3594 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4781 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6823 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4341 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4384 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2563 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    11026 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3279 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2607 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2547 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3288 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3190 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4530 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     9270 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    10536 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    12754 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5306 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5738 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3739 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_owner_details.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    19393 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_project.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2693 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_project_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5013 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2579 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4180 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_schedule_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3279 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2571 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4380 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4765 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2715 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/protobuf_any.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2574 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6648 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3375 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4050 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4143 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_data_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6599 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    20609 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_data_params.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2624 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_data_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3454 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4688 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5621 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4998 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4224 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_metadata.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6051 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_model_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3453 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3654 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4161 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5645 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2728 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    13267 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3218 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5797 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5037 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2753 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2559 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8702 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_agent.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5337 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2745 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8524 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2775 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2519 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6159 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    13366 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2860 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_config_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4337 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3505 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3389 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4997 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6566 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4077 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6407 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3976 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3303 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3478 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3486 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7059 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3324 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6750 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3842 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3407 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3481 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4086 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3371 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7230 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3177 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5393 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3324 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5936 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3212 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7061 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3352 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2527 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2559 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2535 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2539 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2527 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2551 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3371 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2527 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2559 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2539 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2567 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5159 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2563 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4600 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6332 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6606 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3344 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3130 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_float_list.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3160 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3462 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3357 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4523 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6063 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3231 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4115 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3631 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3396 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3501 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3265 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3181 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3457 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3122 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3266 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3394 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3365 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3303 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5967 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6275 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3208 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8929 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3381 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3406 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3288 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8541 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4079 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3292 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8955 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4877 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3110 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3147 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4256 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4226 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4316 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3284 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2519 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4368 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3108 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_int_list.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4063 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6446 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_job_data.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    14784 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2865 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_job_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2617 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_job_view.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2611 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_language.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2904 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2770 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5439 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2672 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4968 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4995 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3283 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4835 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    11090 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5364 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4580 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5385 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5847 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4070 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7152 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5064 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4682 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3431 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4796 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5011 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5555 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5033 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4139 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3335 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5758 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2535 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4727 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3583 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2555 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4904 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3855 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    12972 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2701 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2784 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3900 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_model_card.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3127 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_model_task.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4059 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4134 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3697 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_named_double.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2620 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_order.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4197 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3415 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4616 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4108 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3320 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4337 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3678 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2575 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2535 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2567 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2691 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2666 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3126 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3976 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_search_spec.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2527 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2654 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_severity.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5062 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3831 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3226 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5586 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3178 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3194 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5016 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3304 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4870 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3288 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5859 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3336 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3390 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4438 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2547 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3108 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_str_list.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3289 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2741 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3134 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3854 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4448 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_table_column.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2768 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5133 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2718 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     9660 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3423 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4811 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2869 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2652 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3911 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2698 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_token_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3172 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5196 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2543 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3289 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3481 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3327 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3255 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3425 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3289 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2591 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2567 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2523 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2543 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2531 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3156 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2555 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4875 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5335 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_user_role.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3886 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6815 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3106 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_uuid.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2555 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7431 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_workspace.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7167 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7715 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2841 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4741 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4096 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/role_users_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4673 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4098 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4401 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4797 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6378 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4295 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4319 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6026 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schedule_schedule.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6508 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6690 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2948 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5053 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4051 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5310 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4156 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2790 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3993 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2803 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4121 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4121 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4136 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7276 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6259 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4371 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4136 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4187 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    10280 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6416 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    12809 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4278 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5610 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3485 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     9333 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4444 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2764 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6759 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3436 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3799 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3538 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3641 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3358 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5680 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5790 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3496 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5835 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5553 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5086 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5530 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3520 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3382 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     6503 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    16800 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7005 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    13296 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5304 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    13655 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4663 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    19373 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    11743 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4077 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3410 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/user_private_info.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     2634 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/user_role.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     7844 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/user_user_detail.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3815 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4140 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4196 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8329 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4326 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    13843 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    11044 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    10263 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4396 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8198 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     8401 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5364 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4825 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/validate_request_input.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     3641 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/validate_request_output.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5905 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5093 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5189 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4338 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     4533 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    13063 2024-03-31 01:04:25.000000 rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/rest.py
--rw-rw-r--   0 runner    (1001) runner    (1001)     5257 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/test_batch.py
--rw-rw-r--   0 runner    (1001) runner    (1001)    17414 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/rime_sdk/test_run.py
-drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-31 01:04:26.316152 rime_sdk-2.7.1/rime_sdk.egg-info/
--rw-rw-r--   0 runner    (1001) runner    (1001)     1272 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1001) runner    (1001)    40192 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1001) runner    (1001)        1 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1001) runner    (1001)       80 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk.egg-info/entry_points.txt
--rw-rw-r--   0 runner    (1001) runner    (1001)      161 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk.egg-info/requires.txt
--rw-rw-r--   0 runner    (1001) runner    (1001)        9 2024-03-31 01:04:26.000000 rime_sdk-2.7.1/rime_sdk.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1001) runner    (1001)       38 2024-03-31 01:04:26.340152 rime_sdk-2.7.1/setup.cfg
--rw-rw-r--   0 runner    (1001) runner    (1001)     3903 2024-03-31 01:03:02.000000 rime_sdk-2.7.1/setup.py
+drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-30 17:18:25.514318 rime_sdk-2.8.0rc0/
+-rw-rw-r--   0 runner    (1001) runner    (1001)      566 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/LICENSE
+-rw-rw-r--   0 runner    (1001) runner    (1001)     1275 2024-03-30 17:18:25.514318 rime_sdk-2.8.0rc0/PKG-INFO
+-rw-rw-r--   0 runner    (1001) runner    (1001)      984 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/README.md
+drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-30 17:18:25.474318 rime_sdk-2.8.0rc0/rime_sdk/
+-rw-rw-r--   0 runner    (1001) runner    (1001)     1490 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/__init__.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2268 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/authenticator.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    70820 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/client.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    23353 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/continuous_test.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    12282 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/data_collector.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)      883 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/detection_event.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    24996 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/generative_firewall.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3453 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/generative_model.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4892 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/image_builder.py
+drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-30 17:18:25.474318 rime_sdk-2.8.0rc0/rime_sdk/internal/
+-rw-rw-r--   0 runner    (1001) runner    (1001)        0 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/internal/__init__.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    18350 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/internal/config_parser.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     1004 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/internal/constants.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)      667 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/internal/decorators.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     9740 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/internal/file_upload.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     1973 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/internal/rest_error_handler.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     9376 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/internal/swagger_parser.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2577 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/internal/swagger_utils.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     1081 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/internal/test_helpers.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2681 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/internal/throttle_queue.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3570 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/internal/utils.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    18764 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/job.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5042 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/monitor.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)   107184 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/project.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    38328 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/registry.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4396 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/schedule.py
+drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-30 17:18:25.474318 rime_sdk-2.8.0rc0/rime_sdk/swagger/
+-rw-rw-r--   0 runner    (1001) runner    (1001)        0 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/__init__.py
+drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-30 17:18:25.474318 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/
+-rw-rw-r--   0 runner    (1001) runner    (1001)    59228 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/__init__.py
+drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-30 17:18:25.478318 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2411 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/__init__.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    46640 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/agent_manager_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5851 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/config_validator_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    18207 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    25430 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/data_collector_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    11733 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/detection_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    23108 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/feature_flag_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    17931 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/file_scanning_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    27750 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/file_upload_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    19109 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/firewall_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    23787 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    22695 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/firewall_service_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    10262 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    28916 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/image_registry_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    27170 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/integration_service_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    27728 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/job_reader_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    21865 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/model_card_service_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    14474 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/model_testing_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    35026 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/monitor_service_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    19932 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/notification_setting_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    74338 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/project_service_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    57883 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/registry_service_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    77856 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/results_reader_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4167 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/rime_info_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    18249 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/schedule_service_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    40655 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/user_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    25780 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/validation_service_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    46472 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/workspace_service_api.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    25179 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api_client.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8845 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/configuration.py
+drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-30 17:18:25.514318 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/
+-rw-rw-r--   0 runner    (1001) runner    (1001)    56718 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/__init__.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4210 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4369 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4328 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6669 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5483 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5103 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3706 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3725 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3435 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8968 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3552 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4503 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3582 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2551 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6687 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    17329 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3362 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8011 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4630 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2674 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2695 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7390 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4396 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3292 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6273 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    13500 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8080 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4925 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5748 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2705 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5806 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    14085 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/dataset_dataset.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8545 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3410 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    15539 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/detection_detection_event.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4273 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/detection_event_detail.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2728 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/detection_event_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2587 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4205 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/detection_resolution.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7745 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2744 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2719 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2670 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4176 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    10779 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    10808 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7556 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7459 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3304 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3285 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2555 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3294 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3310 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3232 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     9982 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/firewall_firewall.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5075 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3149 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    10070 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5158 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6961 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2822 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4455 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3382 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generative_testing_result_standard_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4502 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3679 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5387 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4675 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2722 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6459 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2844 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5781 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3291 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2896 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6773 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3517 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3686 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    11464 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4144 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3934 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3740 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_list_firewall_instances_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8681 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3784 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4877 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3752 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3712 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3487 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     9562 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2808 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3447 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5128 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3869 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5046 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4841 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    12694 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2667 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5869 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7850 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_model_connection_spec.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4012 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3664 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3408 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4422 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/googlerpc_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4103 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2821 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2770 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_level.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3403 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3161 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2808 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4550 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5064 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3344 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3915 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/job_data_scan.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4710 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4752 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4794 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4426 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4187 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4033 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6007 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5102 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5050 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4570 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3633 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2543 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6549 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4842 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4373 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3722 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5728 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5076 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3993 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4508 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2674 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    13205 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/model_model.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3523 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4142 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2745 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2515 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6262 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4125 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3518 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4963 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    12705 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_monitor.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2665 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4511 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_threshold.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2667 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3520 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_transform.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2728 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4020 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5602 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_digest_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2543 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3275 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     9399 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_notification.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2774 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_notification_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2644 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_object_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3594 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4781 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6823 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4341 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4384 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2563 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    11026 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_create_project_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3279 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_create_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2607 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2547 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3288 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_get_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3190 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4530 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     9270 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    10536 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    12754 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5306 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5738 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3739 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_owner_details.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    19393 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_project.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2693 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_project_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5013 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_project_with_details.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2579 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4180 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_schedule_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3279 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_update_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2571 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4380 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4765 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2715 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/protobuf_any.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2574 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6648 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_connection_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3375 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4050 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4143 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6599 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    20609 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_params.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2624 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3454 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4688 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5621 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4998 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4224 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_metadata.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6051 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_model_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3453 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3654 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4161 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_pred_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5645 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2728 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_validity_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    13267 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3218 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5797 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5037 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2753 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_actor_role.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2559 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8702 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5337 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2745 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8524 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2775 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2519 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6159 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_category_metric.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    13366 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2860 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_config_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4337 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3505 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3389 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4997 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6566 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4077 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6407 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3976 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3303 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3478 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3486 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7059 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3324 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6750 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3842 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3407 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3481 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4086 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3371 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7230 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3177 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5393 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3324 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5936 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3212 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7061 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3352 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2527 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2559 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2535 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2539 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2527 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2551 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3371 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2527 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2559 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2539 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2567 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5159 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2563 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4600 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_failing_row.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6332 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6606 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3344 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_feature_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3130 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_float_list.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3160 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3462 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3357 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4523 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6063 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3231 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4115 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3631 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3396 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3501 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3265 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3181 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3457 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3122 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3266 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3394 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3365 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3303 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5967 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6275 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3208 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8929 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3381 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3406 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3288 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8541 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4079 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3292 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8955 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4877 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3110 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3147 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4256 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4226 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4316 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3284 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2519 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4368 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_image_reference.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3108 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_int_list.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4063 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_integration_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6446 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_data.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    14784 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2865 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2617 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_view.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2611 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_language.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2904 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_license_feature.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2770 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_license_limit.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5439 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_limit_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2672 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4968 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4995 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3283 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4835 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    11090 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5364 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4580 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5385 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5847 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4070 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7152 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5064 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4682 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3431 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4796 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5011 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5555 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5033 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4139 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3335 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5758 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2535 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4727 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3583 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2555 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4904 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3855 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    12972 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2701 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2784 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3900 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_card.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3127 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_task.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4059 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4134 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3697 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_named_double.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2620 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_order.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4197 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3415 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4616 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4108 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3320 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4337 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3678 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2575 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2535 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2567 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2691 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2666 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3126 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_safe_url.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3976 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_search_spec.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2527 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2654 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_severity.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5062 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3831 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3226 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5586 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3178 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3194 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5016 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3304 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4870 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3288 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5859 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3336 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3390 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4438 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2547 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3108 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_str_list.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3289 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2741 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_subject_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3134 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_suggestion.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3854 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4448 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_table_column.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2768 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5133 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2718 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     9660 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_metric.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3423 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4811 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2869 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2652 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3911 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_time_interval.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2698 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_token_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3172 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5196 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2543 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3289 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3481 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3327 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3255 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3425 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3289 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2591 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2567 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2523 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2543 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2531 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3156 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2555 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4875 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5335 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_role.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3886 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6815 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3106 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_uuid.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2555 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7431 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_workspace.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7167 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7715 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2841 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4741 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4096 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/role_users_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4673 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/role_workspace_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4098 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4401 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4797 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6378 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4295 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4319 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6026 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schedule_schedule.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6508 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6690 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2948 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5053 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4051 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5310 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schemanotification_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4156 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2790 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3993 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2803 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/statedb_job_status.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4121 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4121 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4136 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7276 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6259 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4371 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4136 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4187 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    10280 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6416 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    12809 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4278 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5610 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3485 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     9333 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4444 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2764 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6759 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3436 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3799 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3538 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3641 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3358 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5680 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5790 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3496 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5835 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5553 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5086 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5530 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3520 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3382 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     6503 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    16800 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7005 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    13296 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5304 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    13655 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4663 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    19373 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    11743 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4077 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3410 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/user_private_info.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     2634 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/user_role.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     7844 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/user_user_detail.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3815 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4140 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4196 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8329 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4326 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    13843 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    11044 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    10263 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4396 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8198 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     8401 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5364 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4825 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/validate_request_input.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3641 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/validate_request_output.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5905 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5093 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5189 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4338 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     4533 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    13063 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/rest.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)     5257 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/test_batch.py
+-rw-rw-r--   0 runner    (1001) runner    (1001)    17414 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/rime_sdk/test_run.py
+drwxrwxr-x   0 runner    (1001) runner    (1001)        0 2024-03-30 17:18:25.474318 rime_sdk-2.8.0rc0/rime_sdk.egg-info/
+-rw-rw-r--   0 runner    (1001) runner    (1001)     1275 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1001) runner    (1001)    40192 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1001) runner    (1001)        1 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1001) runner    (1001)       80 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk.egg-info/entry_points.txt
+-rw-rw-r--   0 runner    (1001) runner    (1001)      161 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1001) runner    (1001)        9 2024-03-30 17:18:25.000000 rime_sdk-2.8.0rc0/rime_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1001) runner    (1001)       38 2024-03-30 17:18:25.514318 rime_sdk-2.8.0rc0/setup.cfg
+-rw-rw-r--   0 runner    (1001) runner    (1001)     3903 2024-03-30 17:17:14.000000 rime_sdk-2.8.0rc0/setup.py
```

### Comparing `rime_sdk-2.7.1/LICENSE` & `rime_sdk-2.8.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/PKG-INFO` & `rime_sdk-2.8.0rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime_sdk
-Version: 2.7.1
+Version: 2.8.0rc0
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.7.1/README.md` & `rime_sdk-2.8.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/__init__.py` & `rime_sdk-2.8.0rc0/rime_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/authenticator.py` & `rime_sdk-2.8.0rc0/rime_sdk/authenticator.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/client.py` & `rime_sdk-2.8.0rc0/rime_sdk/client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/continuous_test.py` & `rime_sdk-2.8.0rc0/rime_sdk/continuous_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/data_collector.py` & `rime_sdk-2.8.0rc0/rime_sdk/data_collector.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/detection_event.py` & `rime_sdk-2.8.0rc0/rime_sdk/detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/generative_firewall.py` & `rime_sdk-2.8.0rc0/rime_sdk/generative_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/generative_model.py` & `rime_sdk-2.8.0rc0/rime_sdk/generative_model.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/image_builder.py` & `rime_sdk-2.8.0rc0/rime_sdk/image_builder.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/internal/config_parser.py` & `rime_sdk-2.8.0rc0/rime_sdk/internal/config_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/internal/constants.py` & `rime_sdk-2.8.0rc0/rime_sdk/internal/constants.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/internal/decorators.py` & `rime_sdk-2.8.0rc0/rime_sdk/internal/decorators.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/internal/file_upload.py` & `rime_sdk-2.8.0rc0/rime_sdk/internal/file_upload.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/internal/rest_error_handler.py` & `rime_sdk-2.8.0rc0/rime_sdk/internal/rest_error_handler.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/internal/swagger_parser.py` & `rime_sdk-2.8.0rc0/rime_sdk/internal/swagger_parser.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/internal/swagger_utils.py` & `rime_sdk-2.8.0rc0/rime_sdk/internal/swagger_utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/internal/test_helpers.py` & `rime_sdk-2.8.0rc0/rime_sdk/internal/test_helpers.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/internal/throttle_queue.py` & `rime_sdk-2.8.0rc0/rime_sdk/internal/throttle_queue.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/internal/utils.py` & `rime_sdk-2.8.0rc0/rime_sdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/job.py` & `rime_sdk-2.8.0rc0/rime_sdk/job.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/monitor.py` & `rime_sdk-2.8.0rc0/rime_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/project.py` & `rime_sdk-2.8.0rc0/rime_sdk/project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/registry.py` & `rime_sdk-2.8.0rc0/rime_sdk/registry.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/schedule.py` & `rime_sdk-2.8.0rc0/rime_sdk/schedule.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/__init__.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/__init__.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/agent_manager_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/agent_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/config_validator_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/config_validator_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/customer_managed_key_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/data_collector_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/data_collector_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/detection_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/detection_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/feature_flag_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/feature_flag_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/file_scanning_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/file_scanning_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/file_upload_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/file_upload_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/firewall_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/firewall_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/firewall_instance_manager_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/firewall_service_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/firewall_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/generative_model_testing_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/image_registry_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/image_registry_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/integration_service_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/integration_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/job_reader_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/job_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/model_card_service_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/model_card_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/model_testing_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/model_testing_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/monitor_service_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/monitor_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/notification_setting_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/notification_setting_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/project_service_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/project_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/registry_service_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/registry_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/results_reader_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/results_reader_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/rime_info_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/rime_info_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/schedule_service_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/schedule_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/user_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/user_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/validation_service_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/validation_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api/workspace_service_api.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api/workspace_service_api.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/api_client.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/configuration.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/__init__.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/agent_id_uuid_upgrade_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_category_test_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_subset_test_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/artifact_identifier_test_case_metric_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/config_generation_category_config_generation_service_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/config_generation_profiling_config_generation_service_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/config_generation_test_suite_config_generation_service_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/configvalidator_config_type_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/continuoustests_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_aws_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_azure_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_gcp_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/create_agent_request_local_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/create_firewall_request_scheduled_ct_parameters.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/crossplanetask_cross_plane_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/custom_image_pull_secret.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/custom_metric_custom_metric_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/customermanagedkey_customer_managed_key_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_provider.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/customermanagedkey_key_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/custommonitors_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/data_data_stream_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/data_params_feature_intersection.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/data_params_ranking_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/data_profiling_column_type_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/data_profiling_feature_relationship_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/datacollector_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/datacollector_datapoint_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/dataset_ct_dataset_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/dataset_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/dataset_dataset.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/dataset_dataset.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/dataset_id_prediction_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/datastream_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/detection_detection_event.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/detection_detection_event.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/detection_event_detail.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/detection_event_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/detection_event_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/detection_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/detection_metric_degradation_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/detection_resolution.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/detection_resolution.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/detection_security_event_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/difference_from_target_difference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/difference_from_target_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/digest_config_digest_frequency.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/featureflags_customer_name_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_file_scan_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_file_security_report.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_package_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/filescanning_repo_metadata_license.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/fileserver_check_object_exists_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/fileserver_delete_object_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/fileserver_get_read_object_presigned_link_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/fileserver_get_upload_object_presigned_link_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/fileserver_list_objects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/firewall_firewall.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/firewall_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/firewall_firewall_firewall_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/firewall_latest_run_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/firewall_scheduled_ct_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/firewall_test_category_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/firewallinstance_firewall_instance_firewall_instance_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/flagged_substring_request_body_component.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generative_testing_result_example.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generative_testing_result_standard_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generative_testing_result_standard_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_create_firewall_instance_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_custom_pii_entity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_denial_of_service_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_action.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_instance_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_rule_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_firewall_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_flagged_substring.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_effective_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_get_firewall_instance_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_individual_rules_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_language_detection_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_list_firewall_instances_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_list_firewall_instances_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_off_topic_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_detection_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_pii_entity_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_prompt_injection_v2_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_output.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_rule_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_toxicity_detection_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_unknown_external_source_rule_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_update_firewall_instance_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativefirewall_validate_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_generative_testing_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_get_generative_model_test_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_model_connection_spec.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_model_connection_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_objective_sub_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/generativetesting_start_generative_model_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/googlerpc_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/heartbeat_agent_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/image_reference_reference_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/integration_integration_level.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_schema.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/integration_integration_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/integration_integration_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/integration_variable_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/integrations_integration_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/job_data_continuous_incremental_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/job_data_generative_model_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/job_data_scan.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/job_data_scan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/job_data_stress_test.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/language_detection_details_language_substring.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_agents_request_list_agents_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_datasets_request_datasets_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_file_scan_results_request_file_scan_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_images_request_pip_library_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_aggregated_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metric_without_subsets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_feature_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_metric_identifiers_response_subset_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_models_request_model_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_monitors_request_filter.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_notifications_request_list_notifications_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_prediction_sets_request_prediction_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_summary_tests_request_list_summary_tests_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/list_test_cases_request_list_test_cases_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_package_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_pip_library.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_pip_requirement.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/managed_image_role_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/model_model.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/model_model.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/modelcards_model_card_model_card_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_aggregation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_aggregation_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_anomaly_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_artifact_identifier.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_difference_from_target.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_excluded_transforms.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_metric_degradation_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_monitor.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_monitor_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_threshold.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_threshold.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_threshold_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitor_transform.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitor_transform.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitoring_config_alert_level.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/monitors_monitor_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_digest_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_digest_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_job_action_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_monitoring_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_notification.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_notification_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_notification_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_object_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_object_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notification_webhook_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/notifsettings_notification_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/pii_detection_details_flagged_entity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/predictions_model_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_activate_schedule_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_add_users_to_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_create_project_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_create_project_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_create_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_create_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_deactivate_schedule_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_delete_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_get_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_get_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_get_project_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_get_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_id_uuid_dataset_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_id_uuid_model_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_list_projects_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_list_projects_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_list_users_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_owner_details.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_project.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_project.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_project_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_project_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_project_with_details.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_project_with_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_remove_user_from_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_schedule_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_schedule_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_update_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_update_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_update_user_of_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/project_update_workspace_roles_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/projects_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/protobuf_any.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/protobuf_null_value.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_connection_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_connection_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_collector_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_file_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_data_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_loading_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_data_params.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_data_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_data_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_databricks_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_generative_language_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_hugging_face_data_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_hugging_face_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_metadata.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_model_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_model_path_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_open_ai_chat_completion_model_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_pred_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_pred_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_prediction_params.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registry_validity_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registry_validity_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/registryprediction_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rename_test_run_id_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/repo_metadata_reputation.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/resetpassword_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_actor_role.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_actor_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_add_users_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_agent.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent_desired_state.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_agent_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_agent_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_api_token_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_attack_objective.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_cancel_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_category_metric.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_category_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_category_test_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_config_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_config_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_configure_integration_request_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_configure_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_continuous_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_continuous_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_api_token_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_api_token_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_firewall_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_image_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_integration_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_model_card_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_notification_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_schedule_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_user_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_create_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_custom_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_delete_uploaded_file_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_detailed_upgrade_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_ensure_image_existence_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_failing_row.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_failing_row.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_failing_rows_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_feature_flags.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_feature_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_feature_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_float_list.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_float_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_customer_managed_key_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_file_upload_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_enabled_feature_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_feature_flag_jwt_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_file_scan_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_image_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_job_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_key_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_limit_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_directory_upload_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_monitor_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_project_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_rime_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_test_run_id_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_time_series_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_upgrade_for_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_url_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_validate_dataset_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_validate_model_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_validate_predictions_task_status_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_get_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_heartbeat_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_image_reference.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_image_reference.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_int_list.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_int_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_integration_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_integration_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_job_data.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_data.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_metadata.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_job_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_job_view.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_job_view.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_language.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_language.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_license_feature.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_license_feature.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_license_limit.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_license_limit.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_limit_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_limit_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_limit_status_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_agents_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_api_tokens_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_current_user_roles_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_datasets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_detection_events_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_enabled_features_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_file_scan_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_images_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_images_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_jobs_for_project_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_metric_identifiers_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_model_cards_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_models_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_monitors_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_notifications_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_prediction_sets_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_project_tags_in_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_uploaded_file_urls_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_users_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspace_integrations_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_list_workspaces_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_long_description_tab.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_managed_image.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_managed_image_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_model_card.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_model_task.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_task.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_model_with_owner_details.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_monitor_data_point.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_named_double.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_named_double.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_order.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_order.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_parent_role_subject_role_pair.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_data_stream_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_external_agent_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_internal_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_register_prediction_set_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_remove_user_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_reset_password_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_resolve_detection_event_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_ri_email_recipient.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_ri_plan.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_safe_url.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_safe_url.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_search_spec.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_search_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_send_ri_email_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_severity.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_severity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_severity_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_sort_spec.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_continuous_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_file_scan_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_stress_test_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_dataset_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_model_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_start_validate_predictions_task_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_predictions_request_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_store_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_str_list.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_str_list.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_stress_test_job_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_subject_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_subject_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_suggestion.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_suggestion.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_sync_image_tag_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_table_column.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_table_column.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_table_column_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_case_monitor_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_case_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_metric.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_metric_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_run_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_task_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_test_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_test_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_time_interval.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_time_interval.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_token_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_token_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_toxicity_threat_category.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_build_info_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_build_info_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_firewall_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_integration_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_model_card_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_monitor_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_notification_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_schedule_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_upgrade_status_for_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_user_of_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_user_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_update_workspace_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_upgrade_agent_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_upgrade_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_upsert_feature_flags_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_detail_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_user_role.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_with_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_user_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_uuid.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_uuid.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_validate_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_workspace.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rime_workspace_write_mask.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/rischemaintegration_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/riskscore_risk_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/riskscore_risk_score.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/role_users_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/role_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/role_workspace_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/role_workspace_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_custom_image_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_resource_request.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/runtimeinfo_run_time_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_activate_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schedule_id_uuid_deactivate_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schedule_schedule.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schedule_schedule.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schedules_schedule_schedule_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schemadatacollector_prediction.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schemafilescanning_package_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schemaintegration_integration_variable.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schemamonitor_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/schemanotification_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/schemanotification_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/security_event_details_flagged_datapoint.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/security_event_details_security_event_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/statedb_archived_job_logs.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/statedb_job_status.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/statedb_job_status.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_datapoints_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_latest_logs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/stream_result_of_rime_get_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/stresstests_project_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/test_run_metrics_category_summary_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/test_run_metrics_model_perf_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/test_run_progress_test_batch_progress.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_annotated_test_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_custom_metric.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_data_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_model_profiling.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_profiling_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_ref_eval_datasets.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_category_type.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_run_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_run_incremental_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_sensitivity.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrun_test_suite_config.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_batch_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_category_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_feature_result_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_config_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_get_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_batch_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_feature_results_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_monitor_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_summary_tests_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_cases_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_request_query.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_test_runs_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_list_validation_categories_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_rename_test_run_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_result_summary_counts.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_batch_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_case.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_case_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_feature_result_display.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/testrunresult_test_run_metrics.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/user_favorite_projects.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/user_private_info.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/user_private_info.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/user_role.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/user_role.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/user_user_detail.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/user_user_detail.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/users_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/users_user_user_id_uuid_body1.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1betaintegrationsintegration_id_uuid_integration.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1betamodelcardsmodel_card_model_card_id_uuid_model_card.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1betamonitorsmonitor_id_uuid_monitor.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1firewallfirewall_firewall_id_uuid_firewall.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1notifsettingsnotification_id_uuid_notification.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1projectsproject_id_uuidroleusersuser_user_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1usersuser_id_uuid_user.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/v1workspaceworkspace_workspace_id_uuid_workspace.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/validate_firewall_instance_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/validate_request_input.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/validate_request_input.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/validate_request_output.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/validate_request_output.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/validation_validate_dataset_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/validation_validate_model_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/validation_validate_predictions_response.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/workspace_id_uuid_users_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/models/workspace_workspace_workspace_id_uuid_body.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/swagger/swagger_client/rest.py` & `rime_sdk-2.8.0rc0/rime_sdk/swagger/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/test_batch.py` & `rime_sdk-2.8.0rc0/rime_sdk/test_batch.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk/test_run.py` & `rime_sdk-2.8.0rc0/rime_sdk/test_run.py`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/rime_sdk.egg-info/PKG-INFO` & `rime_sdk-2.8.0rc0/rime_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rime-sdk
-Version: 2.7.1
+Version: 2.8.0rc0
 Summary: Package to programmatically access a RIME deployment
 Home-page: UNKNOWN
 License: OSI Approved :: Apache Software License
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rime_sdk-2.7.1/rime_sdk.egg-info/SOURCES.txt` & `rime_sdk-2.8.0rc0/rime_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rime_sdk-2.7.1/setup.py` & `rime_sdk-2.8.0rc0/setup.py`

 * *Files identical despite different names*

