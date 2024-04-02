# Comparing `tmp/pandasai-2.0a8.tar.gz` & `tmp/pandasai-2.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-2.0a8.tar", max compression
+gzip compressed data, was "pandasai-2.0a9.tar", max compression
```

## Comparing `pandasai-2.0a8.tar` & `pandasai-2.0a9.tar`

### file list

```diff
@@ -1,128 +1,128 @@
--rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-2.0a8/LICENSE
-drwxr-xr-x   0        0        0        0 2023-11-20 22:14:04.721024 pandasai-2.0a8/LICENSES/
--rw-r--r--   0        0        0     7206 2024-02-21 10:04:57.962885 pandasai-2.0a8/README.md
--rw-r--r--   0        0        0      682 2024-02-21 10:04:57.967562 pandasai-2.0a8/pandasai/__init__.py
--rw-r--r--   0        0        0       45 2024-02-19 14:59:32.858258 pandasai-2.0a8/pandasai/agent/__init__.py
--rw-r--r--   0        0        0    13699 2024-02-21 10:04:57.967914 pandasai-2.0a8/pandasai/agent/base.py
--rw-r--r--   0        0        0      994 2024-02-19 14:59:32.858993 pandasai-2.0a8/pandasai/agent/callbacks.py
--rw-r--r--   0        0        0     1227 2024-02-19 14:59:32.859598 pandasai-2.0a8/pandasai/config.py
--rw-r--r--   0        0        0      908 2024-02-21 10:04:57.968102 pandasai-2.0a8/pandasai/connectors/__init__.py
--rw-r--r--   0        0        0     8777 2024-02-21 10:04:57.968280 pandasai-2.0a8/pandasai/connectors/airtable.py
--rw-r--r--   0        0        0     7750 2024-02-21 10:04:57.968449 pandasai-2.0a8/pandasai/connectors/base.py
--rw-r--r--   0        0        0     2880 2024-02-21 10:04:57.968631 pandasai-2.0a8/pandasai/connectors/databricks.py
--rw-r--r--   0        0        0     2226 2024-02-21 10:04:57.968768 pandasai-2.0a8/pandasai/connectors/google_big_query.py
--rw-r--r--   0        0        0     4422 2024-02-21 10:04:57.968938 pandasai-2.0a8/pandasai/connectors/pandas.py
--rw-r--r--   0        0        0     4164 2024-02-21 10:04:57.969097 pandasai-2.0a8/pandasai/connectors/polars.py
--rw-r--r--   0        0        0     3834 2024-02-21 10:04:57.969289 pandasai-2.0a8/pandasai/connectors/snowflake.py
--rw-r--r--   0        0        0    18682 2024-02-21 10:04:57.969437 pandasai-2.0a8/pandasai/connectors/sql.py
--rw-r--r--   0        0        0     5871 2024-02-21 10:04:57.969757 pandasai-2.0a8/pandasai/connectors/yahoo_finance.py
--rw-r--r--   0        0        0     1711 2024-02-21 10:04:57.969904 pandasai-2.0a8/pandasai/constants.py
--rw-r--r--   0        0        0      507 2024-02-21 10:04:57.970176 pandasai-2.0a8/pandasai/engine.py
--rw-r--r--   0        0        0     5284 2024-02-21 10:04:57.970349 pandasai-2.0a8/pandasai/exceptions.py
--rw-r--r--   0        0        0      446 2024-02-21 10:04:57.970515 pandasai-2.0a8/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     4613 2024-02-21 10:04:57.971425 pandasai-2.0a8/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     3019 2024-02-21 10:04:57.971578 pandasai-2.0a8/pandasai/helpers/cache.py
--rw-r--r--   0        0        0    22898 2024-02-21 10:04:57.971835 pandasai-2.0a8/pandasai/helpers/code_manager.py
--rw-r--r--   0        0        0     2397 2024-02-21 10:04:57.972019 pandasai-2.0a8/pandasai/helpers/data_sampler.py
--rw-r--r--   0        0        0     4574 2024-02-21 10:04:57.972177 pandasai-2.0a8/pandasai/helpers/dataframe_serializer.py
--rw-r--r--   0        0        0     5062 2024-02-21 10:04:57.972426 pandasai-2.0a8/pandasai/helpers/df_config_manager.py
--rw-r--r--   0        0        0     1378 2024-02-21 10:04:57.972700 pandasai-2.0a8/pandasai/helpers/df_info.py
--rw-r--r--   0        0        0     3236 2024-02-21 10:04:57.972971 pandasai-2.0a8/pandasai/helpers/df_validator.py
--rw-r--r--   0        0        0      526 2024-02-21 10:04:57.973121 pandasai-2.0a8/pandasai/helpers/env.py
--rw-r--r--   0        0        0      928 2024-02-21 10:04:57.973259 pandasai-2.0a8/pandasai/helpers/file_importer.py
--rw-r--r--   0        0        0      725 2024-02-21 10:04:57.973382 pandasai-2.0a8/pandasai/helpers/folder.py
--rw-r--r--   0        0        0     3717 2024-02-21 10:04:57.973750 pandasai-2.0a8/pandasai/helpers/from_google_sheets.py
--rw-r--r--   0        0        0     4273 2024-02-21 10:04:57.973959 pandasai-2.0a8/pandasai/helpers/logger.py
--rw-r--r--   0        0        0     2770 2024-02-19 14:59:43.492203 pandasai-2.0a8/pandasai/helpers/memory.py
--rw-r--r--   0        0        0      447 2023-09-13 09:35:53.943189 pandasai-2.0a8/pandasai/helpers/node_visitors.py
--rw-r--r--   0        0        0      213 2023-11-20 22:14:04.734116 pandasai-2.0a8/pandasai/helpers/openai.py
--rw-r--r--   0        0        0     6019 2024-02-21 10:04:57.974150 pandasai-2.0a8/pandasai/helpers/openai_info.py
--rw-r--r--   0        0        0     3898 2023-09-04 21:53:07.384708 pandasai-2.0a8/pandasai/helpers/optional.py
--rw-r--r--   0        0        0     1976 2024-02-21 10:04:57.974259 pandasai-2.0a8/pandasai/helpers/output_types/__init__.py
--rw-r--r--   0        0        0     4658 2024-02-21 10:04:57.974363 pandasai-2.0a8/pandasai/helpers/output_types/_output_types.py
--rw-r--r--   0        0        0     2310 2024-02-21 10:04:57.974537 pandasai-2.0a8/pandasai/helpers/output_validator.py
--rw-r--r--   0        0        0     2074 2023-11-20 22:14:04.734712 pandasai-2.0a8/pandasai/helpers/path.py
--rw-r--r--   0        0        0     8550 2024-02-21 10:04:57.974714 pandasai-2.0a8/pandasai/helpers/query_exec_tracker.py
--rw-r--r--   0        0        0     2466 2024-02-21 10:04:57.974868 pandasai-2.0a8/pandasai/helpers/request.py
--rw-r--r--   0        0        0     1061 2024-02-21 10:04:57.975042 pandasai-2.0a8/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     8579 2024-02-21 10:04:57.975494 pandasai-2.0a8/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0     2388 2024-02-21 10:04:57.975669 pandasai-2.0a8/pandasai/helpers/skills_manager.py
--rw-r--r--   0        0        0      426 2024-01-19 10:23:41.929740 pandasai-2.0a8/pandasai/helpers/sql.py
--rw-r--r--   0        0        0      435 2024-02-21 10:04:57.975850 pandasai-2.0a8/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     7002 2024-02-21 10:04:57.977815 pandasai-2.0a8/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0      732 2024-02-21 10:04:57.978008 pandasai-2.0a8/pandasai/llm/bamboo_llm.py
--rw-r--r--   0        0        0    13732 2024-02-21 10:04:57.978209 pandasai-2.0a8/pandasai/llm/base.py
--rw-r--r--   0        0        0      640 2024-02-19 14:59:43.493258 pandasai-2.0a8/pandasai/llm/fake.py
--rw-r--r--   0        0        0     2660 2024-02-21 10:04:57.978791 pandasai-2.0a8/pandasai/llm/google_gemini.py
--rw-r--r--   0        0        0     2737 2024-02-21 10:04:57.979108 pandasai-2.0a8/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0     5687 2024-02-21 10:04:57.979290 pandasai-2.0a8/pandasai/llm/google_vertexai.py
--rw-r--r--   0        0        0     4003 2024-02-21 10:04:57.979493 pandasai-2.0a8/pandasai/llm/huggingface_text_gen.py
--rw-r--r--   0        0        0     1168 2024-02-21 10:04:57.979830 pandasai-2.0a8/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     3236 2024-02-21 10:04:57.980594 pandasai-2.0a8/pandasai/llm/openai.py
--rw-r--r--   0        0        0      352 2024-02-21 10:04:57.980893 pandasai-2.0a8/pandasai/pandas/__init__.py
--rw-r--r--   0        0        0      206 2024-02-19 14:59:32.870508 pandasai-2.0a8/pandasai/pipelines/__init__.py
--rw-r--r--   0        0        0      353 2023-11-20 22:14:04.741653 pandasai-2.0a8/pandasai/pipelines/abstract_pipeline.py
--rw-r--r--   0        0        0     1062 2024-02-19 14:59:32.870645 pandasai-2.0a8/pandasai/pipelines/base_logic_unit.py
--rw-r--r--   0        0        0     1438 2024-02-19 14:59:32.870772 pandasai-2.0a8/pandasai/pipelines/chat/cache_lookup.py
--rw-r--r--   0        0        0     1253 2024-02-21 10:04:57.981058 pandasai-2.0a8/pandasai/pipelines/chat/cache_population.py
--rw-r--r--   0        0        0      572 2024-02-21 10:04:57.981190 pandasai-2.0a8/pandasai/pipelines/chat/chat_pipeline_input.py
--rw-r--r--   0        0        0     4344 2024-02-21 10:04:57.981331 pandasai-2.0a8/pandasai/pipelines/chat/code_execution.py
--rw-r--r--   0        0        0     1473 2024-02-21 10:04:57.981483 pandasai-2.0a8/pandasai/pipelines/chat/code_generator.py
--rw-r--r--   0        0        0     1479 2024-02-21 10:04:57.981659 pandasai-2.0a8/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline.py
--rw-r--r--   0        0        0      240 2024-02-19 14:59:32.872442 pandasai-2.0a8/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline_input.py
--rw-r--r--   0        0        0     3037 2024-02-21 10:04:57.981791 pandasai-2.0a8/pandasai/pipelines/chat/error_correction_pipeline/error_prompt_generation.py
--rw-r--r--   0        0        0     5667 2024-02-21 10:04:57.982189 pandasai-2.0a8/pandasai/pipelines/chat/generate_chat_pipeline.py
--rw-r--r--   0        0        0     2258 2024-02-21 10:04:57.982377 pandasai-2.0a8/pandasai/pipelines/chat/prompt_generation.py
--rw-r--r--   0        0        0     2152 2024-02-21 10:04:57.982525 pandasai-2.0a8/pandasai/pipelines/chat/result_parsing.py
--rw-r--r--   0        0        0     1828 2024-02-21 10:04:57.982661 pandasai-2.0a8/pandasai/pipelines/chat/result_validation.py
--rw-r--r--   0        0        0     1838 2024-02-21 10:04:57.982804 pandasai-2.0a8/pandasai/pipelines/chat/validate_pipeline_input.py
--rw-r--r--   0        0        0      488 2024-02-19 14:59:32.873263 pandasai-2.0a8/pandasai/pipelines/logic_unit_output.py
--rw-r--r--   0        0        0      422 2024-02-21 10:04:57.983209 pandasai-2.0a8/pandasai/pipelines/logic_units/code_executor.py
--rw-r--r--   0        0        0      900 2024-02-21 10:04:57.983722 pandasai-2.0a8/pandasai/pipelines/logic_units/output_logic_unit.py
--rw-r--r--   0        0        0      511 2024-02-21 10:04:57.984328 pandasai-2.0a8/pandasai/pipelines/logic_units/prompt_execution.py
--rw-r--r--   0        0        0     4663 2024-02-21 10:04:57.986931 pandasai-2.0a8/pandasai/pipelines/pipeline.py
--rw-r--r--   0        0        0     1683 2024-02-21 10:04:57.987455 pandasai-2.0a8/pandasai/pipelines/pipeline_context.py
--rw-r--r--   0        0        0      232 2024-02-19 14:59:32.874197 pandasai-2.0a8/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0     1751 2024-02-21 10:04:57.987648 pandasai-2.0a8/pandasai/prompts/base.py
--rw-r--r--   0        0        0      207 2024-02-19 14:59:32.874683 pandasai-2.0a8/pandasai/prompts/check_if_relevant_to_conversation.py
--rw-r--r--   0        0        0      518 2024-02-21 10:04:57.988163 pandasai-2.0a8/pandasai/prompts/clarification_questions_prompt.py
--rw-r--r--   0        0        0      902 2024-02-19 14:59:43.494778 pandasai-2.0a8/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0      975 2024-02-19 14:59:43.494975 pandasai-2.0a8/pandasai/prompts/correct_execute_sql_query_usage_error_prompt.py
--rw-r--r--   0        0        0     1058 2024-02-19 14:59:43.495349 pandasai-2.0a8/pandasai/prompts/correct_output_type_error_prompt.py
--rw-r--r--   0        0        0     1867 2024-02-21 10:04:57.988317 pandasai-2.0a8/pandasai/prompts/direct_sql_prompt.py
--rw-r--r--   0        0        0      159 2024-02-19 14:59:32.875691 pandasai-2.0a8/pandasai/prompts/explain_prompt.py
--rw-r--r--   0        0        0     1274 2024-02-21 10:04:57.989230 pandasai-2.0a8/pandasai/prompts/file_based_prompt.py
--rw-r--r--   0        0        0      879 2024-02-19 14:59:43.495788 pandasai-2.0a8/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      268 2024-02-19 14:59:43.495993 pandasai-2.0a8/pandasai/prompts/generate_python_code_with_sql.py
--rw-r--r--   0        0        0      189 2024-02-19 14:59:32.876351 pandasai-2.0a8/pandasai/prompts/generate_system_message.py
--rw-r--r--   0        0        0      172 2024-02-19 14:59:32.876525 pandasai-2.0a8/pandasai/prompts/rephase_query_prompt.py
--rw-r--r--   0        0        0      199 2024-02-19 14:59:32.876929 pandasai-2.0a8/pandasai/prompts/templates/check_if_relevant_to_conversation.tmpl
--rw-r--r--   0        0        0      571 2024-02-19 14:59:32.877085 pandasai-2.0a8/pandasai/prompts/templates/clarification_questions_prompt.tmpl
--rw-r--r--   0        0        0      342 2024-02-19 14:59:32.877365 pandasai-2.0a8/pandasai/prompts/templates/correct_error_prompt.tmpl
--rw-r--r--   0        0        0      356 2024-02-19 14:59:32.877433 pandasai-2.0a8/pandasai/prompts/templates/correct_execute_sql_query_usage_error_prompt.tmpl
--rw-r--r--   0        0        0      343 2024-02-21 10:04:57.989599 pandasai-2.0a8/pandasai/prompts/templates/correct_output_type_error_prompt.tmpl
--rw-r--r--   0        0        0      325 2024-02-19 14:59:32.878056 pandasai-2.0a8/pandasai/prompts/templates/explain.tmpl
--rw-r--r--   0        0        0      923 2024-02-19 14:59:32.878194 pandasai-2.0a8/pandasai/prompts/templates/generate_python_code.tmpl
--rw-r--r--   0        0        0     1326 2024-02-19 14:59:32.878350 pandasai-2.0a8/pandasai/prompts/templates/generate_python_code_with_sql.tmpl
--rw-r--r--   0        0        0      176 2024-02-19 14:59:32.878491 pandasai-2.0a8/pandasai/prompts/templates/generate_system_message.tmpl
--rw-r--r--   0        0        0      387 2024-02-19 14:59:32.878627 pandasai-2.0a8/pandasai/prompts/templates/rephrase_query.tmpl
--rw-r--r--   0        0        0       91 2024-02-19 14:59:32.878727 pandasai-2.0a8/pandasai/prompts/templates/shared/dataframe.tmpl
--rw-r--r--   0        0        0      916 2024-02-19 14:59:32.878793 pandasai-2.0a8/pandasai/prompts/templates/shared/output_type_template.tmpl
--rw-r--r--   0        0        0      624 2024-02-19 14:59:32.878855 pandasai-2.0a8/pandasai/prompts/templates/shared/vectordb_docs.tmpl
--rw-r--r--   0        0        0      311 2024-02-21 10:04:57.990280 pandasai-2.0a8/pandasai/responses/__init__.py
--rw-r--r--   0        0        0      637 2024-02-19 14:59:32.879294 pandasai-2.0a8/pandasai/responses/context.py
--rw-r--r--   0        0        0     2023 2024-02-21 10:04:57.990747 pandasai-2.0a8/pandasai/responses/response_parser.py
--rw-r--r--   0        0        0     1290 2024-02-21 10:04:57.990963 pandasai-2.0a8/pandasai/responses/response_serializer.py
--rw-r--r--   0        0        0       96 2024-02-19 14:59:32.879758 pandasai-2.0a8/pandasai/responses/response_type.py
--rw-r--r--   0        0        0     1036 2024-02-21 10:04:57.991273 pandasai-2.0a8/pandasai/responses/streamlit_response.py
--rw-r--r--   0        0        0       16 2023-09-04 21:53:07.396618 pandasai-2.0a8/pandasai/schemas/__init__.py
--rw-r--r--   0        0        0     1319 2024-02-21 10:04:57.991469 pandasai-2.0a8/pandasai/schemas/df_config.py
--rw-r--r--   0        0        0     3911 2024-02-21 10:04:57.991644 pandasai-2.0a8/pandasai/skills/__init__.py
--rw-r--r--   0        0        0     8991 2024-02-21 10:04:57.991761 pandasai-2.0a8/pandasai/smart_dataframe/__init__.py
--rw-r--r--   0        0        0     6336 2024-02-21 10:04:57.991865 pandasai-2.0a8/pandasai/smart_datalake/__init__.py
--rw-r--r--   0        0        0      230 2024-02-21 10:04:57.992013 pandasai-2.0a8/pandasai/vectorstores/__init__.py
--rw-r--r--   0        0        0     2394 2024-02-21 10:04:57.992292 pandasai-2.0a8/pandasai/vectorstores/bamboo_vectorstore.py
--rw-r--r--   0        0        0    10443 2024-02-21 10:04:57.993289 pandasai-2.0a8/pandasai/vectorstores/chroma.py
--rw-r--r--   0        0        0     5764 2024-02-21 10:04:57.993455 pandasai-2.0a8/pandasai/vectorstores/vectorstore.py
--rw-r--r--   0        0        0     3203 2024-02-21 10:05:12.381793 pandasai-2.0a8/pyproject.toml
--rw-r--r--   0        0        0    10445 1970-01-01 00:00:00.000000 pandasai-2.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-04-24 05:55:05.323190 pandasai-2.0a9/LICENSE
+drwxr-xr-x   0        0        0        0 2023-11-20 22:14:04.721024 pandasai-2.0a9/LICENSES/
+-rw-r--r--   0        0        0     7206 2024-02-21 10:04:57.962885 pandasai-2.0a9/README.md
+-rw-r--r--   0        0        0      682 2024-02-21 10:04:57.967562 pandasai-2.0a9/pandasai/__init__.py
+-rw-r--r--   0        0        0       45 2024-02-19 14:59:32.858258 pandasai-2.0a9/pandasai/agent/__init__.py
+-rw-r--r--   0        0        0    13699 2024-02-21 10:04:57.967914 pandasai-2.0a9/pandasai/agent/base.py
+-rw-r--r--   0        0        0      994 2024-02-19 14:59:32.858993 pandasai-2.0a9/pandasai/agent/callbacks.py
+-rw-r--r--   0        0        0     1227 2024-02-19 14:59:32.859598 pandasai-2.0a9/pandasai/config.py
+-rw-r--r--   0        0        0      908 2024-02-21 10:04:57.968102 pandasai-2.0a9/pandasai/connectors/__init__.py
+-rw-r--r--   0        0        0     8777 2024-02-21 10:04:57.968280 pandasai-2.0a9/pandasai/connectors/airtable.py
+-rw-r--r--   0        0        0     7750 2024-02-21 10:04:57.968449 pandasai-2.0a9/pandasai/connectors/base.py
+-rw-r--r--   0        0        0     2880 2024-02-21 10:04:57.968631 pandasai-2.0a9/pandasai/connectors/databricks.py
+-rw-r--r--   0        0        0     2226 2024-02-21 10:04:57.968768 pandasai-2.0a9/pandasai/connectors/google_big_query.py
+-rw-r--r--   0        0        0     4422 2024-02-21 10:04:57.968938 pandasai-2.0a9/pandasai/connectors/pandas.py
+-rw-r--r--   0        0        0     4164 2024-02-21 10:04:57.969097 pandasai-2.0a9/pandasai/connectors/polars.py
+-rw-r--r--   0        0        0     3834 2024-02-21 10:04:57.969289 pandasai-2.0a9/pandasai/connectors/snowflake.py
+-rw-r--r--   0        0        0    18682 2024-02-21 10:04:57.969437 pandasai-2.0a9/pandasai/connectors/sql.py
+-rw-r--r--   0        0        0     5871 2024-02-21 10:04:57.969757 pandasai-2.0a9/pandasai/connectors/yahoo_finance.py
+-rw-r--r--   0        0        0     1711 2024-02-21 10:04:57.969904 pandasai-2.0a9/pandasai/constants.py
+-rw-r--r--   0        0        0      507 2024-02-21 10:04:57.970176 pandasai-2.0a9/pandasai/engine.py
+-rw-r--r--   0        0        0     5284 2024-02-21 10:04:57.970349 pandasai-2.0a9/pandasai/exceptions.py
+-rw-r--r--   0        0        0      446 2024-02-21 10:04:57.970515 pandasai-2.0a9/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     4613 2024-02-21 10:04:57.971425 pandasai-2.0a9/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     3019 2024-02-21 10:04:57.971578 pandasai-2.0a9/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0    23368 2024-02-21 18:45:03.820108 pandasai-2.0a9/pandasai/helpers/code_manager.py
+-rw-r--r--   0        0        0     2397 2024-02-21 10:04:57.972019 pandasai-2.0a9/pandasai/helpers/data_sampler.py
+-rw-r--r--   0        0        0     4574 2024-02-21 10:04:57.972177 pandasai-2.0a9/pandasai/helpers/dataframe_serializer.py
+-rw-r--r--   0        0        0     5062 2024-02-21 10:04:57.972426 pandasai-2.0a9/pandasai/helpers/df_config_manager.py
+-rw-r--r--   0        0        0     1378 2024-02-21 10:04:57.972700 pandasai-2.0a9/pandasai/helpers/df_info.py
+-rw-r--r--   0        0        0     3236 2024-02-21 10:04:57.972971 pandasai-2.0a9/pandasai/helpers/df_validator.py
+-rw-r--r--   0        0        0      526 2024-02-21 10:04:57.973121 pandasai-2.0a9/pandasai/helpers/env.py
+-rw-r--r--   0        0        0      928 2024-02-21 10:04:57.973259 pandasai-2.0a9/pandasai/helpers/file_importer.py
+-rw-r--r--   0        0        0      725 2024-02-21 10:04:57.973382 pandasai-2.0a9/pandasai/helpers/folder.py
+-rw-r--r--   0        0        0     3717 2024-02-21 10:04:57.973750 pandasai-2.0a9/pandasai/helpers/from_google_sheets.py
+-rw-r--r--   0        0        0     4273 2024-02-21 10:04:57.973959 pandasai-2.0a9/pandasai/helpers/logger.py
+-rw-r--r--   0        0        0     2770 2024-02-19 14:59:43.492203 pandasai-2.0a9/pandasai/helpers/memory.py
+-rw-r--r--   0        0        0      447 2023-09-13 09:35:53.943189 pandasai-2.0a9/pandasai/helpers/node_visitors.py
+-rw-r--r--   0        0        0      213 2023-11-20 22:14:04.734116 pandasai-2.0a9/pandasai/helpers/openai.py
+-rw-r--r--   0        0        0     6019 2024-02-21 10:04:57.974150 pandasai-2.0a9/pandasai/helpers/openai_info.py
+-rw-r--r--   0        0        0     3898 2023-09-04 21:53:07.384708 pandasai-2.0a9/pandasai/helpers/optional.py
+-rw-r--r--   0        0        0     1976 2024-02-21 10:04:57.974259 pandasai-2.0a9/pandasai/helpers/output_types/__init__.py
+-rw-r--r--   0        0        0     4658 2024-02-21 10:04:57.974363 pandasai-2.0a9/pandasai/helpers/output_types/_output_types.py
+-rw-r--r--   0        0        0     2310 2024-02-21 10:04:57.974537 pandasai-2.0a9/pandasai/helpers/output_validator.py
+-rw-r--r--   0        0        0     2074 2023-11-20 22:14:04.734712 pandasai-2.0a9/pandasai/helpers/path.py
+-rw-r--r--   0        0        0     8344 2024-02-21 18:45:03.820364 pandasai-2.0a9/pandasai/helpers/query_exec_tracker.py
+-rw-r--r--   0        0        0     2466 2024-02-21 10:04:57.974868 pandasai-2.0a9/pandasai/helpers/request.py
+-rw-r--r--   0        0        0     1061 2024-02-21 10:04:57.975042 pandasai-2.0a9/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     8579 2024-02-21 10:04:57.975494 pandasai-2.0a9/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0     2388 2024-02-21 10:04:57.975669 pandasai-2.0a9/pandasai/helpers/skills_manager.py
+-rw-r--r--   0        0        0      426 2024-01-19 10:23:41.929740 pandasai-2.0a9/pandasai/helpers/sql.py
+-rw-r--r--   0        0        0      435 2024-02-21 10:04:57.975850 pandasai-2.0a9/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     7002 2024-02-21 10:04:57.977815 pandasai-2.0a9/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0      732 2024-02-21 10:04:57.978008 pandasai-2.0a9/pandasai/llm/bamboo_llm.py
+-rw-r--r--   0        0        0    13732 2024-02-21 10:04:57.978209 pandasai-2.0a9/pandasai/llm/base.py
+-rw-r--r--   0        0        0      640 2024-02-19 14:59:43.493258 pandasai-2.0a9/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     2660 2024-02-21 10:04:57.978791 pandasai-2.0a9/pandasai/llm/google_gemini.py
+-rw-r--r--   0        0        0     2737 2024-02-21 10:04:57.979108 pandasai-2.0a9/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0     5687 2024-02-21 10:04:57.979290 pandasai-2.0a9/pandasai/llm/google_vertexai.py
+-rw-r--r--   0        0        0     4003 2024-02-21 10:04:57.979493 pandasai-2.0a9/pandasai/llm/huggingface_text_gen.py
+-rw-r--r--   0        0        0     1168 2024-02-21 10:04:57.979830 pandasai-2.0a9/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     3236 2024-02-21 10:04:57.980594 pandasai-2.0a9/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      352 2024-02-21 10:04:57.980893 pandasai-2.0a9/pandasai/pandas/__init__.py
+-rw-r--r--   0        0        0      206 2024-02-19 14:59:32.870508 pandasai-2.0a9/pandasai/pipelines/__init__.py
+-rw-r--r--   0        0        0      353 2023-11-20 22:14:04.741653 pandasai-2.0a9/pandasai/pipelines/abstract_pipeline.py
+-rw-r--r--   0        0        0     1062 2024-02-19 14:59:32.870645 pandasai-2.0a9/pandasai/pipelines/base_logic_unit.py
+-rw-r--r--   0        0        0     1438 2024-02-19 14:59:32.870772 pandasai-2.0a9/pandasai/pipelines/chat/cache_lookup.py
+-rw-r--r--   0        0        0     1253 2024-02-21 10:04:57.981058 pandasai-2.0a9/pandasai/pipelines/chat/cache_population.py
+-rw-r--r--   0        0        0      572 2024-02-21 10:04:57.981190 pandasai-2.0a9/pandasai/pipelines/chat/chat_pipeline_input.py
+-rw-r--r--   0        0        0     4381 2024-02-21 18:45:03.820554 pandasai-2.0a9/pandasai/pipelines/chat/code_execution.py
+-rw-r--r--   0        0        0     1473 2024-02-21 10:04:57.981483 pandasai-2.0a9/pandasai/pipelines/chat/code_generator.py
+-rw-r--r--   0        0        0     1479 2024-02-21 10:04:57.981659 pandasai-2.0a9/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline.py
+-rw-r--r--   0        0        0      240 2024-02-19 14:59:32.872442 pandasai-2.0a9/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline_input.py
+-rw-r--r--   0        0        0     3037 2024-02-21 10:04:57.981791 pandasai-2.0a9/pandasai/pipelines/chat/error_correction_pipeline/error_prompt_generation.py
+-rw-r--r--   0        0        0     5667 2024-02-21 10:04:57.982189 pandasai-2.0a9/pandasai/pipelines/chat/generate_chat_pipeline.py
+-rw-r--r--   0        0        0     2258 2024-02-21 10:04:57.982377 pandasai-2.0a9/pandasai/pipelines/chat/prompt_generation.py
+-rw-r--r--   0        0        0     2152 2024-02-21 10:04:57.982525 pandasai-2.0a9/pandasai/pipelines/chat/result_parsing.py
+-rw-r--r--   0        0        0     1828 2024-02-21 10:04:57.982661 pandasai-2.0a9/pandasai/pipelines/chat/result_validation.py
+-rw-r--r--   0        0        0     1838 2024-02-21 10:04:57.982804 pandasai-2.0a9/pandasai/pipelines/chat/validate_pipeline_input.py
+-rw-r--r--   0        0        0      612 2024-02-21 18:45:03.821564 pandasai-2.0a9/pandasai/pipelines/logic_unit_output.py
+-rw-r--r--   0        0        0      422 2024-02-21 10:04:57.983209 pandasai-2.0a9/pandasai/pipelines/logic_units/code_executor.py
+-rw-r--r--   0        0        0      900 2024-02-21 10:04:57.983722 pandasai-2.0a9/pandasai/pipelines/logic_units/output_logic_unit.py
+-rw-r--r--   0        0        0      511 2024-02-21 10:04:57.984328 pandasai-2.0a9/pandasai/pipelines/logic_units/prompt_execution.py
+-rw-r--r--   0        0        0     4863 2024-02-21 18:45:03.821756 pandasai-2.0a9/pandasai/pipelines/pipeline.py
+-rw-r--r--   0        0        0     1683 2024-02-21 10:04:57.987455 pandasai-2.0a9/pandasai/pipelines/pipeline_context.py
+-rw-r--r--   0        0        0      232 2024-02-19 14:59:32.874197 pandasai-2.0a9/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0     1751 2024-02-21 10:04:57.987648 pandasai-2.0a9/pandasai/prompts/base.py
+-rw-r--r--   0        0        0      207 2024-02-19 14:59:32.874683 pandasai-2.0a9/pandasai/prompts/check_if_relevant_to_conversation.py
+-rw-r--r--   0        0        0      518 2024-02-21 10:04:57.988163 pandasai-2.0a9/pandasai/prompts/clarification_questions_prompt.py
+-rw-r--r--   0        0        0      902 2024-02-19 14:59:43.494778 pandasai-2.0a9/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0      975 2024-02-19 14:59:43.494975 pandasai-2.0a9/pandasai/prompts/correct_execute_sql_query_usage_error_prompt.py
+-rw-r--r--   0        0        0     1058 2024-02-19 14:59:43.495349 pandasai-2.0a9/pandasai/prompts/correct_output_type_error_prompt.py
+-rw-r--r--   0        0        0     1867 2024-02-21 10:04:57.988317 pandasai-2.0a9/pandasai/prompts/direct_sql_prompt.py
+-rw-r--r--   0        0        0      159 2024-02-19 14:59:32.875691 pandasai-2.0a9/pandasai/prompts/explain_prompt.py
+-rw-r--r--   0        0        0     1274 2024-02-21 10:04:57.989230 pandasai-2.0a9/pandasai/prompts/file_based_prompt.py
+-rw-r--r--   0        0        0      879 2024-02-19 14:59:43.495788 pandasai-2.0a9/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      268 2024-02-19 14:59:43.495993 pandasai-2.0a9/pandasai/prompts/generate_python_code_with_sql.py
+-rw-r--r--   0        0        0      189 2024-02-19 14:59:32.876351 pandasai-2.0a9/pandasai/prompts/generate_system_message.py
+-rw-r--r--   0        0        0      172 2024-02-19 14:59:32.876525 pandasai-2.0a9/pandasai/prompts/rephase_query_prompt.py
+-rw-r--r--   0        0        0      199 2024-02-19 14:59:32.876929 pandasai-2.0a9/pandasai/prompts/templates/check_if_relevant_to_conversation.tmpl
+-rw-r--r--   0        0        0      571 2024-02-19 14:59:32.877085 pandasai-2.0a9/pandasai/prompts/templates/clarification_questions_prompt.tmpl
+-rw-r--r--   0        0        0      342 2024-02-19 14:59:32.877365 pandasai-2.0a9/pandasai/prompts/templates/correct_error_prompt.tmpl
+-rw-r--r--   0        0        0      356 2024-02-19 14:59:32.877433 pandasai-2.0a9/pandasai/prompts/templates/correct_execute_sql_query_usage_error_prompt.tmpl
+-rw-r--r--   0        0        0      343 2024-02-21 10:04:57.989599 pandasai-2.0a9/pandasai/prompts/templates/correct_output_type_error_prompt.tmpl
+-rw-r--r--   0        0        0      325 2024-02-19 14:59:32.878056 pandasai-2.0a9/pandasai/prompts/templates/explain.tmpl
+-rw-r--r--   0        0        0      923 2024-02-19 14:59:32.878194 pandasai-2.0a9/pandasai/prompts/templates/generate_python_code.tmpl
+-rw-r--r--   0        0        0     1326 2024-02-19 14:59:32.878350 pandasai-2.0a9/pandasai/prompts/templates/generate_python_code_with_sql.tmpl
+-rw-r--r--   0        0        0      176 2024-02-19 14:59:32.878491 pandasai-2.0a9/pandasai/prompts/templates/generate_system_message.tmpl
+-rw-r--r--   0        0        0      387 2024-02-19 14:59:32.878627 pandasai-2.0a9/pandasai/prompts/templates/rephrase_query.tmpl
+-rw-r--r--   0        0        0       91 2024-02-19 14:59:32.878727 pandasai-2.0a9/pandasai/prompts/templates/shared/dataframe.tmpl
+-rw-r--r--   0        0        0      916 2024-02-19 14:59:32.878793 pandasai-2.0a9/pandasai/prompts/templates/shared/output_type_template.tmpl
+-rw-r--r--   0        0        0      624 2024-02-19 14:59:32.878855 pandasai-2.0a9/pandasai/prompts/templates/shared/vectordb_docs.tmpl
+-rw-r--r--   0        0        0      311 2024-02-21 10:04:57.990280 pandasai-2.0a9/pandasai/responses/__init__.py
+-rw-r--r--   0        0        0      637 2024-02-19 14:59:32.879294 pandasai-2.0a9/pandasai/responses/context.py
+-rw-r--r--   0        0        0     2023 2024-02-21 10:04:57.990747 pandasai-2.0a9/pandasai/responses/response_parser.py
+-rw-r--r--   0        0        0     1290 2024-02-21 10:04:57.990963 pandasai-2.0a9/pandasai/responses/response_serializer.py
+-rw-r--r--   0        0        0       96 2024-02-19 14:59:32.879758 pandasai-2.0a9/pandasai/responses/response_type.py
+-rw-r--r--   0        0        0     1036 2024-02-21 10:04:57.991273 pandasai-2.0a9/pandasai/responses/streamlit_response.py
+-rw-r--r--   0        0        0       16 2023-09-04 21:53:07.396618 pandasai-2.0a9/pandasai/schemas/__init__.py
+-rw-r--r--   0        0        0     1319 2024-02-21 10:04:57.991469 pandasai-2.0a9/pandasai/schemas/df_config.py
+-rw-r--r--   0        0        0     3911 2024-02-21 10:04:57.991644 pandasai-2.0a9/pandasai/skills/__init__.py
+-rw-r--r--   0        0        0     8991 2024-02-21 10:04:57.991761 pandasai-2.0a9/pandasai/smart_dataframe/__init__.py
+-rw-r--r--   0        0        0     6336 2024-02-21 10:04:57.991865 pandasai-2.0a9/pandasai/smart_datalake/__init__.py
+-rw-r--r--   0        0        0      230 2024-02-21 10:04:57.992013 pandasai-2.0a9/pandasai/vectorstores/__init__.py
+-rw-r--r--   0        0        0     2394 2024-02-21 10:04:57.992292 pandasai-2.0a9/pandasai/vectorstores/bamboo_vectorstore.py
+-rw-r--r--   0        0        0    10443 2024-02-21 10:04:57.993289 pandasai-2.0a9/pandasai/vectorstores/chroma.py
+-rw-r--r--   0        0        0     5764 2024-02-21 10:04:57.993455 pandasai-2.0a9/pandasai/vectorstores/vectorstore.py
+-rw-r--r--   0        0        0     3203 2024-02-21 18:45:45.718011 pandasai-2.0a9/pyproject.toml
+-rw-r--r--   0        0        0    10445 1970-01-01 00:00:00.000000 pandasai-2.0a9/PKG-INFO
```

### Comparing `pandasai-2.0a8/LICENSE` & `pandasai-2.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/README.md` & `pandasai-2.0a9/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/__init__.py` & `pandasai-2.0a9/pandasai/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/agent/base.py` & `pandasai-2.0a9/pandasai/agent/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/agent/callbacks.py` & `pandasai-2.0a9/pandasai/agent/callbacks.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/config.py` & `pandasai-2.0a9/pandasai/config.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/connectors/__init__.py` & `pandasai-2.0a9/pandasai/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/connectors/airtable.py` & `pandasai-2.0a9/pandasai/connectors/airtable.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/connectors/base.py` & `pandasai-2.0a9/pandasai/connectors/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/connectors/databricks.py` & `pandasai-2.0a9/pandasai/connectors/databricks.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/connectors/google_big_query.py` & `pandasai-2.0a9/pandasai/connectors/google_big_query.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/connectors/pandas.py` & `pandasai-2.0a9/pandasai/connectors/pandas.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/connectors/polars.py` & `pandasai-2.0a9/pandasai/connectors/polars.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/connectors/snowflake.py` & `pandasai-2.0a9/pandasai/connectors/snowflake.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/connectors/sql.py` & `pandasai-2.0a9/pandasai/connectors/sql.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/connectors/yahoo_finance.py` & `pandasai-2.0a9/pandasai/connectors/yahoo_finance.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/constants.py` & `pandasai-2.0a9/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/exceptions.py` & `pandasai-2.0a9/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/anonymizer.py` & `pandasai-2.0a9/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/cache.py` & `pandasai-2.0a9/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/code_manager.py` & `pandasai-2.0a9/pandasai/helpers/code_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,32 @@
             prompt_id (uuid.UUID): Prompt ID
             skills_manager (SkillsManager): Skills Manager
         """
         self.skills_manager = skills_manager
         self.prompt_id = prompt_id
 
 
+class FunctionCallVisitor(ast.NodeVisitor):
+    """
+    Iterate over the code to find function calls
+    """
+
+    def __init__(self):
+        self.function_calls = []
+
+    def visit_Call(self, node):
+        if isinstance(node.func, ast.Name):
+            self.function_calls.append(node.func.id)
+        elif isinstance(node.func, ast.Attribute) and isinstance(
+            node.func.value, ast.Name
+        ):
+            self.function_calls.append(f"{node.func.value.id}.{node.func.attr}")
+        self.generic_visit(node)
+
+
 class CodeManager:
     _dfs: List
     _config: Union[Config, dict]
     _logger: Logger = None
     _additional_dependencies: List[dict] = []
     _ast_comparator_map: dict = {
         ast.Eq: "=",
@@ -78,14 +96,15 @@
             dfs (List): List of Dataframes
             config (Union[Config, dict]): Config
             logger (Logger): Logger
         """
         self._dfs = dfs
         self._config = config
         self._logger = logger
