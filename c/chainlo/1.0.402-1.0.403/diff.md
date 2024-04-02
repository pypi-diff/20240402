# Comparing `tmp/chainlo-1.0.402.tar.gz` & `tmp/chainlo-1.0.403.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlo-1.0.402.tar", max compression
+gzip compressed data, was "chainlo-1.0.403.tar", max compression
```

## Comparing `chainlo-1.0.402.tar` & `chainlo-1.0.403.tar`

### file list

```diff
@@ -1,187 +1,187 @@
--rw-r--r--   0        0        0        0 2024-03-28 12:59:00.277858 chainlo-1.0.402/README.md
--rw-r--r--   0        0        0     9667 2024-03-28 12:59:00.278103 chainlo-1.0.402/chainlo/__init__.py
--rw-r--r--   0        0        0       87 2024-03-28 12:59:00.278241 chainlo-1.0.402/chainlo/__main__.py
--rw-r--r--   0        0        0     1410 2024-03-28 12:59:00.278372 chainlo-1.0.402/chainlo/action.py
--rw-r--r--   0        0        0    26017 2024-03-29 15:38:21.217731 chainlo-1.0.402/chainlo/agenta_cli/README.md
--rw-r--r--   0        0        0      493 2024-03-29 15:38:21.221195 chainlo-1.0.402/chainlo/agenta_cli/agenta/__init__.py
--rw-r--r--   0        0        0      494 2024-04-02 12:31:57.078250 chainlo-1.0.402/chainlo/agenta_cli/agenta/cli/evaluation_commands.py
--rw-r--r--   0        0        0     6239 2024-04-02 12:26:04.291397 chainlo-1.0.402/chainlo/agenta_cli/agenta/cli/helper.py
--rw-r--r--   0        0        0     9535 2024-04-02 12:37:37.788934 chainlo-1.0.402/chainlo/agenta_cli/agenta/cli/main.py
--rw-r--r--   0        0        0     1337 2024-04-02 12:31:07.654475 chainlo-1.0.402/chainlo/agenta_cli/agenta/cli/telemetry.py
--rw-r--r--   0        0        0    16978 2024-04-02 12:30:50.209025 chainlo-1.0.402/chainlo/agenta_cli/agenta/cli/variant_commands.py
--rw-r--r--   0        0        0     1313 2024-04-02 12:26:21.238617 chainlo-1.0.402/chainlo/agenta_cli/agenta/cli/variant_configs.py
--rw-r--r--   0        0        0     2756 2024-03-29 15:38:21.228131 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/Readme.md
--rw-r--r--   0        0        0        0 2024-03-29 15:38:21.228597 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/__init__.py
--rw-r--r--   0        0        0     2509 2024-04-02 12:31:46.026778 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/api.py
--rw-r--r--   0        0        0      623 2024-03-29 15:38:21.229938 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/api_models.py
--rw-r--r--   0        0        0     2666 2024-03-29 15:38:21.231650 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/__init__.py
--rw-r--r--   0        0        0   259068 2024-03-29 15:38:21.233513 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/client.py
--rw-r--r--   0        0        0      519 2024-03-29 15:38:21.234601 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/core/__init__.py
--rw-r--r--   0        0        0      440 2024-03-29 15:38:21.235211 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/core/api_error.py
--rw-r--r--   0        0        0      972 2024-03-29 15:38:21.235881 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/core/client_wrapper.py
--rw-r--r--   0        0        0     1069 2024-03-29 15:38:21.236559 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/core/datetime_utils.py
--rw-r--r--   0        0        0     3825 2024-03-29 15:38:21.237211 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-29 15:38:21.237761 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      170 2024-03-29 15:38:21.239005 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-03-29 15:38:21.239732 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     4008 2024-03-29 15:38:21.241610 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/__init__.py
--rw-r--r--   0        0        0      211 2024-03-29 15:38:21.242318 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/add_variant_from_base_and_config_response.py
--rw-r--r--   0        0        0     1083 2024-03-29 15:38:21.243231 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/aggregated_result.py
--rw-r--r--   0        0        0      974 2024-03-29 15:38:21.243870 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/app.py
--rw-r--r--   0        0        0     1268 2024-03-29 15:38:21.244420 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output.py
--rw-r--r--   0        0        0     1394 2024-03-29 15:38:21.245000 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output_extended.py
--rw-r--r--   0        0        0     1075 2024-03-29 15:38:21.245538 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/app_variant_revision.py
--rw-r--r--   0        0        0      983 2024-03-29 15:38:21.246051 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/base_output.py
--rw-r--r--   0        0        0     1061 2024-03-29 15:38:21.246493 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/body_import_testset.py
--rw-r--r--   0        0        0     1028 2024-03-29 15:38:21.246936 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/config_db.py
--rw-r--r--   0        0        0      182 2024-03-29 15:38:21.247467 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/container_templates_response.py
--rw-r--r--   0        0        0      986 2024-03-29 15:38:21.248085 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/create_app_output.py
--rw-r--r--   0        0        0      991 2024-03-29 15:38:21.248628 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/delete_evaluation.py
--rw-r--r--   0        0        0      986 2024-03-29 15:38:21.249104 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/docker_env_vars.py
--rw-r--r--   0        0        0     1176 2024-03-29 15:38:21.249534 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/environment_output.py
--rw-r--r--   0        0        0     1376 2024-03-29 15:38:21.249971 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation.py
--rw-r--r--   0        0        0     1497 2024-03-29 15:38:21.250499 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario.py
--rw-r--r--   0        0        0     1027 2024-03-29 15:38:21.251140 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_input.py
--rw-r--r--   0        0        0     1014 2024-03-29 15:38:21.251815 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_output.py
--rw-r--r--   0        0        0     1033 2024-03-29 15:38:21.252247 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_result.py
--rw-r--r--   0        0        0     1102 2024-03-29 15:38:21.252717 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_status_enum.py
--rw-r--r--   0        0        0      644 2024-03-29 15:38:21.253129 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_type.py
--rw-r--r--   0        0        0      971 2024-03-29 15:38:21.253545 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_webhook.py
--rw-r--r--   0        0        0     1046 2024-03-29 15:38:21.254100 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluator.py
--rw-r--r--   0        0        0     1124 2024-03-29 15:38:21.254598 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluator_config.py
--rw-r--r--   0        0        0     1136 2024-03-29 15:38:21.255072 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/feedback.py
--rw-r--r--   0        0        0     1063 2024-03-29 15:38:21.255549 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/get_config_reponse.py
--rw-r--r--   0        0        0     1060 2024-03-29 15:38:21.256152 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/http_validation_error.py
--rw-r--r--   0        0        0     1305 2024-03-29 15:38:21.256706 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation.py
--rw-r--r--   0        0        0     1580 2024-03-29 15:38:21.257151 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario.py
--rw-r--r--   0        0        0     1006 2024-03-29 15:38:21.257665 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_input.py
--rw-r--r--   0        0        0     1010 2024-03-29 15:38:21.258161 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_output.py
--rw-r--r--   0        0        0      134 2024-03-29 15:38:21.258634 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_score.py
--rw-r--r--   0        0        0      140 2024-03-29 15:38:21.259047 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_update_score.py
--rw-r--r--   0        0        0     1048 2024-03-29 15:38:21.259555 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/image.py
--rw-r--r--   0        0        0      965 2024-03-29 15:38:21.260000 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/invite_request.py
--rw-r--r--   0        0        0     1095 2024-03-29 15:38:21.260474 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/list_api_keys_output.py
--rw-r--r--   0        0        0     1045 2024-03-29 15:38:21.260976 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/llm_run_rate_limit.py
--rw-r--r--   0        0        0     1009 2024-03-29 15:38:21.261472 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/new_testset.py
--rw-r--r--   0        0        0     1181 2024-03-29 15:38:21.261911 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/organization.py
--rw-r--r--   0        0        0      981 2024-03-29 15:38:21.262371 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/organization_output.py
--rw-r--r--   0        0        0      996 2024-03-29 15:38:21.262822 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/result.py
--rw-r--r--   0        0        0     1117 2024-03-29 15:38:21.263320 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/simple_evaluation_output.py
--rw-r--r--   0        0        0     1546 2024-03-29 15:38:21.263903 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/span.py
--rw-r--r--   0        0        0     1037 2024-03-29 15:38:21.264526 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/template.py
--rw-r--r--   0        0        0     1189 2024-03-29 15:38:21.265123 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/template_image_info.py
--rw-r--r--   0        0        0     1088 2024-03-29 15:38:21.265659 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/test_set_output_response.py
--rw-r--r--   0        0        0     1004 2024-03-29 15:38:21.266314 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/test_set_simple_response.py
--rw-r--r--   0        0        0     1353 2024-03-29 15:38:21.266828 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/trace.py
--rw-r--r--   0        0        0      953 2024-03-29 15:38:21.267207 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/uri.py
--rw-r--r--   0        0        0     1086 2024-03-29 15:38:21.267670 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-03-29 15:38:21.268112 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1031 2024-03-29 15:38:21.268517 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/variant_action.py
--rw-r--r--   0        0        0      511 2024-03-29 15:38:21.268961 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/variant_action_enum.py
--rw-r--r--   0        0        0    19668 2024-04-02 12:32:12.753248 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/client.py
--rw-r--r--   0        0        0       94 2024-03-29 15:38:21.269971 chainlo-1.0.402/chainlo/agenta_cli/agenta/client/exceptions.py
--rw-r--r--   0        0        0      732 2024-03-29 15:38:21.270473 chainlo-1.0.402/chainlo/agenta_cli/agenta/config.py
--rw-r--r--   0        0        0      223 2024-03-29 15:38:21.270908 chainlo-1.0.402/chainlo/agenta_cli/agenta/config.toml
--rw-r--r--   0        0        0      317 2024-03-29 15:38:21.272321 chainlo-1.0.402/chainlo/agenta_cli/agenta/docker/docker-assets/Dockerfile.cloud.template
--rw-r--r--   0        0        0      241 2024-03-29 15:38:21.272700 chainlo-1.0.402/chainlo/agenta_cli/agenta/docker/docker-assets/Dockerfile.template
--rw-r--r--   0        0        0      102 2024-03-29 15:38:21.273161 chainlo-1.0.402/chainlo/agenta_cli/agenta/docker/docker-assets/README.md
--rwxr-xr-x   0        0        0       74 2024-03-29 15:38:21.273685 chainlo-1.0.402/chainlo/agenta_cli/agenta/docker/docker-assets/entrypoint.sh
--rw-r--r--   0        0        0      102 2024-04-02 15:18:44.554577 chainlo-1.0.402/chainlo/agenta_cli/agenta/docker/docker-assets/lambda_function.py
--rw-r--r--   0        0        0      270 2024-04-02 15:18:34.213398 chainlo-1.0.402/chainlo/agenta_cli/agenta/docker/docker-assets/main.py
--rw-r--r--   0        0        0     3562 2024-04-02 12:31:19.880389 chainlo-1.0.402/chainlo/agenta_cli/agenta/docker/docker_utils.py
--rw-r--r--   0        0        0      565 2024-03-29 15:38:21.275737 chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/__init__.py
--rw-r--r--   0        0        0    15506 2024-04-02 12:23:48.754730 chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/agenta_decorator.py
--rw-r--r--   0        0        0     8065 2024-04-02 12:24:41.742653 chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/agenta_init.py
--rw-r--r--   0        0        0      901 2024-03-29 15:38:21.277386 chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/context.py
--rw-r--r--   0        0        0      269 2024-03-29 15:38:21.277737 chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/router.py
--rw-r--r--   0        0        0     4658 2024-03-29 15:38:21.278086 chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/types.py
--rw-r--r--   0        0        0      380 2024-04-02 12:25:03.766003 chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/utils/globals.py
--rw-r--r--   0        0        0     5877 2024-03-29 15:38:21.279477 chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/utils/helper/openai_cost.py
--rw-r--r--   0        0        0     1278 2024-03-29 15:38:21.279853 chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/utils/preinit.py
--rw-r--r--   0        0        0      308 2024-03-29 15:38:21.281309 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/compose_email/README.md
--rw-r--r--   0        0        0     2384 2024-03-29 15:38:21.281686 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/compose_email/app.py
--rw-r--r--   0        0        0       70 2024-03-29 15:38:21.282049 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/compose_email/env.example
--rw-r--r--   0        0        0       23 2024-03-29 15:38:21.282449 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/compose_email/requirements.txt
--rw-r--r--   0        0        0       47 2024-03-29 15:38:21.282787 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/compose_email/template.toml
--rw-r--r--   0        0        0      308 2024-03-29 15:38:21.283477 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/extract_data_to_json/README.md
--rw-r--r--   0        0        0     1320 2024-03-29 15:38:21.283896 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/extract_data_to_json/app.py
--rw-r--r--   0        0        0       70 2024-03-29 15:38:21.284271 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/extract_data_to_json/env.example
--rw-r--r--   0        0        0       23 2024-03-29 15:38:21.284661 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/extract_data_to_json/requirements.txt
--rw-r--r--   0        0        0       60 2024-03-29 15:38:21.285035 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/extract_data_to_json/template.toml
--rw-r--r--   0        0        0      308 2024-03-29 15:38:21.285928 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/simple_prompt/README.md
--rw-r--r--   0        0        0      665 2024-04-02 15:20:39.242968 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/simple_prompt/app.py
--rw-r--r--   0        0        0       70 2024-03-29 15:38:21.286665 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/simple_prompt/env.example
--rw-r--r--   0        0        0       24 2024-04-02 15:18:01.855024 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/simple_prompt/requirements.txt
--rw-r--r--   0        0        0       60 2024-03-29 15:38:21.287420 chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/simple_prompt/template.toml
--rw-r--r--   0        0        0     1078 2024-04-01 00:20:31.300954 chainlo-1.0.402/chainlo/agenta_cli/pyproject.toml-ex
--rw-r--r--   0        0        0        0 2024-03-29 15:38:21.289373 chainlo-1.0.402/chainlo/agenta_cli/requirements.txt
--rw-r--r--   0        0        0      580 2024-03-29 15:38:21.290495 chainlo-1.0.402/chainlo/agenta_cli/tests/example_projects/simple_langchain/app.py
--rw-r--r--   0        0        0       31 2024-03-29 15:38:21.290969 chainlo-1.0.402/chainlo/agenta_cli/tests/example_projects/simple_langchain/requirements.txt
--rw-r--r--   0        0        0      411 2024-03-29 15:38:21.292434 chainlo-1.0.402/chainlo/agenta_cli/tests/example_projects/test2/README.md
--rw-r--r--   0        0        0     3294 2024-03-29 15:38:21.293249 chainlo-1.0.402/chainlo/agenta_cli/tests/example_projects/test2/agenta.py
--rw-r--r--   0        0        0      580 2024-03-29 15:38:21.294048 chainlo-1.0.402/chainlo/agenta_cli/tests/example_projects/test2/app.py
--rw-r--r--   0        0        0       51 2024-03-29 15:38:21.294746 chainlo-1.0.402/chainlo/agenta_cli/tests/example_projects/test2/config.toml
--rw-r--r--   0        0        0      187 2024-03-29 15:38:21.295361 chainlo-1.0.402/chainlo/agenta_cli/tests/example_projects/test2/main.py
--rw-r--r--   0        0        0       31 2024-03-29 15:38:21.295991 chainlo-1.0.402/chainlo/agenta_cli/tests/example_projects/test2/requirements.txt
--rw-r--r--   0        0        0     2681 2024-03-28 12:59:00.278537 chainlo-1.0.402/chainlo/auth.py
--rw-r--r--   0        0        0     1361 2024-03-28 12:59:00.278680 chainlo-1.0.402/chainlo/cache.py
--rw-r--r--   0        0        0      877 2024-03-28 12:59:00.278813 chainlo-1.0.402/chainlo/chat_settings.py
--rw-r--r--   0        0        0     4786 2024-03-30 14:01:40.889613 chainlo-1.0.402/chainlo/cli/__init__.py
--rw-r--r--   0        0        0      717 2024-03-28 12:59:00.279324 chainlo-1.0.402/chainlo/cli/utils.py
--rw-r--r--   0        0        0    13465 2024-03-28 12:59:00.279531 chainlo-1.0.402/chainlo/config.py
--rw-r--r--   0        0        0     2476 2024-03-28 12:59:00.279723 chainlo-1.0.402/chainlo/context.py
--rw-r--r--   0        0        0     8887 2024-04-02 13:46:34.758455 chainlo-1.0.402/chainlo/copilot/dist/assets/logo_dark-2a3cf740.svg
--rw-r--r--   0        0        0     8889 2024-04-02 13:46:34.756788 chainlo-1.0.402/chainlo/copilot/dist/assets/logo_light-b078e7bc.svg
--rw-r--r--   0        0        0  7013566 2024-04-02 13:46:34.752958 chainlo-1.0.402/chainlo/copilot/dist/index.js
--rw-r--r--   0        0        0    14724 2024-03-28 12:59:00.279971 chainlo-1.0.402/chainlo/data/__init__.py
--rw-r--r--   0        0        0      461 2024-03-28 12:59:00.280107 chainlo-1.0.402/chainlo/data/acl.py
--rw-r--r--   0        0        0    10162 2024-03-28 12:59:00.280281 chainlo-1.0.402/chainlo/element.py
--rw-r--r--   0        0        0    12178 2024-03-28 12:59:00.280461 chainlo-1.0.402/chainlo/emitter.py
--rw-r--r--   0        0        0  3071160 2024-04-02 13:46:34.734588 chainlo-1.0.402/chainlo/frontend/dist/assets/index-7bc2ef31.js
--rw-r--r--   0        0        0     6605 2024-04-02 13:46:34.736982 chainlo-1.0.402/chainlo/frontend/dist/assets/index-d088547c.css
--rw-r--r--   0        0        0     8887 2024-04-02 13:46:34.736163 chainlo-1.0.402/chainlo/frontend/dist/assets/logo_dark-2a3cf740.svg
--rw-r--r--   0        0        0     8889 2024-04-02 13:46:34.735648 chainlo-1.0.402/chainlo/frontend/dist/assets/logo_light-b078e7bc.svg
--rw-r--r--   0        0        0  3763471 2024-04-02 13:46:34.739499 chainlo-1.0.402/chainlo/frontend/dist/assets/react-plotly-70086d41.js
--rw-r--r--   0        0        0     6455 2024-04-02 13:46:34.741377 chainlo-1.0.402/chainlo/frontend/dist/favicon.svg
--rw-r--r--   0        0        0     1005 2024-04-02 13:46:34.731871 chainlo-1.0.402/chainlo/frontend/dist/index.html
--rw-r--r--   0        0        0      217 2024-03-28 12:59:00.280774 chainlo-1.0.402/chainlo/haystack/__init__.py
--rw-r--r--   0        0        0     5209 2024-03-28 12:59:00.280941 chainlo-1.0.402/chainlo/haystack/callbacks.py
--rw-r--r--   0        0        0     3018 2024-03-30 14:45:46.436609 chainlo-1.0.402/chainlo/hello.py
--rw-r--r--   0        0        0     4880 2024-03-28 12:59:00.281252 chainlo-1.0.402/chainlo/input_widget.py
--rw-r--r--   0        0        0      217 2024-03-28 12:59:00.281449 chainlo-1.0.402/chainlo/langchain/__init__.py
--rw-r--r--   0        0        0    20521 2024-03-28 12:59:00.281698 chainlo-1.0.402/chainlo/langchain/callbacks.py
--rw-r--r--   0        0        0      817 2024-03-28 12:59:00.281944 chainlo-1.0.402/chainlo/langflow/__init__.py
--rw-r--r--   0        0        0      227 2024-03-28 12:59:00.282266 chainlo-1.0.402/chainlo/llama_index/__init__.py
--rw-r--r--   0        0        0     6078 2024-03-28 12:59:00.282445 chainlo-1.0.402/chainlo/llama_index/callbacks.py
--rw-r--r--   0        0        0      373 2024-03-28 12:59:00.282615 chainlo-1.0.402/chainlo/logger.py
--rw-r--r--   0        0        0     2025 2024-03-28 12:59:00.282790 chainlo-1.0.402/chainlo/markdown.py
--rw-r--r--   0        0        0    17683 2024-03-28 12:59:00.283051 chainlo-1.0.402/chainlo/message.py
--rw-r--r--   0        0        0    17459 2024-03-28 12:59:00.283259 chainlo-1.0.402/chainlo/oauth_providers.py
--rw-r--r--   0        0        0     2002 2024-03-28 12:59:00.283525 chainlo-1.0.402/chainlo/openai/__init__.py
--rw-r--r--   0        0        0       80 2024-03-28 12:59:00.283801 chainlo-1.0.402/chainlo/playground/__init__.py
--rw-r--r--   0        0        0     1033 2024-03-28 12:59:00.284106 chainlo-1.0.402/chainlo/playground/config.py
--rw-r--r--   0        0        0     3858 2024-03-28 12:59:00.284312 chainlo-1.0.402/chainlo/playground/provider.py
--rw-r--r--   0        0        0      236 2024-03-28 12:59:00.284521 chainlo-1.0.402/chainlo/playground/providers/__init__.py
--rw-r--r--   0        0        0     3495 2024-03-28 12:59:00.284708 chainlo-1.0.402/chainlo/playground/providers/anthropic.py
--rw-r--r--   0        0        0     2130 2024-03-28 12:59:00.284866 chainlo-1.0.402/chainlo/playground/providers/huggingface.py
--rw-r--r--   0        0        0     3103 2024-03-28 12:59:00.285051 chainlo-1.0.402/chainlo/playground/providers/langchain.py
--rw-r--r--   0        0        0    12397 2024-03-28 12:59:00.285216 chainlo-1.0.402/chainlo/playground/providers/openai.py
--rw-r--r--   0        0        0     5084 2024-03-28 12:59:00.285364 chainlo-1.0.402/chainlo/playground/providers/vertexai.py
--rw-r--r--   0        0        0        0 2024-03-28 12:59:00.285429 chainlo-1.0.402/chainlo/py.typed
--rw-r--r--   0        0        0      295 2024-03-28 12:59:00.285564 chainlo-1.0.402/chainlo/secret.py
--rw-r--r--   0        0        0    22602 2024-03-28 12:59:00.285775 chainlo-1.0.402/chainlo/server.py
--rw-r--r--   0        0        0     8844 2024-03-28 12:59:00.285967 chainlo-1.0.402/chainlo/session.py
--rw-r--r--   0        0        0     9846 2024-03-28 12:59:00.286136 chainlo-1.0.402/chainlo/socket.py
--rw-r--r--   0        0        0    12749 2024-03-28 12:59:00.286305 chainlo-1.0.402/chainlo/step.py
--rw-r--r--   0        0        0     1235 2024-03-28 12:59:00.286446 chainlo-1.0.402/chainlo/sync.py
--rw-r--r--   0        0        0     3060 2024-03-28 12:59:00.286585 chainlo-1.0.402/chainlo/telemetry.py
--rw-r--r--   0        0        0     6252 2024-03-28 12:59:00.286806 chainlo-1.0.402/chainlo/translations/de.json
--rw-r--r--   0        0        0     4514 2024-03-28 12:59:00.287261 chainlo-1.0.402/chainlo/translations/en-US.json
--rw-r--r--   0        0        0     4614 2024-03-28 12:59:00.287519 chainlo-1.0.402/chainlo/translations/pt-BR.json
--rw-r--r--   0        0        0     3379 2024-03-28 12:59:00.287730 chainlo-1.0.402/chainlo/types.py
--rw-r--r--   0        0        0      619 2024-03-28 12:59:00.287957 chainlo-1.0.402/chainlo/user.py
--rw-r--r--   0        0        0     1368 2024-03-28 12:59:00.288135 chainlo-1.0.402/chainlo/user_session.py
--rw-r--r--   0        0        0     2571 2024-03-28 12:59:00.288279 chainlo-1.0.402/chainlo/utils.py
--rw-r--r--   0        0        0      196 2024-03-28 12:59:00.288410 chainlo-1.0.402/chainlo/version.py
--rw-r--r--   0        0        0     2361 2024-04-02 15:21:18.504413 chainlo-1.0.402/pyproject.toml
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 chainlo-1.0.402/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-28 12:59:00.277858 chainlo-1.0.403/README.md
+-rw-r--r--   0        0        0     9667 2024-03-28 12:59:00.278103 chainlo-1.0.403/chainlo/__init__.py
+-rw-r--r--   0        0        0       87 2024-03-28 12:59:00.278241 chainlo-1.0.403/chainlo/__main__.py
+-rw-r--r--   0        0        0     1410 2024-03-28 12:59:00.278372 chainlo-1.0.403/chainlo/action.py
+-rw-r--r--   0        0        0    26017 2024-03-29 15:38:21.217731 chainlo-1.0.403/chainlo/agenta_cli/README.md
+-rw-r--r--   0        0        0      493 2024-03-29 15:38:21.221195 chainlo-1.0.403/chainlo/agenta_cli/agenta/__init__.py
+-rw-r--r--   0        0        0      494 2024-04-02 12:31:57.078250 chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/evaluation_commands.py
+-rw-r--r--   0        0        0     6239 2024-04-02 12:26:04.291397 chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/helper.py
+-rw-r--r--   0        0        0     9535 2024-04-02 12:37:37.788934 chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/main.py
+-rw-r--r--   0        0        0     1337 2024-04-02 12:31:07.654475 chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/telemetry.py
+-rw-r--r--   0        0        0    16978 2024-04-02 12:30:50.209025 chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/variant_commands.py
+-rw-r--r--   0        0        0     1313 2024-04-02 12:26:21.238617 chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/variant_configs.py
+-rw-r--r--   0        0        0     2756 2024-03-29 15:38:21.228131 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/Readme.md
+-rw-r--r--   0        0        0        0 2024-03-29 15:38:21.228597 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/__init__.py
+-rw-r--r--   0        0        0     2509 2024-04-02 12:31:46.026778 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/api.py
+-rw-r--r--   0        0        0      623 2024-03-29 15:38:21.229938 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/api_models.py
+-rw-r--r--   0        0        0     2666 2024-03-29 15:38:21.231650 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/__init__.py
+-rw-r--r--   0        0        0   259068 2024-03-29 15:38:21.233513 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/client.py
+-rw-r--r--   0        0        0      519 2024-03-29 15:38:21.234601 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/__init__.py
+-rw-r--r--   0        0        0      440 2024-03-29 15:38:21.235211 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/api_error.py
+-rw-r--r--   0        0        0      972 2024-03-29 15:38:21.235881 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/client_wrapper.py
+-rw-r--r--   0        0        0     1069 2024-03-29 15:38:21.236559 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/datetime_utils.py
+-rw-r--r--   0        0        0     3825 2024-03-29 15:38:21.237211 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-03-29 15:38:21.237761 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      170 2024-03-29 15:38:21.239005 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-03-29 15:38:21.239732 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     4008 2024-03-29 15:38:21.241610 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-29 15:38:21.242318 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/add_variant_from_base_and_config_response.py
+-rw-r--r--   0        0        0     1083 2024-03-29 15:38:21.243231 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/aggregated_result.py
+-rw-r--r--   0        0        0      974 2024-03-29 15:38:21.243870 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app.py
+-rw-r--r--   0        0        0     1268 2024-03-29 15:38:21.244420 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output.py
+-rw-r--r--   0        0        0     1394 2024-03-29 15:38:21.245000 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output_extended.py
+-rw-r--r--   0        0        0     1075 2024-03-29 15:38:21.245538 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app_variant_revision.py
+-rw-r--r--   0        0        0      983 2024-03-29 15:38:21.246051 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/base_output.py
+-rw-r--r--   0        0        0     1061 2024-03-29 15:38:21.246493 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/body_import_testset.py
+-rw-r--r--   0        0        0     1028 2024-03-29 15:38:21.246936 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/config_db.py
+-rw-r--r--   0        0        0      182 2024-03-29 15:38:21.247467 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/container_templates_response.py
+-rw-r--r--   0        0        0      986 2024-03-29 15:38:21.248085 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/create_app_output.py
+-rw-r--r--   0        0        0      991 2024-03-29 15:38:21.248628 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/delete_evaluation.py
+-rw-r--r--   0        0        0      986 2024-03-29 15:38:21.249104 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/docker_env_vars.py
+-rw-r--r--   0        0        0     1176 2024-03-29 15:38:21.249534 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/environment_output.py
+-rw-r--r--   0        0        0     1376 2024-03-29 15:38:21.249971 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation.py
+-rw-r--r--   0        0        0     1497 2024-03-29 15:38:21.250499 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario.py
+-rw-r--r--   0        0        0     1027 2024-03-29 15:38:21.251140 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_input.py
+-rw-r--r--   0        0        0     1014 2024-03-29 15:38:21.251815 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_output.py
+-rw-r--r--   0        0        0     1033 2024-03-29 15:38:21.252247 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_result.py
+-rw-r--r--   0        0        0     1102 2024-03-29 15:38:21.252717 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_status_enum.py
+-rw-r--r--   0        0        0      644 2024-03-29 15:38:21.253129 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_type.py
+-rw-r--r--   0        0        0      971 2024-03-29 15:38:21.253545 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_webhook.py
+-rw-r--r--   0        0        0     1046 2024-03-29 15:38:21.254100 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluator.py
+-rw-r--r--   0        0        0     1124 2024-03-29 15:38:21.254598 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluator_config.py
+-rw-r--r--   0        0        0     1136 2024-03-29 15:38:21.255072 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/feedback.py
+-rw-r--r--   0        0        0     1063 2024-03-29 15:38:21.255549 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/get_config_reponse.py
+-rw-r--r--   0        0        0     1060 2024-03-29 15:38:21.256152 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/http_validation_error.py
+-rw-r--r--   0        0        0     1305 2024-03-29 15:38:21.256706 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation.py
+-rw-r--r--   0        0        0     1580 2024-03-29 15:38:21.257151 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario.py
+-rw-r--r--   0        0        0     1006 2024-03-29 15:38:21.257665 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_input.py
+-rw-r--r--   0        0        0     1010 2024-03-29 15:38:21.258161 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_output.py
+-rw-r--r--   0        0        0      134 2024-03-29 15:38:21.258634 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_score.py
+-rw-r--r--   0        0        0      140 2024-03-29 15:38:21.259047 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_update_score.py
+-rw-r--r--   0        0        0     1048 2024-03-29 15:38:21.259555 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/image.py
+-rw-r--r--   0        0        0      965 2024-03-29 15:38:21.260000 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/invite_request.py
+-rw-r--r--   0        0        0     1095 2024-03-29 15:38:21.260474 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/list_api_keys_output.py
+-rw-r--r--   0        0        0     1045 2024-03-29 15:38:21.260976 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/llm_run_rate_limit.py
+-rw-r--r--   0        0        0     1009 2024-03-29 15:38:21.261472 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/new_testset.py
+-rw-r--r--   0        0        0     1181 2024-03-29 15:38:21.261911 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/organization.py
+-rw-r--r--   0        0        0      981 2024-03-29 15:38:21.262371 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/organization_output.py
+-rw-r--r--   0        0        0      996 2024-03-29 15:38:21.262822 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/result.py
+-rw-r--r--   0        0        0     1117 2024-03-29 15:38:21.263320 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/simple_evaluation_output.py
+-rw-r--r--   0        0        0     1546 2024-03-29 15:38:21.263903 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/span.py
+-rw-r--r--   0        0        0     1037 2024-03-29 15:38:21.264526 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/template.py
+-rw-r--r--   0        0        0     1189 2024-03-29 15:38:21.265123 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/template_image_info.py
+-rw-r--r--   0        0        0     1088 2024-03-29 15:38:21.265659 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/test_set_output_response.py
+-rw-r--r--   0        0        0     1004 2024-03-29 15:38:21.266314 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/test_set_simple_response.py
+-rw-r--r--   0        0        0     1353 2024-03-29 15:38:21.266828 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/trace.py
+-rw-r--r--   0        0        0      953 2024-03-29 15:38:21.267207 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/uri.py
+-rw-r--r--   0        0        0     1086 2024-03-29 15:38:21.267670 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-03-29 15:38:21.268112 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1031 2024-03-29 15:38:21.268517 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/variant_action.py
+-rw-r--r--   0        0        0      511 2024-03-29 15:38:21.268961 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/variant_action_enum.py
+-rw-r--r--   0        0        0    19668 2024-04-02 12:32:12.753248 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/client.py
+-rw-r--r--   0        0        0       94 2024-03-29 15:38:21.269971 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/exceptions.py
+-rw-r--r--   0        0        0      732 2024-03-29 15:38:21.270473 chainlo-1.0.403/chainlo/agenta_cli/agenta/config.py
+-rw-r--r--   0        0        0      223 2024-03-29 15:38:21.270908 chainlo-1.0.403/chainlo/agenta_cli/agenta/config.toml
+-rw-r--r--   0        0        0      317 2024-03-29 15:38:21.272321 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker-assets/Dockerfile.cloud.template
+-rw-r--r--   0        0        0      241 2024-03-29 15:38:21.272700 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker-assets/Dockerfile.template
+-rw-r--r--   0        0        0      102 2024-03-29 15:38:21.273161 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker-assets/README.md
+-rwxr-xr-x   0        0        0       74 2024-03-29 15:38:21.273685 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker-assets/entrypoint.sh
+-rw-r--r--   0        0        0      102 2024-04-02 15:18:44.554577 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker-assets/lambda_function.py
+-rw-r--r--   0        0        0      270 2024-04-02 15:18:34.213398 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker-assets/main.py
+-rw-r--r--   0        0        0     3562 2024-04-02 12:31:19.880389 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker_utils.py
+-rw-r--r--   0        0        0      565 2024-03-29 15:38:21.275737 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/__init__.py
+-rw-r--r--   0        0        0    15506 2024-04-02 12:23:48.754730 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/agenta_decorator.py
+-rw-r--r--   0        0        0     8065 2024-04-02 12:24:41.742653 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/agenta_init.py
+-rw-r--r--   0        0        0      901 2024-03-29 15:38:21.277386 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/context.py
+-rw-r--r--   0        0        0      269 2024-03-29 15:38:21.277737 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/router.py
+-rw-r--r--   0        0        0     4658 2024-03-29 15:38:21.278086 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/types.py
+-rw-r--r--   0        0        0      380 2024-04-02 12:25:03.766003 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/utils/globals.py
+-rw-r--r--   0        0        0     5877 2024-03-29 15:38:21.279477 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/utils/helper/openai_cost.py
+-rw-r--r--   0        0        0     1278 2024-03-29 15:38:21.279853 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/utils/preinit.py
+-rw-r--r--   0        0        0      308 2024-03-29 15:38:21.281309 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/compose_email/README.md
+-rw-r--r--   0        0        0     2384 2024-03-29 15:38:21.281686 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/compose_email/app.py
+-rw-r--r--   0        0        0       70 2024-03-29 15:38:21.282049 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/compose_email/env.example
+-rw-r--r--   0        0        0       23 2024-03-29 15:38:21.282449 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/compose_email/requirements.txt
+-rw-r--r--   0        0        0       47 2024-03-29 15:38:21.282787 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/compose_email/template.toml
+-rw-r--r--   0        0        0      308 2024-03-29 15:38:21.283477 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/extract_data_to_json/README.md
+-rw-r--r--   0        0        0     1320 2024-03-29 15:38:21.283896 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/extract_data_to_json/app.py
+-rw-r--r--   0        0        0       70 2024-03-29 15:38:21.284271 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/extract_data_to_json/env.example
+-rw-r--r--   0        0        0       23 2024-03-29 15:38:21.284661 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/extract_data_to_json/requirements.txt
+-rw-r--r--   0        0        0       60 2024-03-29 15:38:21.285035 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/extract_data_to_json/template.toml
+-rw-r--r--   0        0        0      308 2024-03-29 15:38:21.285928 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/simple_prompt/README.md
+-rw-r--r--   0        0        0      665 2024-04-02 15:20:39.242968 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/simple_prompt/app.py
+-rw-r--r--   0        0        0       70 2024-03-29 15:38:21.286665 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/simple_prompt/env.example
+-rw-r--r--   0        0        0       24 2024-04-02 15:18:01.855024 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/simple_prompt/requirements.txt
+-rw-r--r--   0        0        0       60 2024-03-29 15:38:21.287420 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/simple_prompt/template.toml
+-rw-r--r--   0        0        0     1078 2024-04-01 00:20:31.300954 chainlo-1.0.403/chainlo/agenta_cli/pyproject.toml-ex
+-rw-r--r--   0        0        0        0 2024-03-29 15:38:21.289373 chainlo-1.0.403/chainlo/agenta_cli/requirements.txt
+-rw-r--r--   0        0        0      580 2024-03-29 15:38:21.290495 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/simple_langchain/app.py
+-rw-r--r--   0        0        0       31 2024-03-29 15:38:21.290969 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/simple_langchain/requirements.txt
+-rw-r--r--   0        0        0      411 2024-03-29 15:38:21.292434 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/README.md
+-rw-r--r--   0        0        0     3294 2024-03-29 15:38:21.293249 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/agenta.py
+-rw-r--r--   0        0        0      580 2024-03-29 15:38:21.294048 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/app.py
+-rw-r--r--   0        0        0       51 2024-03-29 15:38:21.294746 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/config.toml
+-rw-r--r--   0        0        0      187 2024-03-29 15:38:21.295361 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/main.py
+-rw-r--r--   0        0        0       31 2024-03-29 15:38:21.295991 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/requirements.txt
+-rw-r--r--   0        0        0     2681 2024-03-28 12:59:00.278537 chainlo-1.0.403/chainlo/auth.py
+-rw-r--r--   0        0        0     1361 2024-03-28 12:59:00.278680 chainlo-1.0.403/chainlo/cache.py
+-rw-r--r--   0        0        0      877 2024-03-28 12:59:00.278813 chainlo-1.0.403/chainlo/chat_settings.py
+-rw-r--r--   0        0        0     4786 2024-03-30 14:01:40.889613 chainlo-1.0.403/chainlo/cli/__init__.py
+-rw-r--r--   0        0        0      717 2024-03-28 12:59:00.279324 chainlo-1.0.403/chainlo/cli/utils.py
+-rw-r--r--   0        0        0    13465 2024-03-28 12:59:00.279531 chainlo-1.0.403/chainlo/config.py
+-rw-r--r--   0        0        0     2476 2024-03-28 12:59:00.279723 chainlo-1.0.403/chainlo/context.py
+-rw-r--r--   0        0        0     8887 2024-04-02 13:46:34.758455 chainlo-1.0.403/chainlo/copilot/dist/assets/logo_dark-2a3cf740.svg
+-rw-r--r--   0        0        0     8889 2024-04-02 13:46:34.756788 chainlo-1.0.403/chainlo/copilot/dist/assets/logo_light-b078e7bc.svg
+-rw-r--r--   0        0        0  7013566 2024-04-02 13:46:34.752958 chainlo-1.0.403/chainlo/copilot/dist/index.js
+-rw-r--r--   0        0        0    14724 2024-03-28 12:59:00.279971 chainlo-1.0.403/chainlo/data/__init__.py
+-rw-r--r--   0        0        0      461 2024-03-28 12:59:00.280107 chainlo-1.0.403/chainlo/data/acl.py
+-rw-r--r--   0        0        0    10162 2024-03-28 12:59:00.280281 chainlo-1.0.403/chainlo/element.py
+-rw-r--r--   0        0        0    12178 2024-03-28 12:59:00.280461 chainlo-1.0.403/chainlo/emitter.py
+-rw-r--r--   0        0        0  3071160 2024-04-02 13:46:34.734588 chainlo-1.0.403/chainlo/frontend/dist/assets/index-7bc2ef31.js
+-rw-r--r--   0        0        0     6605 2024-04-02 13:46:34.736982 chainlo-1.0.403/chainlo/frontend/dist/assets/index-d088547c.css
+-rw-r--r--   0        0        0     8887 2024-04-02 13:46:34.736163 chainlo-1.0.403/chainlo/frontend/dist/assets/logo_dark-2a3cf740.svg
+-rw-r--r--   0        0        0     8889 2024-04-02 13:46:34.735648 chainlo-1.0.403/chainlo/frontend/dist/assets/logo_light-b078e7bc.svg
+-rw-r--r--   0        0        0  3763471 2024-04-02 13:46:34.739499 chainlo-1.0.403/chainlo/frontend/dist/assets/react-plotly-70086d41.js
+-rw-r--r--   0        0        0     6455 2024-04-02 13:46:34.741377 chainlo-1.0.403/chainlo/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0     1005 2024-04-02 13:46:34.731871 chainlo-1.0.403/chainlo/frontend/dist/index.html
+-rw-r--r--   0        0        0      217 2024-03-28 12:59:00.280774 chainlo-1.0.403/chainlo/haystack/__init__.py
+-rw-r--r--   0        0        0     5209 2024-03-28 12:59:00.280941 chainlo-1.0.403/chainlo/haystack/callbacks.py
+-rw-r--r--   0        0        0     3018 2024-03-30 14:45:46.436609 chainlo-1.0.403/chainlo/hello.py
+-rw-r--r--   0        0        0     4880 2024-03-28 12:59:00.281252 chainlo-1.0.403/chainlo/input_widget.py
+-rw-r--r--   0        0        0      217 2024-03-28 12:59:00.281449 chainlo-1.0.403/chainlo/langchain/__init__.py
+-rw-r--r--   0        0        0    20521 2024-03-28 12:59:00.281698 chainlo-1.0.403/chainlo/langchain/callbacks.py
+-rw-r--r--   0        0        0      817 2024-03-28 12:59:00.281944 chainlo-1.0.403/chainlo/langflow/__init__.py
+-rw-r--r--   0        0        0      227 2024-03-28 12:59:00.282266 chainlo-1.0.403/chainlo/llama_index/__init__.py
+-rw-r--r--   0        0        0     6078 2024-03-28 12:59:00.282445 chainlo-1.0.403/chainlo/llama_index/callbacks.py
+-rw-r--r--   0        0        0      373 2024-03-28 12:59:00.282615 chainlo-1.0.403/chainlo/logger.py
+-rw-r--r--   0        0        0     2025 2024-03-28 12:59:00.282790 chainlo-1.0.403/chainlo/markdown.py
+-rw-r--r--   0        0        0    17683 2024-03-28 12:59:00.283051 chainlo-1.0.403/chainlo/message.py
+-rw-r--r--   0        0        0    17459 2024-03-28 12:59:00.283259 chainlo-1.0.403/chainlo/oauth_providers.py
+-rw-r--r--   0        0        0     2002 2024-03-28 12:59:00.283525 chainlo-1.0.403/chainlo/openai/__init__.py
+-rw-r--r--   0        0        0       80 2024-03-28 12:59:00.283801 chainlo-1.0.403/chainlo/playground/__init__.py
+-rw-r--r--   0        0        0     1033 2024-03-28 12:59:00.284106 chainlo-1.0.403/chainlo/playground/config.py
+-rw-r--r--   0        0        0     3858 2024-03-28 12:59:00.284312 chainlo-1.0.403/chainlo/playground/provider.py
+-rw-r--r--   0        0        0      236 2024-03-28 12:59:00.284521 chainlo-1.0.403/chainlo/playground/providers/__init__.py
+-rw-r--r--   0        0        0     3495 2024-03-28 12:59:00.284708 chainlo-1.0.403/chainlo/playground/providers/anthropic.py
+-rw-r--r--   0        0        0     2130 2024-03-28 12:59:00.284866 chainlo-1.0.403/chainlo/playground/providers/huggingface.py
+-rw-r--r--   0        0        0     3103 2024-03-28 12:59:00.285051 chainlo-1.0.403/chainlo/playground/providers/langchain.py
+-rw-r--r--   0        0        0    12397 2024-03-28 12:59:00.285216 chainlo-1.0.403/chainlo/playground/providers/openai.py
+-rw-r--r--   0        0        0     5084 2024-03-28 12:59:00.285364 chainlo-1.0.403/chainlo/playground/providers/vertexai.py
+-rw-r--r--   0        0        0        0 2024-03-28 12:59:00.285429 chainlo-1.0.403/chainlo/py.typed
+-rw-r--r--   0        0        0      295 2024-03-28 12:59:00.285564 chainlo-1.0.403/chainlo/secret.py
+-rw-r--r--   0        0        0    22602 2024-03-28 12:59:00.285775 chainlo-1.0.403/chainlo/server.py
+-rw-r--r--   0        0        0     8844 2024-03-28 12:59:00.285967 chainlo-1.0.403/chainlo/session.py
+-rw-r--r--   0        0        0     9846 2024-03-28 12:59:00.286136 chainlo-1.0.403/chainlo/socket.py
+-rw-r--r--   0        0        0    12749 2024-03-28 12:59:00.286305 chainlo-1.0.403/chainlo/step.py
+-rw-r--r--   0        0        0     1235 2024-03-28 12:59:00.286446 chainlo-1.0.403/chainlo/sync.py
+-rw-r--r--   0        0        0     3060 2024-03-28 12:59:00.286585 chainlo-1.0.403/chainlo/telemetry.py
+-rw-r--r--   0        0        0     6252 2024-03-28 12:59:00.286806 chainlo-1.0.403/chainlo/translations/de.json
+-rw-r--r--   0        0        0     4514 2024-03-28 12:59:00.287261 chainlo-1.0.403/chainlo/translations/en-US.json
+-rw-r--r--   0        0        0     4614 2024-03-28 12:59:00.287519 chainlo-1.0.403/chainlo/translations/pt-BR.json
+-rw-r--r--   0        0        0     3379 2024-03-28 12:59:00.287730 chainlo-1.0.403/chainlo/types.py
+-rw-r--r--   0        0        0      619 2024-03-28 12:59:00.287957 chainlo-1.0.403/chainlo/user.py
+-rw-r--r--   0        0        0     1368 2024-03-28 12:59:00.288135 chainlo-1.0.403/chainlo/user_session.py
+-rw-r--r--   0        0        0     2571 2024-03-28 12:59:00.288279 chainlo-1.0.403/chainlo/utils.py
+-rw-r--r--   0        0        0      196 2024-03-28 12:59:00.288410 chainlo-1.0.403/chainlo/version.py
+-rw-r--r--   0        0        0     2361 2024-04-02 15:45:07.032899 chainlo-1.0.403/pyproject.toml
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 chainlo-1.0.403/PKG-INFO
```

### Comparing `chainlo-1.0.402/chainlo/__init__.py` & `chainlo-1.0.403/chainlo/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/action.py` & `chainlo-1.0.403/chainlo/action.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/README.md` & `chainlo-1.0.403/chainlo/agenta_cli/README.md`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/cli/helper.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/helper.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/cli/main.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/main.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/cli/telemetry.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/cli/variant_commands.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/variant_commands.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/cli/variant_configs.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/variant_configs.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/Readme.md` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/Readme.md`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/api.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/api.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/api_models.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/api_models.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/__init__.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/client.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/client.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/core/__init__.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/core/client_wrapper.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/core/datetime_utils.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/core/jsonable_encoder.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/__init__.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/aggregated_result.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/aggregated_result.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/app.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output_extended.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output_extended.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/app_variant_revision.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app_variant_revision.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/base_output.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/base_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/body_import_testset.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/body_import_testset.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/config_db.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/config_db.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/create_app_output.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/create_app_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/delete_evaluation.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/delete_evaluation.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/docker_env_vars.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/docker_env_vars.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/environment_output.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/environment_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_input.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_input.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_output.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_result.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_result.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_status_enum.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_status_enum.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_type.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_type.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluation_webhook.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_webhook.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluator.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluator.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/evaluator_config.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluator_config.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/feedback.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/feedback.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/get_config_reponse.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/get_config_reponse.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/http_validation_error.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_input.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_input.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_output.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/image.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/image.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/invite_request.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/invite_request.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/list_api_keys_output.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/list_api_keys_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/llm_run_rate_limit.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/llm_run_rate_limit.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/new_testset.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/new_testset.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/organization.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/organization.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/organization_output.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/organization_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/result.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/result.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/simple_evaluation_output.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/simple_evaluation_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/span.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/span.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/template.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/template.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/template_image_info.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/template_image_info.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/test_set_output_response.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/test_set_output_response.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/test_set_simple_response.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/test_set_simple_response.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/trace.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/trace.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/uri.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/uri.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/validation_error.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/backend/types/variant_action.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/variant_action.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/client/client.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/client.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/config.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/config.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/docker/docker_utils.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker_utils.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/__init__.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/agenta_decorator.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/agenta_decorator.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/agenta_init.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/agenta_init.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/context.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/context.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/types.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/types.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/utils/helper/openai_cost.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/utils/helper/openai_cost.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/sdk/utils/preinit.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/utils/preinit.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/compose_email/app.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/compose_email/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/extract_data_to_json/app.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/extract_data_to_json/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/agenta/templates/simple_prompt/app.py` & `chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/simple_prompt/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/pyproject.toml-ex` & `chainlo-1.0.403/chainlo/agenta_cli/pyproject.toml-ex`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/tests/example_projects/simple_langchain/app.py` & `chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/simple_langchain/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/tests/example_projects/test2/agenta.py` & `chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/agenta.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/agenta_cli/tests/example_projects/test2/app.py` & `chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/auth.py` & `chainlo-1.0.403/chainlo/auth.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/cache.py` & `chainlo-1.0.403/chainlo/cache.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/chat_settings.py` & `chainlo-1.0.403/chainlo/chat_settings.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/cli/__init__.py` & `chainlo-1.0.403/chainlo/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/cli/utils.py` & `chainlo-1.0.403/chainlo/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/config.py` & `chainlo-1.0.403/chainlo/config.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/context.py` & `chainlo-1.0.403/chainlo/context.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/copilot/dist/assets/logo_dark-2a3cf740.svg` & `chainlo-1.0.403/chainlo/copilot/dist/assets/logo_dark-2a3cf740.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/copilot/dist/assets/logo_light-b078e7bc.svg` & `chainlo-1.0.403/chainlo/copilot/dist/assets/logo_light-b078e7bc.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/copilot/dist/index.js` & `chainlo-1.0.403/chainlo/copilot/dist/index.js`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/data/__init__.py` & `chainlo-1.0.403/chainlo/data/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/element.py` & `chainlo-1.0.403/chainlo/element.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/emitter.py` & `chainlo-1.0.403/chainlo/emitter.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/frontend/dist/assets/index-7bc2ef31.js` & `chainlo-1.0.403/chainlo/frontend/dist/assets/index-7bc2ef31.js`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/frontend/dist/assets/index-d088547c.css` & `chainlo-1.0.403/chainlo/frontend/dist/assets/index-d088547c.css`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/frontend/dist/assets/logo_dark-2a3cf740.svg` & `chainlo-1.0.403/chainlo/frontend/dist/assets/logo_dark-2a3cf740.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/frontend/dist/assets/logo_light-b078e7bc.svg` & `chainlo-1.0.403/chainlo/frontend/dist/assets/logo_light-b078e7bc.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/frontend/dist/assets/react-plotly-70086d41.js` & `chainlo-1.0.403/chainlo/frontend/dist/assets/react-plotly-70086d41.js`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/frontend/dist/favicon.svg` & `chainlo-1.0.403/chainlo/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/frontend/dist/index.html` & `chainlo-1.0.403/chainlo/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/haystack/callbacks.py` & `chainlo-1.0.403/chainlo/haystack/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/hello.py` & `chainlo-1.0.403/chainlo/hello.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/input_widget.py` & `chainlo-1.0.403/chainlo/input_widget.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/langchain/callbacks.py` & `chainlo-1.0.403/chainlo/langchain/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/langflow/__init__.py` & `chainlo-1.0.403/chainlo/langflow/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/llama_index/callbacks.py` & `chainlo-1.0.403/chainlo/llama_index/callbacks.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/markdown.py` & `chainlo-1.0.403/chainlo/markdown.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/message.py` & `chainlo-1.0.403/chainlo/message.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/oauth_providers.py` & `chainlo-1.0.403/chainlo/oauth_providers.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/openai/__init__.py` & `chainlo-1.0.403/chainlo/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/playground/config.py` & `chainlo-1.0.403/chainlo/playground/config.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/playground/provider.py` & `chainlo-1.0.403/chainlo/playground/provider.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/playground/providers/anthropic.py` & `chainlo-1.0.403/chainlo/playground/providers/anthropic.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/playground/providers/huggingface.py` & `chainlo-1.0.403/chainlo/playground/providers/huggingface.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/playground/providers/langchain.py` & `chainlo-1.0.403/chainlo/playground/providers/langchain.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/playground/providers/openai.py` & `chainlo-1.0.403/chainlo/playground/providers/openai.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/playground/providers/vertexai.py` & `chainlo-1.0.403/chainlo/playground/providers/vertexai.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/server.py` & `chainlo-1.0.403/chainlo/server.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/session.py` & `chainlo-1.0.403/chainlo/session.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/socket.py` & `chainlo-1.0.403/chainlo/socket.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/step.py` & `chainlo-1.0.403/chainlo/step.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/sync.py` & `chainlo-1.0.403/chainlo/sync.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/telemetry.py` & `chainlo-1.0.403/chainlo/telemetry.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/translations/de.json` & `chainlo-1.0.403/chainlo/translations/de.json`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/translations/en-US.json` & `chainlo-1.0.403/chainlo/translations/en-US.json`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/translations/pt-BR.json` & `chainlo-1.0.403/chainlo/translations/pt-BR.json`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/types.py` & `chainlo-1.0.403/chainlo/types.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/user.py` & `chainlo-1.0.403/chainlo/user.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/user_session.py` & `chainlo-1.0.403/chainlo/user_session.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/chainlo/utils.py` & `chainlo-1.0.403/chainlo/utils.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.402/pyproject.toml` & `chainlo-1.0.403/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainlo"
-version = "1.0.402"
+version = "1.0.403"
 keywords = ['LLM', 'Agents', 'gen ai', 'chat ui', 'chatbot ui', 'openai', 'copilot', 'langchain', 'conversational ai']
 description = "Build Conversational AI."
 authors = ["Chainlo"]
 license = "Apache-2.0 license"
 repository = "https://github.com/Chainlit/chainlit"
 readme = "README.md"
 exclude = [
```

### Comparing `chainlo-1.0.402/PKG-INFO` & `chainlo-1.0.403/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlo
-Version: 1.0.402
+Version: 1.0.403
 Summary: Build Conversational AI.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,openai,copilot,langchain,conversational ai
 Author: Chainlo
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
```

