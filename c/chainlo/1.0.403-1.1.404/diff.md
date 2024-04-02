# Comparing `tmp/chainlo-1.0.403.tar.gz` & `tmp/chainlo-1.1.404.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainlo-1.0.403.tar", max compression
+gzip compressed data, was "chainlo-1.1.404.tar", max compression
```

## Comparing `chainlo-1.0.403.tar` & `chainlo-1.1.404.tar`

### file list

```diff
@@ -1,187 +1,187 @@
--rw-r--r--   0        0        0        0 2024-03-28 12:59:00.277858 chainlo-1.0.403/README.md
--rw-r--r--   0        0        0     9667 2024-03-28 12:59:00.278103 chainlo-1.0.403/chainlo/__init__.py
--rw-r--r--   0        0        0       87 2024-03-28 12:59:00.278241 chainlo-1.0.403/chainlo/__main__.py
--rw-r--r--   0        0        0     1410 2024-03-28 12:59:00.278372 chainlo-1.0.403/chainlo/action.py
--rw-r--r--   0        0        0    26017 2024-03-29 15:38:21.217731 chainlo-1.0.403/chainlo/agenta_cli/README.md
--rw-r--r--   0        0        0      493 2024-03-29 15:38:21.221195 chainlo-1.0.403/chainlo/agenta_cli/agenta/__init__.py
--rw-r--r--   0        0        0      494 2024-04-02 12:31:57.078250 chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/evaluation_commands.py
--rw-r--r--   0        0        0     6239 2024-04-02 12:26:04.291397 chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/helper.py
--rw-r--r--   0        0        0     9535 2024-04-02 12:37:37.788934 chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/main.py
--rw-r--r--   0        0        0     1337 2024-04-02 12:31:07.654475 chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/telemetry.py
--rw-r--r--   0        0        0    16978 2024-04-02 12:30:50.209025 chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/variant_commands.py
--rw-r--r--   0        0        0     1313 2024-04-02 12:26:21.238617 chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/variant_configs.py
--rw-r--r--   0        0        0     2756 2024-03-29 15:38:21.228131 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/Readme.md
--rw-r--r--   0        0        0        0 2024-03-29 15:38:21.228597 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/__init__.py
--rw-r--r--   0        0        0     2509 2024-04-02 12:31:46.026778 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/api.py
--rw-r--r--   0        0        0      623 2024-03-29 15:38:21.229938 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/api_models.py
--rw-r--r--   0        0        0     2666 2024-03-29 15:38:21.231650 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/__init__.py
--rw-r--r--   0        0        0   259068 2024-03-29 15:38:21.233513 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/client.py
--rw-r--r--   0        0        0      519 2024-03-29 15:38:21.234601 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/__init__.py
--rw-r--r--   0        0        0      440 2024-03-29 15:38:21.235211 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/api_error.py
--rw-r--r--   0        0        0      972 2024-03-29 15:38:21.235881 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/client_wrapper.py
--rw-r--r--   0        0        0     1069 2024-03-29 15:38:21.236559 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/datetime_utils.py
--rw-r--r--   0        0        0     3825 2024-03-29 15:38:21.237211 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/jsonable_encoder.py
--rw-r--r--   0        0        0      330 2024-03-29 15:38:21.237761 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/remove_none_from_dict.py
--rw-r--r--   0        0        0      170 2024-03-29 15:38:21.239005 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-03-29 15:38:21.239732 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0     4008 2024-03-29 15:38:21.241610 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/__init__.py
--rw-r--r--   0        0        0      211 2024-03-29 15:38:21.242318 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/add_variant_from_base_and_config_response.py
--rw-r--r--   0        0        0     1083 2024-03-29 15:38:21.243231 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/aggregated_result.py
--rw-r--r--   0        0        0      974 2024-03-29 15:38:21.243870 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app.py
--rw-r--r--   0        0        0     1268 2024-03-29 15:38:21.244420 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output.py
--rw-r--r--   0        0        0     1394 2024-03-29 15:38:21.245000 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output_extended.py
--rw-r--r--   0        0        0     1075 2024-03-29 15:38:21.245538 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app_variant_revision.py
--rw-r--r--   0        0        0      983 2024-03-29 15:38:21.246051 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/base_output.py
--rw-r--r--   0        0        0     1061 2024-03-29 15:38:21.246493 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/body_import_testset.py
--rw-r--r--   0        0        0     1028 2024-03-29 15:38:21.246936 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/config_db.py
--rw-r--r--   0        0        0      182 2024-03-29 15:38:21.247467 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/container_templates_response.py
--rw-r--r--   0        0        0      986 2024-03-29 15:38:21.248085 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/create_app_output.py
--rw-r--r--   0        0        0      991 2024-03-29 15:38:21.248628 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/delete_evaluation.py
--rw-r--r--   0        0        0      986 2024-03-29 15:38:21.249104 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/docker_env_vars.py
--rw-r--r--   0        0        0     1176 2024-03-29 15:38:21.249534 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/environment_output.py
--rw-r--r--   0        0        0     1376 2024-03-29 15:38:21.249971 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation.py
--rw-r--r--   0        0        0     1497 2024-03-29 15:38:21.250499 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario.py
--rw-r--r--   0        0        0     1027 2024-03-29 15:38:21.251140 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_input.py
--rw-r--r--   0        0        0     1014 2024-03-29 15:38:21.251815 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_output.py
--rw-r--r--   0        0        0     1033 2024-03-29 15:38:21.252247 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_result.py
--rw-r--r--   0        0        0     1102 2024-03-29 15:38:21.252717 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_status_enum.py
--rw-r--r--   0        0        0      644 2024-03-29 15:38:21.253129 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_type.py
--rw-r--r--   0        0        0      971 2024-03-29 15:38:21.253545 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_webhook.py
--rw-r--r--   0        0        0     1046 2024-03-29 15:38:21.254100 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluator.py
--rw-r--r--   0        0        0     1124 2024-03-29 15:38:21.254598 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluator_config.py
--rw-r--r--   0        0        0     1136 2024-03-29 15:38:21.255072 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/feedback.py
--rw-r--r--   0        0        0     1063 2024-03-29 15:38:21.255549 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/get_config_reponse.py
--rw-r--r--   0        0        0     1060 2024-03-29 15:38:21.256152 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/http_validation_error.py
--rw-r--r--   0        0        0     1305 2024-03-29 15:38:21.256706 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation.py
--rw-r--r--   0        0        0     1580 2024-03-29 15:38:21.257151 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario.py
--rw-r--r--   0        0        0     1006 2024-03-29 15:38:21.257665 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_input.py
--rw-r--r--   0        0        0     1010 2024-03-29 15:38:21.258161 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_output.py
--rw-r--r--   0        0        0      134 2024-03-29 15:38:21.258634 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_score.py
--rw-r--r--   0        0        0      140 2024-03-29 15:38:21.259047 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_update_score.py
--rw-r--r--   0        0        0     1048 2024-03-29 15:38:21.259555 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/image.py
--rw-r--r--   0        0        0      965 2024-03-29 15:38:21.260000 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/invite_request.py
--rw-r--r--   0        0        0     1095 2024-03-29 15:38:21.260474 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/list_api_keys_output.py
--rw-r--r--   0        0        0     1045 2024-03-29 15:38:21.260976 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/llm_run_rate_limit.py
--rw-r--r--   0        0        0     1009 2024-03-29 15:38:21.261472 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/new_testset.py
--rw-r--r--   0        0        0     1181 2024-03-29 15:38:21.261911 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/organization.py
--rw-r--r--   0        0        0      981 2024-03-29 15:38:21.262371 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/organization_output.py
--rw-r--r--   0        0        0      996 2024-03-29 15:38:21.262822 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/result.py
--rw-r--r--   0        0        0     1117 2024-03-29 15:38:21.263320 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/simple_evaluation_output.py
--rw-r--r--   0        0        0     1546 2024-03-29 15:38:21.263903 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/span.py
--rw-r--r--   0        0        0     1037 2024-03-29 15:38:21.264526 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/template.py
--rw-r--r--   0        0        0     1189 2024-03-29 15:38:21.265123 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/template_image_info.py
--rw-r--r--   0        0        0     1088 2024-03-29 15:38:21.265659 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/test_set_output_response.py
--rw-r--r--   0        0        0     1004 2024-03-29 15:38:21.266314 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/test_set_simple_response.py
--rw-r--r--   0        0        0     1353 2024-03-29 15:38:21.266828 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/trace.py
--rw-r--r--   0        0        0      953 2024-03-29 15:38:21.267207 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/uri.py
--rw-r--r--   0        0        0     1086 2024-03-29 15:38:21.267670 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-03-29 15:38:21.268112 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     1031 2024-03-29 15:38:21.268517 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/variant_action.py
--rw-r--r--   0        0        0      511 2024-03-29 15:38:21.268961 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/variant_action_enum.py
--rw-r--r--   0        0        0    19668 2024-04-02 12:32:12.753248 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/client.py
--rw-r--r--   0        0        0       94 2024-03-29 15:38:21.269971 chainlo-1.0.403/chainlo/agenta_cli/agenta/client/exceptions.py
--rw-r--r--   0        0        0      732 2024-03-29 15:38:21.270473 chainlo-1.0.403/chainlo/agenta_cli/agenta/config.py
--rw-r--r--   0        0        0      223 2024-03-29 15:38:21.270908 chainlo-1.0.403/chainlo/agenta_cli/agenta/config.toml
--rw-r--r--   0        0        0      317 2024-03-29 15:38:21.272321 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker-assets/Dockerfile.cloud.template
--rw-r--r--   0        0        0      241 2024-03-29 15:38:21.272700 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker-assets/Dockerfile.template
--rw-r--r--   0        0        0      102 2024-03-29 15:38:21.273161 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker-assets/README.md
--rwxr-xr-x   0        0        0       74 2024-03-29 15:38:21.273685 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker-assets/entrypoint.sh
--rw-r--r--   0        0        0      102 2024-04-02 15:18:44.554577 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker-assets/lambda_function.py
--rw-r--r--   0        0        0      270 2024-04-02 15:18:34.213398 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker-assets/main.py
--rw-r--r--   0        0        0     3562 2024-04-02 12:31:19.880389 chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker_utils.py
--rw-r--r--   0        0        0      565 2024-03-29 15:38:21.275737 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/__init__.py
--rw-r--r--   0        0        0    15506 2024-04-02 12:23:48.754730 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/agenta_decorator.py
--rw-r--r--   0        0        0     8065 2024-04-02 12:24:41.742653 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/agenta_init.py
--rw-r--r--   0        0        0      901 2024-03-29 15:38:21.277386 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/context.py
--rw-r--r--   0        0        0      269 2024-03-29 15:38:21.277737 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/router.py
--rw-r--r--   0        0        0     4658 2024-03-29 15:38:21.278086 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/types.py
--rw-r--r--   0        0        0      380 2024-04-02 12:25:03.766003 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/utils/globals.py
--rw-r--r--   0        0        0     5877 2024-03-29 15:38:21.279477 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/utils/helper/openai_cost.py
--rw-r--r--   0        0        0     1278 2024-03-29 15:38:21.279853 chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/utils/preinit.py
--rw-r--r--   0        0        0      308 2024-03-29 15:38:21.281309 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/compose_email/README.md
--rw-r--r--   0        0        0     2384 2024-03-29 15:38:21.281686 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/compose_email/app.py
--rw-r--r--   0        0        0       70 2024-03-29 15:38:21.282049 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/compose_email/env.example
--rw-r--r--   0        0        0       23 2024-03-29 15:38:21.282449 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/compose_email/requirements.txt
--rw-r--r--   0        0        0       47 2024-03-29 15:38:21.282787 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/compose_email/template.toml
--rw-r--r--   0        0        0      308 2024-03-29 15:38:21.283477 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/extract_data_to_json/README.md
--rw-r--r--   0        0        0     1320 2024-03-29 15:38:21.283896 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/extract_data_to_json/app.py
--rw-r--r--   0        0        0       70 2024-03-29 15:38:21.284271 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/extract_data_to_json/env.example
--rw-r--r--   0        0        0       23 2024-03-29 15:38:21.284661 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/extract_data_to_json/requirements.txt
--rw-r--r--   0        0        0       60 2024-03-29 15:38:21.285035 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/extract_data_to_json/template.toml
--rw-r--r--   0        0        0      308 2024-03-29 15:38:21.285928 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/simple_prompt/README.md
--rw-r--r--   0        0        0      665 2024-04-02 15:20:39.242968 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/simple_prompt/app.py
--rw-r--r--   0        0        0       70 2024-03-29 15:38:21.286665 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/simple_prompt/env.example
--rw-r--r--   0        0        0       24 2024-04-02 15:18:01.855024 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/simple_prompt/requirements.txt
--rw-r--r--   0        0        0       60 2024-03-29 15:38:21.287420 chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/simple_prompt/template.toml
--rw-r--r--   0        0        0     1078 2024-04-01 00:20:31.300954 chainlo-1.0.403/chainlo/agenta_cli/pyproject.toml-ex
--rw-r--r--   0        0        0        0 2024-03-29 15:38:21.289373 chainlo-1.0.403/chainlo/agenta_cli/requirements.txt
--rw-r--r--   0        0        0      580 2024-03-29 15:38:21.290495 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/simple_langchain/app.py
--rw-r--r--   0        0        0       31 2024-03-29 15:38:21.290969 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/simple_langchain/requirements.txt
--rw-r--r--   0        0        0      411 2024-03-29 15:38:21.292434 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/README.md
--rw-r--r--   0        0        0     3294 2024-03-29 15:38:21.293249 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/agenta.py
--rw-r--r--   0        0        0      580 2024-03-29 15:38:21.294048 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/app.py
--rw-r--r--   0        0        0       51 2024-03-29 15:38:21.294746 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/config.toml
--rw-r--r--   0        0        0      187 2024-03-29 15:38:21.295361 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/main.py
--rw-r--r--   0        0        0       31 2024-03-29 15:38:21.295991 chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/requirements.txt
--rw-r--r--   0        0        0     2681 2024-03-28 12:59:00.278537 chainlo-1.0.403/chainlo/auth.py
--rw-r--r--   0        0        0     1361 2024-03-28 12:59:00.278680 chainlo-1.0.403/chainlo/cache.py
--rw-r--r--   0        0        0      877 2024-03-28 12:59:00.278813 chainlo-1.0.403/chainlo/chat_settings.py
--rw-r--r--   0        0        0     4786 2024-03-30 14:01:40.889613 chainlo-1.0.403/chainlo/cli/__init__.py
--rw-r--r--   0        0        0      717 2024-03-28 12:59:00.279324 chainlo-1.0.403/chainlo/cli/utils.py
--rw-r--r--   0        0        0    13465 2024-03-28 12:59:00.279531 chainlo-1.0.403/chainlo/config.py
--rw-r--r--   0        0        0     2476 2024-03-28 12:59:00.279723 chainlo-1.0.403/chainlo/context.py
--rw-r--r--   0        0        0     8887 2024-04-02 13:46:34.758455 chainlo-1.0.403/chainlo/copilot/dist/assets/logo_dark-2a3cf740.svg
--rw-r--r--   0        0        0     8889 2024-04-02 13:46:34.756788 chainlo-1.0.403/chainlo/copilot/dist/assets/logo_light-b078e7bc.svg
--rw-r--r--   0        0        0  7013566 2024-04-02 13:46:34.752958 chainlo-1.0.403/chainlo/copilot/dist/index.js
--rw-r--r--   0        0        0    14724 2024-03-28 12:59:00.279971 chainlo-1.0.403/chainlo/data/__init__.py
--rw-r--r--   0        0        0      461 2024-03-28 12:59:00.280107 chainlo-1.0.403/chainlo/data/acl.py
--rw-r--r--   0        0        0    10162 2024-03-28 12:59:00.280281 chainlo-1.0.403/chainlo/element.py
--rw-r--r--   0        0        0    12178 2024-03-28 12:59:00.280461 chainlo-1.0.403/chainlo/emitter.py
--rw-r--r--   0        0        0  3071160 2024-04-02 13:46:34.734588 chainlo-1.0.403/chainlo/frontend/dist/assets/index-7bc2ef31.js
--rw-r--r--   0        0        0     6605 2024-04-02 13:46:34.736982 chainlo-1.0.403/chainlo/frontend/dist/assets/index-d088547c.css
--rw-r--r--   0        0        0     8887 2024-04-02 13:46:34.736163 chainlo-1.0.403/chainlo/frontend/dist/assets/logo_dark-2a3cf740.svg
--rw-r--r--   0        0        0     8889 2024-04-02 13:46:34.735648 chainlo-1.0.403/chainlo/frontend/dist/assets/logo_light-b078e7bc.svg
--rw-r--r--   0        0        0  3763471 2024-04-02 13:46:34.739499 chainlo-1.0.403/chainlo/frontend/dist/assets/react-plotly-70086d41.js
--rw-r--r--   0        0        0     6455 2024-04-02 13:46:34.741377 chainlo-1.0.403/chainlo/frontend/dist/favicon.svg
--rw-r--r--   0        0        0     1005 2024-04-02 13:46:34.731871 chainlo-1.0.403/chainlo/frontend/dist/index.html
--rw-r--r--   0        0        0      217 2024-03-28 12:59:00.280774 chainlo-1.0.403/chainlo/haystack/__init__.py
--rw-r--r--   0        0        0     5209 2024-03-28 12:59:00.280941 chainlo-1.0.403/chainlo/haystack/callbacks.py
--rw-r--r--   0        0        0     3018 2024-03-30 14:45:46.436609 chainlo-1.0.403/chainlo/hello.py
--rw-r--r--   0        0        0     4880 2024-03-28 12:59:00.281252 chainlo-1.0.403/chainlo/input_widget.py
--rw-r--r--   0        0        0      217 2024-03-28 12:59:00.281449 chainlo-1.0.403/chainlo/langchain/__init__.py
--rw-r--r--   0        0        0    20521 2024-03-28 12:59:00.281698 chainlo-1.0.403/chainlo/langchain/callbacks.py
--rw-r--r--   0        0        0      817 2024-03-28 12:59:00.281944 chainlo-1.0.403/chainlo/langflow/__init__.py
--rw-r--r--   0        0        0      227 2024-03-28 12:59:00.282266 chainlo-1.0.403/chainlo/llama_index/__init__.py
--rw-r--r--   0        0        0     6078 2024-03-28 12:59:00.282445 chainlo-1.0.403/chainlo/llama_index/callbacks.py
--rw-r--r--   0        0        0      373 2024-03-28 12:59:00.282615 chainlo-1.0.403/chainlo/logger.py
--rw-r--r--   0        0        0     2025 2024-03-28 12:59:00.282790 chainlo-1.0.403/chainlo/markdown.py
--rw-r--r--   0        0        0    17683 2024-03-28 12:59:00.283051 chainlo-1.0.403/chainlo/message.py
--rw-r--r--   0        0        0    17459 2024-03-28 12:59:00.283259 chainlo-1.0.403/chainlo/oauth_providers.py
--rw-r--r--   0        0        0     2002 2024-03-28 12:59:00.283525 chainlo-1.0.403/chainlo/openai/__init__.py
--rw-r--r--   0        0        0       80 2024-03-28 12:59:00.283801 chainlo-1.0.403/chainlo/playground/__init__.py
--rw-r--r--   0        0        0     1033 2024-03-28 12:59:00.284106 chainlo-1.0.403/chainlo/playground/config.py
--rw-r--r--   0        0        0     3858 2024-03-28 12:59:00.284312 chainlo-1.0.403/chainlo/playground/provider.py
--rw-r--r--   0        0        0      236 2024-03-28 12:59:00.284521 chainlo-1.0.403/chainlo/playground/providers/__init__.py
--rw-r--r--   0        0        0     3495 2024-03-28 12:59:00.284708 chainlo-1.0.403/chainlo/playground/providers/anthropic.py
--rw-r--r--   0        0        0     2130 2024-03-28 12:59:00.284866 chainlo-1.0.403/chainlo/playground/providers/huggingface.py
--rw-r--r--   0        0        0     3103 2024-03-28 12:59:00.285051 chainlo-1.0.403/chainlo/playground/providers/langchain.py
--rw-r--r--   0        0        0    12397 2024-03-28 12:59:00.285216 chainlo-1.0.403/chainlo/playground/providers/openai.py
--rw-r--r--   0        0        0     5084 2024-03-28 12:59:00.285364 chainlo-1.0.403/chainlo/playground/providers/vertexai.py
--rw-r--r--   0        0        0        0 2024-03-28 12:59:00.285429 chainlo-1.0.403/chainlo/py.typed
--rw-r--r--   0        0        0      295 2024-03-28 12:59:00.285564 chainlo-1.0.403/chainlo/secret.py
--rw-r--r--   0        0        0    22602 2024-03-28 12:59:00.285775 chainlo-1.0.403/chainlo/server.py
--rw-r--r--   0        0        0     8844 2024-03-28 12:59:00.285967 chainlo-1.0.403/chainlo/session.py
--rw-r--r--   0        0        0     9846 2024-03-28 12:59:00.286136 chainlo-1.0.403/chainlo/socket.py
--rw-r--r--   0        0        0    12749 2024-03-28 12:59:00.286305 chainlo-1.0.403/chainlo/step.py
--rw-r--r--   0        0        0     1235 2024-03-28 12:59:00.286446 chainlo-1.0.403/chainlo/sync.py
--rw-r--r--   0        0        0     3060 2024-03-28 12:59:00.286585 chainlo-1.0.403/chainlo/telemetry.py
--rw-r--r--   0        0        0     6252 2024-03-28 12:59:00.286806 chainlo-1.0.403/chainlo/translations/de.json
--rw-r--r--   0        0        0     4514 2024-03-28 12:59:00.287261 chainlo-1.0.403/chainlo/translations/en-US.json
--rw-r--r--   0        0        0     4614 2024-03-28 12:59:00.287519 chainlo-1.0.403/chainlo/translations/pt-BR.json
--rw-r--r--   0        0        0     3379 2024-03-28 12:59:00.287730 chainlo-1.0.403/chainlo/types.py
--rw-r--r--   0        0        0      619 2024-03-28 12:59:00.287957 chainlo-1.0.403/chainlo/user.py
--rw-r--r--   0        0        0     1368 2024-03-28 12:59:00.288135 chainlo-1.0.403/chainlo/user_session.py
--rw-r--r--   0        0        0     2571 2024-03-28 12:59:00.288279 chainlo-1.0.403/chainlo/utils.py
--rw-r--r--   0        0        0      196 2024-03-28 12:59:00.288410 chainlo-1.0.403/chainlo/version.py
--rw-r--r--   0        0        0     2361 2024-04-02 15:45:07.032899 chainlo-1.0.403/pyproject.toml
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 chainlo-1.0.403/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-28 12:59:00.277858 chainlo-1.1.404/README.md
+-rw-r--r--   0        0        0     9640 2024-04-02 18:01:22.602103 chainlo-1.1.404/chainlo/__init__.py
+-rw-r--r--   0        0        0       85 2024-04-02 18:00:53.775192 chainlo-1.1.404/chainlo/__main__.py
+-rw-r--r--   0        0        0     1408 2024-04-02 20:00:55.227821 chainlo-1.1.404/chainlo/action.py
+-rw-r--r--   0        0        0    26017 2024-03-29 15:38:21.217731 chainlo-1.1.404/chainlo/agenta_cli/README.md
+-rw-r--r--   0        0        0      493 2024-03-29 15:38:21.221195 chainlo-1.1.404/chainlo/agenta_cli/agenta/__init__.py
+-rw-r--r--   0        0        0      493 2024-04-02 20:00:55.228018 chainlo-1.1.404/chainlo/agenta_cli/agenta/cli/evaluation_commands.py
+-rw-r--r--   0        0        0     6237 2024-04-02 20:00:55.228164 chainlo-1.1.404/chainlo/agenta_cli/agenta/cli/helper.py
+-rw-r--r--   0        0        0     9530 2024-04-02 20:00:54.885868 chainlo-1.1.404/chainlo/agenta_cli/agenta/cli/main.py
+-rw-r--r--   0        0        0     1336 2024-04-02 20:00:55.228042 chainlo-1.1.404/chainlo/agenta_cli/agenta/cli/telemetry.py
+-rw-r--r--   0        0        0    16972 2024-04-02 20:00:55.228192 chainlo-1.1.404/chainlo/agenta_cli/agenta/cli/variant_commands.py
+-rw-r--r--   0        0        0     1312 2024-04-02 20:00:55.228061 chainlo-1.1.404/chainlo/agenta_cli/agenta/cli/variant_configs.py
+-rw-r--r--   0        0        0     2756 2024-03-29 15:38:21.228131 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/Readme.md
+-rw-r--r--   0        0        0        0 2024-03-29 15:38:21.228597 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/__init__.py
+-rw-r--r--   0        0        0     2505 2024-04-02 20:00:54.885886 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/api.py
+-rw-r--r--   0        0        0      623 2024-03-29 15:38:21.229938 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/api_models.py
+-rw-r--r--   0        0        0     2666 2024-03-29 15:38:21.231650 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/__init__.py
+-rw-r--r--   0        0        0   259068 2024-03-29 15:38:21.233513 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/client.py
+-rw-r--r--   0        0        0      519 2024-03-29 15:38:21.234601 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/core/__init__.py
+-rw-r--r--   0        0        0      440 2024-03-29 15:38:21.235211 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/core/api_error.py
+-rw-r--r--   0        0        0      972 2024-03-29 15:38:21.235881 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/core/client_wrapper.py
+-rw-r--r--   0        0        0     1069 2024-03-29 15:38:21.236559 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/core/datetime_utils.py
+-rw-r--r--   0        0        0     3825 2024-03-29 15:38:21.237211 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      330 2024-03-29 15:38:21.237761 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0      170 2024-03-29 15:38:21.239005 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-03-29 15:38:21.239732 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0     4008 2024-03-29 15:38:21.241610 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/__init__.py
+-rw-r--r--   0        0        0      211 2024-03-29 15:38:21.242318 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/add_variant_from_base_and_config_response.py
+-rw-r--r--   0        0        0     1083 2024-03-29 15:38:21.243231 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/aggregated_result.py
+-rw-r--r--   0        0        0      974 2024-03-29 15:38:21.243870 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/app.py
+-rw-r--r--   0        0        0     1268 2024-03-29 15:38:21.244420 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output.py
+-rw-r--r--   0        0        0     1394 2024-03-29 15:38:21.245000 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output_extended.py
+-rw-r--r--   0        0        0     1075 2024-03-29 15:38:21.245538 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/app_variant_revision.py
+-rw-r--r--   0        0        0      983 2024-03-29 15:38:21.246051 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/base_output.py
+-rw-r--r--   0        0        0     1061 2024-03-29 15:38:21.246493 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/body_import_testset.py
+-rw-r--r--   0        0        0     1028 2024-03-29 15:38:21.246936 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/config_db.py
+-rw-r--r--   0        0        0      182 2024-03-29 15:38:21.247467 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/container_templates_response.py
+-rw-r--r--   0        0        0      986 2024-03-29 15:38:21.248085 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/create_app_output.py
+-rw-r--r--   0        0        0      991 2024-03-29 15:38:21.248628 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/delete_evaluation.py
+-rw-r--r--   0        0        0      986 2024-03-29 15:38:21.249104 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/docker_env_vars.py
+-rw-r--r--   0        0        0     1176 2024-03-29 15:38:21.249534 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/environment_output.py
+-rw-r--r--   0        0        0     1376 2024-03-29 15:38:21.249971 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation.py
+-rw-r--r--   0        0        0     1497 2024-03-29 15:38:21.250499 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario.py
+-rw-r--r--   0        0        0     1027 2024-03-29 15:38:21.251140 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_input.py
+-rw-r--r--   0        0        0     1014 2024-03-29 15:38:21.251815 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_output.py
+-rw-r--r--   0        0        0     1033 2024-03-29 15:38:21.252247 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_result.py
+-rw-r--r--   0        0        0     1102 2024-03-29 15:38:21.252717 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_status_enum.py
+-rw-r--r--   0        0        0      644 2024-03-29 15:38:21.253129 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_type.py
+-rw-r--r--   0        0        0      971 2024-03-29 15:38:21.253545 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_webhook.py
+-rw-r--r--   0        0        0     1046 2024-03-29 15:38:21.254100 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluator.py
+-rw-r--r--   0        0        0     1124 2024-03-29 15:38:21.254598 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluator_config.py
+-rw-r--r--   0        0        0     1136 2024-03-29 15:38:21.255072 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/feedback.py
+-rw-r--r--   0        0        0     1063 2024-03-29 15:38:21.255549 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/get_config_reponse.py
+-rw-r--r--   0        0        0     1060 2024-03-29 15:38:21.256152 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/http_validation_error.py
+-rw-r--r--   0        0        0     1305 2024-03-29 15:38:21.256706 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation.py
+-rw-r--r--   0        0        0     1580 2024-03-29 15:38:21.257151 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario.py
+-rw-r--r--   0        0        0     1006 2024-03-29 15:38:21.257665 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_input.py
+-rw-r--r--   0        0        0     1010 2024-03-29 15:38:21.258161 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_output.py
+-rw-r--r--   0        0        0      134 2024-03-29 15:38:21.258634 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_score.py
+-rw-r--r--   0        0        0      140 2024-03-29 15:38:21.259047 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_update_score.py
+-rw-r--r--   0        0        0     1048 2024-03-29 15:38:21.259555 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/image.py
+-rw-r--r--   0        0        0      965 2024-03-29 15:38:21.260000 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/invite_request.py
+-rw-r--r--   0        0        0     1095 2024-03-29 15:38:21.260474 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/list_api_keys_output.py
+-rw-r--r--   0        0        0     1045 2024-03-29 15:38:21.260976 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/llm_run_rate_limit.py
+-rw-r--r--   0        0        0     1009 2024-03-29 15:38:21.261472 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/new_testset.py
+-rw-r--r--   0        0        0     1181 2024-03-29 15:38:21.261911 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/organization.py
+-rw-r--r--   0        0        0      981 2024-03-29 15:38:21.262371 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/organization_output.py
+-rw-r--r--   0        0        0      996 2024-03-29 15:38:21.262822 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/result.py
+-rw-r--r--   0        0        0     1117 2024-03-29 15:38:21.263320 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/simple_evaluation_output.py
+-rw-r--r--   0        0        0     1546 2024-03-29 15:38:21.263903 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/span.py
+-rw-r--r--   0        0        0     1037 2024-03-29 15:38:21.264526 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/template.py
+-rw-r--r--   0        0        0     1189 2024-03-29 15:38:21.265123 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/template_image_info.py
+-rw-r--r--   0        0        0     1088 2024-03-29 15:38:21.265659 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/test_set_output_response.py
+-rw-r--r--   0        0        0     1004 2024-03-29 15:38:21.266314 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/test_set_simple_response.py
+-rw-r--r--   0        0        0     1353 2024-03-29 15:38:21.266828 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/trace.py
+-rw-r--r--   0        0        0      953 2024-03-29 15:38:21.267207 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/uri.py
+-rw-r--r--   0        0        0     1086 2024-03-29 15:38:21.267670 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-03-29 15:38:21.268112 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     1031 2024-03-29 15:38:21.268517 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/variant_action.py
+-rw-r--r--   0        0        0      511 2024-03-29 15:38:21.268961 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/variant_action_enum.py
+-rw-r--r--   0        0        0    19667 2024-04-02 20:00:54.885983 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/client.py
+-rw-r--r--   0        0        0       94 2024-03-29 15:38:21.269971 chainlo-1.1.404/chainlo/agenta_cli/agenta/client/exceptions.py
+-rw-r--r--   0        0        0      732 2024-03-29 15:38:21.270473 chainlo-1.1.404/chainlo/agenta_cli/agenta/config.py
+-rw-r--r--   0        0        0      223 2024-03-29 15:38:21.270908 chainlo-1.1.404/chainlo/agenta_cli/agenta/config.toml
+-rw-r--r--   0        0        0      317 2024-03-29 15:38:21.272321 chainlo-1.1.404/chainlo/agenta_cli/agenta/docker/docker-assets/Dockerfile.cloud.template
+-rw-r--r--   0        0        0      241 2024-03-29 15:38:21.272700 chainlo-1.1.404/chainlo/agenta_cli/agenta/docker/docker-assets/Dockerfile.template
+-rw-r--r--   0        0        0      102 2024-03-29 15:38:21.273161 chainlo-1.1.404/chainlo/agenta_cli/agenta/docker/docker-assets/README.md
+-rwxr-xr-x   0        0        0       74 2024-03-29 15:38:21.273685 chainlo-1.1.404/chainlo/agenta_cli/agenta/docker/docker-assets/entrypoint.sh
+-rw-r--r--   0        0        0      102 2024-04-02 15:18:44.554577 chainlo-1.1.404/chainlo/agenta_cli/agenta/docker/docker-assets/lambda_function.py
+-rw-r--r--   0        0        0      270 2024-04-02 15:18:34.213398 chainlo-1.1.404/chainlo/agenta_cli/agenta/docker/docker-assets/main.py
+-rw-r--r--   0        0        0     3561 2024-04-02 20:00:54.887775 chainlo-1.1.404/chainlo/agenta_cli/agenta/docker/docker_utils.py
+-rw-r--r--   0        0        0      565 2024-03-29 15:38:21.275737 chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/__init__.py
+-rw-r--r--   0        0        0    15504 2024-04-02 20:00:55.228104 chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/agenta_decorator.py
+-rw-r--r--   0        0        0     8063 2024-04-02 20:00:55.228132 chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/agenta_init.py
+-rw-r--r--   0        0        0      901 2024-03-29 15:38:21.277386 chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/context.py
+-rw-r--r--   0        0        0      269 2024-03-29 15:38:21.277737 chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/router.py
+-rw-r--r--   0        0        0     4658 2024-03-29 15:38:21.278086 chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/types.py
+-rw-r--r--   0        0        0      379 2024-04-02 20:00:55.228081 chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/utils/globals.py
+-rw-r--r--   0        0        0     5877 2024-03-29 15:38:21.279477 chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/utils/helper/openai_cost.py
+-rw-r--r--   0        0        0     1278 2024-03-29 15:38:21.279853 chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/utils/preinit.py
+-rw-r--r--   0        0        0      308 2024-03-29 15:38:21.281309 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/compose_email/README.md
+-rw-r--r--   0        0        0     2384 2024-03-29 15:38:21.281686 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/compose_email/app.py
+-rw-r--r--   0        0        0       70 2024-03-29 15:38:21.282049 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/compose_email/env.example
+-rw-r--r--   0        0        0       23 2024-03-29 15:38:21.282449 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/compose_email/requirements.txt
+-rw-r--r--   0        0        0       47 2024-03-29 15:38:21.282787 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/compose_email/template.toml
+-rw-r--r--   0        0        0      308 2024-03-29 15:38:21.283477 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/extract_data_to_json/README.md
+-rw-r--r--   0        0        0     1320 2024-03-29 15:38:21.283896 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/extract_data_to_json/app.py
+-rw-r--r--   0        0        0       70 2024-03-29 15:38:21.284271 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/extract_data_to_json/env.example
+-rw-r--r--   0        0        0       23 2024-03-29 15:38:21.284661 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/extract_data_to_json/requirements.txt
+-rw-r--r--   0        0        0       60 2024-03-29 15:38:21.285035 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/extract_data_to_json/template.toml
+-rw-r--r--   0        0        0      308 2024-03-29 15:38:21.285928 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/simple_prompt/README.md
+-rw-r--r--   0        0        0      665 2024-04-02 15:20:39.242968 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/simple_prompt/app.py
+-rw-r--r--   0        0        0       70 2024-03-29 15:38:21.286665 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/simple_prompt/env.example
+-rw-r--r--   0        0        0       24 2024-04-02 15:18:01.855024 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/simple_prompt/requirements.txt
+-rw-r--r--   0        0        0       60 2024-03-29 15:38:21.287420 chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/simple_prompt/template.toml
+-rw-r--r--   0        0        0     1078 2024-04-01 00:20:31.300954 chainlo-1.1.404/chainlo/agenta_cli/pyproject.toml-ex
+-rw-r--r--   0        0        0        0 2024-03-29 15:38:21.289373 chainlo-1.1.404/chainlo/agenta_cli/requirements.txt
+-rw-r--r--   0        0        0      580 2024-03-29 15:38:21.290495 chainlo-1.1.404/chainlo/agenta_cli/tests/example_projects/simple_langchain/app.py
+-rw-r--r--   0        0        0       31 2024-03-29 15:38:21.290969 chainlo-1.1.404/chainlo/agenta_cli/tests/example_projects/simple_langchain/requirements.txt
+-rw-r--r--   0        0        0      411 2024-03-29 15:38:21.292434 chainlo-1.1.404/chainlo/agenta_cli/tests/example_projects/test2/README.md
+-rw-r--r--   0        0        0     3294 2024-03-29 15:38:21.293249 chainlo-1.1.404/chainlo/agenta_cli/tests/example_projects/test2/agenta.py
+-rw-r--r--   0        0        0      580 2024-03-29 15:38:21.294048 chainlo-1.1.404/chainlo/agenta_cli/tests/example_projects/test2/app.py
+-rw-r--r--   0        0        0       51 2024-03-29 15:38:21.294746 chainlo-1.1.404/chainlo/agenta_cli/tests/example_projects/test2/config.toml
+-rw-r--r--   0        0        0      187 2024-03-29 15:38:21.295361 chainlo-1.1.404/chainlo/agenta_cli/tests/example_projects/test2/main.py
+-rw-r--r--   0        0        0       31 2024-03-29 15:38:21.295991 chainlo-1.1.404/chainlo/agenta_cli/tests/example_projects/test2/requirements.txt
+-rw-r--r--   0        0        0     2677 2024-04-02 20:00:55.227808 chainlo-1.1.404/chainlo/auth.py
+-rw-r--r--   0        0        0     1359 2024-04-02 20:00:55.227793 chainlo-1.1.404/chainlo/cache.py
+-rw-r--r--   0        0        0      875 2024-04-02 20:00:55.227834 chainlo-1.1.404/chainlo/chat_settings.py
+-rw-r--r--   0        0        0     4777 2024-04-02 20:00:55.228539 chainlo-1.1.404/chainlo/cli/__init__.py
+-rw-r--r--   0        0        0      717 2024-03-28 12:59:00.279324 chainlo-1.1.404/chainlo/cli/utils.py
+-rw-r--r--   0        0        0    13460 2024-04-02 20:00:54.885837 chainlo-1.1.404/chainlo/config.py
+-rw-r--r--   0        0        0     2471 2024-04-02 20:00:55.227752 chainlo-1.1.404/chainlo/context.py
+-rw-r--r--   0        0        0     8887 2024-04-02 13:46:34.758455 chainlo-1.1.404/chainlo/copilot/dist/assets/logo_dark-2a3cf740.svg
+-rw-r--r--   0        0        0     8889 2024-04-02 13:46:34.756788 chainlo-1.1.404/chainlo/copilot/dist/assets/logo_light-b078e7bc.svg
+-rw-r--r--   0        0        0  7013566 2024-04-02 13:46:34.752958 chainlo-1.1.404/chainlo/copilot/dist/index.js
+-rw-r--r--   0        0        0    14716 2024-04-02 20:00:55.191849 chainlo-1.1.404/chainlo/data/__init__.py
+-rw-r--r--   0        0        0      460 2024-04-02 20:00:54.932738 chainlo-1.1.404/chainlo/data/acl.py
+-rw-r--r--   0        0        0    10157 2024-04-02 20:00:55.227734 chainlo-1.1.404/chainlo/element.py
+-rw-r--r--   0        0        0    12170 2024-04-02 20:00:55.227715 chainlo-1.1.404/chainlo/emitter.py
+-rw-r--r--   0        0        0  3071160 2024-04-02 13:46:34.734588 chainlo-1.1.404/chainlo/frontend/dist/assets/index-7bc2ef31.js
+-rw-r--r--   0        0        0     6605 2024-04-02 13:46:34.736982 chainlo-1.1.404/chainlo/frontend/dist/assets/index-d088547c.css
+-rw-r--r--   0        0        0     8887 2024-04-02 13:46:34.736163 chainlo-1.1.404/chainlo/frontend/dist/assets/logo_dark-2a3cf740.svg
+-rw-r--r--   0        0        0     8889 2024-04-02 13:46:34.735648 chainlo-1.1.404/chainlo/frontend/dist/assets/logo_light-b078e7bc.svg
+-rw-r--r--   0        0        0  3763471 2024-04-02 13:46:34.739499 chainlo-1.1.404/chainlo/frontend/dist/assets/react-plotly-70086d41.js
+-rw-r--r--   0        0        0     6455 2024-04-02 13:46:34.741377 chainlo-1.1.404/chainlo/frontend/dist/favicon.svg
+-rw-r--r--   0        0        0     1005 2024-04-02 13:46:34.731871 chainlo-1.1.404/chainlo/frontend/dist/index.html
+-rw-r--r--   0        0        0      216 2024-04-02 20:00:55.228246 chainlo-1.1.404/chainlo/haystack/__init__.py
+-rw-r--r--   0        0        0     5205 2024-04-02 20:00:55.191778 chainlo-1.1.404/chainlo/haystack/callbacks.py
+-rw-r--r--   0        0        0     3015 2024-04-02 20:00:54.885954 chainlo-1.1.404/chainlo/hello.py
+-rw-r--r--   0        0        0     4879 2024-04-02 20:00:54.885927 chainlo-1.1.404/chainlo/input_widget.py
+-rw-r--r--   0        0        0      216 2024-04-02 20:00:55.171891 chainlo-1.1.404/chainlo/langchain/__init__.py
+-rw-r--r--   0        0        0    20518 2024-04-02 20:00:55.171912 chainlo-1.1.404/chainlo/langchain/callbacks.py
+-rw-r--r--   0        0        0      815 2024-04-02 20:00:55.171857 chainlo-1.1.404/chainlo/langflow/__init__.py
+-rw-r--r--   0        0        0      226 2024-04-02 20:00:55.171832 chainlo-1.1.404/chainlo/llama_index/__init__.py
+-rw-r--r--   0        0        0     6075 2024-04-02 20:00:55.134912 chainlo-1.1.404/chainlo/llama_index/callbacks.py
+-rw-r--r--   0        0        0      373 2024-03-28 12:59:00.282615 chainlo-1.1.404/chainlo/logger.py
+-rw-r--r--   0        0        0     2024 2024-04-02 20:00:55.227774 chainlo-1.1.404/chainlo/markdown.py
+-rw-r--r--   0        0        0    17674 2024-04-02 20:00:55.227695 chainlo-1.1.404/chainlo/message.py
+-rw-r--r--   0        0        0    17458 2024-04-02 20:00:55.227664 chainlo-1.1.404/chainlo/oauth_providers.py
+-rw-r--r--   0        0        0     1998 2024-04-02 20:00:54.975014 chainlo-1.1.404/chainlo/openai/__init__.py
+-rw-r--r--   0        0        0       80 2024-03-28 12:59:00.283801 chainlo-1.1.404/chainlo/playground/__init__.py
+-rw-r--r--   0        0        0     1031 2024-04-02 20:00:54.974932 chainlo-1.1.404/chainlo/playground/config.py
+-rw-r--r--   0        0        0     3854 2024-04-02 20:00:54.974863 chainlo-1.1.404/chainlo/playground/provider.py
+-rw-r--r--   0        0        0      236 2024-03-28 12:59:00.284521 chainlo-1.1.404/chainlo/playground/providers/__init__.py
+-rw-r--r--   0        0        0     3493 2024-04-02 20:00:54.974475 chainlo-1.1.404/chainlo/playground/providers/anthropic.py
+-rw-r--r--   0        0        0     2127 2024-04-02 20:00:54.954439 chainlo-1.1.404/chainlo/playground/providers/huggingface.py
+-rw-r--r--   0        0        0     3100 2024-04-02 20:00:54.932814 chainlo-1.1.404/chainlo/playground/providers/langchain.py
+-rw-r--r--   0        0        0    12395 2024-04-02 20:00:54.952587 chainlo-1.1.404/chainlo/playground/providers/openai.py
+-rw-r--r--   0        0        0     5081 2024-04-02 20:00:54.887826 chainlo-1.1.404/chainlo/playground/providers/vertexai.py
+-rw-r--r--   0        0        0        0 2024-03-28 12:59:00.285429 chainlo-1.1.404/chainlo/py.typed
+-rw-r--r--   0        0        0      295 2024-03-28 12:59:00.285564 chainlo-1.1.404/chainlo/secret.py
+-rw-r--r--   0        0        0    22585 2024-04-02 20:05:16.016202 chainlo-1.1.404/chainlo/server.py
+-rw-r--r--   0        0        0     8837 2024-04-02 20:00:55.227631 chainlo-1.1.404/chainlo/session.py
+-rw-r--r--   0        0        0     9834 2024-04-02 20:00:55.228438 chainlo-1.1.404/chainlo/socket.py
+-rw-r--r--   0        0        0    12742 2024-04-02 20:00:55.227568 chainlo-1.1.404/chainlo/step.py
+-rw-r--r--   0        0        0     1234 2024-04-02 20:00:55.191939 chainlo-1.1.404/chainlo/sync.py
+-rw-r--r--   0        0        0     3058 2024-04-02 20:00:55.191900 chainlo-1.1.404/chainlo/telemetry.py
+-rw-r--r--   0        0        0     6252 2024-03-28 12:59:00.286806 chainlo-1.1.404/chainlo/translations/de.json
+-rw-r--r--   0        0        0     4514 2024-03-28 12:59:00.287261 chainlo-1.1.404/chainlo/translations/en-US.json
+-rw-r--r--   0        0        0     4614 2024-03-28 12:59:00.287519 chainlo-1.1.404/chainlo/translations/pt-BR.json
+-rw-r--r--   0        0        0     3376 2024-04-02 20:00:55.191876 chainlo-1.1.404/chainlo/types.py
+-rw-r--r--   0        0        0      619 2024-03-28 12:59:00.287957 chainlo-1.1.404/chainlo/user.py
+-rw-r--r--   0        0        0     1367 2024-04-02 20:00:55.228294 chainlo-1.1.404/chainlo/user_session.py
+-rw-r--r--   0        0        0     2568 2024-04-02 20:00:55.191815 chainlo-1.1.404/chainlo/utils.py
+-rw-r--r--   0        0        0      196 2024-03-28 12:59:00.288410 chainlo-1.1.404/chainlo/version.py
+-rw-r--r--   0        0        0     2360 2024-04-02 16:56:24.933603 chainlo-1.1.404/pyproject.toml
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 chainlo-1.1.404/PKG-INFO
```

### Comparing `chainlo-1.0.403/chainlo/__init__.py` & `chainlo-1.1.404/chainlo/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,59 +8,59 @@
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional
 
 from fastapi import Request, Response
 from pydantic.dataclasses import dataclass
 from starlette.datastructures import Headers
 
 if TYPE_CHECKING:
