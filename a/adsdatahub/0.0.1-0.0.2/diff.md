# Comparing `tmp/adsdatahub-0.0.1.tar.gz` & `tmp/adsdatahub-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adsdatahub-0.0.1.tar", max compression
+gzip compressed data, was "adsdatahub-0.0.2.tar", max compression
```

## Comparing `adsdatahub-0.0.1.tar` & `adsdatahub-0.0.2.tar`

### file list

```diff
@@ -1,70 +1,77 @@
--rw-r--r--   0        0        0      195 2024-03-04 01:50:45.454141 adsdatahub-0.0.1/README.md
--rw-r--r--   0        0        0     1241 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      206 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/__init__.py
--rw-r--r--   0        0        0      137 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/client/__init__.py
--rw-r--r--   0        0        0      992 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/client/client.py
--rw-r--r--   0        0        0      835 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/client/customer.py
--rw-r--r--   0        0        0      448 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/client/mock_client.py
--rw-r--r--   0        0        0     1157 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/client/mock_customer.py
--rw-r--r--   0        0        0     3863 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/client/parameters.py
--rw-r--r--   0        0        0     1086 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/client/query_result.py
--rw-r--r--   0        0        0     1105 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/client/real_client.py
--rw-r--r--   0        0        0     2572 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/client/real_customer.py
--rw-r--r--   0        0        0     3737 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/exceptions.py
--rw-r--r--   0        0        0        0 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/py.typed
--rw-r--r--   0        0        0      137 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/__init__.py
--rw-r--r--   0        0        0     2188 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/_helpers.py
--rw-r--r--   0        0        0     4149 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/client.py
--rw-r--r--   0        0        0      137 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/http/__init__.py
--rw-r--r--   0        0        0     2125 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/http/client.py
--rw-r--r--   0        0        0     2671 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/http/mock_client.py
--rw-r--r--   0        0        0     1791 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/http/real_client.py
--rw-r--r--   0        0        0     2305 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/mock_client.py
--rw-r--r--   0        0        0     4849 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/real_client.py
--rw-r--r--   0        0        0        0 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/resources/__init__.py
--rw-r--r--   0        0        0     6048 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/resources/analysis_queries/__init__.py
--rw-r--r--   0        0        0     1450 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/resources/analysis_queries/list.py
--rw-r--r--   0        0        0     1203 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/resources/analysis_queries/start_transient.py
--rw-r--r--   0        0        0     3634 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/resources/analysis_queries/validate.py
--rw-r--r--   0        0        0     5073 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/resources/analysis_query/__init__.py
--rw-r--r--   0        0        0     1105 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/resources/analysis_query/start.py
--rw-r--r--   0        0        0     6604 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/resources/operation/__init__.py
--rw-r--r--   0        0        0      727 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/resources/operation/wait.py
--rw-r--r--   0        0        0     2909 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/resources/operations/__init__.py
--rw-r--r--   0        0        0      911 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/resources/operations/list.py
--rw-r--r--   0        0        0        0 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/__init__.py
--rw-r--r--   0        0        0      234 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/_model.py
--rw-r--r--   0        0        0     1743 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/analysis_queries_start.py
--rw-r--r--   0        0        0    12487 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/analysis_query.py
--rw-r--r--   0        0        0     1180 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/analysis_query_metadata.py
--rw-r--r--   0        0        0      214 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/column.py
--rw-r--r--   0        0        0      735 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/column_info.py
--rw-r--r--   0        0        0      671 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/column_summary_rule.py
--rw-r--r--   0        0        0     1422 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/date.py
--rw-r--r--   0        0        0     2450 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/destination_table_info.py
--rw-r--r--   0        0        0     1364 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/field_type.py
--rw-r--r--   0        0        0      936 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/filtered_row_summary.py
--rw-r--r--   0        0        0     1202 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/merge_column.py
--rw-r--r--   0        0        0      442 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/merge_spec.py
--rw-r--r--   0        0        0      636 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/merge_type.py
--rw-r--r--   0        0        0      677 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/noise_impact.py
--rw-r--r--   0        0        0     3132 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/operation.py
--rw-r--r--   0        0        0      661 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/output_artifacts.py
--rw-r--r--   0        0        0     1131 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/parameter_type.py
--rw-r--r--   0        0        0     1012 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/parameter_value.py
--rw-r--r--   0        0        0      508 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/privacy_message.py
--rw-r--r--   0        0        0     2349 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/privacy_message_type.py
--rw-r--r--   0        0        0     3861 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_execution_spec.py
--rw-r--r--   0        0        0     2565 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_metadata.py
--rw-r--r--   0        0        0      977 2024-03-04 01:50:45.458141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_performance_info.py
--rw-r--r--   0        0        0     1995 2024-03-04 01:50:45.462141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_response.py
--rw-r--r--   0        0        0      504 2024-03-04 01:50:45.462141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_share.py
--rw-r--r--   0        0        0      536 2024-03-04 01:50:45.462141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_state.py
--rw-r--r--   0        0        0      567 2024-03-04 01:50:45.462141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_type.py
--rw-r--r--   0        0        0      559 2024-03-04 01:50:45.462141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/share_type.py
--rw-r--r--   0        0        0     1680 2024-03-04 01:50:45.462141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/status.py
--rw-r--r--   0        0        0      661 2024-03-04 01:50:45.462141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/summary_type.py
--rw-r--r--   0        0        0     1015 2024-03-04 01:50:45.462141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/table_noise_impact.py
--rw-r--r--   0        0        0     2411 2024-03-04 01:50:45.462141 adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/temp_table.py
--rw-r--r--   0        0        0      562 2024-03-04 01:50:45.462141 adsdatahub-0.0.1/src/adsdatahub/types.py
--rw-r--r--   0        0        0      815 1970-01-01 00:00:00.000000 adsdatahub-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      292 2024-04-02 08:41:16.592272 adsdatahub-0.0.2/README.md
+-rw-r--r--   0        0        0     1241 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      206 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/__init__.py
+-rw-r--r--   0        0        0     2188 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/_helpers.py
+-rw-r--r--   0        0        0      137 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/__init__.py
+-rw-r--r--   0        0        0     1001 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/client.py
+-rw-r--r--   0        0        0        0 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/customer/__init__.py
+-rw-r--r--   0        0        0      888 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/customer/customer.py
+-rw-r--r--   0        0        0     2209 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/customer/mock_customer.py
+-rw-r--r--   0        0        0     2756 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/customer/real_customer.py
+-rw-r--r--   0        0        0      450 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/mock_client.py
+-rw-r--r--   0        0        0     1969 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/parameters/__init__.py
+-rw-r--r--   0        0        0     3165 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/parameters/primitive_parameters.py
+-rw-r--r--   0        0        0     4213 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/parameters/pydantic_parameters.py
+-rw-r--r--   0        0        0        0 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/query_job/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/query_job/mock_query_job.py
+-rw-r--r--   0        0        0      148 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/query_job/query_job.py
+-rw-r--r--   0        0        0      310 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/query_job/real_query_job.py
+-rw-r--r--   0        0        0     1101 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/query_result.py
+-rw-r--r--   0        0        0     1114 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/client/real_client.py
+-rw-r--r--   0        0        0     4135 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/py.typed
+-rw-r--r--   0        0        0      137 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/__init__.py
+-rw-r--r--   0        0        0     4149 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/client.py
+-rw-r--r--   0        0        0      137 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/http/__init__.py
+-rw-r--r--   0        0        0     2117 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/http/client.py
+-rw-r--r--   0        0        0     2663 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/http/mock_client.py
+-rw-r--r--   0        0        0     1783 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/http/real_client.py
+-rw-r--r--   0        0        0     2305 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/mock_client.py
+-rw-r--r--   0        0        0     4849 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/real_client.py
+-rw-r--r--   0        0        0        0 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/__init__.py
+-rw-r--r--   0        0        0     6040 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/__init__.py
+-rw-r--r--   0        0        0     1450 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/list.py
+-rw-r--r--   0        0        0     1203 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/start_transient.py
+-rw-r--r--   0        0        0     3634 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/validate.py
+-rw-r--r--   0        0        0     5065 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_query/__init__.py
+-rw-r--r--   0        0        0     1105 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_query/start.py
+-rw-r--r--   0        0        0     6604 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operation/__init__.py
+-rw-r--r--   0        0        0      727 2024-04-02 08:41:16.596272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operation/wait.py
+-rw-r--r--   0        0        0     2909 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operations/__init__.py
+-rw-r--r--   0        0        0      911 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operations/list.py
+-rw-r--r--   0        0        0        0 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/__init__.py
+-rw-r--r--   0        0        0      234 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/_model.py
+-rw-r--r--   0        0        0     1743 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/analysis_queries_start.py
+-rw-r--r--   0        0        0    12487 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/analysis_query.py
+-rw-r--r--   0        0        0     1180 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/analysis_query_metadata.py
+-rw-r--r--   0        0        0      214 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/column.py
+-rw-r--r--   0        0        0      735 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/column_info.py
+-rw-r--r--   0        0        0      671 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/column_summary_rule.py
+-rw-r--r--   0        0        0     1422 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/date.py
+-rw-r--r--   0        0        0     2450 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/destination_table_info.py
+-rw-r--r--   0        0        0     1364 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/field_type.py
+-rw-r--r--   0        0        0      936 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/filtered_row_summary.py
+-rw-r--r--   0        0        0     1202 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/merge_column.py
+-rw-r--r--   0        0        0      442 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/merge_spec.py
+-rw-r--r--   0        0        0      636 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/merge_type.py
+-rw-r--r--   0        0        0      677 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/noise_impact.py
+-rw-r--r--   0        0        0     3132 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/operation.py
+-rw-r--r--   0        0        0      661 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/output_artifacts.py
+-rw-r--r--   0        0        0     1188 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/parameter_type.py
+-rw-r--r--   0        0        0     1012 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/parameter_value.py
+-rw-r--r--   0        0        0      508 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/privacy_message.py
+-rw-r--r--   0        0        0     2349 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/privacy_message_type.py
+-rw-r--r--   0        0        0     3861 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_execution_spec.py
+-rw-r--r--   0        0        0     2565 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_metadata.py
+-rw-r--r--   0        0        0      977 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_performance_info.py
+-rw-r--r--   0        0        0     1995 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_response.py
+-rw-r--r--   0        0        0      504 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_share.py
+-rw-r--r--   0        0        0      536 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_state.py
+-rw-r--r--   0        0        0      567 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_type.py
+-rw-r--r--   0        0        0      559 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/share_type.py
+-rw-r--r--   0        0        0     1680 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/status.py
+-rw-r--r--   0        0        0      661 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/summary_type.py
+-rw-r--r--   0        0        0     1015 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/table_noise_impact.py
+-rw-r--r--   0        0        0     2411 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/temp_table.py
+-rw-r--r--   0        0        0      562 2024-04-02 08:41:16.600272 adsdatahub-0.0.2/src/adsdatahub/types.py
+-rw-r--r--   0        0        0      912 1970-01-01 00:00:00.000000 adsdatahub-0.0.2/PKG-INFO
```

### Comparing `adsdatahub-0.0.1/pyproject.toml` & `adsdatahub-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tool.poetry]
 name = "adsdatahub"