+        self._function_call_vistor = FunctionCallVisitor()
 
     def _required_dfs(self, code: str) -> List[str]:
         """
         List the index of the DataFrames that are needed to execute the code. The goal
         is to avoid to run the connectors if the code does not need them.
 
         Args:
@@ -314,22 +333,14 @@
         )
 
     def check_skill_func_def_exists(self, node: ast.AST, context: CodeExecutionContext):
         return isinstance(
             node, ast.FunctionDef
         ) and context.skills_manager.skill_exists(node.name)
 
-    def check_direct_sql_func_usage_exists(self, node: ast.AST):
-        return (
-            self._validate_direct_sql(self._dfs)
-            and isinstance(node.value, ast.Call)
-            and isinstance(node.value.func, ast.Name)
-            and node.value.func.id == "execute_sql_query"
-        )
-
     def _validate_direct_sql(self, dfs: List[BaseConnector]) -> bool:
         """
         Raises error if they don't belong sqlconnector or have different credentials
         Args:
             dfs (List[BaseConnector]): list of BaseConnectors
 
         Raises:
@@ -380,14 +391,17 @@
 
         tree = ast.parse(code)
 
         # Check for imports and the node where analyze_data is defined
         new_body = []
         execute_sql_query_used = False
 
+        # find function calls
+        self._function_call_vistor.visit(tree)
+
         for node in tree.body:
             if isinstance(node, (ast.Import, ast.ImportFrom)):
                 self._check_imports(node)
                 continue
 
             if (
                 self._is_df_overwrite(node)
@@ -401,15 +415,18 @@
             if self.check_direct_sql_func_def_exists(node):
                 continue
 
             if self.check_skill_func_def_exists(node, context):
                 continue
 
             # if generated code contain execute_sql_query usage
-            if self.check_direct_sql_func_usage_exists(node):
+            if (
+                self._validate_direct_sql(self._dfs)
+                and "execute_sql_query" in self._function_call_vistor.function_calls
+            ):
                 execute_sql_query_used = True
 
             # Sanity for sql query the code should only use allowed tables
             if (
                 isinstance(node, ast.Assign)
                 and self._config.direct_sql
                 and (unauthorized_tables := self._get_sql_irrelevant_tables(node))
```

### Comparing `pandasai-2.0a8/pandasai/helpers/data_sampler.py` & `pandasai-2.0a9/pandasai/helpers/data_sampler.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/dataframe_serializer.py` & `pandasai-2.0a9/pandasai/helpers/dataframe_serializer.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/df_config_manager.py` & `pandasai-2.0a9/pandasai/helpers/df_config_manager.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/df_info.py` & `pandasai-2.0a9/pandasai/helpers/df_info.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/df_validator.py` & `pandasai-2.0a9/pandasai/helpers/df_validator.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/env.py` & `pandasai-2.0a9/pandasai/helpers/env.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/file_importer.py` & `pandasai-2.0a9/pandasai/helpers/file_importer.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/folder.py` & `pandasai-2.0a9/pandasai/helpers/folder.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/from_google_sheets.py` & `pandasai-2.0a9/pandasai/helpers/from_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/logger.py` & `pandasai-2.0a9/pandasai/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/memory.py` & `pandasai-2.0a9/pandasai/helpers/memory.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/openai_info.py` & `pandasai-2.0a9/pandasai/helpers/openai_info.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/optional.py` & `pandasai-2.0a9/pandasai/helpers/optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/output_types/__init__.py` & `pandasai-2.0a9/pandasai/helpers/output_types/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/output_types/_output_types.py` & `pandasai-2.0a9/pandasai/helpers/output_types/_output_types.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/output_validator.py` & `pandasai-2.0a9/pandasai/helpers/output_validator.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/path.py` & `pandasai-2.0a9/pandasai/helpers/path.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/query_exec_tracker.py` & `pandasai-2.0a9/pandasai/helpers/query_exec_tracker.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,25 +88,19 @@
 
     def add_step(self, step: dict) -> None:
         """
         Add Custom Step that is performed for additional information
         Args:
             step (dict): dictionary containing information
         """
-        # Exception step to store serializable output response from the generated code
-        if (
-            "type" in step
-            and step["type"] == "CodeExecution"
-            and step["data"] is not None
-            and step["data"]["content_type"] == "response"
-        ):
-            self._response = step["data"]["value"]
-
         self._steps.append(step)
 
+    def set_final_response(self, response: Any):
+        self._response = response
+
     def execute_func(self, function, *args, **kwargs) -> Any:
         """
         Tracks function executions, calculates execution time and prepare data
         Args:
             function (function): Function that is to be executed
 
         Returns:
@@ -232,19 +226,19 @@
         """
         Publish Query Summary to remote logging server
         """
         api_key = None
         server_url = None
 
         if self._server_config is None:
-            server_url = os.environ.get("PANDASAI_API_URL")
+            server_url = os.environ.get("PANDASAI_API_URL", "https://api.domer.ai")
             api_key = os.environ.get("PANDASAI_API_KEY")
         else:
             server_url = self._server_config.get(
-                "server_url", os.environ.get("PANDASAI_API_URL")
+                "server_url", os.environ.get("PANDASAI_API_URL", "https://api.domer.ai")
             )
             api_key = self._server_config.get(
                 "api_key", os.environ.get("PANDASAI_API_KEY")
             )
 
         if api_key is None or server_url is None:
             return
```

### Comparing `pandasai-2.0a8/pandasai/helpers/request.py` & `pandasai-2.0a9/pandasai/helpers/request.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/save_chart.py` & `pandasai-2.0a9/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/shortcuts.py` & `pandasai-2.0a9/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/helpers/skills_manager.py` & `pandasai-2.0a9/pandasai/helpers/skills_manager.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/llm/azure_openai.py` & `pandasai-2.0a9/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/llm/bamboo_llm.py` & `pandasai-2.0a9/pandasai/llm/bamboo_llm.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/llm/base.py` & `pandasai-2.0a9/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/llm/fake.py` & `pandasai-2.0a9/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/llm/google_gemini.py` & `pandasai-2.0a9/pandasai/llm/google_gemini.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/llm/google_palm.py` & `pandasai-2.0a9/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/llm/google_vertexai.py` & `pandasai-2.0a9/pandasai/llm/google_vertexai.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/llm/huggingface_text_gen.py` & `pandasai-2.0a9/pandasai/llm/huggingface_text_gen.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/llm/langchain.py` & `pandasai-2.0a9/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/llm/openai.py` & `pandasai-2.0a9/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/base_logic_unit.py` & `pandasai-2.0a9/pandasai/pipelines/base_logic_unit.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/chat/cache_lookup.py` & `pandasai-2.0a9/pandasai/pipelines/chat/cache_lookup.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/chat/cache_population.py` & `pandasai-2.0a9/pandasai/pipelines/chat/cache_population.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/chat/chat_pipeline_input.py` & `pandasai-2.0a9/pandasai/pipelines/chat/chat_pipeline_input.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/chat/code_execution.py` & `pandasai-2.0a9/pandasai/pipelines/chat/code_execution.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
                 )
 
         return LogicUnitOutput(
             result,
             True,
             "Code Executed Successfully",
             {"content_type": "response", "value": ResponseSerializer.serialize(result)},
+            final_track_output=True,
         )
 
     def _retry_run_code(
         self,
         code: str,
         context: PipelineContext,
         logger: Logger,
```

### Comparing `pandasai-2.0a8/pandasai/pipelines/chat/code_generator.py` & `pandasai-2.0a9/pandasai/pipelines/chat/code_generator.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline.py` & `pandasai-2.0a9/pandasai/pipelines/chat/error_correction_pipeline/error_correction_pipeline.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/chat/error_correction_pipeline/error_prompt_generation.py` & `pandasai-2.0a9/pandasai/pipelines/chat/error_correction_pipeline/error_prompt_generation.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/chat/generate_chat_pipeline.py` & `pandasai-2.0a9/pandasai/pipelines/chat/generate_chat_pipeline.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/chat/prompt_generation.py` & `pandasai-2.0a9/pandasai/pipelines/chat/prompt_generation.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/chat/result_parsing.py` & `pandasai-2.0a9/pandasai/pipelines/chat/result_parsing.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/chat/result_validation.py` & `pandasai-2.0a9/pandasai/pipelines/chat/result_validation.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/chat/validate_pipeline_input.py` & `pandasai-2.0a9/pandasai/pipelines/chat/validate_pipeline_input.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/logic_units/output_logic_unit.py` & `pandasai-2.0a9/pandasai/pipelines/logic_units/output_logic_unit.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/pipelines/pipeline.py` & `pandasai-2.0a9/pandasai/pipelines/pipeline.py`

 * *Files 11% similar despite different names*

```diff
@@ -115,14 +115,19 @@
                             "success": step_output.success,
                             "message": step_output.message,
                             "execution_time": execution_time,
                             "data": step_output.metadata,
                         }
                     )
 
+                    if step_output.final_track_output:
+                        self._query_exec_tracker.set_final_response(
+                            step_output.metadata
+                        )
+
                     data = step_output.output
                 else:
                     data = step_output
 
                 # Callback function after execution
                 if logic.on_execution is not None:
                     logic.on_execution(data)
```

### Comparing `pandasai-2.0a8/pandasai/pipelines/pipeline_context.py` & `pandasai-2.0a9/pandasai/pipelines/pipeline_context.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/base.py` & `pandasai-2.0a9/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/clarification_questions_prompt.py` & `pandasai-2.0a9/pandasai/prompts/clarification_questions_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/correct_error_prompt.py` & `pandasai-2.0a9/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/correct_execute_sql_query_usage_error_prompt.py` & `pandasai-2.0a9/pandasai/prompts/correct_execute_sql_query_usage_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/correct_output_type_error_prompt.py` & `pandasai-2.0a9/pandasai/prompts/correct_output_type_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/direct_sql_prompt.py` & `pandasai-2.0a9/pandasai/prompts/direct_sql_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/file_based_prompt.py` & `pandasai-2.0a9/pandasai/prompts/file_based_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/generate_python_code.py` & `pandasai-2.0a9/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/templates/clarification_questions_prompt.tmpl` & `pandasai-2.0a9/pandasai/prompts/templates/clarification_questions_prompt.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/templates/generate_python_code.tmpl` & `pandasai-2.0a9/pandasai/prompts/templates/generate_python_code.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/templates/generate_python_code_with_sql.tmpl` & `pandasai-2.0a9/pandasai/prompts/templates/generate_python_code_with_sql.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/templates/shared/output_type_template.tmpl` & `pandasai-2.0a9/pandasai/prompts/templates/shared/output_type_template.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/prompts/templates/shared/vectordb_docs.tmpl` & `pandasai-2.0a9/pandasai/prompts/templates/shared/vectordb_docs.tmpl`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/responses/context.py` & `pandasai-2.0a9/pandasai/responses/context.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/responses/response_parser.py` & `pandasai-2.0a9/pandasai/responses/response_parser.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/responses/response_serializer.py` & `pandasai-2.0a9/pandasai/responses/response_serializer.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/responses/streamlit_response.py` & `pandasai-2.0a9/pandasai/responses/streamlit_response.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/schemas/df_config.py` & `pandasai-2.0a9/pandasai/schemas/df_config.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/skills/__init__.py` & `pandasai-2.0a9/pandasai/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/smart_dataframe/__init__.py` & `pandasai-2.0a9/pandasai/smart_dataframe/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/smart_datalake/__init__.py` & `pandasai-2.0a9/pandasai/smart_datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/vectorstores/bamboo_vectorstore.py` & `pandasai-2.0a9/pandasai/vectorstores/bamboo_vectorstore.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/vectorstores/chroma.py` & `pandasai-2.0a9/pandasai/vectorstores/chroma.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pandasai/vectorstores/vectorstore.py` & `pandasai-2.0a9/pandasai/vectorstores/vectorstore.py`

 * *Files identical despite different names*

### Comparing `pandasai-2.0a8/pyproject.toml` & `pandasai-2.0a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "2.0a8"
+version = "2.0a9"
 description = "PandasAI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-2.0a8/PKG-INFO` & `pandasai-2.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 2.0a8
+Version: 2.0a9
 Summary: PandasAI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