-    from chainlit.haystack.callbacks import HaystackAgentCallbackHandler
-    from chainlit.langchain.callbacks import (
+    from chainlo.haystack.callbacks import HaystackAgentCallbackHandler
+    from chainlo.langchain.callbacks import (
         LangchainCallbackHandler,
         AsyncLangchainCallbackHandler,
     )
-    from chainlit.llama_index.callbacks import LlamaIndexCallbackHandler
-    from chainlit.openai import instrument_openai
+    from chainlo.llama_index.callbacks import LlamaIndexCallbackHandler
+    from chainlo.openai import instrument_openai
 
-import chainlit.input_widget as input_widget
-from chainlit.action import Action
-from chainlit.cache import cache
-from chainlit.chat_settings import ChatSettings
-from chainlit.config import config
-from chainlit.context import context
-from chainlit.element import (
+import chainlo.input_widget as input_widget
+from chainlo.action import Action
+from chainlo.cache import cache
+from chainlo.chat_settings import ChatSettings
+from chainlo.config import config
+from chainlo.context import context
+from chainlo.element import (
     Audio,
     Avatar,
     File,
     Image,
     Pdf,
     Plotly,
     Pyplot,
     Task,
     TaskList,
     TaskStatus,
     Text,
     Video,
 )
-from chainlit.logger import logger
-from chainlit.message import (
+from chainlo.logger import logger
+from chainlo.message import (
     AskActionMessage,
     AskFileMessage,
     AskUserMessage,
     ErrorMessage,
     Message,
 )
-from chainlit.oauth_providers import get_configured_oauth_providers
-from chainlit.step import Step, step
-from chainlit.sync import make_async, run_sync
-from chainlit.telemetry import trace
-from chainlit.types import ChatProfile, ThreadDict
-from chainlit.user import PersistedUser, User
-from chainlit.user_session import user_session
-from chainlit.utils import make_module_getattr, wrap_user_function
-from chainlit.version import __version__
+from chainlo.oauth_providers import get_configured_oauth_providers
+from chainlo.step import Step, step
+from chainlo.sync import make_async, run_sync
+from chainlo.telemetry import trace
+from chainlo.types import ChatProfile, ThreadDict
+from chainlo.user import PersistedUser, User
+from chainlo.user_session import user_session
+from chainlo.utils import make_module_getattr, wrap_user_function
+from chainlo.version import __version__
 from literalai import ChatGeneration, CompletionGeneration, GenerationMessage
 
 if env_found:
     logger.info("Loaded .env file")
 
 
 @trace
@@ -303,19 +303,19 @@
 
     def acall(self):
         return context.emitter.send_call_fn(self.name, self.args)
 
 
 __getattr__ = make_module_getattr(
     {
-        "LangchainCallbackHandler": "chainlit.langchain.callbacks",
-        "AsyncLangchainCallbackHandler": "chainlit.langchain.callbacks",
-        "LlamaIndexCallbackHandler": "chainlit.llama_index.callbacks",
-        "HaystackAgentCallbackHandler": "chainlit.haystack.callbacks",
-        "instrument_openai": "chainlit.openai",
+        "LangchainCallbackHandler": "chainlo.langchain.callbacks",
+        "AsyncLangchainCallbackHandler": "chainlo.langchain.callbacks",
+        "LlamaIndexCallbackHandler": "chainlo.llama_index.callbacks",
+        "HaystackAgentCallbackHandler": "chainlo.haystack.callbacks",
+        "instrument_openai": "chainlo.openai",
     }
 )
 
 __all__ = [
     "user_session",
     "CopilotFunction",
     "Action",
```

### Comparing `chainlo-1.0.403/chainlo/action.py` & `chainlo-1.1.404/chainlo/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import uuid
 from typing import Optional
 
-from chainlit.context import context
-from chainlit.telemetry import trace_event
+from chainlo.context import context
+from chainlo.telemetry import trace_event
 from dataclasses_json import DataClassJsonMixin
 from pydantic.dataclasses import Field, dataclass
 
 
 @dataclass
 class Action(DataClassJsonMixin):
     # Name of the action, this should be used in the action_callback
```

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/README.md` & `chainlo-1.1.404/chainlo/agenta_cli/README.md`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/helper.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/cli/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import sys
 import toml
 import click
 import questionary
 from pathlib import Path
 from typing import Any, List, MutableMapping
-from chainlit.agenta_cli.agenta.client.api_models import AppVariant
+from chainlo.agenta_cli.agenta.client.api_models import AppVariant
 
 
 from typing import Any, Optional
 from pathlib import Path
 import toml
 
-from chainlit.agenta_cli.agenta.client.backend.client import AgentaApi
+from chainlo.agenta_cli.agenta.client.backend.client import AgentaApi
 
 BACKEND_URL_SUFFIX = os.environ.get("BACKEND_URL_SUFFIX", "api")
 
 
 def get_global_config(var_name: str) -> Optional[Any]:
     """
     Get the value of a global configuration variable.
```

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/main.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from typing import Union
 from pathlib import Path
 
 import click
 import questionary
 import toml
 
-from chainlit.agenta_cli.agenta.cli import helper
-from chainlit.agenta_cli.agenta.cli import variant_configs
-from chainlit.agenta_cli.agenta.cli import variant_commands
-from chainlit.agenta_cli.agenta.cli import evaluation_commands
+from chainlo.agenta_cli.agenta.cli import helper
+from chainlo.agenta_cli.agenta.cli import variant_configs
+from chainlo.agenta_cli.agenta.cli import variant_commands
+from chainlo.agenta_cli.agenta.cli import evaluation_commands
 
-from chainlit.agenta_cli.agenta.client.backend.client import AgentaApi
+from chainlo.agenta_cli.agenta.client.backend.client import AgentaApi
 
 BACKEND_URL_SUFFIX = os.environ.get("BACKEND_URL_SUFFIX", "api")
 
 
 def print_version(ctx, param, value):
     if not value or ctx.resilient_parsing:
         return
```

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/telemetry.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/cli/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Stdlib Imports
 from uuid import uuid4
 
 # Own Imports
-from chainlit.agenta_cli.agenta.cli import helper
+from chainlo.agenta_cli.agenta.cli import helper
 
 # Third party Imports
 from posthog import Posthog
 
 
 # Load telemetry configuration
 helper.init_telemetry_config()
```

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/variant_commands.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/cli/variant_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 from pathlib import Path
 
 from requests.exceptions import ConnectionError
 
 import click
 import questionary
 import toml
-from chainlit.agenta_cli.agenta.cli import helper
-from chainlit.agenta_cli.agenta.cli.telemetry import event_track
-from chainlit.agenta_cli.agenta.client.api_models import AppVariant, Image
-from chainlit.agenta_cli.agenta.docker.docker_utils import build_tar_docker_container
+from chainlo.agenta_cli.agenta.cli import helper
+from chainlo.agenta_cli.agenta.cli.telemetry import event_track
+from chainlo.agenta_cli.agenta.client.api_models import AppVariant, Image
+from chainlo.agenta_cli.agenta.docker.docker_utils import build_tar_docker_container
 
-from chainlit.agenta_cli.agenta.client.api import add_variant_to_server
-from chainlit.agenta_cli.agenta.client.backend.client import AgentaApi
+from chainlo.agenta_cli.agenta.client.api import add_variant_to_server
+from chainlo.agenta_cli.agenta.client.backend.client import AgentaApi
 
 BACKEND_URL_SUFFIX = os.environ.get("BACKEND_URL_SUFFIX", "api")
 
 
 @click.group()
 def variant():
     """Commands for variants"""
```

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/cli/variant_configs.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/cli/variant_configs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import click
-from chainlit.agenta_cli.agenta.cli import helper
+from chainlo.agenta_cli.agenta.cli import helper
 
 
 @click.group()
 def config():
     """Commands for variants configurations"""
     pass
```

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/Readme.md` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/Readme.md`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/api.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 import toml
 import time
 import click
 from typing import Dict
 from pathlib import Path
-from chainlit.agenta_cli.agenta.client.backend import client
-from chainlit.agenta_cli.agenta.client.api_models import Image
+from chainlo.agenta_cli.agenta.client.backend import client
+from chainlo.agenta_cli.agenta.client.api_models import Image
 from requests.exceptions import RequestException
-from chainlit.agenta_cli.agenta.client.backend.client import AgentaApi
-from chainlit.agenta_cli.agenta.client.exceptions import APIRequestError
+from chainlo.agenta_cli.agenta.client.backend.client import AgentaApi
+from chainlo.agenta_cli.agenta.client.exceptions import APIRequestError
 
 
 def add_variant_to_server(
     app_id: str,
     base_name: str,
     image: Image,
     backend_url: str,
```

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/api_models.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/api_models.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/__init__.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/client.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/client.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/__init__.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/core/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/client_wrapper.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/core/client_wrapper.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/datetime_utils.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/core/jsonable_encoder.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/__init__.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/aggregated_result.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/aggregated_result.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output_extended.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/app_variant_output_extended.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/app_variant_revision.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/app_variant_revision.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/base_output.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/base_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/body_import_testset.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/body_import_testset.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/config_db.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/config_db.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/create_app_output.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/create_app_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/delete_evaluation.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/delete_evaluation.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/docker_env_vars.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/docker_env_vars.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/environment_output.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/environment_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_input.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_input.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_output.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_result.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_scenario_result.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_status_enum.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_status_enum.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_type.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_type.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluation_webhook.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluation_webhook.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluator.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluator.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/evaluator_config.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/evaluator_config.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/feedback.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/feedback.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/get_config_reponse.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/get_config_reponse.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/http_validation_error.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_input.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_input.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_output.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/human_evaluation_scenario_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/image.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/image.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/invite_request.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/invite_request.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/list_api_keys_output.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/list_api_keys_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/llm_run_rate_limit.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/llm_run_rate_limit.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/new_testset.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/new_testset.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/organization.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/organization.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/organization_output.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/organization_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/result.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/result.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/simple_evaluation_output.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/simple_evaluation_output.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/span.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/span.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/template.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/template.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/template_image_info.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/template_image_info.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/test_set_output_response.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/test_set_output_response.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/test_set_simple_response.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/test_set_simple_response.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/trace.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/trace.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/uri.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/uri.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/validation_error.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/backend/types/variant_action.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/backend/types/variant_action.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/client/client.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/client/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 import time
 import click
 from pathlib import Path
 from typing import List, Optional, Dict, Any
 
 import requests
-from chainlit.agenta_cli.agenta.client.api_models import AppVariant, Image, VariantConfigPayload
+from chainlo.agenta_cli.agenta.client.api_models import AppVariant, Image, VariantConfigPayload
 from docker.models.images import Image as DockerImage
 from requests.exceptions import RequestException
 
 BACKEND_URL_SUFFIX = os.environ.get("BACKEND_URL_SUFFIX", "api")
 
 
 class APIRequestError(Exception):
```

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/config.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/config.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/docker/docker_utils.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/docker/docker_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import shutil
 import tarfile
 import tempfile
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 import docker
-from chainlit.agenta_cli.agenta.config import settings
+from chainlo.agenta_cli.agenta.config import settings
 from docker.models.images import Image
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 
 DEBUG = False
```

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/__init__.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/agenta_decorator.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/agenta_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from tempfile import NamedTemporaryFile
 from typing import Any, Callable, Dict, Optional, Tuple, List, Union
 
 from fastapi import Body, FastAPI, UploadFile
 from fastapi.responses import JSONResponse
 from fastapi.middleware.cors import CORSMiddleware
 
-import chainlit.agenta_cli.agenta
+import chainlo.agenta_cli.agenta
 from .context import save_context
 from .router import router as router
 from .types import (
     Context,
     DictInput,
     FloatParam,
     InFile,
@@ -28,15 +28,15 @@
     TextParam,
     MessagesInput,
     FileInputURL,
     FuncResponse,
     BinaryParam,
 )
 
-from chainlit.server import app
+from chainlo.server import app
 
 # app = FastAPI()
 
 # origins = [
 #     "*",
 # ]
```

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/agenta_init.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/agenta_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from chainlit.agenta_cli.agenta.client.exceptions import APIRequestError
-from chainlit.agenta_cli.agenta.client.backend.client import AgentaApi
+from chainlo.agenta_cli.agenta.client.exceptions import APIRequestError
+from chainlo.agenta_cli.agenta.client.backend.client import AgentaApi
 import os
 import logging
 from typing import Any, Optional
 
 from .utils.globals import set_global
 
 logger = logging.getLogger(__name__)
```

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/context.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/context.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/types.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/types.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/utils/helper/openai_cost.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/utils/helper/openai_cost.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/sdk/utils/preinit.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/sdk/utils/preinit.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/compose_email/app.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/compose_email/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/extract_data_to_json/app.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/extract_data_to_json/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/agenta/templates/simple_prompt/app.py` & `chainlo-1.1.404/chainlo/agenta_cli/agenta/templates/simple_prompt/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/pyproject.toml-ex` & `chainlo-1.1.404/chainlo/agenta_cli/pyproject.toml-ex`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/simple_langchain/app.py` & `chainlo-1.1.404/chainlo/agenta_cli/tests/example_projects/simple_langchain/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/agenta.py` & `chainlo-1.1.404/chainlo/agenta_cli/tests/example_projects/test2/agenta.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/agenta_cli/tests/example_projects/test2/app.py` & `chainlo-1.1.404/chainlo/agenta_cli/tests/example_projects/test2/app.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/auth.py` & `chainlo-1.1.404/chainlo/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 from datetime import datetime, timedelta
 from typing import Any, Dict
 
 import jwt
-from chainlit.config import config
-from chainlit.data import get_data_layer
-from chainlit.oauth_providers import get_configured_oauth_providers
-from chainlit.user import User
+from chainlo.config import config
+from chainlo.data import get_data_layer
+from chainlo.oauth_providers import get_configured_oauth_providers
+from chainlo.user import User
 from fastapi import Depends, HTTPException
 from fastapi.security import OAuth2PasswordBearer
 
 reuseable_oauth = OAuth2PasswordBearer(tokenUrl="/login", auto_error=False)
 
 
 def get_jwt_secret():
```

### Comparing `chainlo-1.0.403/chainlo/cache.py` & `chainlo-1.1.404/chainlo/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import threading
 
-from chainlit.config import config
-from chainlit.logger import logger
+from chainlo.config import config
+from chainlo.logger import logger
 
 
 def init_lc_cache():
     use_cache = config.project.cache is True and config.run.no_cache is False
 
     if use_cache:
         try:
```

### Comparing `chainlo-1.0.403/chainlo/chat_settings.py` & `chainlo-1.1.404/chainlo/chat_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List
 
-from chainlit.context import context
-from chainlit.input_widget import InputWidget
+from chainlo.context import context
+from chainlo.input_widget import InputWidget
 from pydantic.dataclasses import Field, dataclass
 
 
 @dataclass
 class ChatSettings:
     """Useful to create chat settings that the user can change."""
```

### Comparing `chainlo-1.0.403/chainlo/cli/__init__.py` & `chainlo-1.1.404/chainlo/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 
 import click
 import nest_asyncio
 import uvicorn
 
 nest_asyncio.apply()
 
-from chainlit.auth import ensure_jwt_secret
-from chainlit.cache import init_lc_cache
-from chainlit.cli.utils import check_file
-from chainlit.config import (
+from chainlo.auth import ensure_jwt_secret
+from chainlo.cache import init_lc_cache
+from chainlo.cli.utils import check_file
+from chainlo.config import (
     BACKEND_ROOT,
     DEFAULT_HOST,
     DEFAULT_PORT,
     config,
     init_config,
     load_module,
 )
-from chainlit.logger import logger
-from chainlit.markdown import init_markdown
-from chainlit.secret import random_secret
-from chainlit.server import app, register_wildcard_route_handler
-from chainlit.telemetry import trace_event
+from chainlo.logger import logger
+from chainlo.markdown import init_markdown
+from chainlo.secret import random_secret
+from chainlo.server import app, register_wildcard_route_handler
+from chainlo.telemetry import trace_event
 
 
 # Create the main command group for Chainlit CLI
 @click.group(context_settings={"auto_envvar_prefix": "CHAINLIT"})
 @click.version_option(prog_name="Chainlit")
 def cli():
     return
```

### Comparing `chainlo-1.0.403/chainlo/cli/utils.py` & `chainlo-1.1.404/chainlo/cli/utils.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/config.py` & `chainlo-1.1.404/chainlo/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 import os
 import sys
 from importlib import util
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Union
 
 import tomli
-from chainlit.logger import logger
-from chainlit.version import __version__
+from chainlo.logger import logger
+from chainlo.version import __version__
 from dataclasses_json import DataClassJsonMixin
 from pydantic.dataclasses import Field, dataclass
 from starlette.datastructures import Headers
 
 if TYPE_CHECKING:
-    from chainlit.action import Action
-    from chainlit.types import ChatProfile, ThreadDict
-    from chainlit.user import User
+    from chainlo.action import Action
+    from chainlo.types import ChatProfile, ThreadDict
+    from chainlo.user import User
     from fastapi import Request, Response
 
 
 BACKEND_ROOT = os.path.dirname(__file__)
 PACKAGE_ROOT = os.path.dirname(os.path.dirname(BACKEND_ROOT))
 TRANSLATIONS_DIR = os.path.join(BACKEND_ROOT, "translations")
```

### Comparing `chainlo-1.0.403/chainlo/context.py` & `chainlo-1.1.404/chainlo/context.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import asyncio
 import uuid
 from contextvars import ContextVar
 from typing import TYPE_CHECKING, Dict, Optional, Union, List
 
-from chainlit.session import HTTPSession, WebsocketSession
+from chainlo.session import HTTPSession, WebsocketSession
 from lazify import LazyProxy
 
 if TYPE_CHECKING:
-    from chainlit.emitter import BaseChainlitEmitter
-    from chainlit.user import PersistedUser, User
-    from chainlit.step import Step
+    from chainlo.emitter import BaseChainlitEmitter
+    from chainlo.user import PersistedUser, User
+    from chainlo.step import Step
 
 
 class ChainlitContextException(Exception):
     def __init__(self, msg="Chainlit context not found", *args, **kwargs):
         super().__init__(msg, *args, **kwargs)
 
 
@@ -25,15 +25,15 @@
 
     @property
     def current_step(self):
         if self.active_steps:
             return self.active_steps[-1]
 
     def __init__(self, session: Union["HTTPSession", "WebsocketSession"]):
-        from chainlit.emitter import BaseChainlitEmitter, ChainlitEmitter
+        from chainlo.emitter import BaseChainlitEmitter, ChainlitEmitter
 
         self.loop = asyncio.get_running_loop()
         self.session = session
         self.active_steps = []
         if isinstance(self.session, HTTPSession):
             self.emitter = BaseChainlitEmitter(self.session)
         elif isinstance(self.session, WebsocketSession):
```

### Comparing `chainlo-1.0.403/chainlo/copilot/dist/assets/logo_dark-2a3cf740.svg` & `chainlo-1.1.404/chainlo/copilot/dist/assets/logo_dark-2a3cf740.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/copilot/dist/assets/logo_light-b078e7bc.svg` & `chainlo-1.1.404/chainlo/copilot/dist/assets/logo_light-b078e7bc.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/copilot/dist/index.js` & `chainlo-1.1.404/chainlo/copilot/dist/index.js`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/data/__init__.py` & `chainlo-1.1.404/chainlo/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import functools
 import json
 import os
 from collections import deque
 from typing import TYPE_CHECKING, Dict, List, Optional, Union
 
 import aiofiles
-from chainlit.config import config
-from chainlit.context import context
-from chainlit.logger import logger
-from chainlit.session import WebsocketSession
-from chainlit.types import Feedback, Pagination, ThreadDict, ThreadFilter
-from chainlit.user import PersistedUser, User, UserDict
+from chainlo.config import config
+from chainlo.context import context
+from chainlo.logger import logger
+from chainlo.session import WebsocketSession
+from chainlo.types import Feedback, Pagination, ThreadDict, ThreadFilter
+from chainlo.user import PersistedUser, User, UserDict
 from literalai import Attachment
 from literalai import Feedback as ClientFeedback
 from literalai import PageInfo, PaginatedResponse
 from literalai import Step as ClientStep
 from literalai.step import StepDict as ClientStepDict
 from literalai.thread import NumberListFilter, StringFilter, StringListFilter
 from literalai.thread import ThreadFilter as ClientThreadFilter
 
 if TYPE_CHECKING:
-    from chainlit.element import Element, ElementDict
-    from chainlit.step import FeedbackDict, StepDict
+    from chainlo.element import Element, ElementDict
+    from chainlo.step import FeedbackDict, StepDict
 
 
 def queue_until_user_message():
     def decorator(method):
         @functools.wraps(method)
         async def wrapper(self, *args, **kwargs):
             if (
```

### Comparing `chainlo-1.0.403/chainlo/element.py` & `chainlo-1.1.404/chainlo/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import json
 import uuid
 from enum import Enum
 from io import BytesIO
 from typing import Any, ClassVar, List, Literal, Optional, TypedDict, TypeVar, Union
 
 import filetype
-from chainlit.context import context
-from chainlit.data import get_data_layer
-from chainlit.logger import logger
-from chainlit.telemetry import trace_event
-from chainlit.types import FileDict
+from chainlo.context import context
+from chainlo.data import get_data_layer
+from chainlo.logger import logger
+from chainlo.telemetry import trace_event
+from chainlo.types import FileDict
 from pydantic.dataclasses import Field, dataclass
 from syncer import asyncio
 
 mime_types = {
     "text": "text/plain",
     "tasklist": "application/json",
     "plotly": "application/json",
```

### Comparing `chainlo-1.0.403/chainlo/emitter.py` & `chainlo-1.1.404/chainlo/emitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import asyncio
 import uuid
 from typing import Any, Dict, List, Literal, Optional, Union, cast
 
-from chainlit.data import get_data_layer
-from chainlit.element import Element, File
-from chainlit.logger import logger
-from chainlit.message import Message
-from chainlit.session import BaseSession, WebsocketSession
-from chainlit.step import StepDict
-from chainlit.types import (
+from chainlo.data import get_data_layer
+from chainlo.element import Element, File
+from chainlo.logger import logger
+from chainlo.message import Message
+from chainlo.session import BaseSession, WebsocketSession
+from chainlo.step import StepDict
+from chainlo.types import (
     AskActionResponse,
     AskSpec,
     FileDict,
     FileReference,
     ThreadDict,
     UIMessagePayload,
 )
-from chainlit.user import PersistedUser
+from chainlo.user import PersistedUser
 from literalai.helper import utc_now
 from socketio.exceptions import TimeoutError
 
 
 class BaseChainlitEmitter:
     """
     Chainlit Emitter Stub class. This class is used for testing purposes.
```

### Comparing `chainlo-1.0.403/chainlo/frontend/dist/assets/index-7bc2ef31.js` & `chainlo-1.1.404/chainlo/frontend/dist/assets/index-7bc2ef31.js`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/frontend/dist/assets/index-d088547c.css` & `chainlo-1.1.404/chainlo/frontend/dist/assets/index-d088547c.css`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/frontend/dist/assets/logo_dark-2a3cf740.svg` & `chainlo-1.1.404/chainlo/frontend/dist/assets/logo_dark-2a3cf740.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/frontend/dist/assets/logo_light-b078e7bc.svg` & `chainlo-1.1.404/chainlo/frontend/dist/assets/logo_light-b078e7bc.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/frontend/dist/assets/react-plotly-70086d41.js` & `chainlo-1.1.404/chainlo/frontend/dist/assets/react-plotly-70086d41.js`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/frontend/dist/favicon.svg` & `chainlo-1.1.404/chainlo/frontend/dist/favicon.svg`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/frontend/dist/index.html` & `chainlo-1.1.404/chainlo/frontend/dist/index.html`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/haystack/callbacks.py` & `chainlo-1.1.404/chainlo/haystack/callbacks.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import re
 from typing import Any, Generic, List, Optional, TypeVar
 
-from chainlit.context import context
-from chainlit.step import Step
-from chainlit.sync import run_sync
+from chainlo.context import context
+from chainlo.step import Step
+from chainlo.sync import run_sync
 from haystack.agents import Agent, Tool
 from haystack.agents.agent_step import AgentStep
 from literalai.helper import utc_now
 
-from chainlit import Message
+from chainlo import Message
 
 T = TypeVar("T")
 
 
 class Stack(Generic[T]):
     def __init__(self) -> None:
         self.items: List[T] = []
```

### Comparing `chainlo-1.0.403/chainlo/hello.py` & `chainlo-1.1.404/chainlo/hello.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This is a simple example of a chainlit app.
 
 from typing import Optional
 
-from chainlit import AskUserMessage, Message, on_chat_start
+from chainlo import AskUserMessage, Message, on_chat_start
 
-import chainlit as cl
+import chainlo as cl
 
-from chainlit.input_widget import Select, Switch, Slider
+from chainlo.input_widget import Select, Switch, Slider
 
 
 @cl.on_chat_start
 async def start():
     settings = await cl.ChatSettings(
         [
             Select(
```

### Comparing `chainlo-1.0.403/chainlo/input_widget.py` & `chainlo-1.1.404/chainlo/input_widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod
 from collections import defaultdict
 from typing import Any, Dict, List, Optional
 
-from chainlit.types import InputWidgetType
+from chainlo.types import InputWidgetType
 from pydantic.dataclasses import Field, dataclass
 
 
 @dataclass
 class InputWidget:
     id: str
     label: str
```

### Comparing `chainlo-1.0.403/chainlo/langchain/callbacks.py` & `chainlo-1.1.404/chainlo/langchain/callbacks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import time
 from typing import Any, Dict, List, Optional, TypedDict, Union
 from uuid import UUID
 
-from chainlit.context import context_var
-from chainlit.message import Message
-from chainlit.step import Step
+from chainlo.context import context_var
+from chainlo.message import Message
+from chainlo.step import Step
 from langchain.callbacks.tracers.base import BaseTracer
 from langchain.callbacks.tracers.schemas import Run
 from langchain.schema import BaseMessage
 from langchain.schema.output import ChatGenerationChunk, GenerationChunk
 from langchain_core.outputs import ChatGenerationChunk, GenerationChunk
 from literalai import ChatGeneration, CompletionGeneration, GenerationMessage
 from literalai.helper import utc_now
```

### Comparing `chainlo-1.0.403/chainlo/langflow/__init__.py` & `chainlo-1.1.404/chainlo/langflow/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from chainlit.utils import check_module_version
+from chainlo.utils import check_module_version
 
 if not check_module_version("langflow", "0.1.4"):
     raise ValueError(
         "Expected Langflow version >= 0.1.4. Run `pip install langflow --upgrade`"
     )
 
 from typing import Dict, Optional, Union
 
 import httpx
-from chainlit.telemetry import trace_event
+from chainlo.telemetry import trace_event
 
 
 async def load_flow(schema: Union[Dict, str], tweaks: Optional[Dict] = None):
     from langflow import load_flow_from_json
 
     trace_event("load_langflow")
```

### Comparing `chainlo-1.0.403/chainlo/llama_index/callbacks.py` & `chainlo-1.1.404/chainlo/llama_index/callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Dict, List, Optional
 
-from chainlit.context import context_var
-from chainlit.element import Text
-from chainlit.step import Step, StepType
+from chainlo.context import context_var
+from chainlo.element import Text
+from chainlo.step import Step, StepType
 from literalai import ChatGeneration, CompletionGeneration, GenerationMessage
 from literalai.helper import utc_now
 from llama_index.core.callbacks import TokenCountingHandler
 from llama_index.core.callbacks.schema import CBEventType, EventPayload
 from llama_index.core.llms import ChatMessage, ChatResponse, CompletionResponse
 
 DEFAULT_IGNORE = [
```

### Comparing `chainlo-1.0.403/chainlo/markdown.py` & `chainlo-1.1.404/chainlo/markdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from chainlit.logger import logger
+from chainlo.logger import logger
 
 # Default chainlit.md file created if none exists
 DEFAULT_MARKDOWN_STR = """# Welcome to Chainlit! 🚀🤖
 
 Hi there, Developer! 👋 We're excited to have you on board. Chainlit is a powerful tool designed to help you prototype, debug and share applications built on top of LLMs.
 
 ## Useful Links 🔗
```

### Comparing `chainlo-1.0.403/chainlo/message.py` & `chainlo-1.1.404/chainlo/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import asyncio
 import json
 import time
 import uuid
 from abc import ABC
 from typing import Dict, List, Optional, Union, cast
 
-from chainlit.action import Action
-from chainlit.config import config
-from chainlit.context import context
-from chainlit.data import get_data_layer
-from chainlit.element import ElementBased
-from chainlit.logger import logger
-from chainlit.step import StepDict
-from chainlit.telemetry import trace_event
-from chainlit.types import (
+from chainlo.action import Action
+from chainlo.config import config
+from chainlo.context import context
+from chainlo.data import get_data_layer
+from chainlo.element import ElementBased
+from chainlo.logger import logger
+from chainlo.step import StepDict
+from chainlo.telemetry import trace_event
+from chainlo.types import (
     AskActionResponse,
     AskActionSpec,
     AskFileResponse,
     AskFileSpec,
     AskSpec,
     FileDict,
 )
```

### Comparing `chainlo-1.0.403/chainlo/oauth_providers.py` & `chainlo-1.1.404/chainlo/oauth_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import os
 import urllib.parse
 from typing import Dict, List, Optional, Tuple
 
 import httpx
-from chainlit.user import User
+from chainlo.user import User
 from fastapi import HTTPException
 
 
 class OAuthProvider:
     id: str
     env: List[str]
     client_id: str
```

### Comparing `chainlo-1.0.403/chainlo/openai/__init__.py` & `chainlo-1.1.404/chainlo/openai/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Union
 
-from chainlit.context import get_context
-from chainlit.step import Step
-from chainlit.sync import run_sync
-from chainlit.utils import check_module_version
+from chainlo.context import get_context
+from chainlo.step import Step
+from chainlo.sync import run_sync
+from chainlo.utils import check_module_version
 from literalai import ChatGeneration, CompletionGeneration
 from literalai.helper import timestamp_utc
 
 
 def instrument_openai():
     if not check_module_version("openai", "1.0.0"):
         raise ValueError(
```

### Comparing `chainlo-1.0.403/chainlo/playground/config.py` & `chainlo-1.1.404/chainlo/playground/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict
 
-from chainlit.playground.provider import BaseProvider
-from chainlit.playground.providers import (
+from chainlo.playground.provider import BaseProvider
+from chainlo.playground.providers import (
     Anthropic,
     AzureChatOpenAI,
     AzureOpenAI,
     ChatOpenAI,
     OpenAI,
     ChatVertexAI,
     GenerationVertexAI,
```

### Comparing `chainlo-1.0.403/chainlo/playground/provider.py` & `chainlo-1.1.404/chainlo/playground/provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
 from typing import Any, Dict, List, Optional, Union
 
-from chainlit.config import config
-from chainlit.telemetry import trace_event
-from chainlit.types import GenerationRequest
+from chainlo.config import config
+from chainlo.telemetry import trace_event
+from chainlo.types import GenerationRequest
 from fastapi import HTTPException
 from literalai import BaseGeneration, ChatGeneration, GenerationMessage
 from pydantic.dataclasses import dataclass
 
-from chainlit import input_widget
+from chainlo import input_widget
 
 
 @dataclass
 class BaseProvider:
     id: str
     name: str
     env_vars: Dict[str, str]
```

### Comparing `chainlo-1.0.403/chainlo/playground/providers/anthropic.py` & `chainlo-1.1.404/chainlo/playground/providers/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from chainlit.input_widget import Select, Slider, Tags
-from chainlit.playground.provider import BaseProvider
+from chainlo.input_widget import Select, Slider, Tags
+from chainlo.playground.provider import BaseProvider
 from fastapi import HTTPException
 from fastapi.responses import StreamingResponse
 from literalai import GenerationMessage
 
 
 class AnthropicProvider(BaseProvider):
     def message_to_string(self, message: GenerationMessage) -> str:
```

### Comparing `chainlo-1.0.403/chainlo/playground/providers/huggingface.py` & `chainlo-1.1.404/chainlo/playground/providers/huggingface.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
-from chainlit.input_widget import Slider
-from chainlit.playground.provider import BaseProvider
-from chainlit.sync import make_async
+from chainlo.input_widget import Slider
+from chainlo.playground.provider import BaseProvider
+from chainlo.sync import make_async
 from fastapi import HTTPException
 from fastapi.responses import StreamingResponse
 from pydantic.dataclasses import dataclass
 
 
 @dataclass
 class BaseHuggingFaceProvider(BaseProvider):
```

### Comparing `chainlo-1.0.403/chainlo/playground/providers/langchain.py` & `chainlo-1.1.404/chainlo/playground/providers/langchain.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Union
 
-from chainlit.input_widget import InputWidget
-from chainlit.playground.provider import BaseProvider
-from chainlit.sync import make_async
+from chainlo.input_widget import InputWidget
+from chainlo.playground.provider import BaseProvider
+from chainlo.sync import make_async
 from fastapi.responses import StreamingResponse
 from literalai import GenerationMessage
 
 
 class LangchainGenericProvider(BaseProvider):
     from langchain.chat_models.base import BaseChatModel
     from langchain.llms.base import LLM
```

### Comparing `chainlo-1.0.403/chainlo/playground/providers/openai.py` & `chainlo-1.1.404/chainlo/playground/providers/openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import json
 from contextlib import contextmanager
 
-from chainlit.input_widget import Select, Slider, Tags
-from chainlit.playground.provider import BaseProvider
+from chainlo.input_widget import Select, Slider, Tags
+from chainlo.playground.provider import BaseProvider
 from fastapi import HTTPException
 from fastapi.responses import StreamingResponse
 
 
 def stringify_function_call(function_call):
     if isinstance(function_call, dict):
         _function_call = function_call.copy()
```

### Comparing `chainlo-1.0.403/chainlo/playground/providers/vertexai.py` & `chainlo-1.1.404/chainlo/playground/providers/vertexai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import chainlit as cl
+import chainlo as cl
 from fastapi import HTTPException
 
 from fastapi.responses import StreamingResponse
 
-from chainlit.input_widget import Select, Slider, Tags
-from chainlit.playground.provider import BaseProvider
+from chainlo.input_widget import Select, Slider, Tags
+from chainlo.playground.provider import BaseProvider
 
 vertexai_common_inputs = [
     Slider(
         id="temperature",
         label="Temperature",
         min=0.0,
         max=0.99,
```

### Comparing `chainlo-1.0.403/chainlo/server.py` & `chainlo-1.1.404/chainlo/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,51 +2,51 @@
 import json
 import mimetypes
 import re
 import shutil
 import urllib.parse
 from typing import Any, Optional, Union
 
-from chainlit.oauth_providers import get_oauth_provider
-from chainlit.secret import random_secret
+from chainlo.oauth_providers import get_oauth_provider
+from chainlo.secret import random_secret
 
 mimetypes.add_type("application/javascript", ".js")
 mimetypes.add_type("text/css", ".css")
 
 import asyncio
 import os
 import webbrowser
 from contextlib import asynccontextmanager
 from pathlib import Path
 
-from chainlit.auth import create_jwt, get_configuration, get_current_user
-from chainlit.config import (
+from chainlo.auth import create_jwt, get_configuration, get_current_user
+from chainlo.config import (
     APP_ROOT,
     BACKEND_ROOT,
     DEFAULT_HOST,
     FILES_DIRECTORY,
     PACKAGE_ROOT,
     config,
     load_module,
     reload_config,
 )
-from chainlit.data import get_data_layer
-from chainlit.data.acl import is_thread_author
-from chainlit.logger import logger
-from chainlit.markdown import get_markdown_str
-from chainlit.playground.config import get_llm_providers
-from chainlit.telemetry import trace_event
-from chainlit.types import (
+from chainlo.data import get_data_layer
+from chainlo.data.acl import is_thread_author
+from chainlo.logger import logger
+from chainlo.markdown import get_markdown_str
+from chainlo.playground.config import get_llm_providers
+from chainlo.telemetry import trace_event
+from chainlo.types import (
     DeleteThreadRequest,
     GenerationRequest,
     GetThreadsRequest,
     Theme,
     UpdateFeedbackRequest,
 )
-from chainlit.user import PersistedUser, User
+from chainlo.user import PersistedUser, User
 from fastapi import (
     Depends,
     FastAPI,
     HTTPException,
     Query,
     Request,
     Response,
@@ -156,24 +156,24 @@
 
 app = FastAPI(lifespan=lifespan)
 
 app.mount("/public", StaticFiles(directory="public", check_dir=False), name="public")
 app.mount(
     "/assets",
     StaticFiles(
-        packages=[("chainlit", os.path.join(build_dir, "assets"))],
+        packages=[("chainlo", os.path.join(build_dir, "assets"))],
         follow_symlink=config.project.follow_symlink,
     ),
     name="assets",
 )
 
 app.mount(
     "/copilot",
     StaticFiles(
-        packages=[("chainlit", copilot_build_dir)],
+        packages=[("chainlo", copilot_build_dir)],
         follow_symlink=config.project.follow_symlink,
     ),
     name="copilot",
 )
 
 
 app.add_middleware(
@@ -634,15 +634,15 @@
 async def upload_file(
     session_id: str,
     file: UploadFile,
     current_user: Annotated[
         Union[None, User, PersistedUser], Depends(get_current_user)
     ],
 ):
-    from chainlit.session import WebsocketSession
+    from chainlo.session import WebsocketSession
 
     session = WebsocketSession.get_by_id(session_id)
 
     if not session:
         raise HTTPException(
             status_code=404,
             detail="Session not found",
@@ -667,15 +667,15 @@
 
 
 @app.get("/project/file/{file_id}")
 async def get_file(
     file_id: str,
     session_id: Optional[str] = None,
 ):
-    from chainlit.session import WebsocketSession
+    from chainlo.session import WebsocketSession
 
     session = WebsocketSession.get_by_id(session_id) if session_id else None
 
     if not session:
         raise HTTPException(
             status_code=404,
             detail="Session not found",
@@ -749,8 +749,8 @@
         html_template = get_html_template()
         """Serve the UI files."""
         response = HTMLResponse(content=html_template, status_code=200)
 
         return response
 
 
-import chainlit.socket  # noqa
+import chainlo.socket  # noqa
```

### Comparing `chainlo-1.0.403/chainlo/session.py` & `chainlo-1.1.404/chainlo/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
     List,
     Literal,
     Optional,
     Union,
 )
 
 import aiofiles
-from chainlit.logger import logger
+from chainlo.logger import logger
 
 if TYPE_CHECKING:
-    from chainlit.message import Message
-    from chainlit.step import Step
-    from chainlit.types import FileDict, FileReference
-    from chainlit.user import PersistedUser, User
+    from chainlo.message import Message
+    from chainlo.step import Step
+    from chainlo.types import FileDict, FileReference
+    from chainlo.user import PersistedUser, User
 
 ClientType = Literal["app", "copilot", "teams", "slack"]
 
 
 class JSONEncoderIgnoreNonSerializable(json.JSONEncoder):
     def default(self, obj):
         try:
@@ -85,15 +85,15 @@
         mime: str,
         path: Optional[str] = None,
         content: Optional[Union[bytes, str]] = None,
     ):
         return None
 
     def to_persistable(self) -> Dict:
-        from chainlit.user_session import user_sessions
+        from chainlo.user_session import user_sessions
 
         user_session = user_sessions.get(self.id) or {}  # type: Dict
         user_session["chat_settings"] = self.chat_settings
         user_session["chat_profile"] = self.chat_profile
         metadata = clean_metadata(user_session)
         return metadata
 
@@ -186,15 +186,15 @@
         self.files = {}  # type: Dict[str, "FileDict"]
 
         ws_sessions_id[self.id] = self
         ws_sessions_sid[socket_id] = self
 
     @property
     def files_dir(self):
-        from chainlit.config import FILES_DIRECTORY
+        from chainlo.config import FILES_DIRECTORY
 
         return FILES_DIRECTORY / self.id
 
     async def persist_file(
         self,
         name: str,
         mime: str,
```

### Comparing `chainlo-1.0.403/chainlo/socket.py` & `chainlo-1.1.404/chainlo/socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import asyncio
 import json
 import time
 import uuid
 from typing import Any, Dict, Literal
 
-from chainlit.action import Action
-from chainlit.auth import get_current_user, require_login
-from chainlit.config import config
-from chainlit.context import init_ws_context
-from chainlit.data import get_data_layer
-from chainlit.logger import logger
-from chainlit.message import ErrorMessage, Message
-from chainlit.server import socket
-from chainlit.session import WebsocketSession
-from chainlit.telemetry import trace_event
-from chainlit.types import UIMessagePayload
-from chainlit.user_session import user_sessions
+from chainlo.action import Action
+from chainlo.auth import get_current_user, require_login
+from chainlo.config import config
+from chainlo.context import init_ws_context
+from chainlo.data import get_data_layer
+from chainlo.logger import logger
+from chainlo.message import ErrorMessage, Message
+from chainlo.server import socket
+from chainlo.session import WebsocketSession
+from chainlo.telemetry import trace_event
+from chainlo.types import UIMessagePayload
+from chainlo.user_session import user_sessions
 
 
 def restore_existing_session(sid, session_id, emit_fn, emit_call_fn):
     """Restore a session from the sessionId provided by the client."""
     if session := WebsocketSession.get_by_id(session_id):
         session.restore(new_socket_id=sid)
         session.emit = emit_fn
```

### Comparing `chainlo-1.0.403/chainlo/step.py` & `chainlo-1.1.404/chainlo/step.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 import inspect
 import json
 import time
 import uuid
 from functools import wraps
 from typing import Callable, Dict, List, Optional, TypedDict, Union
 
-from chainlit.config import config
-from chainlit.context import context, local_steps
-from chainlit.data import get_data_layer
-from chainlit.element import Element
-from chainlit.logger import logger
-from chainlit.telemetry import trace_event
-from chainlit.types import FeedbackDict
+from chainlo.config import config
+from chainlo.context import context, local_steps
+from chainlo.data import get_data_layer
+from chainlo.element import Element
+from chainlo.logger import logger
+from chainlo.telemetry import trace_event
+from chainlo.types import FeedbackDict
 from literalai import BaseGeneration
 from literalai.helper import utc_now
 from literalai.step import StepType, TrueStepType
 
 
 class StepDict(TypedDict, total=False):
     name: str
```

### Comparing `chainlo-1.0.403/chainlo/sync.py` & `chainlo-1.1.404/chainlo/sync.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 else:
     from typing_extensions import ParamSpec
 
 import asyncio
 import threading
 
 from asyncer import asyncify
-from chainlit.context import context_var
+from chainlo.context import context_var
 from syncer import sync
 
 make_async = asyncify
 
 T_Retval = TypeVar("T_Retval")
 T_ParamSpec = ParamSpec("T_ParamSpec")
 T = TypeVar("T")
```

### Comparing `chainlo-1.0.403/chainlo/telemetry.py` & `chainlo-1.1.404/chainlo/telemetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
     from opentelemetry.trace import Tracer
 
 import hashlib
 import logging
 from functools import wraps
 from socket import gethostname
 
-from chainlit.config import config
-from chainlit.version import __version__
+from chainlo.config import config
+from chainlo.version import __version__
 
 
 class ChainlitTelemetry:
     def __init__(self):
         self._tracer = None
 
     # Patch uptrace.py to hash the hostname to avoid leaking it.
```

### Comparing `chainlo-1.0.403/chainlo/translations/de.json` & `chainlo-1.1.404/chainlo/translations/de.json`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/translations/en-US.json` & `chainlo-1.1.404/chainlo/translations/en-US.json`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/translations/pt-BR.json` & `chainlo-1.1.404/chainlo/translations/pt-BR.json`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/types.py` & `chainlo-1.1.404/chainlo/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from enum import Enum
 from typing import TYPE_CHECKING, Dict, List, Literal, Optional, TypedDict, Union
 
 if TYPE_CHECKING:
-    from chainlit.element import ElementDict
-    from chainlit.user import UserDict
-    from chainlit.step import StepDict
+    from chainlo.element import ElementDict
+    from chainlo.user import UserDict
+    from chainlo.step import StepDict
 
 from dataclasses_json import DataClassJsonMixin
 from literalai import ChatGeneration, CompletionGeneration
 from pydantic import BaseModel
 from pydantic.dataclasses import dataclass
 
 InputWidgetType = Literal[
```

### Comparing `chainlo-1.0.403/chainlo/user.py` & `chainlo-1.1.404/chainlo/user.py`

 * *Files identical despite different names*

### Comparing `chainlo-1.0.403/chainlo/user_session.py` & `chainlo-1.1.404/chainlo/user_session.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Dict
 
-from chainlit.context import context
+from chainlo.context import context
 
 user_sessions: Dict[str, Dict] = {}
 
 
 class UserSession:
     """
     Developer facing user session class.
```

### Comparing `chainlo-1.0.403/chainlo/utils.py` & `chainlo-1.1.404/chainlo/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import functools
 import importlib
 import inspect
 from typing import Callable
 
-from chainlit.context import context
-from chainlit.logger import logger
-from chainlit.message import ErrorMessage
+from chainlo.context import context
+from chainlo.logger import logger
+from chainlo.message import ErrorMessage
 from packaging import version
 
 
 def wrap_user_function(user_function: Callable, with_task=False) -> Callable:
     """
     Wraps a user-defined function to accept arguments as a dictionary.
```

### Comparing `chainlo-1.0.403/pyproject.toml` & `chainlo-1.1.404/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainlo"
-version = "1.0.403"
+version = "1.1.404"
 keywords = ['LLM', 'Agents', 'gen ai', 'chat ui', 'chatbot ui', 'openai', 'copilot', 'langchain', 'conversational ai']
 description = "Build Conversational AI."
 authors = ["Chainlo"]
 license = "Apache-2.0 license"
 repository = "https://github.com/Chainlit/chainlit"
 readme = "README.md"
 exclude = [
@@ -14,15 +14,15 @@
 include = [
     "**/frontend/dist/**/*",
     "**/copilot/dist/**/*",
 ]
 
 [tool.poetry.scripts]
 # command_name = module_for_handler : function_for_handler
-chainlit = 'chainlo.cli:cli'
+chainlo = 'chainlo.cli:cli'
 agenta = "chainlo.agenta_cli.agenta.cli.main:cli"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0.0"
 httpx = ">=0.23.0"
 literalai = "0.0.300"
 dataclasses_json = "^0.5.7"
```

### Comparing `chainlo-1.0.403/PKG-INFO` & `chainlo-1.1.404/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainlo
-Version: 1.0.403
+Version: 1.1.404
 Summary: Build Conversational AI.
 Home-page: https://github.com/Chainlit/chainlit
 License: Apache-2.0 license
 Keywords: LLM,Agents,gen ai,chat ui,chatbot ui,openai,copilot,langchain,conversational ai
 Author: Chainlo
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
```