-version = "0.0.1"
+version = "0.0.2"
 description = "Ads Data Hub API client for Python"
 authors = ["yassun7010 <yassun7010@outlook.com>"]
 readme = "README.md"
 packages = [{ include = "adsdatahub", from = "src" }]
 
 [tool.poetry.dependencies]
 python = "^3.11"
 google-api-python-client = "^2.114.0"
+google-cloud-bigquery = "^3.17.2"
+httpx = "^0.26.0"
 pydantic = "^2.6.1"
 typing-extensions = "^4.9.0"
-httpx = "^0.26.0"
-google-cloud-bigquery = "^3.17.2"
 
 
 [tool.poetry.group.dev.dependencies]
+db-dtypes = "^1.2.0"
 google-api-python-client-stubs = "^1.23.0"
-pytest = "^8.0.2"
-taskipy = "^1.12.2"
-pyright = "^1.1.348"
 ipython = "^8.20.0"
-ruff = "^0.3.0"
-pytest-xdist = "^3.5.0"
+pandas = "^2.2.1"
+pyright = "^1.1.348"
+pytest = "^8.0.2"
 pytest-asyncio = "^0.23.5"
 pytest-cov = "^4.1.0"
-pandas = "^2.2.1"
-db-dtypes = "^1.2.0"
+pytest-xdist = "^3.5.0"
+ruff = "^0.3.0"
+taskipy = "^1.12.2"
 
 [tool.taskipy.tasks]
 format = "ruff format ."
 lint = "ruff check ."
 typecheck = "pyright src/** tests/** examples/**"
 test = "pytest -n auto --cov=src --cov-report=term --cov-report=xml tests"
 ci = "task format && task lint && task typecheck && task test"
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/client/client.py` & `adsdatahub-0.0.2/src/adsdatahub/client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from google.cloud import bigquery
 
 import adsdatahub.restapi
 from adsdatahub.restapi.real_client import RealRestApiClientConstructerKwargs
 from adsdatahub.types import CustomerId
 
 if TYPE_CHECKING:
-    from adsdatahub.client.customer import CustomerClient
+    from adsdatahub.client.customer.customer import CustomerClient
 
 
 class Client:
     def __new__(
         cls,
         restapi_client: adsdatahub.restapi.Client | None = None,
         bigquery_client: bigquery.Client | None = None,
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/client/customer.py` & `adsdatahub-0.0.2/src/adsdatahub/client/customer/customer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import datetime
 from abc import ABC, abstractmethod
 
+from pydantic import BaseModel
+
 import adsdatahub
-from adsdatahub.client.parameters import PythonParameterType
+from adsdatahub.client.parameters import (
+    PythonParameter,
+)
 from adsdatahub.client.query_result import QueryResult
 from adsdatahub.types import CustomerId
 
 
 class CustomerClient(ABC):
     def __init__(
         self,
@@ -15,21 +19,21 @@
     ): ...
 
     @abstractmethod
     def query(
         self,
         query_text: str,
         /,
-        parameters: dict[str, PythonParameterType] | None = None,
+        parameters: dict[str, PythonParameter] | BaseModel | None = None,
         *,
         start_date: str | datetime.date,
         end_date: str | datetime.date,
         dest_table: str,
     ) -> QueryResult: ...
 
     @abstractmethod
     def validate(
         self,
         query_text: str,
         /,
-        parameters: dict[str, PythonParameterType] | None = None,
+        parameters: dict[str, PythonParameter] | BaseModel | None = None,
     ) -> None: ...
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/client/parameters.py` & `adsdatahub-0.0.2/src/adsdatahub/client/parameters/primitive_parameters.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,56 +12,44 @@
 from adsdatahub.restapi.schemas.parameter_value import (
     ArrayValueDict,
     ArrayValueValuesDict,
     ParameterValueDict,
     ValueDict,
 )
 
-# TODO: 配列の型、デフォルト値などをサポートする必要があるが、後回し。
-#
-# TODO: デフォルト値や NULL のサポートをするためには、 dataclass や pydantic を利用する必要がある。
-#
-# NOTE: ドキュメントの記載は一貫性がない。
-#       1. STRING または INT64 のプリミティブ型に加えて、配列と構造体をサポートしているように見える。
-#          https://developers.google.com/ads-data-hub/reference/rest/v1/FieldType?hl=ja
-#
-#       2. AdsDataHub のコンソールからはさらに多くのパラメータの型を扱うことができるようだ。
-#          https://developers.google.com/ads-data-hub/guides/run-queries?hl=ja#parameter_types
-#
-PythonParameterType = (
+PrimitivePythonParameter = (
     str
     | int
     | float
     | bool
     | datetime.date
     | datetime.datetime
-    | list["PythonParameterType"]
+    | list["PrimitivePythonParameter"]
 )
-"""
-クエリのパラメータとして使える Python の型。
-"""
 
 
-def convert_param_types(
-    params: dict[str, PythonParameterType],
+def convert_primitive_parameter_types(
+    params: dict[str, PrimitivePythonParameter],
 ) -> dict[str, ParameterTypeDict]:
     return {
-        key: ParameterTypeDict({"type": convert_parameter_type(value)})
+        key: ParameterTypeDict({"type": convert_primitive_parameter_type(value)})
         for key, value in params.items()
     }
 
 
-def convert_param_values(
-    params: dict[str, PythonParameterType],
+def convert_primitive_parameter_values(
+    params: dict[str, PrimitivePythonParameter],
 ) -> dict[str, ParameterValueDict]:
-    return {key: convert_parameter_value(value) for key, value in params.items()}
+    return {
+        key: convert_primitive_parameter_value(value) for key, value in params.items()
+    }
 
 
-def convert_parameter_type(
-    value: PythonParameterType,
+def convert_primitive_parameter_type(
+    value: PrimitivePythonParameter,
 ) -> FieldTypeDict:
     match value:
         case str():
             return TypeDict({"type": "STRING"})
 
         case int():
             return TypeDict({"type": "INT64"})
@@ -77,50 +65,50 @@
 
         case datetime.datetime():
             return TypeDict({"type": "TIMESTAMP"})
 
         case list():
             return ArrayTypeDict(
                 {
-                    "arrayType": convert_parameter_type(
+                    "arrayType": convert_primitive_parameter_type(
                         # NOTE: 配列の要素が空の場合は、型を推測できないため、文字列を仮に入れる。
                         #       クエリ文の側でパラメータの型が明確である場合、文字列は自動で変換処理されるため、最も安全な選択肢となる。
                         value[0] if len(value) > 0 else "STRING"
                     )
                 }
             )
 
         case _ as unreachable:
             assert_never(unreachable)
 
 
-def convert_parameter_value(value: PythonParameterType) -> ParameterValueDict:
+def convert_primitive_parameter_value(
+    value: PrimitivePythonParameter,
+) -> ParameterValueDict:
     match value:
         case str():
             return ValueDict({"value": value})
 
-        case int():
-            return ValueDict({"value": str(value)})
-
-        case float():
-            return ValueDict({"value": str(value)})
-
         case bool():
-            return ValueDict({"value": str(value)})
+            return ValueDict({"value": str(value).upper()})
 
-        case datetime.date():
-            return ValueDict({"value": value.isoformat()})
+        case int() | float():
+            return ValueDict({"value": str(value)})
 
-        case datetime.datetime():
+        case datetime.date() | datetime.datetime():
             return ValueDict({"value": value.isoformat()})
 
         case list():
             return ArrayValueDict(
                 {
                     "arrayValue": ArrayValueValuesDict(
-                        {"values": [convert_parameter_value(v) for v in value]}
+                        {
+                            "values": [
+                                convert_primitive_parameter_value(v) for v in value
+                            ]
+                        }
                     )
                 }
             )
 
         case _ as unreachable:
             assert_never(unreachable)
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/client/query_result.py` & `adsdatahub-0.0.2/src/adsdatahub/client/query_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from functools import cache
 
-from google.cloud import bigquery
-
+from adsdatahub.client.query_job.query_job import QueryJob
 from adsdatahub.exceptions import AdsDataHubDestinationTableInfoNotFound
 from adsdatahub.restapi.schemas.analysis_query_metadata import (
     AnalysisQueryMetadataModel,
 )
 from adsdatahub.restapi.schemas.destination_table_info import DestinationTableInfoModel
 from adsdatahub.restapi.schemas.operation import (
     OperationModel,
@@ -14,15 +13,15 @@
 
 class QueryResult:
     def __init__(
         self,
         *,
         dest_table: str,
         operation: OperationModel[AnalysisQueryMetadataModel],
-        job: bigquery.QueryJob,
+        job: QueryJob,
     ) -> None:
         self.dest_table = dest_table
         self.operation = operation
         self.job = job
 
     @property
     @cache
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/client/real_client.py` & `adsdatahub-0.0.2/src/adsdatahub/client/real_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,10 +26,10 @@
             bigquery_client = bigquery.Client(**kwargs)
 
         self.restapi = restapi_client
         self.bigquery_client = bigquery_client
 
     @override
     def customer(self, customer_id: CustomerId):
-        from adsdatahub.client.real_customer import RealCustomerClient
+        from adsdatahub.client.customer.real_customer import RealCustomerClient
 
         return RealCustomerClient(self, customer_id)
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/client/real_customer.py` & `adsdatahub-0.0.2/src/adsdatahub/client/customer/real_customer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import datetime
 from time import sleep
 
+from pydantic import BaseModel
 from typing_extensions import override
 
 import adsdatahub
-from adsdatahub.client.customer import CustomerClient
+from adsdatahub.client.customer.customer import CustomerClient
 from adsdatahub.client.parameters import (
-    PythonParameterType,
-    convert_param_types,
-    convert_param_values,
+    PythonParameter,
+    convert_parameter_types,
+    convert_parameter_values,
 )
+from adsdatahub.client.query_job.real_query_job import RealQueryJob
 from adsdatahub.client.query_result import QueryResult
 from adsdatahub.types import CustomerId
 
 
 class RealCustomerClient(CustomerClient):
     def __init__(
         self,
@@ -24,33 +26,33 @@
         self.customer_id = customer_id
 
     @override
     def query(
         self,
         query_text: str,
         /,
-        parameters: dict[str, PythonParameterType] | None = None,
+        parameters: dict[str, PythonParameter] | BaseModel | None = None,
         *,
         start_date: str | datetime.date,
         end_date: str | datetime.date,
         dest_table: str,
     ) -> QueryResult:
         operation = self._client.restapi.resource(
             "https://adsdatahub.googleapis.com/v1/customers/{customer_id}/analysisQueries",
             customer_id=self.customer_id,
         ).start_transient(
             {
                 "query": {
                     "queryText": query_text,
-                    "parameterTypes": convert_param_types(parameters or {}),
+                    "parameterTypes": convert_parameter_types(parameters or {}),
                 },
                 "spec": {
                     "startDate": start_date,
                     "endDate": end_date,
-                    "parameterValues": convert_param_values(parameters or {}),
+                    "parameterValues": convert_parameter_values(parameters or {}),
                 },
                 "destTable": dest_table,
             }
         )
 
         while not (
             operation := self._client.restapi.resource(
@@ -59,28 +61,30 @@
             ).wait()
         ).done:
             sleep(3)
 
         return QueryResult(
             dest_table=dest_table,
             operation=operation,
-            job=self._client.bigquery_client.query(f"SELECT * FROM {dest_table}"),
+            job=RealQueryJob(
+                self._client.bigquery_client.query(f"SELECT * FROM {dest_table}")
+            ),
         )
 
     @override
     def validate(
         self,
         query_text: str,
         /,
-        parameters: dict[str, PythonParameterType] | None = None,
+        parameters: dict[str, PythonParameter] | BaseModel | None = None,
     ) -> None:
         self._client.restapi.resource(
             "https://adsdatahub.googleapis.com/v1/customers/{customer_id}/analysisQueries",
             customer_id=self.customer_id,
         ).validate(
             {
                 "query": {
                     "queryText": query_text,
-                    "parameterTypes": convert_param_types(parameters or {}),
+                    "parameterTypes": convert_parameter_types(parameters or {}),
                 }
             }
         )
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/exceptions.py` & `adsdatahub-0.0.2/src/adsdatahub/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,14 +81,27 @@
         return f"ResponseBody has error: {json.dumps(self.error, ensure_ascii=False)}"
 
 
 class AdsDataHubMockError(AdsDataHubError):
     pass
 
 
+class AdsDataHubMockMethodError(AdsDataHubMockError, ValueError):
+    """Mock method error for adsdatahub."""
+
+    def __init__(self, method: str, expected_method: str) -> None:
+        self.method = method
+        self.expected_method = expected_method
+
+    @property
+    @override
+    def message(self) -> str:
+        return f"Mock Method Error {self.method}: expected {self.expected_method}"
+
+
 class AdsDataHubMockDataTypeError(AdsDataHubMockError, TypeError):
     """Mock data type error for adsdatahub."""
 
     def __init__(self, response_type: type, expected_type: type) -> None:
         self.response_type = response_type
         self.expected_type = expected_type
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/_helpers.py` & `adsdatahub-0.0.2/src/adsdatahub/_helpers.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/client.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/client.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/http/client.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/http/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     RequestData,
     RequestExtensions,
     RequestFiles,
     TimeoutTypes,
     URLTypes,
 )
 
-from adsdatahub.restapi._helpers import GenericResponseBody
+from adsdatahub._helpers import GenericResponseBody
 
 
 class HttpRequestKwargs(typing.TypedDict):
     content: typing.NotRequired[typing.Optional[RequestContent]]
     data: typing.NotRequired[typing.Optional[RequestData]]
     files: typing.NotRequired[typing.Optional[RequestFiles]]
     json: typing.NotRequired[typing.Optional[typing.Any]]
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/http/mock_client.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/http/mock_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import typing
 from types import NoneType
 
 from typing_extensions import override
 
+from adsdatahub._helpers import (
+    GenericResponseBody,
+)
 from adsdatahub.exceptions import (
     AdsDataHubMockDataTypeError,
     AdsDataHubMockStoreDataEmptyError,
     AdsDataHubMockStoreKeyError,
 )
-from adsdatahub.restapi._helpers import (
-    GenericResponseBody,
-)
 from adsdatahub.restapi.http.client import HttpRequestKwargs
 from adsdatahub.restapi.schemas._model import Model
 from adsdatahub.types import TimeoutTypes, URLTypes
 
 from .client import Client
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/http/real_client.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/http/real_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import httpx
 from httpx._types import (
     HeaderTypes,
     URLTypes,
 )
 from typing_extensions import override
 
-from adsdatahub.restapi._helpers import (
+from adsdatahub._helpers import (
     GenericResponseBody,
     parse_response_body,
     validate_status_code,
 )
 from adsdatahub.restapi.http.client import Client, HttpRequestKwargs
 from adsdatahub.types import TimeoutTypes
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/mock_client.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/mock_client.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/real_client.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/real_client.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/resources/analysis_queries/__init__.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TYPE_CHECKING, Literal, TypedDict, Unpack
 
-from adsdatahub.restapi._helpers import convert_json_value
+from adsdatahub._helpers import convert_json_value
 from adsdatahub.restapi.resources.analysis_queries.list import (
     AnalysisQueryListQueryParams,
     AnalysisQueryListResponse,
 )
 from adsdatahub.restapi.resources.analysis_queries.start_transient import (
     AnalysisQueriesStartTransientQueryParams,
 )
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/resources/analysis_queries/list.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/list.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/resources/analysis_queries/start_transient.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/start_transient.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/resources/analysis_queries/validate.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_queries/validate.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/resources/analysis_query/__init__.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_query/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import TYPE_CHECKING, Literal, TypedDict, Unpack
 
-from adsdatahub.restapi._helpers import (
+from adsdatahub._helpers import (
     convert_json_value,
 )
 from adsdatahub.restapi.resources.analysis_query.start import (
     AnalysisQueryStartRequestBody,
 )
 from adsdatahub.restapi.schemas.analysis_query import (
     AnalysisQueryModel,
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/resources/analysis_query/start.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/analysis_query/start.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/resources/operation/__init__.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/resources/operation/wait.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operation/wait.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/resources/operations/__init__.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/resources/operations/list.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/resources/operations/list.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/analysis_queries_start.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/analysis_queries_start.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/analysis_query.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/analysis_query.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/analysis_query_metadata.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/analysis_query_metadata.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/column_info.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/column_info.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/column_summary_rule.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/column_summary_rule.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/date.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/date.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/destination_table_info.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/destination_table_info.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/field_type.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/field_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/filtered_row_summary.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/filtered_row_summary.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/merge_column.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/merge_column.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/merge_type.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/merge_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/noise_impact.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/noise_impact.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/operation.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/operation.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/output_artifacts.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/output_artifacts.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/parameter_type.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/parameter_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,7 +42,10 @@
     パラメータの説明。
     """
 
     defaultValue: ParameterValueModel | None = None
     """
     パラメータ値が指定されていない場合に使用する値。
     """
+
+
+ParameterType = ParameterTypeDict | ParameterTypeModel
```

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/parameter_value.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/parameter_value.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/privacy_message_type.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/privacy_message_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_execution_spec.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_execution_spec.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_metadata.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_metadata.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_performance_info.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_performance_info.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_response.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_response.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_state.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_state.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/query_type.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/query_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/share_type.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/share_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/status.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/status.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/summary_type.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/summary_type.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/table_noise_impact.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/table_noise_impact.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/restapi/schemas/temp_table.py` & `adsdatahub-0.0.2/src/adsdatahub/restapi/schemas/temp_table.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/src/adsdatahub/types.py` & `adsdatahub-0.0.2/src/adsdatahub/types.py`

 * *Files identical despite different names*

### Comparing `adsdatahub-0.0.1/PKG-INFO` & `adsdatahub-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adsdatahub
-Version: 0.0.1
+Version: 0.0.2
 Summary: Ads Data Hub API client for Python
 Author: yassun7010
 Author-email: yassun7010@outlook.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -13,11 +13,13 @@
 Requires-Dist: httpx (>=0.26.0,<0.27.0)
 Requires-Dist: pydantic (>=2.6.1,<3.0.0)
 Requires-Dist: typing-extensions (>=4.9.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Google の Ads Data Hub を Python で利用するためのライブラリ
 
+[![pypi package](https://badge.fury.io/py/adsdatahub.svg)](https://pypi.org/project/adsdatahub)
+
 ## 使い方
 
 [examples](https://github.com/yassun7010/adsdatahub-py/tree/main/examples) を参考にすること。
```

