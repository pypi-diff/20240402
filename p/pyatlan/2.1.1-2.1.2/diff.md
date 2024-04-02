# Comparing `tmp/pyatlan-2.1.1.tar.gz` & `tmp/pyatlan-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyatlan-2.1.1.tar", last modified: Thu Mar 28 14:52:41 2024, max compression
+gzip compressed data, was "pyatlan-2.1.2.tar", last modified: Tue Apr  2 18:15:08 2024, max compression
```

## Comparing `pyatlan-2.1.1.tar` & `pyatlan-2.1.2.tar`

### file list

```diff
@@ -1,452 +1,467 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.674620 pyatlan-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-03-28 14:52:34.000000 pyatlan-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-28 14:52:34.000000 pyatlan-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-28 14:52:34.000000 pyatlan-2.1.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-28 14:52:41.674620 pyatlan-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-03-28 14:52:34.000000 pyatlan-2.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.606620 pyatlan-2.1.1/pyatlan/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.606620 pyatlan-2.1.1/pyatlan/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/cache/atlan_tag_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/cache/custom_metadata_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/cache/enum_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/cache/group_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/cache/role_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/cache/user_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.610620 pyatlan-2.1.1/pyatlan/client/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)    76552 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)    57627 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/atlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/impersonate.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/role.py
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/search_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/typedef.py
--rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/client/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    32143 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.610620 pyatlan-2.1.1/pyatlan/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/events/atlan_event_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/events/atlan_lambda_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.610620 pyatlan-2.1.1/pyatlan/generator/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31989 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/class_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/create_typedefs_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.610620 pyatlan-2.1.1/pyatlan/generator/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/templates/enums.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/templates/globals.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/templates/imports.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/templates/init.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/templates/macros.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/templates/module.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/templates/properties.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/templates/referenceable_attributes.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/templates/referenceable_methods.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/generator/templates/structs.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/logging.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.618620 pyatlan-2.1.1/pyatlan/model/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/api_tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.654620 pyatlan-2.1.1/pyatlan/model/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    21284 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/a_d_l_s.py
--rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/a_d_l_s_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/a_d_l_s_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    19392 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/a_d_l_s_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5448 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/a_p_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     9135 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/a_p_i_path.py
--rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/a_p_i_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     6852 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/a_w_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     8080 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     7210 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/airflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/airflow_dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    12232 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/airflow_task.py
--rw-r--r--   0 runner    (1001) docker     (127)   121086 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/atlas_glossary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10927 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/atlas_glossary_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    21251 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/atlas_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (127)    15161 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/auth_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4743 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/auth_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/azure_event_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/azure_event_hub_consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/b_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     2404 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/b_i_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/badge.py
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/calculation_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     4341 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    51924 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/column_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    25572 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/data_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    14949 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/data_product.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/data_quality.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/data_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/data_studio.py
--rw-r--r--   0 runner    (1001) docker     (127)    13402 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/data_studio_asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/database.py
--rw-r--r--   0 runner    (1001) docker     (127)    13410 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dbt.py
--rw-r--r--   0 runner    (1001) docker     (127)    19591 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dbt_column_process.py
--rw-r--r--   0 runner    (1001) docker     (127)    20408 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dbt_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    13968 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dbt_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     6280 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dbt_model_column.py
--rw-r--r--   0 runner    (1001) docker     (127)    18841 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dbt_process.py
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dbt_source.py
--rw-r--r--   0 runner    (1001) docker     (127)    16351 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dbt_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dbt_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/domo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/domo_card.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/domo_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     5769 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/domo_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/domo_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     5436 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dynamo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    29177 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dynamo_d_b_secondary_index.py
--rw-r--r--   0 runner    (1001) docker     (127)    31870 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/dynamo_dbtable.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/event_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     7643 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/function.py
--rw-r--r--   0 runner    (1001) docker     (127)    14423 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/g_c_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     9968 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/g_c_s_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    16171 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/g_c_s_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     6787 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/google.py
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/insight.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/kafka.py
--rw-r--r--   0 runner    (1001) docker     (127)     5935 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/kafka_consumer_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    10046 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/link.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/looker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8176 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/looker_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6272 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/looker_explore.py
--rw-r--r--   0 runner    (1001) docker     (127)     8719 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/looker_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/looker_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/looker_look.py
--rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/looker_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/looker_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/looker_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7268 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/looker_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4508 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/looker_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     6696 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/m_c_incident.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/m_c_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    12363 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/materialised_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/matillion.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/matillion_component.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/matillion_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     7953 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/matillion_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     6794 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/matillion_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/metabase.py
--rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/metabase_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/metabase_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/metabase_question.py
--rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)    10984 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/micro_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_cube.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_dossier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3979 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_fact.py
--rw-r--r--   0 runner    (1001) docker     (127)    15005 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8488 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     7556 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/mode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/mode_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/mode_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/mode_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/mode_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/mode_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/mongo_d_b.py
--rw-r--r--   0 runner    (1001) docker     (127)    36442 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/mongo_d_b_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16686 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/mongo_d_b_database.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/monte_carlo.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/no_s_q_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     9646 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/persona.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/power_b_i.py
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/power_b_i_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4451 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/power_b_i_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/power_b_i_dataflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6486 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/power_b_i_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/power_b_i_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     5242 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/power_b_i_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     3391 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/power_b_i_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     6435 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/power_b_i_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     7494 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/power_b_i_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4741 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/power_b_i_tile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6923 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/power_b_i_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4652 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/preset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/preset_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)    11459 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/preset_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     6780 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/preset_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11972 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/preset_workspace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2378 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/process.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/process_execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/purpose.py
--rw-r--r--   0 runner    (1001) docker     (127)     6583 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/qlik.py
--rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/qlik_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     4583 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/qlik_chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     4815 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/qlik_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/qlik_sheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3155 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/qlik_space.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/qlik_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    12633 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/quick_sight.py
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/quick_sight_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/quick_sight_analysis_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/quick_sight_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     3255 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/quick_sight_dashboard_visual.py
--rw-r--r--   0 runner    (1001) docker     (127)     5244 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/quick_sight_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/quick_sight_dataset_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5605 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/quick_sight_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/readme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/readme_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/redash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/redash_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     7359 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/redash_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     4417 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/redash_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    10967 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/referenceable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     8146 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/s3_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    14946 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/s3_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/s_q_l.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/saa_s.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/salesforce.py
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/salesforce_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12998 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/salesforce_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/salesforce_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/salesforce_organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4507 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/salesforce_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    12216 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/schema_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     8956 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/schema_registry_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     6318 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sigma.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sigma_data_element.py
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sigma_data_element_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sigma_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sigma_dataset_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sigma_page.py
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sigma_workbook.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sisense.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sisense_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    10613 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sisense_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    10997 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sisense_datamodel_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     5474 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sisense_folder.py
--rw-r--r--   0 runner    (1001) docker     (127)     8166 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/sisense_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/snowflake_dynamic_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     4670 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/snowflake_pipe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6074 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/snowflake_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    20152 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/snowflake_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/soda.py
--rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/soda_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    16432 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    14072 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/table_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tableau.py
--rw-r--r--   0 runner    (1001) docker     (127)    10726 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tableau_calculated_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tableau_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    12818 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tableau_datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)    16136 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tableau_datasource_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     7128 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tableau_flow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5085 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tableau_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     8342 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tableau_project.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tableau_site.py
--rw-r--r--   0 runner    (1001) docker     (127)     7962 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tableau_workbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tableau_worksheet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4079 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/tag_attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     4233 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/thoughtspot.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_answer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8564 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_column.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_dashlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_liveboard.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_worksheet.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/assets/view.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/atlan_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    12548 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/data_mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    75781 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/events.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.654620 pyatlan-2.1.1/pyatlan/model/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    67647 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/fields/atlan_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/fluent_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/fluent_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/group.py
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/keycloak_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/lineage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.658620 pyatlan-2.1.1/pyatlan/model/packages/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/packages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.658620 pyatlan-2.1.1/pyatlan/model/packages/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/packages/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/packages/base/crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/packages/base/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/packages/confluent_kafka_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/packages/dbt_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/packages/glue_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/packages/powerbi_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/packages/sigma_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/packages/snowflake_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/packages/sql_server_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/packages/tableau_crawler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    66000 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/search.py
--rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/search_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     8459 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/task.py
--rw-r--r--   0 runner    (1001) docker     (127)    42530 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/typedef.py
--rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/model/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/multipart_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.658620 pyatlan-2.1.1/pyatlan/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/pkg/create_package_files.py
--rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/pkg/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.658620 pyatlan-2.1.1/pyatlan/pkg/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/pkg/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/pkg/templates/default_configmap.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/pkg/templates/default_template.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/pkg/templates/package_config.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/pkg/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/pkg/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33619 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/pkg/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    14145 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-28 14:52:34.000000 pyatlan-2.1.1/pyatlan/version.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.674620 pyatlan-2.1.1/pyatlan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-03-28 14:52:41.000000 pyatlan-2.1.1/pyatlan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15049 2024-03-28 14:52:41.000000 pyatlan-2.1.1/pyatlan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:52:41.000000 pyatlan-2.1.1/pyatlan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:52:41.000000 pyatlan-2.1.1/pyatlan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-28 14:52:41.000000 pyatlan-2.1.1/pyatlan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-28 14:52:41.000000 pyatlan-2.1.1/pyatlan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-28 14:52:34.000000 pyatlan-2.1.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-28 14:52:34.000000 pyatlan-2.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 14:52:41.674620 pyatlan-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-03-28 14:52:34.000000 pyatlan-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.658620 pyatlan-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.662620 pyatlan-2.1.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/adls_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/admin_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/api_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/atlan_tag_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    38552 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/custom_metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/custom_package_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/data_mesh_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/data_studio_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/gcs_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26890 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    26620 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/lineage_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/owner_propagator_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/persona_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/preset_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/purpose_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/requests_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/s3_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28660 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    12961 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/test_index_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/test_sql_assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/test_task_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/integration/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.666620 pyatlan-2.1.1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    22096 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.674620 pyatlan-2.1.1/tests/unit/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/a_d_l_s_account_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/a_d_l_s_container_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/a_d_l_s_object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/a_p_i_path_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/a_p_i_spec_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/badge_condition_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/badge_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/column_process_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/column_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/connection_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/data_domain_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/data_product_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/data_studio_asset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/database_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.674620 pyatlan-2.1.1/tests/unit/model/fields/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/fields/atlan_fields_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/file_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/gcs_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/gcs_object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/glossary_category_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/glossary_term_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/glossary_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/materialised_view_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/preset_chart_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/preset_dashboard_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/preset_dataset_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/preset_workspace_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/process_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/readme_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/s3_bucket_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/s3object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/table_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/model/view_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:41.674620 pyatlan-2.1.1/tests/unit/pkg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/pkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/pkg/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/pkg/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/pkg/test_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/pkg/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    53584 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/pkg/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_atlan_tag_name.py
--rw-r--r--   0 runner    (1001) docker     (127)    64064 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_credential_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_custom_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_glossary_term.py
--rw-r--r--   0 runner    (1001) docker     (127)    36843 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_lineage.py
--rw-r--r--   0 runner    (1001) docker     (127)    33878 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_query_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_search_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_task_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14731 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_typedef_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-03-28 14:52:34.000000 pyatlan-2.1.1/tests/unit/test_workflow_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.684664 pyatlan-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-04-02 18:14:59.000000 pyatlan-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-02 18:14:59.000000 pyatlan-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-02 18:14:59.000000 pyatlan-2.1.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-02 18:15:08.684664 pyatlan-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-04-02 18:14:59.000000 pyatlan-2.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.600663 pyatlan-2.1.2/pyatlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.604663 pyatlan-2.1.2/pyatlan/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/cache/atlan_tag_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19611 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/cache/custom_metadata_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/cache/enum_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/cache/group_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/cache/role_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/cache/user_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.608663 pyatlan-2.1.2/pyatlan/client/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76624 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57645 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/atlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13720 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/impersonate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/search_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10060 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16727 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10743 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/client/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32143 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.608663 pyatlan-2.1.2/pyatlan/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9218 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/events/atlan_event_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/events/atlan_lambda_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.608663 pyatlan-2.1.2/pyatlan/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32114 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/class_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/create_typedefs_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.612663 pyatlan-2.1.2/pyatlan/generator/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/templates/enums.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/templates/globals.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/templates/imports.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/templates/init.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/templates/macros.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/templates/module.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/templates/properties.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/templates/referenceable_attributes.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/templates/referenceable_methods.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/generator/templates/structs.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/logging.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.616664 pyatlan-2.1.2/pyatlan/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/api_tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.660664 pyatlan-2.1.2/pyatlan/model/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    22599 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9774 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/a_d_l_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12560 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/a_d_l_s_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10410 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/a_d_l_s_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19431 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/a_d_l_s_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5487 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/a_p_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9174 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/a_p_i_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/a_p_i_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6891 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/a_w_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8119 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/airflow_dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12271 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/airflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)   122057 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/atlas_glossary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10966 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/atlas_glossary_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21290 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/atlas_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15200 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/auth_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/auth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1957 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/azure_event_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/azure_event_hub_consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/b_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/b_i_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/badge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/calculation_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5893 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/cognite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/cognite3_d_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/cognite_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/cognite_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/cognite_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/cognite_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/cognite_time_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51963 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/column_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25611 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/cube_dimension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7553 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/cube_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/cube_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6310 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/data_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3078 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14988 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/data_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/data_quality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/data_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11570 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/data_studio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13441 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/data_studio_asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4823 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20274 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dbt_column_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20447 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dbt_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dbt_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6319 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dbt_model_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19524 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dbt_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dbt_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16390 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dbt_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dbt_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/domo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/domo_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4271 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/domo_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5808 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/domo_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/domo_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dynamo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2097 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29820 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dynamo_d_b_secondary_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32513 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/dynamo_dbtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/event_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7682 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15975 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/g_c_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10007 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/g_c_s_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16210 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/g_c_s_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/insight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/kafka.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/kafka_consumer_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10085 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/looker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/looker_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/looker_explore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/looker_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/looker_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10701 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/looker_look.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4899 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/looker_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/looker_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/looker_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/looker_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4547 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/looker_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/m_c_incident.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16268 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/m_c_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12402 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/materialised_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/matillion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10098 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/matillion_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/matillion_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/matillion_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6833 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/matillion_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/metabase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5719 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/metabase_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/metabase_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/metabase_question.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6138 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11023 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/micro_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5624 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_cube.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_dossier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_fact.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8527 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6163 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7595 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/mode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/mode_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4044 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/mode_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/mode_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/mode_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2724 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/mode_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/mongo_d_b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37085 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/mongo_d_b_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/mongo_d_b_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/monte_carlo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6245 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/multi_dimensional_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/no_s_q_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9685 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/persona.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/power_b_i.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6916 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/power_b_i_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/power_b_i_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/power_b_i_dataflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6525 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/power_b_i_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/power_b_i_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/power_b_i_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/power_b_i_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/power_b_i_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7533 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/power_b_i_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4780 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/power_b_i_tile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/power_b_i_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/preset_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11498 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/preset_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/preset_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12011 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/preset_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10574 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/process_execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/purpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/qlik.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6386 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/qlik_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/qlik_chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/qlik_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/qlik_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/qlik_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/qlik_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12672 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/quick_sight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/quick_sight_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/quick_sight_analysis_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5612 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/quick_sight_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/quick_sight_dashboard_visual.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/quick_sight_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/quick_sight_dataset_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/quick_sight_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/readme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/readme_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/redash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/redash_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7398 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/redash_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/redash_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10967 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/referenceable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8185 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6791 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/s3_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14985 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/s3_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16566 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/s_q_l.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/saa_s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/salesforce.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/salesforce_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13037 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/salesforce_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5718 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/salesforce_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/salesforce_organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/salesforce_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13297 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/schema_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8995 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/schema_registry_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sigma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5256 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sigma_data_element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3968 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sigma_data_element_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sigma_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sigma_dataset_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sigma_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sigma_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sisense.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5568 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sisense_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10652 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sisense_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11036 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sisense_datamodel_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5513 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sisense_folder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8205 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/sisense_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/snowflake_dynamic_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/snowflake_pipe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6113 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/snowflake_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20191 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/snowflake_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/soda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6425 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/soda_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5258 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/spark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4303 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/spark_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17075 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14111 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/table_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tableau.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tableau_calculated_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6646 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tableau_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12857 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tableau_datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16175 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tableau_datasource_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7167 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tableau_flow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tableau_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tableau_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tableau_site.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8001 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tableau_workbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8259 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tableau_worksheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2875 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/tag_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/thoughtspot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_answer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8603 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_dashlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_liveboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_worksheet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/assets/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/atlan_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10775 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12589 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3531 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/data_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75818 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6387 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/events.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.660664 pyatlan-2.1.2/pyatlan/model/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67647 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/fields/atlan_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15521 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/fluent_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/fluent_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/keycloak_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25077 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/lineage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.660664 pyatlan-2.1.2/pyatlan/model/packages/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/packages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.664664 pyatlan-2.1.2/pyatlan/model/packages/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/packages/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/packages/base/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/packages/base/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/packages/confluent_kafka_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10049 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/packages/dbt_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8141 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/packages/glue_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9586 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/packages/powerbi_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8037 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/packages/sigma_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11135 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/packages/snowflake_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8327 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/packages/sql_server_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/packages/tableau_crawler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16364 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66000 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15452 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/search_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8953 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6984 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43068 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/typedef.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13722 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5697 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/model/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/multipart_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.664664 pyatlan-2.1.2/pyatlan/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4336 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/pkg/create_package_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11206 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/pkg/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.664664 pyatlan-2.1.2/pyatlan/pkg/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/pkg/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/pkg/templates/default_configmap.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/pkg/templates/default_template.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/pkg/templates/package_config.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/pkg/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/pkg/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33619 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/pkg/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12901 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-02 18:14:59.000000 pyatlan-2.1.2/pyatlan/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.684664 pyatlan-2.1.2/pyatlan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-04-02 18:15:08.000000 pyatlan-2.1.2/pyatlan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15603 2024-04-02 18:15:08.000000 pyatlan-2.1.2/pyatlan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:15:08.000000 pyatlan-2.1.2/pyatlan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:15:08.000000 pyatlan-2.1.2/pyatlan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 18:15:08.000000 pyatlan-2.1.2/pyatlan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-02 18:15:08.000000 pyatlan-2.1.2/pyatlan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 18:14:59.000000 pyatlan-2.1.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-04-02 18:14:59.000000 pyatlan-2.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:15:08.684664 pyatlan-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-04-02 18:14:59.000000 pyatlan-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.664664 pyatlan-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.672664 pyatlan-2.1.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/adls_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9488 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/admin_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7826 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/api_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/atlan_tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39630 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/custom_metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/custom_package_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/data_mesh_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10773 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/data_studio_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/gcs_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26890 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26620 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/lineage_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/owner_propagator_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/persona_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10933 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/preset_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11082 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/purpose_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/requests_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/s3_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28660 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12961 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/test_index_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19321 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/test_sql_assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/test_task_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/integration/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.676664 pyatlan-2.1.2/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22096 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.680664 pyatlan-2.1.2/tests/unit/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/a_d_l_s_account_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/a_d_l_s_container_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/a_d_l_s_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/a_p_i_path_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/a_p_i_spec_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/badge_condition_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3133 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/badge_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/column_process_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/column_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/connection_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/data_domain_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/data_product_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4143 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/data_studio_asset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/database_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.680664 pyatlan-2.1.2/tests/unit/model/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/fields/atlan_fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/file_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/gcs_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1961 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/gcs_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/glossary_category_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/glossary_term_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/glossary_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/materialised_view_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/preset_chart_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/preset_dashboard_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/preset_dataset_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/preset_workspace_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/process_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/readme_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3355 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/s3_bucket_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8949 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/s3object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/table_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/model/view_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:15:08.684664 pyatlan-2.1.2/tests/unit/pkg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/pkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/pkg/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5147 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/pkg/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/pkg/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/pkg/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53584 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/pkg/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_atlan_tag_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64064 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6056 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6104 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_credential_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8366 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_custom_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18206 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8734 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_glossary_term.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36843 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_lineage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33878 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14579 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_query_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42984 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_search_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_task_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_typedef_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8096 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10431 2024-04-02 18:14:59.000000 pyatlan-2.1.2/tests/unit/test_workflow_client.py
```

### Comparing `pyatlan-2.1.1/LICENSE` & `pyatlan-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/PKG-INFO` & `pyatlan-2.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 2.1.1
+Version: 2.1.2
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyatlan-2.1.1/README.md` & `pyatlan-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/cache/atlan_tag_cache.py` & `pyatlan-2.1.2/pyatlan/cache/atlan_tag_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/cache/custom_metadata_cache.py` & `pyatlan-2.1.2/pyatlan/cache/custom_metadata_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/cache/enum_cache.py` & `pyatlan-2.1.2/pyatlan/cache/enum_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/cache/group_cache.py` & `pyatlan-2.1.2/pyatlan/cache/group_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/cache/role_cache.py` & `pyatlan-2.1.2/pyatlan/cache/role_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/cache/user_cache.py` & `pyatlan-2.1.2/pyatlan/cache/user_cache.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/admin.py` & `pyatlan-2.1.2/pyatlan/client/admin.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/asset.py` & `pyatlan-2.1.2/pyatlan/client/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -738,24 +738,24 @@
         api: API,
         asset_type: Type[A],
         qualified_name: str,
         atlan_tag_names: List[str],
         propagate: bool = True,
         remove_propagation_on_delete: bool = True,
         restrict_lineage_propagation: bool = True,
-        propagation_only_through_lineage: bool = False,
+        restrict_propagation_through_hierarchy: bool = False,
     ) -> None:
         atlan_tags = AtlanTags(
             __root__=[
                 AtlanTag(
                     type_name=AtlanTagName(display_text=name),
                     propagate=propagate,
                     remove_propagations_on_entity_delete=remove_propagation_on_delete,
                     restrict_propagation_through_lineage=restrict_lineage_propagation,
-                    propagation_only_through_lineage=propagation_only_through_lineage,
+                    restrict_propagation_through_hierarchy=restrict_propagation_through_hierarchy,
                 )
                 for name in atlan_tag_names
             ]
         )
         query_params = {"attr:qualifiedName": qualified_name}
         self._client._call_api(
             api.format_path_with_params(asset_type.__name__, "classifications"),
@@ -768,81 +768,81 @@
         self,
         asset_type: Type[A],
         qualified_name: str,
         atlan_tag_names: List[str],
         propagate: bool = True,
         remove_propagation_on_delete: bool = True,
         restrict_lineage_propagation: bool = True,
-        propagation_only_through_lineage: bool = False,
+        restrict_propagation_through_hierarchy: bool = False,
     ) -> None:
         """
         Add one or more Atlan tags to the provided asset.
         Note: if one or more of the provided Atlan tags already exist on the asset, an error
         will be raised. (In other words, this operation is NOT idempotent.)
 
         :param asset_type: type of asset to which to add the Atlan tags
         :param qualified_name: qualified_name of the asset to which to add the Atlan tags
         :param atlan_tag_names: human-readable names of the Atlan tags to add to the asset
         :param propagate: whether to propagate the Atlan tag (True) or not (False)
         :param remove_propagation_on_delete: whether to remove the propagated Atlan tags
         when the Atlan tag is removed from this asset (True) or not (False)
         :param restrict_lineage_propagation: whether to avoid propagating
         through lineage (True) or do propagate through lineage (False)
-        :param propagation_only_through_lineage: if specified as `True`,
-        propagation will only occur downstream lineage and not within hierarchy, defaults to `False`.
+        :param restrict_propagation_through_hierarchy: whether to prevent this Atlan tag from
+        propagating through hierarchy (True) or allow it to propagate through hierarchy (False)
         :raises AtlanError: on any API communication issue
         """
         self._modify_tags(
             UPDATE_ENTITY_BY_ATTRIBUTE,
             asset_type,
             qualified_name,
             atlan_tag_names,
             propagate,
             remove_propagation_on_delete,
             restrict_lineage_propagation,
-            propagation_only_through_lineage,
+            restrict_propagation_through_hierarchy,
         )
 
     @validate_arguments
     def update_atlan_tags(
         self,
         asset_type: Type[A],
         qualified_name: str,
         atlan_tag_names: List[str],
         propagate: bool = True,
         remove_propagation_on_delete: bool = True,
         restrict_lineage_propagation: bool = True,
-        propagation_only_through_lineage: bool = False,
+        restrict_propagation_through_hierarchy: bool = False,
     ) -> None:
         """
         Update one or more Atlan tags to the provided asset.
         Note: if one or more of the provided Atlan tags already exist on the asset, an error
         will be raised. (In other words, this operation is NOT idempotent.)
 
         :param asset_type: type of asset to which to update the Atlan tags
         :param qualified_name: qualified_name of the asset to which to update the Atlan tags
         :param atlan_tag_names: human-readable names of the Atlan tags to update to the asset
         :param propagate: whether to propagate the Atlan tag (True) or not (False)
         :param remove_propagation_on_delete: whether to remove the propagated Atlan tags
         when the Atlan tag is removed from this asset (True) or not (False)
         :param restrict_lineage_propagation: whether to avoid propagating
         through lineage (True) or do propagate through lineage (False)
-        :param propagation_only_through_lineage: if specified as `True`,
-        propagation will only occur downstream lineage and not within hierarchy, defaults to `False`.
+        :param restrict_propagation_through_hierarchy: whether to prevent this Atlan tag from
+        propagating through hierarchy (True) or allow it to propagate through hierarchy (False)
         :raises AtlanError: on any API communication issue
         """
         self._modify_tags(
             PARTIAL_UPDATE_ENTITY_BY_ATTRIBUTE,
             asset_type,
             qualified_name,
             atlan_tag_names,
             propagate,
             remove_propagation_on_delete,
             restrict_lineage_propagation,
-            propagation_only_through_lineage,
+            restrict_propagation_through_hierarchy,
         )
 
     @validate_arguments
     def remove_atlan_tag(
         self, asset_type: Type[A], qualified_name: str, atlan_tag_name: str
     ) -> None:
         """
```

### Comparing `pyatlan-2.1.1/pyatlan/client/atlan.py` & `pyatlan-2.1.2/pyatlan/client/atlan.py`

 * *Files 0% similar despite different names*

```diff
@@ -967,15 +967,15 @@
         self,
         asset_type: Type[A],
         qualified_name: str,
         atlan_tag_names: List[str],
         propagate: bool = True,
         remove_propagation_on_delete: bool = True,
         restrict_lineage_propagation: bool = True,
-        propagation_only_through_lineage: bool = False,
+        restrict_propagation_through_hierarchy: bool = False,
     ) -> None:
         """Deprecated - use asset.add_atlan_tags() instead."""
         warn(
             "This method is deprecated, please use 'asset.add_atlan_tags' instead, which offers identical "
             "functionality.",
             DeprecationWarning,
             stacklevel=2,
@@ -983,15 +983,15 @@
         self.asset.add_atlan_tags(
             asset_type=asset_type,
             qualified_name=qualified_name,
             atlan_tag_names=atlan_tag_names,
             propagate=propagate,
             remove_propagation_on_delete=remove_propagation_on_delete,
             restrict_lineage_propagation=restrict_lineage_propagation,
-            propagation_only_through_lineage=propagation_only_through_lineage,
+            restrict_propagation_through_hierarchy=restrict_propagation_through_hierarchy,
         )
 
     @validate_arguments
     def remove_atlan_tag(
         self, asset_type: Type[A], qualified_name: str, atlan_tag_name: str
     ) -> None:
         """Deprecated - use asset.remove_atlan_tag() instead."""
```

### Comparing `pyatlan-2.1.1/pyatlan/client/audit.py` & `pyatlan-2.1.2/pyatlan/client/audit.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/common.py` & `pyatlan-2.1.2/pyatlan/client/common.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/constants.py` & `pyatlan-2.1.2/pyatlan/client/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/credential.py` & `pyatlan-2.1.2/pyatlan/client/credential.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/group.py` & `pyatlan-2.1.2/pyatlan/client/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/impersonate.py` & `pyatlan-2.1.2/pyatlan/client/impersonate.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/query.py` & `pyatlan-2.1.2/pyatlan/client/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/role.py` & `pyatlan-2.1.2/pyatlan/client/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/search_log.py` & `pyatlan-2.1.2/pyatlan/client/search_log.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/task.py` & `pyatlan-2.1.2/pyatlan/client/task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/token.py` & `pyatlan-2.1.2/pyatlan/client/token.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/typedef.py` & `pyatlan-2.1.2/pyatlan/client/typedef.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/user.py` & `pyatlan-2.1.2/pyatlan/client/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/client/workflow.py` & `pyatlan-2.1.2/pyatlan/client/workflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/errors.py` & `pyatlan-2.1.2/pyatlan/errors.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/events/atlan_event_handler.py` & `pyatlan-2.1.2/pyatlan/events/atlan_event_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/events/atlan_lambda_handler.py` & `pyatlan-2.1.2/pyatlan/events/atlan_lambda_handler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/generator/class_generator.py` & `pyatlan-2.1.2/pyatlan/generator/class_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -788,15 +788,17 @@
             key = f"{key[:pos]}_{key[pos:]}"
         key = key.upper().replace(".", "_").replace("-", "_")
         return KeyValue(key, value)
 
     @classmethod
     def create(cls, enum_defs):
         for enum_def in enum_defs:
-            cls.enum_def_info.append(EnumDefInfo(enum_def))
+            # Only pick `atlas_core` enums, not user-created ones.
+            if enum_def.service_type == "atlas_core":
+                cls.enum_def_info.append(EnumDefInfo(enum_def))
         cls.enum_def_info = sorted(cls.enum_def_info, key=lambda e: e.name)
 
 
 def filter_attributes_of_custom_entity_type():
     for entity_def in type_defs.reserved_entity_defs:
         if entity_def.attribute_defs:
             filtered_attribute_defs = [
```

### Comparing `pyatlan-2.1.1/pyatlan/generator/create_typedefs_file.py` & `pyatlan-2.1.2/pyatlan/generator/create_typedefs_file.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/generator/templates/globals.jinja2` & `pyatlan-2.1.2/pyatlan/generator/templates/globals.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/generator/templates/imports.jinja2` & `pyatlan-2.1.2/pyatlan/generator/templates/imports.jinja2`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,14 @@
     MCRuleSchedule,
     PopularityInsights,
     SourceTagAttribute,
     StarredDetails,
 )
 from pyatlan.utils import (
     init_guid,
-    move_struct,
     next_id,
     to_camel_case,
     validate_required_fields,
     validate_single_required_field,
     get_parent_qualified_name,
 )
 from pyatlan.model.data_mesh import DataProductsAssetsDSL
```

### Comparing `pyatlan-2.1.1/pyatlan/generator/templates/macros.jinja2` & `pyatlan-2.1.2/pyatlan/generator/templates/macros.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/generator/templates/module.jinja2` & `pyatlan-2.1.2/pyatlan/generator/templates/module.jinja2`

 * *Files 3% similar despite different names*

```diff
@@ -57,18 +57,21 @@
         {%- set type = attribute_def.typeName | get_type %}
         {{attribute_def.name | to_snake_case }}: Optional[{{type}}]= Field(default=None, description='') # relationship
         {%- endfor %}
         {% set file_name = 'methods/attribute/' + entity_def.name | to_snake_case + '.jinja2' %}
         {%  if existz('templates/' + file_name) %}
             {% include file_name %}
         {% endif %}
-    attributes: '{{entity_def.name}}.Attributes' = Field(
+    attributes: {{entity_def.name}}.Attributes = Field(
         default_factory = lambda: {{entity_def.name}}.Attributes(),
-        description='Map of attributes in the instance and their values. The specific keys of this map will vary by '
-                    'type, so are described in the sub-types of this schema.\n',
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
     {%- endif %}
 {% endif %}
 
 {%  if asset_info.module_name == 'referenceable' %}
 # Imports required for fixing circular dependencies:
 from .asset import Asset  # noqa # isort:skip
```

### Comparing `pyatlan-2.1.1/pyatlan/generator/templates/properties.jinja2` & `pyatlan-2.1.2/pyatlan/generator/templates/properties.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/generator/templates/referenceable_attributes.jinja2` & `pyatlan-2.1.2/pyatlan/generator/templates/referenceable_attributes.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/generator/templates/referenceable_methods.jinja2` & `pyatlan-2.1.2/pyatlan/generator/templates/referenceable_methods.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/generator/templates/structs.jinja2` & `pyatlan-2.1.2/pyatlan/generator/templates/structs.jinja2`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-# Copyright 2022 Atlan Pte. Ltd.
+# SPDX-License-Identifier: Apache-2.0
+# Copyright 2024 Atlan Pte. Ltd.
+
 from __future__ import annotations
+
 from datetime import datetime
-from typing import Dict, List, Optional, Set, Union
+from typing import Dict, List, Optional, Set, Union, Any
 
-from pydantic.v1 import BaseModel, Extra, Field
+from pydantic.v1 import BaseModel, Extra, Field, root_validator
 
 from pyatlan.model.enums import (
     BadgeComparisonOperator,
     BadgeConditionColor,
     SourceCostUnitType,
 )
 from pyatlan.model.utils import to_camel_case
@@ -17,14 +20,26 @@
     class Config:
         allow_population_by_field_name = True
         alias_generator = to_camel_case
         extra = Extra.ignore
         json_encoders = {datetime: lambda v: int(v.timestamp() * 1000)}
         validate_assignment = True
 
+    @root_validator(pre=True)
+    def flatten_structs_attributes(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        """
+        Flatten the 'attributes' of the struct models.
+
+        :param values: dictionary containing the attributes.
+        :returns: modified dictionary with attributes flattened.
+        """
+        attributes = values.pop("attributes", {})
+        values = {**values, **attributes}
+        return values
+
 
 {% for struct in struct_defs %}
 class {{struct.name}}(AtlanObject):
     """Description"""
     {%- if struct.name == "BadgeCondition" %}
     @classmethod
     def create(
```

### Comparing `pyatlan-2.1.1/pyatlan/logging.conf` & `pyatlan-2.1.2/pyatlan/logging.conf`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/aggregation.py` & `pyatlan-2.1.2/pyatlan/model/aggregation.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/api_tokens.py` & `pyatlan-2.1.2/pyatlan/model/api_tokens.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/__init__.py` & `pyatlan-2.1.2/pyatlan/model/assets/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,22 +27,24 @@
 from .folder import Folder
 from .airflow import Airflow
 from .object_store import ObjectStore
 from .data_quality import DataQuality
 from .b_i import BI
 from .saa_s import SaaS
 from .resource import Resource
+from .multi_dimensional_dataset import MultiDimensionalDataset
 from .data_mesh import DataMesh
 from .s_q_l import SQL
 from .event_store import EventStore
 from .no_s_q_l import NoSQL
 from .matillion import Matillion
 from .dbt import Dbt
 from .insight import Insight
 from .a_p_i import API
+from .spark import Spark
 from .tag import Tag
 from .schema_registry import SchemaRegistry
 from .google import Google
 from .azure import Azure
 from .a_w_s import AWS
 from .dbt_column_process import DbtColumnProcess
 from .airflow_dag import AirflowDag
@@ -64,33 +66,38 @@
 from .data_studio import DataStudio
 from .metabase import Metabase
 from .quick_sight import QuickSight
 from .thoughtspot import Thoughtspot
 from .power_b_i import PowerBI
 from .micro_strategy import MicroStrategy
 from .qlik import Qlik
+from .cognite import Cognite
 from .salesforce import Salesforce
 from .readme_template import ReadmeTemplate
 from .readme import Readme
 from .file import File
 from .link import Link
+from .cube import Cube
+from .cube_hierarchy import CubeHierarchy
+from .cube_field import CubeField
+from .cube_dimension import CubeDimension
 from .data_domain import DataDomain
 from .data_product import DataProduct
 from .table import Table
 from .query import Query
 from .schema import Schema
 from .snowflake_pipe import SnowflakePipe
 from .view import View
 from .materialised_view import MaterialisedView
 from .function import Function
 from .table_partition import TablePartition
 from .column import Column
 from .snowflake_stream import SnowflakeStream
-from .database import Database
 from .calculation_view import CalculationView
+from .database import Database
 from .procedure import Procedure
 from .snowflake_tag import SnowflakeTag
 from .kafka import Kafka
 from .dynamo_d_b import DynamoDB
 from .mongo_d_b import MongoDB
 from .matillion_group import MatillionGroup
 from .matillion_job import MatillionJob
@@ -100,14 +107,15 @@
 from .dbt_tag import DbtTag
 from .dbt_test import DbtTest
 from .dbt_model import DbtModel
 from .dbt_metric import DbtMetric
 from .dbt_source import DbtSource
 from .a_p_i_spec import APISpec
 from .a_p_i_path import APIPath
+from .spark_job import SparkJob
 from .schema_registry_subject import SchemaRegistrySubject
 from .data_studio_asset import DataStudioAsset
 from .s3_bucket import S3Bucket
 from .s3_object import S3Object
 from .a_d_l_s_account import ADLSAccount
 from .a_d_l_s_container import ADLSContainer
 from .a_d_l_s_object import ADLSObject
@@ -201,14 +209,20 @@
 from .micro_strategy_attribute import MicroStrategyAttribute
 from .micro_strategy_visualization import MicroStrategyVisualization
 from .qlik_space import QlikSpace
 from .qlik_app import QlikApp
 from .qlik_chart import QlikChart
 from .qlik_dataset import QlikDataset
 from .qlik_sheet import QlikSheet
+from .cognite_event import CogniteEvent
+from .cognite_asset import CogniteAsset
+from .cognite_sequence import CogniteSequence
+from .cognite3_d_model import Cognite3DModel
+from .cognite_time_series import CogniteTimeSeries
+from .cognite_file import CogniteFile
 from .salesforce_object import SalesforceObject
 from .salesforce_field import SalesforceField
 from .salesforce_organization import SalesforceOrganization
 from .salesforce_dashboard import SalesforceDashboard
 from .salesforce_report import SalesforceReport
 from .snowflake_dynamic_table import SnowflakeDynamicTable
 from .mongo_d_b_collection import MongoDBCollection
@@ -253,22 +267,24 @@
 Folder.Attributes.update_forward_refs(**localns)
 Airflow.Attributes.update_forward_refs(**localns)
 ObjectStore.Attributes.update_forward_refs(**localns)
 DataQuality.Attributes.update_forward_refs(**localns)
 BI.Attributes.update_forward_refs(**localns)
 SaaS.Attributes.update_forward_refs(**localns)
 Resource.Attributes.update_forward_refs(**localns)
+MultiDimensionalDataset.Attributes.update_forward_refs(**localns)
 DataMesh.Attributes.update_forward_refs(**localns)
 SQL.Attributes.update_forward_refs(**localns)
 EventStore.Attributes.update_forward_refs(**localns)
 NoSQL.Attributes.update_forward_refs(**localns)
 Matillion.Attributes.update_forward_refs(**localns)
 Dbt.Attributes.update_forward_refs(**localns)
 Insight.Attributes.update_forward_refs(**localns)
 API.Attributes.update_forward_refs(**localns)
+Spark.Attributes.update_forward_refs(**localns)
 Tag.Attributes.update_forward_refs(**localns)
 SchemaRegistry.Attributes.update_forward_refs(**localns)
 Google.Attributes.update_forward_refs(**localns)
 Azure.Attributes.update_forward_refs(**localns)
 AWS.Attributes.update_forward_refs(**localns)
 DbtColumnProcess.Attributes.update_forward_refs(**localns)
 AirflowDag.Attributes.update_forward_refs(**localns)
@@ -290,33 +306,38 @@
 DataStudio.Attributes.update_forward_refs(**localns)
 Metabase.Attributes.update_forward_refs(**localns)
 QuickSight.Attributes.update_forward_refs(**localns)
 Thoughtspot.Attributes.update_forward_refs(**localns)
 PowerBI.Attributes.update_forward_refs(**localns)
 MicroStrategy.Attributes.update_forward_refs(**localns)
 Qlik.Attributes.update_forward_refs(**localns)
+Cognite.Attributes.update_forward_refs(**localns)
 Salesforce.Attributes.update_forward_refs(**localns)
 ReadmeTemplate.Attributes.update_forward_refs(**localns)
 Readme.Attributes.update_forward_refs(**localns)
 File.Attributes.update_forward_refs(**localns)
 Link.Attributes.update_forward_refs(**localns)
+Cube.Attributes.update_forward_refs(**localns)
+CubeHierarchy.Attributes.update_forward_refs(**localns)
+CubeField.Attributes.update_forward_refs(**localns)
+CubeDimension.Attributes.update_forward_refs(**localns)
 DataDomain.Attributes.update_forward_refs(**localns)
 DataProduct.Attributes.update_forward_refs(**localns)
 Table.Attributes.update_forward_refs(**localns)
 Query.Attributes.update_forward_refs(**localns)
 Schema.Attributes.update_forward_refs(**localns)
 SnowflakePipe.Attributes.update_forward_refs(**localns)
 View.Attributes.update_forward_refs(**localns)
 MaterialisedView.Attributes.update_forward_refs(**localns)
 Function.Attributes.update_forward_refs(**localns)
 TablePartition.Attributes.update_forward_refs(**localns)
 Column.Attributes.update_forward_refs(**localns)
 SnowflakeStream.Attributes.update_forward_refs(**localns)
-Database.Attributes.update_forward_refs(**localns)
 CalculationView.Attributes.update_forward_refs(**localns)
+Database.Attributes.update_forward_refs(**localns)
 Procedure.Attributes.update_forward_refs(**localns)
 SnowflakeTag.Attributes.update_forward_refs(**localns)
 Kafka.Attributes.update_forward_refs(**localns)
 DynamoDB.Attributes.update_forward_refs(**localns)
 MongoDB.Attributes.update_forward_refs(**localns)
 MatillionGroup.Attributes.update_forward_refs(**localns)
 MatillionJob.Attributes.update_forward_refs(**localns)
@@ -326,14 +347,15 @@
 DbtTag.Attributes.update_forward_refs(**localns)
 DbtTest.Attributes.update_forward_refs(**localns)
 DbtModel.Attributes.update_forward_refs(**localns)
 DbtMetric.Attributes.update_forward_refs(**localns)
 DbtSource.Attributes.update_forward_refs(**localns)
 APISpec.Attributes.update_forward_refs(**localns)
 APIPath.Attributes.update_forward_refs(**localns)
+SparkJob.Attributes.update_forward_refs(**localns)
 SchemaRegistrySubject.Attributes.update_forward_refs(**localns)
 DataStudioAsset.Attributes.update_forward_refs(**localns)
 S3Bucket.Attributes.update_forward_refs(**localns)
 S3Object.Attributes.update_forward_refs(**localns)
 ADLSAccount.Attributes.update_forward_refs(**localns)
 ADLSContainer.Attributes.update_forward_refs(**localns)
 ADLSObject.Attributes.update_forward_refs(**localns)
@@ -427,14 +449,20 @@
 MicroStrategyAttribute.Attributes.update_forward_refs(**localns)
 MicroStrategyVisualization.Attributes.update_forward_refs(**localns)
 QlikSpace.Attributes.update_forward_refs(**localns)
 QlikApp.Attributes.update_forward_refs(**localns)
 QlikChart.Attributes.update_forward_refs(**localns)
 QlikDataset.Attributes.update_forward_refs(**localns)
 QlikSheet.Attributes.update_forward_refs(**localns)
+CogniteEvent.Attributes.update_forward_refs(**localns)
+CogniteAsset.Attributes.update_forward_refs(**localns)
+CogniteSequence.Attributes.update_forward_refs(**localns)
+Cognite3DModel.Attributes.update_forward_refs(**localns)
+CogniteTimeSeries.Attributes.update_forward_refs(**localns)
+CogniteFile.Attributes.update_forward_refs(**localns)
 SalesforceObject.Attributes.update_forward_refs(**localns)
 SalesforceField.Attributes.update_forward_refs(**localns)
 SalesforceOrganization.Attributes.update_forward_refs(**localns)
 SalesforceDashboard.Attributes.update_forward_refs(**localns)
 SalesforceReport.Attributes.update_forward_refs(**localns)
 SnowflakeDynamicTable.Attributes.update_forward_refs(**localns)
 MongoDBCollection.Attributes.update_forward_refs(**localns)
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/a_d_l_s.py` & `pyatlan-2.1.2/pyatlan/model/assets/snowflake_pipe.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,144 +4,145 @@
 
 from __future__ import annotations
 
 from typing import ClassVar, List, Optional
 
 from pydantic.v1 import Field, validator
 
-from pyatlan.model.fields.atlan_fields import KeywordField, KeywordTextField
-from pyatlan.model.structs import AzureTag
+from pyatlan.model.fields.atlan_fields import (
+    BooleanField,
+    KeywordField,
+    KeywordTextField,
+    RelationField,
+)
 
-from .object_store import ObjectStore
+from .s_q_l import SQL
 
 
-class ADLS(ObjectStore):
+class SnowflakePipe(SQL):
     """Description"""
 
-    type_name: str = Field(default="ADLS", allow_mutation=False)
+    type_name: str = Field(default="SnowflakePipe", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "ADLS":
-            raise ValueError("must be ADLS")
+        if v != "SnowflakePipe":
+            raise ValueError("must be SnowflakePipe")
         return v
 
     def __setattr__(self, name, value):
-        if name in ADLS._convenience_properties:
+        if name in SnowflakePipe._convenience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    ADLS_ACCOUNT_QUALIFIED_NAME: ClassVar[KeywordTextField] = KeywordTextField(
-        "adlsAccountQualifiedName",
-        "adlsAccountQualifiedName",
-        "adlsAccountQualifiedName.text",
-    )
-    """
-    Unique name of the account for this ADLS asset.
-    """
-    AZURE_RESOURCE_ID: ClassVar[KeywordTextField] = KeywordTextField(
-        "azureResourceId", "azureResourceId", "azureResourceId.text"
-    )
+    DEFINITION: ClassVar[KeywordField] = KeywordField("definition", "definition")
     """
-    Resource identifier of this asset in Azure.
+    SQL definition of this pipe.
     """
-    AZURE_LOCATION: ClassVar[KeywordField] = KeywordField(
-        "azureLocation", "azureLocation"
+    SNOWFLAKE_PIPE_IS_AUTO_INGEST_ENABLED: ClassVar[BooleanField] = BooleanField(
+        "snowflakePipeIsAutoIngestEnabled", "snowflakePipeIsAutoIngestEnabled"
     )
     """
-    Location of this asset in Azure.
+    Whether auto-ingest is enabled for this pipe (true) or not (false).
     """
-    ADLS_ACCOUNT_SECONDARY_LOCATION: ClassVar[KeywordField] = KeywordField(
-        "adlsAccountSecondaryLocation", "adlsAccountSecondaryLocation"
+    SNOWFLAKE_PIPE_NOTIFICATION_CHANNEL_NAME: ClassVar[KeywordTextField] = (
+        KeywordTextField(
+            "snowflakePipeNotificationChannelName",
+            "snowflakePipeNotificationChannelName",
+            "snowflakePipeNotificationChannelName.text",
+        )
     )
     """
-    Secondary location of the ADLS account.
+    Name of the notification channel for this pipe.
     """
-    AZURE_TAGS: ClassVar[KeywordField] = KeywordField("azureTags", "azureTags")
+
+    ATLAN_SCHEMA: ClassVar[RelationField] = RelationField("atlanSchema")
     """
-    Tags that have been applied to this asset in Azure.
+    TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
-        "adls_account_qualified_name",
-        "azure_resource_id",
-        "azure_location",
-        "adls_account_secondary_location",
-        "azure_tags",
+        "definition",
+        "snowflake_pipe_is_auto_ingest_enabled",
+        "snowflake_pipe_notification_channel_name",
+        "atlan_schema",
     ]
 
     @property
-    def adls_account_qualified_name(self) -> Optional[str]:
-        return (
-            None
-            if self.attributes is None
-            else self.attributes.adls_account_qualified_name
-        )
-
-    @adls_account_qualified_name.setter
-    def adls_account_qualified_name(self, adls_account_qualified_name: Optional[str]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.adls_account_qualified_name = adls_account_qualified_name
-
-    @property
-    def azure_resource_id(self) -> Optional[str]:
-        return None if self.attributes is None else self.attributes.azure_resource_id
+    def definition(self) -> Optional[str]:
+        return None if self.attributes is None else self.attributes.definition
 
-    @azure_resource_id.setter
-    def azure_resource_id(self, azure_resource_id: Optional[str]):
+    @definition.setter
+    def definition(self, definition: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.azure_resource_id = azure_resource_id
+        self.attributes.definition = definition
 
     @property
-    def azure_location(self) -> Optional[str]:
-        return None if self.attributes is None else self.attributes.azure_location
+    def snowflake_pipe_is_auto_ingest_enabled(self) -> Optional[bool]:
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.snowflake_pipe_is_auto_ingest_enabled
+        )
 
-    @azure_location.setter
-    def azure_location(self, azure_location: Optional[str]):
+    @snowflake_pipe_is_auto_ingest_enabled.setter
+    def snowflake_pipe_is_auto_ingest_enabled(
+        self, snowflake_pipe_is_auto_ingest_enabled: Optional[bool]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.azure_location = azure_location
+        self.attributes.snowflake_pipe_is_auto_ingest_enabled = (
+            snowflake_pipe_is_auto_ingest_enabled
+        )
 
     @property
-    def adls_account_secondary_location(self) -> Optional[str]:
+    def snowflake_pipe_notification_channel_name(self) -> Optional[str]:
         return (
             None
             if self.attributes is None
-            else self.attributes.adls_account_secondary_location
+            else self.attributes.snowflake_pipe_notification_channel_name
         )
 
-    @adls_account_secondary_location.setter
-    def adls_account_secondary_location(
-        self, adls_account_secondary_location: Optional[str]
+    @snowflake_pipe_notification_channel_name.setter
+    def snowflake_pipe_notification_channel_name(
+        self, snowflake_pipe_notification_channel_name: Optional[str]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.adls_account_secondary_location = (
-            adls_account_secondary_location
+        self.attributes.snowflake_pipe_notification_channel_name = (
+            snowflake_pipe_notification_channel_name
         )
 
     @property
-    def azure_tags(self) -> Optional[List[AzureTag]]:
-        return None if self.attributes is None else self.attributes.azure_tags
+    def atlan_schema(self) -> Optional[Schema]:
+        return None if self.attributes is None else self.attributes.atlan_schema
 
-    @azure_tags.setter
-    def azure_tags(self, azure_tags: Optional[List[AzureTag]]):
+    @atlan_schema.setter
+    def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.azure_tags = azure_tags
+        self.attributes.atlan_schema = atlan_schema
 
-    class Attributes(ObjectStore.Attributes):
-        adls_account_qualified_name: Optional[str] = Field(default=None, description="")
-        azure_resource_id: Optional[str] = Field(default=None, description="")
-        azure_location: Optional[str] = Field(default=None, description="")
-        adls_account_secondary_location: Optional[str] = Field(
+    class Attributes(SQL.Attributes):
+        definition: Optional[str] = Field(default=None, description="")
+        snowflake_pipe_is_auto_ingest_enabled: Optional[bool] = Field(
+            default=None, description=""
+        )
+        snowflake_pipe_notification_channel_name: Optional[str] = Field(
             default=None, description=""
         )
-        azure_tags: Optional[List[AzureTag]] = Field(default=None, description="")
+        atlan_schema: Optional[Schema] = Field(
+            default=None, description=""
+        )  # relationship
 
-    attributes: "ADLS.Attributes" = Field(
-        default_factory=lambda: ADLS.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+    attributes: SnowflakePipe.Attributes = Field(
+        default_factory=lambda: SnowflakePipe.Attributes(),
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
+
+
+from .schema import Schema  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/a_d_l_s_account.py` & `pyatlan-2.1.2/pyatlan/model/assets/a_d_l_s_account.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,15 +350,18 @@
             return ADLSAccount.Attributes(
                 name=name,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connection_qualified_name=connection_qualified_name,
                 connector_name=connector_type.value,
             )
 
-    attributes: "ADLSAccount.Attributes" = Field(
+    attributes: ADLSAccount.Attributes = Field(
         default_factory=lambda: ADLSAccount.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .a_d_l_s_container import ADLSContainer  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/a_d_l_s_container.py` & `pyatlan-2.1.2/pyatlan/model/assets/a_d_l_s_container.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,16 +281,19 @@
                 qualified_name=f"{adls_account_qualified_name}/{name}",
                 connector_name=connector_type.value,
                 adls_account=ADLSAccount.ref_by_qualified_name(
                     adls_account_qualified_name
                 ),
             )
 
-    attributes: "ADLSContainer.Attributes" = Field(
+    attributes: ADLSContainer.Attributes = Field(
         default_factory=lambda: ADLSContainer.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .a_d_l_s_account import ADLSAccount  # noqa
 from .a_d_l_s_object import ADLSObject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/a_d_l_s_object.py` & `pyatlan-2.1.2/pyatlan/model/assets/a_d_l_s_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -543,15 +543,18 @@
                 connector_name=connector_type.value,
                 adls_container=ADLSContainer.ref_by_qualified_name(
                     adls_container_qualified_name
                 ),
                 adls_account_qualified_name=adls_account_qualified_name,
             )
 
-    attributes: "ADLSObject.Attributes" = Field(
+    attributes: ADLSObject.Attributes = Field(
         default_factory=lambda: ADLSObject.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .a_d_l_s_container import ADLSContainer  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/a_p_i.py` & `pyatlan-2.1.2/pyatlan/model/assets/a_p_i.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,12 +145,15 @@
         api_spec_name: Optional[str] = Field(default=None, description="")
         api_spec_qualified_name: Optional[str] = Field(default=None, description="")
         api_external_docs: Optional[Dict[str, str]] = Field(
             default=None, description=""
         )
         api_is_auth_optional: Optional[bool] = Field(default=None, description="")
 
-    attributes: "API.Attributes" = Field(
+    attributes: API.Attributes = Field(
         default_factory=lambda: API.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/a_p_i_path.py` & `pyatlan-2.1.2/pyatlan/model/assets/a_p_i_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,18 @@
                 api_spec_qualified_name=spec_qualified_name,
                 connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
                 qualified_name=f"{spec_qualified_name}{path_raw_uri}",
                 connector_name=connector_type.value,
                 api_spec=APISpec.ref_by_qualified_name(spec_qualified_name),
             )
 
-    attributes: "APIPath.Attributes" = Field(
+    attributes: APIPath.Attributes = Field(
         default_factory=lambda: APIPath.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .a_p_i_spec import APISpec  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/a_p_i_spec.py` & `pyatlan-2.1.2/pyatlan/model/assets/a_p_i_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,18 @@
             return APISpec.Attributes(
                 name=name,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connection_qualified_name=connection_qualified_name,
                 connector_name=connector_type.value,
             )
 
-    attributes: "APISpec.Attributes" = Field(
+    attributes: APISpec.Attributes = Field(
         default_factory=lambda: APISpec.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .a_p_i_path import APIPath  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/a_w_s.py` & `pyatlan-2.1.2/pyatlan/model/assets/a_w_s.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,12 +184,15 @@
         aws_region: Optional[str] = Field(default=None, description="")
         aws_account_id: Optional[str] = Field(default=None, description="")
         aws_resource_id: Optional[str] = Field(default=None, description="")
         aws_owner_name: Optional[str] = Field(default=None, description="")
         aws_owner_id: Optional[str] = Field(default=None, description="")
         aws_tags: Optional[List[AwsTag]] = Field(default=None, description="")
 
-    attributes: "AWS.Attributes" = Field(
+    attributes: AWS.Attributes = Field(
         default_factory=lambda: AWS.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/access_control.py` & `pyatlan-2.1.2/pyatlan/model/assets/access_control.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,18 @@
         deny_navigation_pages: Optional[Set[str]] = Field(default=None, description="")
         default_navigation: Optional[str] = Field(default=None, description="")
         display_preferences: Optional[Set[str]] = Field(default=None, description="")
         policies: Optional[List[AuthPolicy]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "AccessControl.Attributes" = Field(
+    attributes: AccessControl.Attributes = Field(
         default_factory=lambda: AccessControl.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .auth_policy import AuthPolicy  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/airflow.py` & `pyatlan-2.1.2/pyatlan/model/assets/airflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,12 +195,15 @@
         airflow_run_type: Optional[str] = Field(default=None, description="")
         airflow_run_start_time: Optional[datetime] = Field(default=None, description="")
         airflow_run_end_time: Optional[datetime] = Field(default=None, description="")
         airflow_run_open_lineage_state: Optional[OpenLineageRunState] = Field(
             default=None, description=""
         )
 
-    attributes: "Airflow.Attributes" = Field(
+    attributes: Airflow.Attributes = Field(
         default_factory=lambda: Airflow.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/airflow_dag.py` & `pyatlan-2.1.2/pyatlan/model/assets/airflow_dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,18 @@
     class Attributes(Airflow.Attributes):
         airflow_dag_schedule: Optional[str] = Field(default=None, description="")
         airflow_dag_schedule_delta: Optional[int] = Field(default=None, description="")
         airflow_tasks: Optional[List[AirflowTask]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "AirflowDag.Attributes" = Field(
+    attributes: AirflowDag.Attributes = Field(
         default_factory=lambda: AirflowDag.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .airflow_task import AirflowTask  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/airflow_task.py` & `pyatlan-2.1.2/pyatlan/model/assets/airflow_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,17 +337,20 @@
         inputs: Optional[List[Catalog]] = Field(
             default=None, description=""
         )  # relationship
         airflow_dag: Optional[AirflowDag] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "AirflowTask.Attributes" = Field(
+    attributes: AirflowTask.Attributes = Field(
         default_factory=lambda: AirflowTask.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .airflow_dag import AirflowDag  # noqa
 from .catalog import Catalog  # noqa
 from .process import Process  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/asset.py` & `pyatlan-2.1.2/pyatlan/model/assets/asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     KeywordTextStemmedField,
     NumericField,
     NumericRankField,
     RelationField,
     TextField,
 )
 from pyatlan.model.structs import PopularityInsights, StarredDetails
-from pyatlan.utils import init_guid, move_struct, validate_required_fields
+from pyatlan.utils import init_guid, validate_required_fields
 
 from .referenceable import Referenceable
 
 SelfAsset = TypeVar("SelfAsset", bound="Asset")
 
 
 class Asset(Referenceable):
@@ -159,15 +159,14 @@
         sub = cls._subtypes_.get(data_type)
         if sub is None:
             sub = getattr(sys.modules["pyatlan.model.assets"], data_type)
 
         if sub is None:
             raise TypeError(f"Unsupport sub-type: {data_type}")
 
-        move_struct(data)
         return sub(**data)
 
     if TYPE_CHECKING:
         from pyatlan.model.lineage import FluentLineage
 
     @classmethod
     def lineage(cls, guid: str, include_archived: bool = False) -> "FluentLineage":
@@ -557,14 +556,20 @@
     """
     DBT_QUALIFIED_NAME: ClassVar[KeywordTextField] = KeywordTextField(
         "dbtQualifiedName", "dbtQualifiedName", "dbtQualifiedName.text"
     )
     """
     Unique name of this asset in dbt.
     """
+    ASSET_DBT_WORKFLOW_LAST_UPDATED: ClassVar[KeywordField] = KeywordField(
+        "assetDbtWorkflowLastUpdated", "assetDbtWorkflowLastUpdated"
+    )
+    """
+    Name of the DBT workflow in Atlan that last updated the asset.
+    """
     ASSET_DBT_ALIAS: ClassVar[KeywordTextField] = KeywordTextField(
         "assetDbtAlias", "assetDbtAlias.keyword", "assetDbtAlias"
     )
     """
     Alias of this asset in dbt.
     """
     ASSET_DBT_META: ClassVar[KeywordField] = KeywordField(
@@ -1086,14 +1091,15 @@
         "source_read_top_user_record_list",
         "source_read_popular_query_record_list",
         "source_read_expensive_query_record_list",
         "source_read_slow_query_record_list",
         "source_query_compute_cost_list",
         "source_query_compute_cost_record_list",
         "dbt_qualified_name",
+        "asset_dbt_workflow_last_updated",
         "asset_dbt_alias",
         "asset_dbt_meta",
         "asset_dbt_unique_id",
         "asset_dbt_account_name",
         "asset_dbt_project_name",
         "asset_dbt_package_name",
         "asset_dbt_job_name",
@@ -1831,14 +1837,32 @@
     @dbt_qualified_name.setter
     def dbt_qualified_name(self, dbt_qualified_name: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.dbt_qualified_name = dbt_qualified_name
 
     @property
+    def asset_dbt_workflow_last_updated(self) -> Optional[str]:
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.asset_dbt_workflow_last_updated
+        )
+
+    @asset_dbt_workflow_last_updated.setter
+    def asset_dbt_workflow_last_updated(
+        self, asset_dbt_workflow_last_updated: Optional[str]
+    ):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.asset_dbt_workflow_last_updated = (
+            asset_dbt_workflow_last_updated
+        )
+
+    @property
     def asset_dbt_alias(self) -> Optional[str]:
         return None if self.attributes is None else self.attributes.asset_dbt_alias
 
     @asset_dbt_alias.setter
     def asset_dbt_alias(self, asset_dbt_alias: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -3016,14 +3040,17 @@
         source_query_compute_cost_list: Optional[Set[str]] = Field(
             default=None, description=""
         )
         source_query_compute_cost_record_list: Optional[List[PopularityInsights]] = (
             Field(default=None, description="")
         )
         dbt_qualified_name: Optional[str] = Field(default=None, description="")
+        asset_dbt_workflow_last_updated: Optional[str] = Field(
+            default=None, description=""
+        )
         asset_dbt_alias: Optional[str] = Field(default=None, description="")
         asset_dbt_meta: Optional[str] = Field(default=None, description="")
         asset_dbt_unique_id: Optional[str] = Field(default=None, description="")
         asset_dbt_account_name: Optional[str] = Field(default=None, description="")
         asset_dbt_project_name: Optional[str] = Field(default=None, description="")
         asset_dbt_package_name: Optional[str] = Field(default=None, description="")
         asset_dbt_job_name: Optional[str] = Field(default=None, description="")
@@ -3211,18 +3238,21 @@
             self.certificate_status_message = None
 
         def remove_announcement(self):
             self.announcement_message = None
             self.announcement_title = None
             self.announcement_type = None
 
-    attributes: "Asset.Attributes" = Field(
+    attributes: Asset.Attributes = Field(
         default_factory=lambda: Asset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .atlas_glossary_term import AtlasGlossaryTerm  # noqa
 from .data_product import DataProduct  # noqa
 from .file import File  # noqa
 from .link import Link  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/atlas_glossary.py` & `pyatlan-2.1.2/pyatlan/model/assets/atlas_glossary.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,16 +223,19 @@
         ) -> AtlasGlossary.Attributes:
             validate_required_fields(["name"], [name])
             icon_str = icon.value if icon is not None else None
             return AtlasGlossary.Attributes(
                 name=name, qualified_name=next_id(), asset_icon=icon_str
             )
 
-    attributes: "AtlasGlossary.Attributes" = Field(
+    attributes: AtlasGlossary.Attributes = Field(
         default_factory=lambda: AtlasGlossary.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .atlas_glossary_category import AtlasGlossaryCategory  # noqa
 from .atlas_glossary_term import AtlasGlossaryTerm  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/atlas_glossary_category.py` & `pyatlan-2.1.2/pyatlan/model/assets/atlas_glossary_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,16 +302,19 @@
             return AtlasGlossaryCategory.Attributes(
                 name=name,
                 anchor=anchor,
                 parent_category=parent_category,
                 qualified_name=next_id(),
             )
 
-    attributes: "AtlasGlossaryCategory.Attributes" = Field(
+    attributes: AtlasGlossaryCategory.Attributes = Field(
         default_factory=lambda: AtlasGlossaryCategory.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .atlas_glossary import AtlasGlossary  # noqa
 from .atlas_glossary_term import AtlasGlossaryTerm  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/atlas_glossary_term.py` & `pyatlan-2.1.2/pyatlan/model/assets/atlas_glossary_term.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,17 +583,20 @@
             return AtlasGlossaryTerm.Attributes(
                 name=name,
                 anchor=anchor,
                 categories=categories,
                 qualified_name=next_id(),
             )
 
-    attributes: "AtlasGlossaryTerm.Attributes" = Field(
+    attributes: AtlasGlossaryTerm.Attributes = Field(
         default_factory=lambda: AtlasGlossaryTerm.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .atlas_glossary import AtlasGlossary  # noqa
 from .atlas_glossary_category import AtlasGlossaryCategory  # noqa
 from .referenceable import Referenceable  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/auth_policy.py` & `pyatlan-2.1.2/pyatlan/model/assets/auth_policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,18 @@
         @classmethod
         def __create(cls, name: str) -> AuthPolicy.Attributes:
             validate_required_fields(["name"], [name])
             return AuthPolicy.Attributes(
                 qualified_name=name, name=name, display_name=""
             )
 
-    attributes: "AuthPolicy.Attributes" = Field(
+    attributes: AuthPolicy.Attributes = Field(
         default_factory=lambda: AuthPolicy.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .access_control import AccessControl  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/auth_service.py` & `pyatlan-2.1.2/pyatlan/model/assets/auth_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,12 +131,15 @@
         auth_service_config: Optional[Dict[str, str]] = Field(
             default=None, description=""
         )
         auth_service_policy_last_sync: Optional[int] = Field(
             default=None, description=""
         )
 
-    attributes: "AuthService.Attributes" = Field(
+    attributes: AuthService.Attributes = Field(
         default_factory=lambda: AuthService.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/azure.py` & `pyatlan-2.1.2/pyatlan/model/assets/azure.py`

 * *Files 5% similar despite different names*

```diff
@@ -112,12 +112,15 @@
         azure_resource_id: Optional[str] = Field(default=None, description="")
         azure_location: Optional[str] = Field(default=None, description="")
         adls_account_secondary_location: Optional[str] = Field(
             default=None, description=""
         )
         azure_tags: Optional[List[AzureTag]] = Field(default=None, description="")
 
-    attributes: "Azure.Attributes" = Field(
+    attributes: Azure.Attributes = Field(
         default_factory=lambda: Azure.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/azure_event_hub.py` & `pyatlan-2.1.2/pyatlan/model/assets/azure_event_hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,12 +51,15 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.azure_event_hub_status = azure_event_hub_status
 
     class Attributes(KafkaTopic.Attributes):
         azure_event_hub_status: Optional[str] = Field(default=None, description="")
 
-    attributes: "AzureEventHub.Attributes" = Field(
+    attributes: AzureEventHub.Attributes = Field(
         default_factory=lambda: AzureEventHub.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/azure_event_hub_consumer_group.py` & `pyatlan-2.1.2/pyatlan/model/assets/azure_event_hub_consumer_group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/b_i.py` & `pyatlan-2.1.2/pyatlan/model/assets/b_i.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/b_i_process.py` & `pyatlan-2.1.2/pyatlan/model/assets/b_i_process.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,15 +67,18 @@
         outputs: Optional[List[Catalog]] = Field(
             default=None, description=""
         )  # relationship
         inputs: Optional[List[Catalog]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "BIProcess.Attributes" = Field(
+    attributes: BIProcess.Attributes = Field(
         default_factory=lambda: BIProcess.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .catalog import Catalog  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/badge.py` & `pyatlan-2.1.2/pyatlan/model/assets/badge.py`

 * *Files 3% similar despite different names*

```diff
@@ -149,12 +149,15 @@
             return Badge.Attributes(
                 name=name,
                 qualified_name=f"badges/global/{cm_id}.{cm_attr_id}",
                 badge_metadata_attribute=f"{cm_id}.{cm_attr_id}",
                 badge_conditions=badge_conditions,
             )
 
-    attributes: "Badge.Attributes" = Field(
+    attributes: Badge.Attributes = Field(
         default_factory=lambda: Badge.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/calculation_view.py` & `pyatlan-2.1.2/pyatlan/model/assets/calculation_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,16 +159,19 @@
         columns: Optional[List[Column]] = Field(
             default=None, description=""
         )  # relationship
         atlan_schema: Optional[Schema] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "CalculationView.Attributes" = Field(
+    attributes: CalculationView.Attributes = Field(
         default_factory=lambda: CalculationView.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .column import Column  # noqa
 from .schema import Schema  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/catalog.py` & `pyatlan-2.1.2/pyatlan/model/assets/catalog.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,14 +35,24 @@
     """
     OUTPUT_FROM_AIRFLOW_TASKS: ClassVar[RelationField] = RelationField(
         "outputFromAirflowTasks"
     )
     """
     TBC
     """
+    INPUT_TO_SPARK_JOBS: ClassVar[RelationField] = RelationField("inputToSparkJobs")
+    """
+    TBC
+    """
+    OUTPUT_FROM_SPARK_JOBS: ClassVar[RelationField] = RelationField(
+        "outputFromSparkJobs"
+    )
+    """
+    TBC
+    """
     INPUT_TO_AIRFLOW_TASKS: ClassVar[RelationField] = RelationField(
         "inputToAirflowTasks"
     )
     """
     TBC
     """
     OUTPUT_FROM_PROCESSES: ClassVar[RelationField] = RelationField(
@@ -51,14 +61,16 @@
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
         "input_to_processes",
         "output_from_airflow_tasks",
+        "input_to_spark_jobs",
+        "output_from_spark_jobs",
         "input_to_airflow_tasks",
         "output_from_processes",
     ]
 
     @property
     def input_to_processes(self) -> Optional[List[Process]]:
         return None if self.attributes is None else self.attributes.input_to_processes
@@ -82,14 +94,36 @@
         self, output_from_airflow_tasks: Optional[List[AirflowTask]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_from_airflow_tasks = output_from_airflow_tasks
 
     @property
+    def input_to_spark_jobs(self) -> Optional[List[SparkJob]]:
+        return None if self.attributes is None else self.attributes.input_to_spark_jobs
+
+    @input_to_spark_jobs.setter
+    def input_to_spark_jobs(self, input_to_spark_jobs: Optional[List[SparkJob]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.input_to_spark_jobs = input_to_spark_jobs
+
+    @property
+    def output_from_spark_jobs(self) -> Optional[List[SparkJob]]:
+        return (
+            None if self.attributes is None else self.attributes.output_from_spark_jobs
+        )
+
+    @output_from_spark_jobs.setter
+    def output_from_spark_jobs(self, output_from_spark_jobs: Optional[List[SparkJob]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.output_from_spark_jobs = output_from_spark_jobs
+
+    @property
     def input_to_airflow_tasks(self) -> Optional[List[AirflowTask]]:
         return (
             None if self.attributes is None else self.attributes.input_to_airflow_tasks
         )
 
     @input_to_airflow_tasks.setter
     def input_to_airflow_tasks(
@@ -114,23 +148,33 @@
     class Attributes(Asset.Attributes):
         input_to_processes: Optional[List[Process]] = Field(
             default=None, description=""
         )  # relationship
         output_from_airflow_tasks: Optional[List[AirflowTask]] = Field(
             default=None, description=""
         )  # relationship
+        input_to_spark_jobs: Optional[List[SparkJob]] = Field(
+            default=None, description=""
+        )  # relationship
+        output_from_spark_jobs: Optional[List[SparkJob]] = Field(
+            default=None, description=""
+        )  # relationship
         input_to_airflow_tasks: Optional[List[AirflowTask]] = Field(
             default=None, description=""
         )  # relationship
         output_from_processes: Optional[List[Process]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "Catalog.Attributes" = Field(
+    attributes: Catalog.Attributes = Field(
         default_factory=lambda: Catalog.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .airflow_task import AirflowTask  # noqa
 from .process import Process  # noqa
+from .spark_job import SparkJob  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/cloud.py` & `pyatlan-2.1.2/pyatlan/model/assets/cloud.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/collection.py` & `pyatlan-2.1.2/pyatlan/model/assets/collection.py`

 * *Files 9% similar despite different names*

```diff
@@ -64,12 +64,15 @@
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
     class Attributes(Namespace.Attributes):
         icon: Optional[str] = Field(default=None, description="")
         icon_type: Optional[IconType] = Field(default=None, description="")
 
-    attributes: "Collection.Attributes" = Field(
+    attributes: Collection.Attributes = Field(
         default_factory=lambda: Collection.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/column.py` & `pyatlan-2.1.2/pyatlan/model/assets/column.py`

 * *Files 0% similar despite different names*

```diff
@@ -1396,18 +1396,21 @@
                 ret_value.view_name = fields[5]
             else:
                 raise ValueError(
                     "parent_type must be either Table, View or MaterializeView"
                 )
             return ret_value
 
-    attributes: "Column.Attributes" = Field(
+    attributes: Column.Attributes = Field(
         default_factory=lambda: Column.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .calculation_view import CalculationView  # noqa
 from .dbt_metric import DbtMetric  # noqa
 from .dbt_model_column import DbtModelColumn  # noqa
 from .materialised_view import MaterialisedView  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/column_process.py` & `pyatlan-2.1.2/pyatlan/model/assets/column_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,16 +166,19 @@
                 connector_name=connector_name,
                 connection_qualified_name=connection_qualified_name,
                 inputs=inputs,
                 outputs=outputs,
                 process=parent,
             )
 
-    attributes: "ColumnProcess.Attributes" = Field(
+    attributes: ColumnProcess.Attributes = Field(
         default_factory=lambda: ColumnProcess.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .catalog import Catalog  # noqa
 from .process import Process  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/connection.py` & `pyatlan-2.1.2/pyatlan/model/assets/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,12 +683,15 @@
         def admin_groups_valid(cls, admin_groups, values):
             from pyatlan.cache.group_cache import GroupCache
 
             if values.get("is_loaded", False):
                 GroupCache.validate_aliases(aliases=admin_groups)
                 return admin_groups
 
-    attributes: "Connection.Attributes" = Field(
+    attributes: Connection.Attributes = Field(
         default_factory=lambda: Connection.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/data_domain.py` & `pyatlan-2.1.2/pyatlan/model/assets/data_domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,15 +187,18 @@
             return DataDomain.Attributes(
                 name=name,
                 qualified_name=qualified_name,
                 parent_domain=parent_domain,
                 parent_domain_qualified_name=parent_domain_qualified_name,
             )
 
-    attributes: "DataDomain.Attributes" = Field(
+    attributes: DataDomain.Attributes = Field(
         default_factory=lambda: DataDomain.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .data_product import DataProduct  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/data_mesh.py` & `pyatlan-2.1.2/pyatlan/model/assets/data_mesh.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,12 +81,15 @@
 
     class Attributes(Catalog.Attributes):
         parent_domain_qualified_name: Optional[str] = Field(
             default=None, description=""
         )
         super_domain_qualified_name: Optional[str] = Field(default=None, description="")
 
-    attributes: "DataMesh.Attributes" = Field(
+    attributes: DataMesh.Attributes = Field(
         default_factory=lambda: DataMesh.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/data_product.py` & `pyatlan-2.1.2/pyatlan/model/assets/data_product.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,16 +422,19 @@
                 data_product_assets_playbook_filter=ASSETS_PLAYBOOK_FILTER,
                 parent_domain_qualified_name=domain_qualified_name,
                 super_domain_qualified_name=cls.get_super_domain_qualified_name(
                     domain_qualified_name
                 ),
             )
 
-    attributes: "DataProduct.Attributes" = Field(
+    attributes: DataProduct.Attributes = Field(
         default_factory=lambda: DataProduct.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .asset import Asset  # noqa
 from .data_domain import DataDomain  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/data_quality.py` & `pyatlan-2.1.2/pyatlan/model/assets/data_quality.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/data_set.py` & `pyatlan-2.1.2/pyatlan/model/assets/data_set.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/data_studio.py` & `pyatlan-2.1.2/pyatlan/model/assets/data_studio.py`

 * *Files 12% similar despite different names*

```diff
@@ -86,14 +86,24 @@
     """
     OUTPUT_FROM_AIRFLOW_TASKS: ClassVar[RelationField] = RelationField(
         "outputFromAirflowTasks"
     )
     """
     TBC
     """
+    INPUT_TO_SPARK_JOBS: ClassVar[RelationField] = RelationField("inputToSparkJobs")
+    """
+    TBC
+    """
+    OUTPUT_FROM_SPARK_JOBS: ClassVar[RelationField] = RelationField(
+        "outputFromSparkJobs"
+    )
+    """
+    TBC
+    """
     INPUT_TO_AIRFLOW_TASKS: ClassVar[RelationField] = RelationField(
         "inputToAirflowTasks"
     )
     """
     TBC
     """
     OUTPUT_FROM_PROCESSES: ClassVar[RelationField] = RelationField(
@@ -110,14 +120,16 @@
         "google_project_number",
         "google_location",
         "google_location_type",
         "google_labels",
         "google_tags",
         "input_to_processes",
         "output_from_airflow_tasks",
+        "input_to_spark_jobs",
+        "output_from_spark_jobs",
         "input_to_airflow_tasks",
         "output_from_processes",
     ]
 
     @property
     def google_service(self) -> Optional[str]:
         return None if self.attributes is None else self.attributes.google_service
@@ -223,14 +235,36 @@
         self, output_from_airflow_tasks: Optional[List[AirflowTask]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_from_airflow_tasks = output_from_airflow_tasks
 
     @property
+    def input_to_spark_jobs(self) -> Optional[List[SparkJob]]:
+        return None if self.attributes is None else self.attributes.input_to_spark_jobs
+
+    @input_to_spark_jobs.setter
+    def input_to_spark_jobs(self, input_to_spark_jobs: Optional[List[SparkJob]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.input_to_spark_jobs = input_to_spark_jobs
+
+    @property
+    def output_from_spark_jobs(self) -> Optional[List[SparkJob]]:
+        return (
+            None if self.attributes is None else self.attributes.output_from_spark_jobs
+        )
+
+    @output_from_spark_jobs.setter
+    def output_from_spark_jobs(self, output_from_spark_jobs: Optional[List[SparkJob]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.output_from_spark_jobs = output_from_spark_jobs
+
+    @property
     def input_to_airflow_tasks(self) -> Optional[List[AirflowTask]]:
         return (
             None if self.attributes is None else self.attributes.input_to_airflow_tasks
         )
 
     @input_to_airflow_tasks.setter
     def input_to_airflow_tasks(
@@ -263,23 +297,33 @@
         google_tags: Optional[List[GoogleTag]] = Field(default=None, description="")
         input_to_processes: Optional[List[Process]] = Field(
             default=None, description=""
         )  # relationship
         output_from_airflow_tasks: Optional[List[AirflowTask]] = Field(
             default=None, description=""
         )  # relationship
+        input_to_spark_jobs: Optional[List[SparkJob]] = Field(
+            default=None, description=""
+        )  # relationship
+        output_from_spark_jobs: Optional[List[SparkJob]] = Field(
+            default=None, description=""
+        )  # relationship
         input_to_airflow_tasks: Optional[List[AirflowTask]] = Field(
             default=None, description=""
         )  # relationship
         output_from_processes: Optional[List[Process]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "DataStudio.Attributes" = Field(
+    attributes: DataStudio.Attributes = Field(
         default_factory=lambda: DataStudio.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .airflow_task import AirflowTask  # noqa
 from .process import Process  # noqa
+from .spark_job import SparkJob  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/data_studio_asset.py` & `pyatlan-2.1.2/pyatlan/model/assets/data_studio_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -361,12 +361,15 @@
                 name=name,
                 qualified_name=f"{connection_qualified_name}/{gdsid}",
                 connection_qualified_name=connection_qualified_name,
                 connector_name=connector_type.value,
                 data_studio_asset_type=data_studio_asset_type,
             )
 
-    attributes: "DataStudioAsset.Attributes" = Field(
+    attributes: DataStudioAsset.Attributes = Field(
         default_factory=lambda: DataStudioAsset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/database.py` & `pyatlan-2.1.2/pyatlan/model/assets/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,18 @@
             return Database.Attributes(
                 name=name,
                 connection_qualified_name=connection_qualified_name,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connector_name=connector_type.value,
             )
 
-    attributes: "Database.Attributes" = Field(
+    attributes: Database.Attributes = Field(
         default_factory=lambda: Database.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .schema import Schema  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dbt.py` & `pyatlan-2.1.2/pyatlan/model/assets/dbt.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,12 +388,15 @@
         dbt_environment_dbt_version: Optional[str] = Field(default=None, description="")
         dbt_tags: Optional[Set[str]] = Field(default=None, description="")
         dbt_connection_context: Optional[str] = Field(default=None, description="")
         dbt_semantic_layer_proxy_url: Optional[str] = Field(
             default=None, description=""
         )
 
-    attributes: "Dbt.Attributes" = Field(
+    attributes: Dbt.Attributes = Field(
         default_factory=lambda: Dbt.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dbt_column_process.py` & `pyatlan-2.1.2/pyatlan/model/assets/dbt_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,32 +15,32 @@
     NumericField,
     RelationField,
 )
 
 from .dbt import Dbt
 
 
-class DbtColumnProcess(Dbt):
+class DbtProcess(Dbt):
     """Description"""
 
-    type_name: str = Field(default="DbtColumnProcess", allow_mutation=False)
+    type_name: str = Field(default="DbtProcess", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "DbtColumnProcess":
-            raise ValueError("must be DbtColumnProcess")
+        if v != "DbtProcess":
+            raise ValueError("must be DbtProcess")
         return v
 
     def __setattr__(self, name, value):
-        if name in DbtColumnProcess._convenience_properties:
+        if name in DbtProcess._convenience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    DBT_COLUMN_PROCESS_JOB_STATUS: ClassVar[KeywordField] = KeywordField(
-        "dbtColumnProcessJobStatus", "dbtColumnProcessJobStatus"
+    DBT_PROCESS_JOB_STATUS: ClassVar[KeywordField] = KeywordField(
+        "dbtProcessJobStatus", "dbtProcessJobStatus"
     )
     """
 
     """
     DBT_ALIAS: ClassVar[KeywordTextField] = KeywordTextField(
         "dbtAlias", "dbtAlias.keyword", "dbtAlias"
     )
@@ -164,29 +164,29 @@
     Parsed AST of the code or SQL statements that describe the logic of this process.
     """
 
     MATILLION_COMPONENT: ClassVar[RelationField] = RelationField("matillionComponent")
     """
     TBC
     """
-    PROCESS: ClassVar[RelationField] = RelationField("process")
+    AIRFLOW_TASKS: ClassVar[RelationField] = RelationField("airflowTasks")
     """
     TBC
     """
-    AIRFLOW_TASKS: ClassVar[RelationField] = RelationField("airflowTasks")
+    COLUMN_PROCESSES: ClassVar[RelationField] = RelationField("columnProcesses")
     """
     TBC
     """
-    COLUMN_PROCESSES: ClassVar[RelationField] = RelationField("columnProcesses")
+    SPARK_JOBS: ClassVar[RelationField] = RelationField("sparkJobs")
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
-        "dbt_column_process_job_status",
+        "dbt_process_job_status",
         "dbt_alias",
         "dbt_meta",
         "dbt_unique_id",
         "dbt_account_name",
         "dbt_project_name",
         "dbt_package_name",
         "dbt_job_name",
@@ -203,34 +203,30 @@
         "dbt_semantic_layer_proxy_url",
         "inputs",
         "outputs",
         "code",
         "sql",
         "ast",
         "matillion_component",
-        "process",
         "airflow_tasks",
         "column_processes",
+        "spark_jobs",
     ]
 
     @property
-    def dbt_column_process_job_status(self) -> Optional[str]:
+    def dbt_process_job_status(self) -> Optional[str]:
         return (
-            None
-            if self.attributes is None
-            else self.attributes.dbt_column_process_job_status
+            None if self.attributes is None else self.attributes.dbt_process_job_status
         )
 
-    @dbt_column_process_job_status.setter
-    def dbt_column_process_job_status(
-        self, dbt_column_process_job_status: Optional[str]
-    ):
+    @dbt_process_job_status.setter
+    def dbt_process_job_status(self, dbt_process_job_status: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.dbt_column_process_job_status = dbt_column_process_job_status
+        self.attributes.dbt_process_job_status = dbt_process_job_status
 
     @property
     def dbt_alias(self) -> Optional[str]:
         return None if self.attributes is None else self.attributes.dbt_alias
 
     @dbt_alias.setter
     def dbt_alias(self, dbt_alias: Optional[str]):
@@ -487,24 +483,14 @@
     @matillion_component.setter
     def matillion_component(self, matillion_component: Optional[MatillionComponent]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.matillion_component = matillion_component
 
     @property
-    def process(self) -> Optional[Process]:
-        return None if self.attributes is None else self.attributes.process
-
-    @process.setter
-    def process(self, process: Optional[Process]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.process = process
-
-    @property
     def airflow_tasks(self) -> Optional[List[AirflowTask]]:
         return None if self.attributes is None else self.attributes.airflow_tasks
 
     @airflow_tasks.setter
     def airflow_tasks(self, airflow_tasks: Optional[List[AirflowTask]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -516,18 +502,26 @@
 
     @column_processes.setter
     def column_processes(self, column_processes: Optional[List[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_processes = column_processes
 
+    @property
+    def spark_jobs(self) -> Optional[List[SparkJob]]:
+        return None if self.attributes is None else self.attributes.spark_jobs
+
+    @spark_jobs.setter
+    def spark_jobs(self, spark_jobs: Optional[List[SparkJob]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.spark_jobs = spark_jobs
+
     class Attributes(Dbt.Attributes):
-        dbt_column_process_job_status: Optional[str] = Field(
-            default=None, description=""
-        )
+        dbt_process_job_status: Optional[str] = Field(default=None, description="")
         dbt_alias: Optional[str] = Field(default=None, description="")
         dbt_meta: Optional[str] = Field(default=None, description="")
         dbt_unique_id: Optional[str] = Field(default=None, description="")
         dbt_account_name: Optional[str] = Field(default=None, description="")
         dbt_project_name: Optional[str] = Field(default=None, description="")
         dbt_package_name: Optional[str] = Field(default=None, description="")
         dbt_job_name: Optional[str] = Field(default=None, description="")
@@ -550,27 +544,32 @@
         outputs: Optional[List[Catalog]] = Field(default=None, description="")
         code: Optional[str] = Field(default=None, description="")
         sql: Optional[str] = Field(default=None, description="")
         ast: Optional[str] = Field(default=None, description="")
         matillion_component: Optional[MatillionComponent] = Field(
             default=None, description=""
         )  # relationship
-        process: Optional[Process] = Field(default=None, description="")  # relationship
         airflow_tasks: Optional[List[AirflowTask]] = Field(
             default=None, description=""
         )  # relationship
         column_processes: Optional[List[ColumnProcess]] = Field(
             default=None, description=""
         )  # relationship
+        spark_jobs: Optional[List[SparkJob]] = Field(
+            default=None, description=""
+        )  # relationship
 
-    attributes: "DbtColumnProcess.Attributes" = Field(
-        default_factory=lambda: DbtColumnProcess.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+    attributes: DbtProcess.Attributes = Field(
+        default_factory=lambda: DbtProcess.Attributes(),
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .airflow_task import AirflowTask  # noqa
 from .catalog import Catalog  # noqa
 from .column_process import ColumnProcess  # noqa
 from .matillion_component import MatillionComponent  # noqa
-from .process import Process  # noqa
+from .spark_job import SparkJob  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dbt_metric.py` & `pyatlan-2.1.2/pyatlan/model/assets/dbt_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -588,17 +588,20 @@
         metric_dimension_columns: Optional[List[Column]] = Field(
             default=None, description=""
         )  # relationship
         dbt_metric_filter_columns: Optional[List[Column]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "DbtMetric.Attributes" = Field(
+    attributes: DbtMetric.Attributes = Field(
         default_factory=lambda: DbtMetric.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .asset import Asset  # noqa
 from .column import Column  # noqa
 from .dbt_model import DbtModel  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dbt_model.py` & `pyatlan-2.1.2/pyatlan/model/assets/dbt_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,18 +401,21 @@
             default=None, description=""
         )  # relationship
         dbt_model_columns: Optional[List[DbtModelColumn]] = Field(
             default=None, description=""
         )  # relationship
         sql_asset: Optional[SQL] = Field(default=None, description="")  # relationship
 
-    attributes: "DbtModel.Attributes" = Field(
+    attributes: DbtModel.Attributes = Field(
         default_factory=lambda: DbtModel.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .dbt_metric import DbtMetric  # noqa
 from .dbt_model_column import DbtModelColumn  # noqa
 from .dbt_test import DbtTest  # noqa
 from .s_q_l import SQL  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dbt_model_column.py` & `pyatlan-2.1.2/pyatlan/model/assets/dbt_model_column.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,17 +181,20 @@
         dbt_model_column_sql_columns: Optional[List[Column]] = Field(
             default=None, description=""
         )  # relationship
         dbt_tests: Optional[List[DbtTest]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "DbtModelColumn.Attributes" = Field(
+    attributes: DbtModelColumn.Attributes = Field(
         default_factory=lambda: DbtModelColumn.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .column import Column  # noqa
 from .dbt_model import DbtModel  # noqa
 from .dbt_test import DbtTest  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dbt_process.py` & `pyatlan-2.1.2/pyatlan/model/assets/dbt_column_process.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,32 +15,32 @@
     NumericField,
     RelationField,
 )
 
 from .dbt import Dbt
 
 
-class DbtProcess(Dbt):
+class DbtColumnProcess(Dbt):
     """Description"""
 
-    type_name: str = Field(default="DbtProcess", allow_mutation=False)
+    type_name: str = Field(default="DbtColumnProcess", allow_mutation=False)
 
     @validator("type_name")
     def validate_type_name(cls, v):
-        if v != "DbtProcess":
-            raise ValueError("must be DbtProcess")
+        if v != "DbtColumnProcess":
+            raise ValueError("must be DbtColumnProcess")
         return v
 
     def __setattr__(self, name, value):
-        if name in DbtProcess._convenience_properties:
+        if name in DbtColumnProcess._convenience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    DBT_PROCESS_JOB_STATUS: ClassVar[KeywordField] = KeywordField(
-        "dbtProcessJobStatus", "dbtProcessJobStatus"
+    DBT_COLUMN_PROCESS_JOB_STATUS: ClassVar[KeywordField] = KeywordField(
+        "dbtColumnProcessJobStatus", "dbtColumnProcessJobStatus"
     )
     """
 
     """
     DBT_ALIAS: ClassVar[KeywordTextField] = KeywordTextField(
         "dbtAlias", "dbtAlias.keyword", "dbtAlias"
     )
@@ -164,25 +164,33 @@
     Parsed AST of the code or SQL statements that describe the logic of this process.
     """
 
     MATILLION_COMPONENT: ClassVar[RelationField] = RelationField("matillionComponent")
     """
     TBC
     """
+    PROCESS: ClassVar[RelationField] = RelationField("process")
+    """
+    TBC
+    """
     AIRFLOW_TASKS: ClassVar[RelationField] = RelationField("airflowTasks")
     """
     TBC
     """
     COLUMN_PROCESSES: ClassVar[RelationField] = RelationField("columnProcesses")
     """
     TBC
     """
+    SPARK_JOBS: ClassVar[RelationField] = RelationField("sparkJobs")
+    """
+    TBC
+    """
 
     _convenience_properties: ClassVar[List[str]] = [
-        "dbt_process_job_status",
+        "dbt_column_process_job_status",
         "dbt_alias",
         "dbt_meta",
         "dbt_unique_id",
         "dbt_account_name",
         "dbt_project_name",
         "dbt_package_name",
         "dbt_job_name",
@@ -199,29 +207,35 @@
         "dbt_semantic_layer_proxy_url",
         "inputs",
         "outputs",
         "code",
         "sql",
         "ast",
         "matillion_component",
+        "process",
         "airflow_tasks",
         "column_processes",
+        "spark_jobs",
     ]
 
     @property
-    def dbt_process_job_status(self) -> Optional[str]:
+    def dbt_column_process_job_status(self) -> Optional[str]:
         return (
-            None if self.attributes is None else self.attributes.dbt_process_job_status
+            None
+            if self.attributes is None
+            else self.attributes.dbt_column_process_job_status
         )
 
-    @dbt_process_job_status.setter
-    def dbt_process_job_status(self, dbt_process_job_status: Optional[str]):
+    @dbt_column_process_job_status.setter
+    def dbt_column_process_job_status(
+        self, dbt_column_process_job_status: Optional[str]
+    ):
         if self.attributes is None:
             self.attributes = self.Attributes()
-        self.attributes.dbt_process_job_status = dbt_process_job_status
+        self.attributes.dbt_column_process_job_status = dbt_column_process_job_status
 
     @property
     def dbt_alias(self) -> Optional[str]:
         return None if self.attributes is None else self.attributes.dbt_alias
 
     @dbt_alias.setter
     def dbt_alias(self, dbt_alias: Optional[str]):
@@ -478,14 +492,24 @@
     @matillion_component.setter
     def matillion_component(self, matillion_component: Optional[MatillionComponent]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.matillion_component = matillion_component
 
     @property
+    def process(self) -> Optional[Process]:
+        return None if self.attributes is None else self.attributes.process
+
+    @process.setter
+    def process(self, process: Optional[Process]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.process = process
+
+    @property
     def airflow_tasks(self) -> Optional[List[AirflowTask]]:
         return None if self.attributes is None else self.attributes.airflow_tasks
 
     @airflow_tasks.setter
     def airflow_tasks(self, airflow_tasks: Optional[List[AirflowTask]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -497,16 +521,28 @@
 
     @column_processes.setter
     def column_processes(self, column_processes: Optional[List[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_processes = column_processes
 
+    @property
+    def spark_jobs(self) -> Optional[List[SparkJob]]:
+        return None if self.attributes is None else self.attributes.spark_jobs
+
+    @spark_jobs.setter
+    def spark_jobs(self, spark_jobs: Optional[List[SparkJob]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.spark_jobs = spark_jobs
+
     class Attributes(Dbt.Attributes):
-        dbt_process_job_status: Optional[str] = Field(default=None, description="")
+        dbt_column_process_job_status: Optional[str] = Field(
+            default=None, description=""
+        )
         dbt_alias: Optional[str] = Field(default=None, description="")
         dbt_meta: Optional[str] = Field(default=None, description="")
         dbt_unique_id: Optional[str] = Field(default=None, description="")
         dbt_account_name: Optional[str] = Field(default=None, description="")
         dbt_project_name: Optional[str] = Field(default=None, description="")
         dbt_package_name: Optional[str] = Field(default=None, description="")
         dbt_job_name: Optional[str] = Field(default=None, description="")
@@ -529,25 +565,34 @@
         outputs: Optional[List[Catalog]] = Field(default=None, description="")
         code: Optional[str] = Field(default=None, description="")
         sql: Optional[str] = Field(default=None, description="")
         ast: Optional[str] = Field(default=None, description="")
         matillion_component: Optional[MatillionComponent] = Field(
             default=None, description=""
         )  # relationship
+        process: Optional[Process] = Field(default=None, description="")  # relationship
         airflow_tasks: Optional[List[AirflowTask]] = Field(
             default=None, description=""
         )  # relationship
         column_processes: Optional[List[ColumnProcess]] = Field(
             default=None, description=""
         )  # relationship
+        spark_jobs: Optional[List[SparkJob]] = Field(
+            default=None, description=""
+        )  # relationship
 
-    attributes: "DbtProcess.Attributes" = Field(
-        default_factory=lambda: DbtProcess.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+    attributes: DbtColumnProcess.Attributes = Field(
+        default_factory=lambda: DbtColumnProcess.Attributes(),
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .airflow_task import AirflowTask  # noqa
 from .catalog import Catalog  # noqa
 from .column_process import ColumnProcess  # noqa
 from .matillion_component import MatillionComponent  # noqa
+from .process import Process  # noqa
+from .spark_job import SparkJob  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dbt_source.py` & `pyatlan-2.1.2/pyatlan/model/assets/dbt_source.py`

 * *Files 6% similar despite different names*

```diff
@@ -120,16 +120,19 @@
             default=None, description=""
         )  # relationship
         dbt_tests: Optional[List[DbtTest]] = Field(
             default=None, description=""
         )  # relationship
         sql_asset: Optional[SQL] = Field(default=None, description="")  # relationship
 
-    attributes: "DbtSource.Attributes" = Field(
+    attributes: DbtSource.Attributes = Field(
         default_factory=lambda: DbtSource.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .dbt_test import DbtTest  # noqa
 from .s_q_l import SQL  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dbt_tag.py` & `pyatlan-2.1.2/pyatlan/model/assets/dbt_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -463,12 +463,15 @@
         tag_id: Optional[str] = Field(default=None, description="")
         tag_attributes: Optional[List[SourceTagAttribute]] = Field(
             default=None, description=""
         )
         tag_allowed_values: Optional[Set[str]] = Field(default=None, description="")
         mapped_atlan_tag_name: Optional[str] = Field(default=None, description="")
 
-    attributes: "DbtTag.Attributes" = Field(
+    attributes: DbtTag.Attributes = Field(
         default_factory=lambda: DbtTag.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dbt_test.py` & `pyatlan-2.1.2/pyatlan/model/assets/dbt_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,18 +256,21 @@
         dbt_models: Optional[List[DbtModel]] = Field(
             default=None, description=""
         )  # relationship
         dbt_model_columns: Optional[List[DbtModelColumn]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "DbtTest.Attributes" = Field(
+    attributes: DbtTest.Attributes = Field(
         default_factory=lambda: DbtTest.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .dbt_model import DbtModel  # noqa
 from .dbt_model_column import DbtModelColumn  # noqa
 from .dbt_source import DbtSource  # noqa
 from .s_q_l import SQL  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/domo.py` & `pyatlan-2.1.2/pyatlan/model/assets/domo.py`

 * *Files 15% similar despite different names*

```diff
@@ -63,12 +63,15 @@
             self.attributes = self.Attributes()
         self.attributes.domo_owner_id = domo_owner_id
 
     class Attributes(BI.Attributes):
         domo_id: Optional[str] = Field(default=None, description="")
         domo_owner_id: Optional[str] = Field(default=None, description="")
 
-    attributes: "Domo.Attributes" = Field(
+    attributes: Domo.Attributes = Field(
         default_factory=lambda: Domo.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/domo_card.py` & `pyatlan-2.1.2/pyatlan/model/assets/domo_card.py`

 * *Files 19% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 
     DOMO_CARD_TYPE: ClassVar[KeywordField] = KeywordField(
         "domoCardType", "domoCardType"
     )
     """
     Type of the Domo Card.
     """
+    DOMO_CARD_TYPE_VALUE: ClassVar[KeywordField] = KeywordField(
+        "domoCardTypeValue", "domoCardTypeValue"
+    )
+    """
+    Type of the Domo Card.
+    """
     DOMO_CARD_DASHBOARD_COUNT: ClassVar[NumericField] = NumericField(
         "domoCardDashboardCount", "domoCardDashboardCount"
     )
     """
     Number of dashboards linked to this card.
     """
 
@@ -50,14 +56,15 @@
     DOMO_DATASET: ClassVar[RelationField] = RelationField("domoDataset")
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
         "domo_card_type",
+        "domo_card_type_value",
         "domo_card_dashboard_count",
         "domo_dashboards",
         "domo_dataset",
     ]
 
     @property
     def domo_card_type(self) -> Optional[DomoCardType]:
@@ -66,14 +73,24 @@
     @domo_card_type.setter
     def domo_card_type(self, domo_card_type: Optional[DomoCardType]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.domo_card_type = domo_card_type
 
     @property
+    def domo_card_type_value(self) -> Optional[str]:
+        return None if self.attributes is None else self.attributes.domo_card_type_value
+
+    @domo_card_type_value.setter
+    def domo_card_type_value(self, domo_card_type_value: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.domo_card_type_value = domo_card_type_value
+
+    @property
     def domo_card_dashboard_count(self) -> Optional[int]:
         return (
             None
             if self.attributes is None
             else self.attributes.domo_card_dashboard_count
         )
 
@@ -101,24 +118,28 @@
     def domo_dataset(self, domo_dataset: Optional[DomoDataset]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.domo_dataset = domo_dataset
 
     class Attributes(Domo.Attributes):
         domo_card_type: Optional[DomoCardType] = Field(default=None, description="")
+        domo_card_type_value: Optional[str] = Field(default=None, description="")
         domo_card_dashboard_count: Optional[int] = Field(default=None, description="")
         domo_dashboards: Optional[List[DomoDashboard]] = Field(
             default=None, description=""
         )  # relationship
         domo_dataset: Optional[DomoDataset] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "DomoCard.Attributes" = Field(
+    attributes: DomoCard.Attributes = Field(
         default_factory=lambda: DomoCard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .domo_dashboard import DomoDashboard  # noqa
 from .domo_dataset import DomoDataset  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/domo_dashboard.py` & `pyatlan-2.1.2/pyatlan/model/assets/domo_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,15 +118,18 @@
         domo_dashboard_children: Optional[List[DomoDashboard]] = Field(
             default=None, description=""
         )  # relationship
         domo_cards: Optional[List[DomoCard]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "DomoDashboard.Attributes" = Field(
+    attributes: DomoDashboard.Attributes = Field(
         default_factory=lambda: DomoDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .domo_card import DomoCard  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/domo_dataset.py` & `pyatlan-2.1.2/pyatlan/model/assets/domo_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,16 +152,19 @@
         domo_dataset_columns: Optional[List[DomoDatasetColumn]] = Field(
             default=None, description=""
         )  # relationship
         domo_cards: Optional[List[DomoCard]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "DomoDataset.Attributes" = Field(
+    attributes: DomoDataset.Attributes = Field(
         default_factory=lambda: DomoDataset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .domo_card import DomoCard  # noqa
 from .domo_dataset_column import DomoDatasetColumn  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/domo_dataset_column.py` & `pyatlan-2.1.2/pyatlan/model/assets/domo_dataset_column.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,15 +94,18 @@
     class Attributes(Domo.Attributes):
         domo_dataset_column_type: Optional[str] = Field(default=None, description="")
         domo_dataset_qualified_name: Optional[str] = Field(default=None, description="")
         domo_dataset: Optional[DomoDataset] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "DomoDatasetColumn.Attributes" = Field(
+    attributes: DomoDatasetColumn.Attributes = Field(
         default_factory=lambda: DomoDatasetColumn.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .domo_dataset import DomoDataset  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dynamo_d_b.py` & `pyatlan-2.1.2/pyatlan/model/assets/dynamo_d_b.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,12 +146,15 @@
         dynamo_d_b_read_capacity_units: Optional[int] = Field(
             default=None, description=""
         )
         dynamo_d_b_write_capacity_units: Optional[int] = Field(
             default=None, description=""
         )
 
-    attributes: "DynamoDB.Attributes" = Field(
+    attributes: DynamoDB.Attributes = Field(
         default_factory=lambda: DynamoDB.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py` & `pyatlan-2.1.2/pyatlan/model/assets/dynamo_d_b_global_secondary_index.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,15 +49,18 @@
         self.attributes.dynamo_dbtable = dynamo_dbtable
 
     class Attributes(DynamoDBSecondaryIndex.Attributes):
         dynamo_dbtable: Optional[DynamoDBTable] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "DynamoDBGlobalSecondaryIndex.Attributes" = Field(
+    attributes: DynamoDBGlobalSecondaryIndex.Attributes = Field(
         default_factory=lambda: DynamoDBGlobalSecondaryIndex.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .dynamo_dbtable import DynamoDBTable  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py` & `pyatlan-2.1.2/pyatlan/model/assets/dynamo_d_b_local_secondary_index.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,18 @@
         self.attributes.dynamo_dbtable = dynamo_dbtable
 
     class Attributes(DynamoDBSecondaryIndex.Attributes):
         dynamo_dbtable: Optional[DynamoDBTable] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "DynamoDBLocalSecondaryIndex.Attributes" = Field(
+    attributes: DynamoDBLocalSecondaryIndex.Attributes = Field(
         default_factory=lambda: DynamoDBLocalSecondaryIndex.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .dynamo_dbtable import DynamoDBTable  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dynamo_d_b_secondary_index.py` & `pyatlan-2.1.2/pyatlan/model/assets/dynamo_d_b_secondary_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,14 +113,18 @@
     """
     PARTITION_LIST: ClassVar[KeywordField] = KeywordField(
         "partitionList", "partitionList"
     )
     """
     List of partitions in this table.
     """
+    IS_SHARDED: ClassVar[BooleanField] = BooleanField("isSharded", "isSharded")
+    """
+    Whether this table is a sharded table (true) or not (false).
+    """
     QUERY_COUNT: ClassVar[NumericField] = NumericField("queryCount", "queryCount")
     """
     Number of times this asset has been queried.
     """
     QUERY_USER_COUNT: ClassVar[NumericField] = NumericField(
         "queryUserCount", "queryUserCount"
     )
@@ -258,14 +262,15 @@
         "external_location",
         "external_location_region",
         "external_location_format",
         "is_partitioned",
         "partition_strategy",
         "partition_count",
         "partition_list",
+        "is_sharded",
         "query_count",
         "query_user_count",
         "query_user_map",
         "query_count_updated_at",
         "database_name",
         "database_qualified_name",
         "schema_name",
@@ -454,14 +459,24 @@
     @partition_list.setter
     def partition_list(self, partition_list: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_list = partition_list
 
     @property
+    def is_sharded(self) -> Optional[bool]:
+        return None if self.attributes is None else self.attributes.is_sharded
+
+    @is_sharded.setter
+    def is_sharded(self, is_sharded: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.is_sharded = is_sharded
+
+    @property
     def query_count(self) -> Optional[int]:
         return None if self.attributes is None else self.attributes.query_count
 
     @query_count.setter
     def query_count(self, query_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -731,14 +746,15 @@
         external_location: Optional[str] = Field(default=None, description="")
         external_location_region: Optional[str] = Field(default=None, description="")
         external_location_format: Optional[str] = Field(default=None, description="")
         is_partitioned: Optional[bool] = Field(default=None, description="")
         partition_strategy: Optional[str] = Field(default=None, description="")
         partition_count: Optional[int] = Field(default=None, description="")
         partition_list: Optional[str] = Field(default=None, description="")
+        is_sharded: Optional[bool] = Field(default=None, description="")
         query_count: Optional[int] = Field(default=None, description="")
         query_user_count: Optional[int] = Field(default=None, description="")
         query_user_map: Optional[Dict[str, int]] = Field(default=None, description="")
         query_count_updated_at: Optional[datetime] = Field(default=None, description="")
         database_name: Optional[str] = Field(default=None, description="")
         database_qualified_name: Optional[str] = Field(default=None, description="")
         schema_name: Optional[str] = Field(default=None, description="")
@@ -762,12 +778,15 @@
             default=None, description=""
         )
         dynamo_d_b_write_capacity_units: Optional[int] = Field(
             default=None, description=""
         )
         no_s_q_l_schema_definition: Optional[str] = Field(default=None, description="")
 
-    attributes: "DynamoDBSecondaryIndex.Attributes" = Field(
+    attributes: DynamoDBSecondaryIndex.Attributes = Field(
         default_factory=lambda: DynamoDBSecondaryIndex.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/dynamo_dbtable.py` & `pyatlan-2.1.2/pyatlan/model/assets/dynamo_dbtable.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,14 +120,18 @@
     """
     PARTITION_LIST: ClassVar[KeywordField] = KeywordField(
         "partitionList", "partitionList"
     )
     """
     List of partitions in this table.
     """
+    IS_SHARDED: ClassVar[BooleanField] = BooleanField("isSharded", "isSharded")
+    """
+    Whether this table is a sharded table (true) or not (false).
+    """
     QUERY_COUNT: ClassVar[NumericField] = NumericField("queryCount", "queryCount")
     """
     Number of times this asset has been queried.
     """
     QUERY_USER_COUNT: ClassVar[NumericField] = NumericField(
         "queryUserCount", "queryUserCount"
     )
@@ -279,14 +283,15 @@
         "external_location",
         "external_location_region",
         "external_location_format",
         "is_partitioned",
         "partition_strategy",
         "partition_count",
         "partition_list",
+        "is_sharded",
         "query_count",
         "query_user_count",
         "query_user_map",
         "query_count_updated_at",
         "database_name",
         "database_qualified_name",
         "schema_name",
@@ -482,14 +487,24 @@
     @partition_list.setter
     def partition_list(self, partition_list: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_list = partition_list
 
     @property
+    def is_sharded(self) -> Optional[bool]:
+        return None if self.attributes is None else self.attributes.is_sharded
+
+    @is_sharded.setter
+    def is_sharded(self, is_sharded: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.is_sharded = is_sharded
+
+    @property
     def query_count(self) -> Optional[int]:
         return None if self.attributes is None else self.attributes.query_count
 
     @query_count.setter
     def query_count(self, query_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -802,14 +817,15 @@
         external_location: Optional[str] = Field(default=None, description="")
         external_location_region: Optional[str] = Field(default=None, description="")
         external_location_format: Optional[str] = Field(default=None, description="")
         is_partitioned: Optional[bool] = Field(default=None, description="")
         partition_strategy: Optional[str] = Field(default=None, description="")
         partition_count: Optional[int] = Field(default=None, description="")
         partition_list: Optional[str] = Field(default=None, description="")
+        is_sharded: Optional[bool] = Field(default=None, description="")
         query_count: Optional[int] = Field(default=None, description="")
         query_user_count: Optional[int] = Field(default=None, description="")
         query_user_map: Optional[Dict[str, int]] = Field(default=None, description="")
         query_count_updated_at: Optional[datetime] = Field(default=None, description="")
         database_name: Optional[str] = Field(default=None, description="")
         database_qualified_name: Optional[str] = Field(default=None, description="")
         schema_name: Optional[str] = Field(default=None, description="")
@@ -843,16 +859,19 @@
         )  # relationship
         dynamo_d_b_global_secondary_indexes: Optional[
             List[DynamoDBGlobalSecondaryIndex]
         ] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "DynamoDBTable.Attributes" = Field(
+    attributes: DynamoDBTable.Attributes = Field(
         default_factory=lambda: DynamoDBTable.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .dynamo_d_b_global_secondary_index import DynamoDBGlobalSecondaryIndex  # noqa
 from .dynamo_d_b_local_secondary_index import DynamoDBLocalSecondaryIndex  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/event_store.py` & `pyatlan-2.1.2/pyatlan/model/assets/event_store.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/file.py` & `pyatlan-2.1.2/pyatlan/model/assets/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -133,15 +133,18 @@
             return File.Attributes(
                 name=name,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connection_qualified_name=connection_qualified_name,
                 file_type=file_type,
             )
 
-    attributes: "File.Attributes" = Field(
+    attributes: File.Attributes = Field(
         default_factory=lambda: File.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .asset import Asset  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/folder.py` & `pyatlan-2.1.2/pyatlan/model/assets/folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,18 @@
     class Attributes(Namespace.Attributes):
         parent_qualified_name: Optional[str] = Field(default=None, description="")
         collection_qualified_name: Optional[str] = Field(default=None, description="")
         parent: Optional[Namespace] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "Folder.Attributes" = Field(
+    attributes: Folder.Attributes = Field(
         default_factory=lambda: Folder.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .namespace import Namespace  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/function.py` & `pyatlan-2.1.2/pyatlan/model/assets/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,18 @@
         function_is_external: Optional[bool] = Field(default=None, description="")
         function_is_secure: Optional[bool] = Field(default=None, description="")
         function_is_memoizable: Optional[bool] = Field(default=None, description="")
         function_schema: Optional[Schema] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "Function.Attributes" = Field(
+    attributes: Function.Attributes = Field(
         default_factory=lambda: Function.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .schema import Schema  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/g_c_s.py` & `pyatlan-2.1.2/pyatlan/model/assets/g_c_s.py`

 * *Files 12% similar despite different names*

```diff
@@ -121,14 +121,24 @@
     """
     OUTPUT_FROM_AIRFLOW_TASKS: ClassVar[RelationField] = RelationField(
         "outputFromAirflowTasks"
     )
     """
     TBC
     """
+    INPUT_TO_SPARK_JOBS: ClassVar[RelationField] = RelationField("inputToSparkJobs")
+    """
+    TBC
+    """
+    OUTPUT_FROM_SPARK_JOBS: ClassVar[RelationField] = RelationField(
+        "outputFromSparkJobs"
+    )
+    """
+    TBC
+    """
     INPUT_TO_AIRFLOW_TASKS: ClassVar[RelationField] = RelationField(
         "inputToAirflowTasks"
     )
     """
     TBC
     """
     OUTPUT_FROM_PROCESSES: ClassVar[RelationField] = RelationField(
@@ -151,14 +161,16 @@
         "google_project_number",
         "google_location",
         "google_location_type",
         "google_labels",
         "google_tags",
         "input_to_processes",
         "output_from_airflow_tasks",
+        "input_to_spark_jobs",
+        "output_from_spark_jobs",
         "input_to_airflow_tasks",
         "output_from_processes",
     ]
 
     @property
     def gcs_storage_class(self) -> Optional[str]:
         return None if self.attributes is None else self.attributes.gcs_storage_class
@@ -326,14 +338,36 @@
         self, output_from_airflow_tasks: Optional[List[AirflowTask]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.output_from_airflow_tasks = output_from_airflow_tasks
 
     @property
+    def input_to_spark_jobs(self) -> Optional[List[SparkJob]]:
+        return None if self.attributes is None else self.attributes.input_to_spark_jobs
+
+    @input_to_spark_jobs.setter
+    def input_to_spark_jobs(self, input_to_spark_jobs: Optional[List[SparkJob]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.input_to_spark_jobs = input_to_spark_jobs
+
+    @property
+    def output_from_spark_jobs(self) -> Optional[List[SparkJob]]:
+        return (
+            None if self.attributes is None else self.attributes.output_from_spark_jobs
+        )
+
+    @output_from_spark_jobs.setter
+    def output_from_spark_jobs(self, output_from_spark_jobs: Optional[List[SparkJob]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.output_from_spark_jobs = output_from_spark_jobs
+
+    @property
     def input_to_airflow_tasks(self) -> Optional[List[AirflowTask]]:
         return (
             None if self.attributes is None else self.attributes.input_to_airflow_tasks
         )
 
     @input_to_airflow_tasks.setter
     def input_to_airflow_tasks(
@@ -372,23 +406,33 @@
         google_tags: Optional[List[GoogleTag]] = Field(default=None, description="")
         input_to_processes: Optional[List[Process]] = Field(
             default=None, description=""
         )  # relationship
         output_from_airflow_tasks: Optional[List[AirflowTask]] = Field(
             default=None, description=""
         )  # relationship
+        input_to_spark_jobs: Optional[List[SparkJob]] = Field(
+            default=None, description=""
+        )  # relationship
+        output_from_spark_jobs: Optional[List[SparkJob]] = Field(
+            default=None, description=""
+        )  # relationship
         input_to_airflow_tasks: Optional[List[AirflowTask]] = Field(
             default=None, description=""
         )  # relationship
         output_from_processes: Optional[List[Process]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "GCS.Attributes" = Field(
+    attributes: GCS.Attributes = Field(
         default_factory=lambda: GCS.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .airflow_task import AirflowTask  # noqa
 from .process import Process  # noqa
+from .spark_job import SparkJob  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/g_c_s_bucket.py` & `pyatlan-2.1.2/pyatlan/model/assets/g_c_s_bucket.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,15 +273,18 @@
             return GCSBucket.Attributes(
                 name=name,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connection_qualified_name=connection_qualified_name,
                 connector_name=connector_type.value,
             )
 
-    attributes: "GCSBucket.Attributes" = Field(
+    attributes: GCSBucket.Attributes = Field(
         default_factory=lambda: GCSBucket.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .g_c_s_object import GCSObject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/g_c_s_object.py` & `pyatlan-2.1.2/pyatlan/model/assets/g_c_s_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -437,15 +437,18 @@
                 gcs_bucket_qualified_name=gcs_bucket_qualified_name,
                 connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
                 qualified_name=f"{gcs_bucket_qualified_name}/{name}",
                 connector_name=connector_type.value,
                 gcs_bucket=GCSBucket.ref_by_qualified_name(gcs_bucket_qualified_name),
             )
 
-    attributes: "GCSObject.Attributes" = Field(
+    attributes: GCSObject.Attributes = Field(
         default_factory=lambda: GCSObject.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .g_c_s_bucket import GCSBucket  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/google.py` & `pyatlan-2.1.2/pyatlan/model/assets/google.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,12 +178,15 @@
         google_project_id: Optional[str] = Field(default=None, description="")
         google_project_number: Optional[int] = Field(default=None, description="")
         google_location: Optional[str] = Field(default=None, description="")
         google_location_type: Optional[str] = Field(default=None, description="")
         google_labels: Optional[List[GoogleLabel]] = Field(default=None, description="")
         google_tags: Optional[List[GoogleTag]] = Field(default=None, description="")
 
-    attributes: "Google.Attributes" = Field(
+    attributes: Google.Attributes = Field(
         default_factory=lambda: Google.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/infrastructure.py` & `pyatlan-2.1.2/pyatlan/model/assets/infrastructure.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/insight.py` & `pyatlan-2.1.2/pyatlan/model/assets/insight.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/kafka.py` & `pyatlan-2.1.2/pyatlan/model/assets/kafka.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/kafka_consumer_group.py` & `pyatlan-2.1.2/pyatlan/model/assets/kafka_consumer_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,15 +159,18 @@
         kafka_topic_qualified_names: Optional[Set[str]] = Field(
             default=None, description=""
         )
         kafka_topics: Optional[List[KafkaTopic]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "KafkaConsumerGroup.Attributes" = Field(
+    attributes: KafkaConsumerGroup.Attributes = Field(
         default_factory=lambda: KafkaConsumerGroup.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .kafka_topic import KafkaTopic  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/kafka_topic.py` & `pyatlan-2.1.2/pyatlan/model/assets/kafka_topic.py`

 * *Files 1% similar despite different names*

```diff
@@ -278,15 +278,18 @@
         kafka_topic_cleanup_policy: Optional[KafkaTopicCleanupPolicy] = Field(
             default=None, description=""
         )
         kafka_consumer_groups: Optional[List[KafkaConsumerGroup]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "KafkaTopic.Attributes" = Field(
+    attributes: KafkaTopic.Attributes = Field(
         default_factory=lambda: KafkaTopic.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .kafka_consumer_group import KafkaConsumerGroup  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/link.py` & `pyatlan-2.1.2/pyatlan/model/assets/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,18 @@
             return Link.Attributes(
                 qualified_name=qn,
                 name=name,
                 link=link,
                 asset=asset.trim_to_reference(),
             )
 
-    attributes: "Link.Attributes" = Field(
+    attributes: Link.Attributes = Field(
         default_factory=lambda: Link.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .asset import Asset  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/looker.py` & `pyatlan-2.1.2/pyatlan/model/assets/looker.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/looker_dashboard.py` & `pyatlan-2.1.2/pyatlan/model/assets/looker_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,17 +219,20 @@
         looks: Optional[List[LookerLook]] = Field(
             default=None, description=""
         )  # relationship
         folder: Optional[LookerFolder] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "LookerDashboard.Attributes" = Field(
+    attributes: LookerDashboard.Attributes = Field(
         default_factory=lambda: LookerDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .looker_folder import LookerFolder  # noqa
 from .looker_look import LookerLook  # noqa
 from .looker_tile import LookerTile  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/looker_explore.py` & `pyatlan-2.1.2/pyatlan/model/assets/looker_explore.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,17 +178,20 @@
         model: Optional[LookerModel] = Field(
             default=None, description=""
         )  # relationship
         fields: Optional[List[LookerField]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "LookerExplore.Attributes" = Field(
+    attributes: LookerExplore.Attributes = Field(
         default_factory=lambda: LookerExplore.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .looker_field import LookerField  # noqa
 from .looker_model import LookerModel  # noqa
 from .looker_project import LookerProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/looker_field.py` & `pyatlan-2.1.2/pyatlan/model/assets/looker_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,18 +247,21 @@
             default=None, description=""
         )  # relationship
         view: Optional[LookerView] = Field(default=None, description="")  # relationship
         model: Optional[LookerModel] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "LookerField.Attributes" = Field(
+    attributes: LookerField.Attributes = Field(
         default_factory=lambda: LookerField.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .looker_explore import LookerExplore  # noqa
 from .looker_model import LookerModel  # noqa
 from .looker_project import LookerProject  # noqa
 from .looker_view import LookerView  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/looker_folder.py` & `pyatlan-2.1.2/pyatlan/model/assets/looker_folder.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,16 +180,19 @@
         looks: Optional[List[LookerLook]] = Field(
             default=None, description=""
         )  # relationship
         looker_parent_folder: Optional[LookerFolder] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "LookerFolder.Attributes" = Field(
+    attributes: LookerFolder.Attributes = Field(
         default_factory=lambda: LookerFolder.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .looker_dashboard import LookerDashboard  # noqa
 from .looker_look import LookerLook  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/looker_look.py` & `pyatlan-2.1.2/pyatlan/model/assets/looker_look.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,18 +291,21 @@
         model: Optional[LookerModel] = Field(
             default=None, description=""
         )  # relationship
         dashboard: Optional[LookerDashboard] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "LookerLook.Attributes" = Field(
+    attributes: LookerLook.Attributes = Field(
         default_factory=lambda: LookerLook.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .looker_dashboard import LookerDashboard  # noqa
 from .looker_folder import LookerFolder  # noqa
 from .looker_model import LookerModel  # noqa
 from .looker_query import LookerQuery  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/looker_model.py` & `pyatlan-2.1.2/pyatlan/model/assets/looker_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -136,18 +136,21 @@
         queries: Optional[List[LookerQuery]] = Field(
             default=None, description=""
         )  # relationship
         fields: Optional[List[LookerField]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "LookerModel.Attributes" = Field(
+    attributes: LookerModel.Attributes = Field(
         default_factory=lambda: LookerModel.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .looker_explore import LookerExplore  # noqa
 from .looker_field import LookerField  # noqa
 from .looker_look import LookerLook  # noqa
 from .looker_project import LookerProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/looker_project.py` & `pyatlan-2.1.2/pyatlan/model/assets/looker_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,18 +103,21 @@
         fields: Optional[List[LookerField]] = Field(
             default=None, description=""
         )  # relationship
         views: Optional[List[LookerView]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "LookerProject.Attributes" = Field(
+    attributes: LookerProject.Attributes = Field(
         default_factory=lambda: LookerProject.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .looker_explore import LookerExplore  # noqa
 from .looker_field import LookerField  # noqa
 from .looker_model import LookerModel  # noqa
 from .looker_view import LookerView  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/looker_query.py` & `pyatlan-2.1.2/pyatlan/model/assets/looker_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,17 +164,20 @@
         looks: Optional[List[LookerLook]] = Field(
             default=None, description=""
         )  # relationship
         model: Optional[LookerModel] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "LookerQuery.Attributes" = Field(
+    attributes: LookerQuery.Attributes = Field(
         default_factory=lambda: LookerQuery.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .looker_look import LookerLook  # noqa
 from .looker_model import LookerModel  # noqa
 from .looker_tile import LookerTile  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/looker_tile.py` & `pyatlan-2.1.2/pyatlan/model/assets/looker_tile.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,17 +202,20 @@
             default=None, description=""
         )  # relationship
         look: Optional[LookerLook] = Field(default=None, description="")  # relationship
         dashboard: Optional[LookerDashboard] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "LookerTile.Attributes" = Field(
+    attributes: LookerTile.Attributes = Field(
         default_factory=lambda: LookerTile.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .looker_dashboard import LookerDashboard  # noqa
 from .looker_look import LookerLook  # noqa
 from .looker_query import LookerQuery  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/looker_view.py` & `pyatlan-2.1.2/pyatlan/model/assets/looker_view.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,16 +124,19 @@
         project: Optional[LookerProject] = Field(
             default=None, description=""
         )  # relationship
         fields: Optional[List[LookerField]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "LookerView.Attributes" = Field(
+    attributes: LookerView.Attributes = Field(
         default_factory=lambda: LookerView.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .looker_field import LookerField  # noqa
 from .looker_project import LookerProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/m_c_incident.py` & `pyatlan-2.1.2/pyatlan/model/assets/m_c_incident.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,16 +180,19 @@
         mc_monitor: Optional[MCMonitor] = Field(
             default=None, description=""
         )  # relationship
         mc_incident_assets: Optional[List[Asset]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MCIncident.Attributes" = Field(
+    attributes: MCIncident.Attributes = Field(
         default_factory=lambda: MCIncident.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .asset import Asset  # noqa
 from .m_c_monitor import MCMonitor  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/m_c_monitor.py` & `pyatlan-2.1.2/pyatlan/model/assets/m_c_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,18 @@
         mc_monitor_rule_is_snoozed: Optional[bool] = Field(default=None, description="")
         mc_monitor_breach_rate: Optional[float] = Field(default=None, description="")
         mc_monitor_incident_count: Optional[int] = Field(default=None, description="")
         mc_monitor_assets: Optional[List[Asset]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MCMonitor.Attributes" = Field(
+    attributes: MCMonitor.Attributes = Field(
         default_factory=lambda: MCMonitor.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .asset import Asset  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/materialised_view.py` & `pyatlan-2.1.2/pyatlan/model/assets/materialised_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -330,16 +330,19 @@
                 qualified_name=f"{schema_qualified_name}/{name}",
                 schema_qualified_name=schema_qualified_name,
                 schema_name=fields[4],
                 connector_name=connector_type.value,
                 atlan_schema=Schema.ref_by_qualified_name(schema_qualified_name),
             )
 
-    attributes: "MaterialisedView.Attributes" = Field(
+    attributes: MaterialisedView.Attributes = Field(
         default_factory=lambda: MaterialisedView.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .column import Column  # noqa
 from .schema import Schema  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/matillion.py` & `pyatlan-2.1.2/pyatlan/model/assets/matillion.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,12 +49,15 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.matillion_version = matillion_version
 
     class Attributes(Catalog.Attributes):
         matillion_version: Optional[str] = Field(default=None, description="")
 
-    attributes: "Matillion.Attributes" = Field(
+    attributes: Matillion.Attributes = Field(
         default_factory=lambda: Matillion.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/matillion_component.py` & `pyatlan-2.1.2/pyatlan/model/assets/matillion_component.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,16 +270,19 @@
         matillion_process: Optional[Process] = Field(
             default=None, description=""
         )  # relationship
         matillion_job: Optional[MatillionJob] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MatillionComponent.Attributes" = Field(
+    attributes: MatillionComponent.Attributes = Field(
         default_factory=lambda: MatillionComponent.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .matillion_job import MatillionJob  # noqa
 from .process import Process  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/matillion_group.py` & `pyatlan-2.1.2/pyatlan/model/assets/matillion_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,18 @@
 
     class Attributes(Matillion.Attributes):
         matillion_project_count: Optional[int] = Field(default=None, description="")
         matillion_projects: Optional[List[MatillionProject]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MatillionGroup.Attributes" = Field(
+    attributes: MatillionGroup.Attributes = Field(
         default_factory=lambda: MatillionGroup.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .matillion_project import MatillionProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/matillion_job.py` & `pyatlan-2.1.2/pyatlan/model/assets/matillion_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,16 +210,19 @@
         matillion_project: Optional[MatillionProject] = Field(
             default=None, description=""
         )  # relationship
         matillion_components: Optional[List[MatillionComponent]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MatillionJob.Attributes" = Field(
+    attributes: MatillionJob.Attributes = Field(
         default_factory=lambda: MatillionJob.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .matillion_component import MatillionComponent  # noqa
 from .matillion_project import MatillionProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/matillion_project.py` & `pyatlan-2.1.2/pyatlan/model/assets/matillion_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,19 @@
         matillion_jobs: Optional[List[MatillionJob]] = Field(
             default=None, description=""
         )  # relationship
         matillion_group: Optional[MatillionGroup] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MatillionProject.Attributes" = Field(
+    attributes: MatillionProject.Attributes = Field(
         default_factory=lambda: MatillionProject.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .matillion_group import MatillionGroup  # noqa
 from .matillion_job import MatillionJob  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/metabase.py` & `pyatlan-2.1.2/pyatlan/model/assets/metabase.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,12 +85,15 @@
 
     class Attributes(BI.Attributes):
         metabase_collection_name: Optional[str] = Field(default=None, description="")
         metabase_collection_qualified_name: Optional[str] = Field(
             default=None, description=""
         )
 
-    attributes: "Metabase.Attributes" = Field(
+    attributes: Metabase.Attributes = Field(
         default_factory=lambda: Metabase.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/metabase_collection.py` & `pyatlan-2.1.2/pyatlan/model/assets/metabase_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,16 +157,19 @@
         metabase_dashboards: Optional[List[MetabaseDashboard]] = Field(
             default=None, description=""
         )  # relationship
         metabase_questions: Optional[List[MetabaseQuestion]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MetabaseCollection.Attributes" = Field(
+    attributes: MetabaseCollection.Attributes = Field(
         default_factory=lambda: MetabaseCollection.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .metabase_dashboard import MetabaseDashboard  # noqa
 from .metabase_question import MetabaseQuestion  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/metabase_dashboard.py` & `pyatlan-2.1.2/pyatlan/model/assets/metabase_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,16 +88,19 @@
         metabase_questions: Optional[List[MetabaseQuestion]] = Field(
             default=None, description=""
         )  # relationship
         metabase_collection: Optional[MetabaseCollection] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MetabaseDashboard.Attributes" = Field(
+    attributes: MetabaseDashboard.Attributes = Field(
         default_factory=lambda: MetabaseDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .metabase_collection import MetabaseCollection  # noqa
 from .metabase_question import MetabaseQuestion  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/metabase_question.py` & `pyatlan-2.1.2/pyatlan/model/assets/metabase_question.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,16 +132,19 @@
         metabase_dashboards: Optional[List[MetabaseDashboard]] = Field(
             default=None, description=""
         )  # relationship
         metabase_collection: Optional[MetabaseCollection] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MetabaseQuestion.Attributes" = Field(
+    attributes: MetabaseQuestion.Attributes = Field(
         default_factory=lambda: MetabaseQuestion.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .metabase_collection import MetabaseCollection  # noqa
 from .metabase_dashboard import MetabaseDashboard  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/metric.py` & `pyatlan-2.1.2/pyatlan/model/assets/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,18 +164,21 @@
         assets: Optional[List[Asset]] = Field(
             default=None, description=""
         )  # relationship
         metric_dimension_columns: Optional[List[Column]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "Metric.Attributes" = Field(
+    attributes: Metric.Attributes = Field(
         default_factory=lambda: Metric.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 # Imports required for fixing circular dependencies:
 from .asset import Asset  # noqa # isort:skip
 from .catalog import Catalog  # noqa # isort:skip
 from .s_q_l import SQL  # noqa # isort:skip
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/micro_strategy.py` & `pyatlan-2.1.2/pyatlan/model/assets/micro_strategy.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,12 +305,15 @@
         micro_strategy_certified_at: Optional[datetime] = Field(
             default=None, description=""
         )
         micro_strategy_location: Optional[List[Dict[str, str]]] = Field(
             default=None, description=""
         )
 
-    attributes: "MicroStrategy.Attributes" = Field(
+    attributes: MicroStrategy.Attributes = Field(
         default_factory=lambda: MicroStrategy.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_attribute.py` & `pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_attribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,18 +150,21 @@
         micro_strategy_cubes: Optional[List[MicroStrategyCube]] = Field(
             default=None, description=""
         )  # relationship
         micro_strategy_project: Optional[MicroStrategyProject] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MicroStrategyAttribute.Attributes" = Field(
+    attributes: MicroStrategyAttribute.Attributes = Field(
         default_factory=lambda: MicroStrategyAttribute.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .micro_strategy_cube import MicroStrategyCube  # noqa
 from .micro_strategy_metric import MicroStrategyMetric  # noqa
 from .micro_strategy_project import MicroStrategyProject  # noqa
 from .micro_strategy_report import MicroStrategyReport  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_cube.py` & `pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_cube.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,17 +150,20 @@
         micro_strategy_project: Optional[MicroStrategyProject] = Field(
             default=None, description=""
         )  # relationship
         micro_strategy_attributes: Optional[List[MicroStrategyAttribute]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MicroStrategyCube.Attributes" = Field(
+    attributes: MicroStrategyCube.Attributes = Field(
         default_factory=lambda: MicroStrategyCube.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .micro_strategy_attribute import MicroStrategyAttribute  # noqa
 from .micro_strategy_metric import MicroStrategyMetric  # noqa
 from .micro_strategy_project import MicroStrategyProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_document.py` & `pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_document.py`

 * *Files 14% similar despite different names*

```diff
@@ -55,15 +55,18 @@
         self.attributes.micro_strategy_project = micro_strategy_project
 
     class Attributes(MicroStrategy.Attributes):
         micro_strategy_project: Optional[MicroStrategyProject] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MicroStrategyDocument.Attributes" = Field(
+    attributes: MicroStrategyDocument.Attributes = Field(
         default_factory=lambda: MicroStrategyDocument.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .micro_strategy_project import MicroStrategyProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_dossier.py` & `pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_dossier.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,16 +112,19 @@
         micro_strategy_visualizations: Optional[List[MicroStrategyVisualization]] = (
             Field(default=None, description="")
         )  # relationship
         micro_strategy_project: Optional[MicroStrategyProject] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MicroStrategyDossier.Attributes" = Field(
+    attributes: MicroStrategyDossier.Attributes = Field(
         default_factory=lambda: MicroStrategyDossier.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .micro_strategy_project import MicroStrategyProject  # noqa
 from .micro_strategy_visualization import MicroStrategyVisualization  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_fact.py` & `pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_fact.py`

 * *Files 4% similar despite different names*

```diff
@@ -108,16 +108,19 @@
         micro_strategy_metrics: Optional[List[MicroStrategyMetric]] = Field(
             default=None, description=""
         )  # relationship
         micro_strategy_project: Optional[MicroStrategyProject] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MicroStrategyFact.Attributes" = Field(
+    attributes: MicroStrategyFact.Attributes = Field(
         default_factory=lambda: MicroStrategyFact.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .micro_strategy_metric import MicroStrategyMetric  # noqa
 from .micro_strategy_project import MicroStrategyProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_metric.py` & `pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,18 +408,21 @@
         micro_strategy_project: Optional[MicroStrategyProject] = Field(
             default=None, description=""
         )  # relationship
         micro_strategy_attributes: Optional[List[MicroStrategyAttribute]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MicroStrategyMetric.Attributes" = Field(
+    attributes: MicroStrategyMetric.Attributes = Field(
         default_factory=lambda: MicroStrategyMetric.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .micro_strategy_attribute import MicroStrategyAttribute  # noqa
 from .micro_strategy_cube import MicroStrategyCube  # noqa
 from .micro_strategy_fact import MicroStrategyFact  # noqa
 from .micro_strategy_project import MicroStrategyProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_project.py` & `pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,18 +223,21 @@
         micro_strategy_dossiers: Optional[List[MicroStrategyDossier]] = Field(
             default=None, description=""
         )  # relationship
         micro_strategy_attributes: Optional[List[MicroStrategyAttribute]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MicroStrategyProject.Attributes" = Field(
+    attributes: MicroStrategyProject.Attributes = Field(
         default_factory=lambda: MicroStrategyProject.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .micro_strategy_attribute import MicroStrategyAttribute  # noqa
 from .micro_strategy_cube import MicroStrategyCube  # noqa
 from .micro_strategy_document import MicroStrategyDocument  # noqa
 from .micro_strategy_dossier import MicroStrategyDossier  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_report.py` & `pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,17 +128,20 @@
         micro_strategy_project: Optional[MicroStrategyProject] = Field(
             default=None, description=""
         )  # relationship
         micro_strategy_attributes: Optional[List[MicroStrategyAttribute]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MicroStrategyReport.Attributes" = Field(
+    attributes: MicroStrategyReport.Attributes = Field(
         default_factory=lambda: MicroStrategyReport.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .micro_strategy_attribute import MicroStrategyAttribute  # noqa
 from .micro_strategy_metric import MicroStrategyMetric  # noqa
 from .micro_strategy_project import MicroStrategyProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/micro_strategy_visualization.py` & `pyatlan-2.1.2/pyatlan/model/assets/micro_strategy_visualization.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,16 +168,19 @@
         micro_strategy_dossier: Optional[MicroStrategyDossier] = Field(
             default=None, description=""
         )  # relationship
         micro_strategy_project: Optional[MicroStrategyProject] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MicroStrategyVisualization.Attributes" = Field(
+    attributes: MicroStrategyVisualization.Attributes = Field(
         default_factory=lambda: MicroStrategyVisualization.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .micro_strategy_dossier import MicroStrategyDossier  # noqa
 from .micro_strategy_project import MicroStrategyProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/mode.py` & `pyatlan-2.1.2/pyatlan/model/assets/mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,12 +215,15 @@
             default=None, description=""
         )
         mode_report_name: Optional[str] = Field(default=None, description="")
         mode_report_qualified_name: Optional[str] = Field(default=None, description="")
         mode_query_name: Optional[str] = Field(default=None, description="")
         mode_query_qualified_name: Optional[str] = Field(default=None, description="")
 
-    attributes: "Mode.Attributes" = Field(
+    attributes: Mode.Attributes = Field(
         default_factory=lambda: Mode.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/mode_chart.py` & `pyatlan-2.1.2/pyatlan/model/assets/mode_chart.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,15 +68,18 @@
 
     class Attributes(Mode.Attributes):
         mode_chart_type: Optional[str] = Field(default=None, description="")
         mode_query: Optional[ModeQuery] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "ModeChart.Attributes" = Field(
+    attributes: ModeChart.Attributes = Field(
         default_factory=lambda: ModeChart.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .mode_query import ModeQuery  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/mode_collection.py` & `pyatlan-2.1.2/pyatlan/model/assets/mode_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,19 @@
         mode_workspace: Optional[ModeWorkspace] = Field(
             default=None, description=""
         )  # relationship
         mode_reports: Optional[List[ModeReport]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "ModeCollection.Attributes" = Field(
+    attributes: ModeCollection.Attributes = Field(
         default_factory=lambda: ModeCollection.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .mode_report import ModeReport  # noqa
 from .mode_workspace import ModeWorkspace  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/mode_query.py` & `pyatlan-2.1.2/pyatlan/model/assets/mode_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,19 @@
         mode_charts: Optional[List[ModeChart]] = Field(
             default=None, description=""
         )  # relationship
         mode_report: Optional[ModeReport] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "ModeQuery.Attributes" = Field(
+    attributes: ModeQuery.Attributes = Field(
         default_factory=lambda: ModeQuery.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .mode_chart import ModeChart  # noqa
 from .mode_report import ModeReport  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/mode_report.py` & `pyatlan-2.1.2/pyatlan/model/assets/mode_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,16 +209,19 @@
         mode_queries: Optional[List[ModeQuery]] = Field(
             default=None, description=""
         )  # relationship
         mode_collections: Optional[List[ModeCollection]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "ModeReport.Attributes" = Field(
+    attributes: ModeReport.Attributes = Field(
         default_factory=lambda: ModeReport.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .mode_collection import ModeCollection  # noqa
 from .mode_query import ModeQuery  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/mode_workspace.py` & `pyatlan-2.1.2/pyatlan/model/assets/mode_workspace.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,15 +70,18 @@
 
     class Attributes(Mode.Attributes):
         mode_collection_count: Optional[int] = Field(default=None, description="")
         mode_collections: Optional[List[ModeCollection]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "ModeWorkspace.Attributes" = Field(
+    attributes: ModeWorkspace.Attributes = Field(
         default_factory=lambda: ModeWorkspace.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .mode_collection import ModeCollection  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/mongo_d_b.py` & `pyatlan-2.1.2/pyatlan/model/assets/mongo_d_b.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/mongo_d_b_collection.py` & `pyatlan-2.1.2/pyatlan/model/assets/mongo_d_b_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,18 @@
     """
     PARTITION_LIST: ClassVar[KeywordField] = KeywordField(
         "partitionList", "partitionList"
     )
     """
     List of partitions in this table.
     """
+    IS_SHARDED: ClassVar[BooleanField] = BooleanField("isSharded", "isSharded")
+    """
+    Whether this table is a sharded table (true) or not (false).
+    """
     QUERY_COUNT: ClassVar[NumericField] = NumericField("queryCount", "queryCount")
     """
     Number of times this asset has been queried.
     """
     QUERY_USER_COUNT: ClassVar[NumericField] = NumericField(
         "queryUserCount", "queryUserCount"
     )
@@ -312,14 +316,15 @@
         "external_location",
         "external_location_region",
         "external_location_format",
         "is_partitioned",
         "partition_strategy",
         "partition_count",
         "partition_list",
+        "is_sharded",
         "query_count",
         "query_user_count",
         "query_user_map",
         "query_count_updated_at",
         "database_name",
         "database_qualified_name",
         "schema_name",
@@ -689,14 +694,24 @@
     @partition_list.setter
     def partition_list(self, partition_list: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_list = partition_list
 
     @property
+    def is_sharded(self) -> Optional[bool]:
+        return None if self.attributes is None else self.attributes.is_sharded
+
+    @is_sharded.setter
+    def is_sharded(self, is_sharded: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.is_sharded = is_sharded
+
+    @property
     def query_count(self) -> Optional[int]:
         return None if self.attributes is None else self.attributes.query_count
 
     @query_count.setter
     def query_count(self, query_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -941,14 +956,15 @@
         external_location: Optional[str] = Field(default=None, description="")
         external_location_region: Optional[str] = Field(default=None, description="")
         external_location_format: Optional[str] = Field(default=None, description="")
         is_partitioned: Optional[bool] = Field(default=None, description="")
         partition_strategy: Optional[str] = Field(default=None, description="")
         partition_count: Optional[int] = Field(default=None, description="")
         partition_list: Optional[str] = Field(default=None, description="")
+        is_sharded: Optional[bool] = Field(default=None, description="")
         query_count: Optional[int] = Field(default=None, description="")
         query_user_count: Optional[int] = Field(default=None, description="")
         query_user_map: Optional[Dict[str, int]] = Field(default=None, description="")
         query_count_updated_at: Optional[datetime] = Field(default=None, description="")
         database_name: Optional[str] = Field(default=None, description="")
         database_qualified_name: Optional[str] = Field(default=None, description="")
         schema_name: Optional[str] = Field(default=None, description="")
@@ -964,15 +980,18 @@
         is_profiled: Optional[bool] = Field(default=None, description="")
         last_profiled_at: Optional[datetime] = Field(default=None, description="")
         no_s_q_l_schema_definition: Optional[str] = Field(default=None, description="")
         mongo_d_b_database: Optional[MongoDBDatabase] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MongoDBCollection.Attributes" = Field(
+    attributes: MongoDBCollection.Attributes = Field(
         default_factory=lambda: MongoDBCollection.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .mongo_d_b_database import MongoDBDatabase  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/mongo_d_b_database.py` & `pyatlan-2.1.2/pyatlan/model/assets/mongo_d_b_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -430,15 +430,18 @@
         is_profiled: Optional[bool] = Field(default=None, description="")
         last_profiled_at: Optional[datetime] = Field(default=None, description="")
         no_s_q_l_schema_definition: Optional[str] = Field(default=None, description="")
         mongo_d_b_collections: Optional[List[MongoDBCollection]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "MongoDBDatabase.Attributes" = Field(
+    attributes: MongoDBDatabase.Attributes = Field(
         default_factory=lambda: MongoDBDatabase.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .mongo_d_b_collection import MongoDBCollection  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/monte_carlo.py` & `pyatlan-2.1.2/pyatlan/model/assets/monte_carlo.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,12 +71,15 @@
 
     class Attributes(DataQuality.Attributes):
         mc_labels: Optional[Set[str]] = Field(default=None, description="")
         mc_asset_qualified_names: Optional[Set[str]] = Field(
             default=None, description=""
         )
 
-    attributes: "MonteCarlo.Attributes" = Field(
+    attributes: MonteCarlo.Attributes = Field(
         default_factory=lambda: MonteCarlo.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/namespace.py` & `pyatlan-2.1.2/pyatlan/model/assets/namespace.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,58 +25,61 @@
         return v
 
     def __setattr__(self, name, value):
         if name in Namespace._convenience_properties:
             return object.__setattr__(self, name, value)
         super().__setattr__(name, value)
 
-    CHILDREN_QUERIES: ClassVar[RelationField] = RelationField("childrenQueries")
+    CHILDREN_FOLDERS: ClassVar[RelationField] = RelationField("childrenFolders")
     """
     TBC
     """
-    CHILDREN_FOLDERS: ClassVar[RelationField] = RelationField("childrenFolders")
+    CHILDREN_QUERIES: ClassVar[RelationField] = RelationField("childrenQueries")
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
-        "children_queries",
         "children_folders",
+        "children_queries",
     ]
 
     @property
-    def children_queries(self) -> Optional[List[Query]]:
-        return None if self.attributes is None else self.attributes.children_queries
-
-    @children_queries.setter
-    def children_queries(self, children_queries: Optional[List[Query]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.children_queries = children_queries
-
-    @property
     def children_folders(self) -> Optional[List[Folder]]:
         return None if self.attributes is None else self.attributes.children_folders
 
     @children_folders.setter
     def children_folders(self, children_folders: Optional[List[Folder]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.children_folders = children_folders
 
+    @property
+    def children_queries(self) -> Optional[List[Query]]:
+        return None if self.attributes is None else self.attributes.children_queries
+
+    @children_queries.setter
+    def children_queries(self, children_queries: Optional[List[Query]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.children_queries = children_queries
+
     class Attributes(Asset.Attributes):
-        children_queries: Optional[List[Query]] = Field(
+        children_folders: Optional[List[Folder]] = Field(
             default=None, description=""
         )  # relationship
-        children_folders: Optional[List[Folder]] = Field(
+        children_queries: Optional[List[Query]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "Namespace.Attributes" = Field(
+    attributes: Namespace.Attributes = Field(
         default_factory=lambda: Namespace.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .folder import Folder  # noqa
 from .query import Query  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/no_s_q_l.py` & `pyatlan-2.1.2/pyatlan/model/assets/no_s_q_l.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,12 +53,15 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.no_s_q_l_schema_definition = no_s_q_l_schema_definition
 
     class Attributes(Catalog.Attributes):
         no_s_q_l_schema_definition: Optional[str] = Field(default=None, description="")
 
-    attributes: "NoSQL.Attributes" = Field(
+    attributes: NoSQL.Attributes = Field(
         default_factory=lambda: NoSQL.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/object_store.py` & `pyatlan-2.1.2/pyatlan/model/assets/object_store.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/persona.py` & `pyatlan-2.1.2/pyatlan/model/assets/persona.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,12 +277,15 @@
                 qualified_name=name,
                 name=name,
                 display_name=name,
                 is_access_control_enabled=True,
                 description="",
             )
 
-    attributes: "Persona.Attributes" = Field(
+    attributes: Persona.Attributes = Field(
         default_factory=lambda: Persona.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/power_b_i.py` & `pyatlan-2.1.2/pyatlan/model/assets/power_b_i.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,12 +126,15 @@
             default=None, description=""
         )
         power_b_i_format_string: Optional[str] = Field(default=None, description="")
         power_b_i_endorsement: Optional[PowerbiEndorsement] = Field(
             default=None, description=""
         )
 
-    attributes: "PowerBI.Attributes" = Field(
+    attributes: PowerBI.Attributes = Field(
         default_factory=lambda: PowerBI.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/power_b_i_column.py` & `pyatlan-2.1.2/pyatlan/model/assets/power_b_i_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,15 +188,18 @@
         power_b_i_column_summarize_by: Optional[str] = Field(
             default=None, description=""
         )
         table: Optional[PowerBITable] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "PowerBIColumn.Attributes" = Field(
+    attributes: PowerBIColumn.Attributes = Field(
         default_factory=lambda: PowerBIColumn.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .power_b_i_table import PowerBITable  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/power_b_i_dashboard.py` & `pyatlan-2.1.2/pyatlan/model/assets/power_b_i_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,16 +122,19 @@
         workspace: Optional[PowerBIWorkspace] = Field(
             default=None, description=""
         )  # relationship
         tiles: Optional[List[PowerBITile]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "PowerBIDashboard.Attributes" = Field(
+    attributes: PowerBIDashboard.Attributes = Field(
         default_factory=lambda: PowerBIDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .power_b_i_tile import PowerBITile  # noqa
 from .power_b_i_workspace import PowerBIWorkspace  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/power_b_i_dataflow.py` & `pyatlan-2.1.2/pyatlan/model/assets/power_b_i_dataflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,16 +106,19 @@
         workspace: Optional[PowerBIWorkspace] = Field(
             default=None, description=""
         )  # relationship
         datasets: Optional[List[PowerBIDataset]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "PowerBIDataflow.Attributes" = Field(
+    attributes: PowerBIDataflow.Attributes = Field(
         default_factory=lambda: PowerBIDataflow.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .power_b_i_dataset import PowerBIDataset  # noqa
 from .power_b_i_workspace import PowerBIWorkspace  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/power_b_i_dataset.py` & `pyatlan-2.1.2/pyatlan/model/assets/power_b_i_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,18 +178,21 @@
         tables: Optional[List[PowerBITable]] = Field(
             default=None, description=""
         )  # relationship
         datasources: Optional[List[PowerBIDatasource]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "PowerBIDataset.Attributes" = Field(
+    attributes: PowerBIDataset.Attributes = Field(
         default_factory=lambda: PowerBIDataset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .power_b_i_dataflow import PowerBIDataflow  # noqa
 from .power_b_i_datasource import PowerBIDatasource  # noqa
 from .power_b_i_report import PowerBIReport  # noqa
 from .power_b_i_table import PowerBITable  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/power_b_i_datasource.py` & `pyatlan-2.1.2/pyatlan/model/assets/power_b_i_datasource.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,18 @@
         connection_details: Optional[Dict[str, str]] = Field(
             default=None, description=""
         )
         datasets: Optional[List[PowerBIDataset]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "PowerBIDatasource.Attributes" = Field(
+    attributes: PowerBIDatasource.Attributes = Field(
         default_factory=lambda: PowerBIDatasource.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .power_b_i_dataset import PowerBIDataset  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/power_b_i_measure.py` & `pyatlan-2.1.2/pyatlan/model/assets/power_b_i_measure.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,18 @@
         power_b_i_is_external_measure: Optional[bool] = Field(
             default=None, description=""
         )
         table: Optional[PowerBITable] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "PowerBIMeasure.Attributes" = Field(
+    attributes: PowerBIMeasure.Attributes = Field(
         default_factory=lambda: PowerBIMeasure.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .power_b_i_table import PowerBITable  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/power_b_i_page.py` & `pyatlan-2.1.2/pyatlan/model/assets/power_b_i_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,18 @@
     class Attributes(PowerBI.Attributes):
         workspace_qualified_name: Optional[str] = Field(default=None, description="")
         report_qualified_name: Optional[str] = Field(default=None, description="")
         report: Optional[PowerBIReport] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "PowerBIPage.Attributes" = Field(
+    attributes: PowerBIPage.Attributes = Field(
         default_factory=lambda: PowerBIPage.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .power_b_i_report import PowerBIReport  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/power_b_i_report.py` & `pyatlan-2.1.2/pyatlan/model/assets/power_b_i_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,18 +178,21 @@
         pages: Optional[List[PowerBIPage]] = Field(
             default=None, description=""
         )  # relationship
         dataset: Optional[PowerBIDataset] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "PowerBIReport.Attributes" = Field(
+    attributes: PowerBIReport.Attributes = Field(
         default_factory=lambda: PowerBIReport.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .power_b_i_dataset import PowerBIDataset  # noqa
 from .power_b_i_page import PowerBIPage  # noqa
 from .power_b_i_tile import PowerBITile  # noqa
 from .power_b_i_workspace import PowerBIWorkspace  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/power_b_i_table.py` & `pyatlan-2.1.2/pyatlan/model/assets/power_b_i_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,17 +206,20 @@
         measures: Optional[List[PowerBIMeasure]] = Field(
             default=None, description=""
         )  # relationship
         dataset: Optional[PowerBIDataset] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "PowerBITable.Attributes" = Field(
+    attributes: PowerBITable.Attributes = Field(
         default_factory=lambda: PowerBITable.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .power_b_i_column import PowerBIColumn  # noqa
 from .power_b_i_dataset import PowerBIDataset  # noqa
 from .power_b_i_measure import PowerBIMeasure  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/power_b_i_tile.py` & `pyatlan-2.1.2/pyatlan/model/assets/power_b_i_tile.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,17 +130,20 @@
         dataset: Optional[PowerBIDataset] = Field(
             default=None, description=""
         )  # relationship
         dashboard: Optional[PowerBIDashboard] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "PowerBITile.Attributes" = Field(
+    attributes: PowerBITile.Attributes = Field(
         default_factory=lambda: PowerBITile.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .power_b_i_dashboard import PowerBIDashboard  # noqa
 from .power_b_i_dataset import PowerBIDataset  # noqa
 from .power_b_i_report import PowerBIReport  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/power_b_i_workspace.py` & `pyatlan-2.1.2/pyatlan/model/assets/power_b_i_workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,18 +188,21 @@
         dashboards: Optional[List[PowerBIDashboard]] = Field(
             default=None, description=""
         )  # relationship
         dataflows: Optional[List[PowerBIDataflow]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "PowerBIWorkspace.Attributes" = Field(
+    attributes: PowerBIWorkspace.Attributes = Field(
         default_factory=lambda: PowerBIWorkspace.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .power_b_i_dashboard import PowerBIDashboard  # noqa
 from .power_b_i_dataflow import PowerBIDataflow  # noqa
 from .power_b_i_dataset import PowerBIDataset  # noqa
 from .power_b_i_report import PowerBIReport  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/preset.py` & `pyatlan-2.1.2/pyatlan/model/assets/preset.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,12 +127,15 @@
             default=None, description=""
         )
         preset_dashboard_id: Optional[int] = Field(default=None, description="")
         preset_dashboard_qualified_name: Optional[str] = Field(
             default=None, description=""
         )
 
-    attributes: "Preset.Attributes" = Field(
+    attributes: Preset.Attributes = Field(
         default_factory=lambda: Preset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/preset_chart.py` & `pyatlan-2.1.2/pyatlan/model/assets/preset_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,15 +161,18 @@
                 qualified_name=f"{preset_dashboard_qualified_name}/{name}",
                 connector_name=connector_type.value,
                 preset_dashboard=PresetDashboard.ref_by_qualified_name(
                     preset_dashboard_qualified_name
                 ),
             )
 
-    attributes: "PresetChart.Attributes" = Field(
+    attributes: PresetChart.Attributes = Field(
         default_factory=lambda: PresetChart.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .preset_dashboard import PresetDashboard  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/preset_dashboard.py` & `pyatlan-2.1.2/pyatlan/model/assets/preset_dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,17 +322,20 @@
                 qualified_name=f"{preset_workspace_qualified_name}/{name}",
                 connector_name=connector_type.value,
                 preset_workspace=PresetWorkspace.ref_by_qualified_name(
                     preset_workspace_qualified_name
                 ),
             )
 
-    attributes: "PresetDashboard.Attributes" = Field(
+    attributes: PresetDashboard.Attributes = Field(
         default_factory=lambda: PresetDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .preset_chart import PresetChart  # noqa
 from .preset_dataset import PresetDataset  # noqa
 from .preset_workspace import PresetWorkspace  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/preset_dataset.py` & `pyatlan-2.1.2/pyatlan/model/assets/preset_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -187,15 +187,18 @@
                 qualified_name=f"{preset_dashboard_qualified_name}/{name}",
                 connector_name=connector_type.value,
                 preset_dashboard=PresetDashboard.ref_by_qualified_name(
                     preset_dashboard_qualified_name
                 ),
             )
 
-    attributes: "PresetDataset.Attributes" = Field(
+    attributes: PresetDataset.Attributes = Field(
         default_factory=lambda: PresetDataset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .preset_dashboard import PresetDashboard  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/preset_workspace.py` & `pyatlan-2.1.2/pyatlan/model/assets/preset_workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,15 +334,18 @@
             return PresetWorkspace.Attributes(
                 name=name,
                 qualified_name=f"{connection_qualified_name}/{name}",
                 connection_qualified_name=connection_qualified_name,
                 connector_name=connector_type.value,
             )
 
-    attributes: "PresetWorkspace.Attributes" = Field(
+    attributes: PresetWorkspace.Attributes = Field(
         default_factory=lambda: PresetWorkspace.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .preset_dashboard import PresetDashboard  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/procedure.py` & `pyatlan-2.1.2/pyatlan/model/assets/procedure.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,15 +66,18 @@
 
     class Attributes(SQL.Attributes):
         definition: Optional[str] = Field(default=None, description="")
         atlan_schema: Optional[Schema] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "Procedure.Attributes" = Field(
+    attributes: Procedure.Attributes = Field(
         default_factory=lambda: Procedure.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .schema import Schema  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/process.py` & `pyatlan-2.1.2/pyatlan/model/assets/process.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,24 +104,29 @@
     """
     TBC
     """
     COLUMN_PROCESSES: ClassVar[RelationField] = RelationField("columnProcesses")
     """
     TBC
     """
+    SPARK_JOBS: ClassVar[RelationField] = RelationField("sparkJobs")
+    """
+    TBC
+    """
 
     _convenience_properties: ClassVar[List[str]] = [
         "inputs",
         "outputs",
         "code",
         "sql",
         "ast",
         "matillion_component",
         "airflow_tasks",
         "column_processes",
+        "spark_jobs",
     ]
 
     @property
     def inputs(self) -> Optional[List[Catalog]]:
         return None if self.attributes is None else self.attributes.inputs
 
     @inputs.setter
@@ -196,14 +201,24 @@
 
     @column_processes.setter
     def column_processes(self, column_processes: Optional[List[ColumnProcess]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.column_processes = column_processes
 
+    @property
+    def spark_jobs(self) -> Optional[List[SparkJob]]:
+        return None if self.attributes is None else self.attributes.spark_jobs
+
+    @spark_jobs.setter
+    def spark_jobs(self, spark_jobs: Optional[List[SparkJob]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.spark_jobs = spark_jobs
+
     class Attributes(Asset.Attributes):
         inputs: Optional[List[Catalog]] = Field(default=None, description="")
         outputs: Optional[List[Catalog]] = Field(default=None, description="")
         code: Optional[str] = Field(default=None, description="")
         sql: Optional[str] = Field(default=None, description="")
         ast: Optional[str] = Field(default=None, description="")
         matillion_component: Optional[MatillionComponent] = Field(
@@ -211,14 +226,17 @@
         )  # relationship
         airflow_tasks: Optional[List[AirflowTask]] = Field(
             default=None, description=""
         )  # relationship
         column_processes: Optional[List[ColumnProcess]] = Field(
             default=None, description=""
         )  # relationship
+        spark_jobs: Optional[List[SparkJob]] = Field(
+            default=None, description=""
+        )  # relationship
 
         @staticmethod
         def generate_qualified_name(
             name: str,
             connection_qualified_name: str,
             inputs: List["Catalog"],
             outputs: List["Catalog"],
@@ -277,18 +295,22 @@
                 qualified_name=qualified_name,
                 connector_name=connector_name,
                 connection_qualified_name=connection_qualified_name,
                 inputs=inputs,
                 outputs=outputs,
             )
 
-    attributes: "Process.Attributes" = Field(
+    attributes: Process.Attributes = Field(
         default_factory=lambda: Process.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .airflow_task import AirflowTask  # noqa
 from .catalog import Catalog  # noqa
 from .column_process import ColumnProcess  # noqa
 from .matillion_component import MatillionComponent  # noqa
+from .spark_job import SparkJob  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/process_execution.py` & `pyatlan-2.1.2/pyatlan/model/assets/process_execution.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/purpose.py` & `pyatlan-2.1.2/pyatlan/model/assets/purpose.py`

 * *Files 1% similar despite different names*

```diff
@@ -253,12 +253,15 @@
                 name=name,
                 display_name=name,
                 is_access_control_enabled=True,
                 description="",
                 purpose_atlan_tags=atlan_tags,
             )
 
-    attributes: "Purpose.Attributes" = Field(
+    attributes: Purpose.Attributes = Field(
         default_factory=lambda: Purpose.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/qlik.py` & `pyatlan-2.1.2/pyatlan/model/assets/qlik.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,12 +179,15 @@
         qlik_space_id: Optional[str] = Field(default=None, description="")
         qlik_space_qualified_name: Optional[str] = Field(default=None, description="")
         qlik_app_id: Optional[str] = Field(default=None, description="")
         qlik_app_qualified_name: Optional[str] = Field(default=None, description="")
         qlik_owner_id: Optional[str] = Field(default=None, description="")
         qlik_is_published: Optional[bool] = Field(default=None, description="")
 
-    attributes: "Qlik.Attributes" = Field(
+    attributes: Qlik.Attributes = Field(
         default_factory=lambda: Qlik.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/qlik_app.py` & `pyatlan-2.1.2/pyatlan/model/assets/qlik_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,16 +173,19 @@
         qlik_space: Optional[QlikSpace] = Field(
             default=None, description=""
         )  # relationship
         qlik_sheets: Optional[List[QlikSheet]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "QlikApp.Attributes" = Field(
+    attributes: QlikApp.Attributes = Field(
         default_factory=lambda: QlikApp.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .qlik_sheet import QlikSheet  # noqa
 from .qlik_space import QlikSpace  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/qlik_chart.py` & `pyatlan-2.1.2/pyatlan/model/assets/qlik_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,18 @@
         qlik_chart_footnote: Optional[str] = Field(default=None, description="")
         qlik_chart_orientation: Optional[str] = Field(default=None, description="")
         qlik_chart_type: Optional[str] = Field(default=None, description="")
         qlik_sheet: Optional[QlikSheet] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "QlikChart.Attributes" = Field(
+    attributes: QlikChart.Attributes = Field(
         default_factory=lambda: QlikChart.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .qlik_sheet import QlikSheet  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/qlik_dataset.py` & `pyatlan-2.1.2/pyatlan/model/assets/qlik_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,18 @@
         qlik_dataset_type: Optional[str] = Field(default=None, description="")
         qlik_dataset_uri: Optional[str] = Field(default=None, description="")
         qlik_dataset_subtype: Optional[str] = Field(default=None, description="")
         qlik_space: Optional[QlikSpace] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "QlikDataset.Attributes" = Field(
+    attributes: QlikDataset.Attributes = Field(
         default_factory=lambda: QlikDataset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .qlik_space import QlikSpace  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/qlik_sheet.py` & `pyatlan-2.1.2/pyatlan/model/assets/qlik_sheet.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,16 +88,19 @@
         qlik_app: Optional[QlikApp] = Field(
             default=None, description=""
         )  # relationship
         qlik_charts: Optional[List[QlikChart]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "QlikSheet.Attributes" = Field(
+    attributes: QlikSheet.Attributes = Field(
         default_factory=lambda: QlikSheet.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .qlik_app import QlikApp  # noqa
 from .qlik_chart import QlikChart  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/qlik_space.py` & `pyatlan-2.1.2/pyatlan/model/assets/qlik_space.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,16 +86,19 @@
         qlik_datasets: Optional[List[QlikDataset]] = Field(
             default=None, description=""
         )  # relationship
         qlik_apps: Optional[List[QlikApp]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "QlikSpace.Attributes" = Field(
+    attributes: QlikSpace.Attributes = Field(
         default_factory=lambda: QlikSpace.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .qlik_app import QlikApp  # noqa
 from .qlik_dataset import QlikDataset  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/qlik_stream.py` & `pyatlan-2.1.2/pyatlan/model/assets/qlik_stream.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/query.py` & `pyatlan-2.1.2/pyatlan/model/assets/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -357,18 +357,21 @@
         tables: Optional[List[Table]] = Field(
             default=None, description=""
         )  # relationship
         views: Optional[List[View]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "Query.Attributes" = Field(
+    attributes: Query.Attributes = Field(
         default_factory=lambda: Query.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .column import Column  # noqa
 from .namespace import Namespace  # noqa
 from .table import Table  # noqa
 from .view import View  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/quick_sight.py` & `pyatlan-2.1.2/pyatlan/model/assets/quick_sight.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,12 +87,15 @@
         self.attributes.quick_sight_sheet_name = quick_sight_sheet_name
 
     class Attributes(BI.Attributes):
         quick_sight_id: Optional[str] = Field(default=None, description="")
         quick_sight_sheet_id: Optional[str] = Field(default=None, description="")
         quick_sight_sheet_name: Optional[str] = Field(default=None, description="")
 
-    attributes: "QuickSight.Attributes" = Field(
+    attributes: QuickSight.Attributes = Field(
         default_factory=lambda: QuickSight.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/quick_sight_analysis.py` & `pyatlan-2.1.2/pyatlan/model/assets/quick_sight_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -196,16 +196,19 @@
         quick_sight_analysis_visuals: Optional[List[QuickSightAnalysisVisual]] = Field(
             default=None, description=""
         )  # relationship
         quick_sight_analysis_folders: Optional[List[QuickSightFolder]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "QuickSightAnalysis.Attributes" = Field(
+    attributes: QuickSightAnalysis.Attributes = Field(
         default_factory=lambda: QuickSightAnalysis.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .quick_sight_analysis_visual import QuickSightAnalysisVisual  # noqa
 from .quick_sight_folder import QuickSightFolder  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/quick_sight_analysis_visual.py` & `pyatlan-2.1.2/pyatlan/model/assets/quick_sight_analysis_visual.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,15 +80,18 @@
         quick_sight_analysis_qualified_name: Optional[str] = Field(
             default=None, description=""
         )
         quick_sight_analysis: Optional[QuickSightAnalysis] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "QuickSightAnalysisVisual.Attributes" = Field(
+    attributes: QuickSightAnalysisVisual.Attributes = Field(
         default_factory=lambda: QuickSightAnalysisVisual.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .quick_sight_analysis import QuickSightAnalysis  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/quick_sight_dashboard.py` & `pyatlan-2.1.2/pyatlan/model/assets/quick_sight_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,16 +146,19 @@
         quick_sight_dashboard_folders: Optional[List[QuickSightFolder]] = Field(
             default=None, description=""
         )  # relationship
         quick_sight_dashboard_visuals: Optional[List[QuickSightDashboardVisual]] = (
             Field(default=None, description="")
         )  # relationship
 
-    attributes: "QuickSightDashboard.Attributes" = Field(
+    attributes: QuickSightDashboard.Attributes = Field(
         default_factory=lambda: QuickSightDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .quick_sight_dashboard_visual import QuickSightDashboardVisual  # noqa
 from .quick_sight_folder import QuickSightFolder  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/quick_sight_dashboard_visual.py` & `pyatlan-2.1.2/pyatlan/model/assets/quick_sight_dashboard_visual.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,18 @@
         quick_sight_dashboard_qualified_name: Optional[str] = Field(
             default=None, description=""
         )
         quick_sight_dashboard: Optional[QuickSightDashboard] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "QuickSightDashboardVisual.Attributes" = Field(
+    attributes: QuickSightDashboardVisual.Attributes = Field(
         default_factory=lambda: QuickSightDashboardVisual.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .quick_sight_dashboard import QuickSightDashboard  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/quick_sight_dataset.py` & `pyatlan-2.1.2/pyatlan/model/assets/quick_sight_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,16 +141,19 @@
         quick_sight_dataset_folders: Optional[List[QuickSightFolder]] = Field(
             default=None, description=""
         )  # relationship
         quick_sight_dataset_fields: Optional[List[QuickSightDatasetField]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "QuickSightDataset.Attributes" = Field(
+    attributes: QuickSightDataset.Attributes = Field(
         default_factory=lambda: QuickSightDataset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .quick_sight_dataset_field import QuickSightDatasetField  # noqa
 from .quick_sight_folder import QuickSightFolder  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/quick_sight_dataset_field.py` & `pyatlan-2.1.2/pyatlan/model/assets/quick_sight_dataset_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,15 +111,18 @@
         quick_sight_dataset_qualified_name: Optional[str] = Field(
             default=None, description=""
         )
         quick_sight_dataset: Optional[QuickSightDataset] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "QuickSightDatasetField.Attributes" = Field(
+    attributes: QuickSightDatasetField.Attributes = Field(
         default_factory=lambda: QuickSightDatasetField.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .quick_sight_dataset import QuickSightDataset  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/quick_sight_folder.py` & `pyatlan-2.1.2/pyatlan/model/assets/quick_sight_folder.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,17 +147,20 @@
         quick_sight_datasets: Optional[List[QuickSightDataset]] = Field(
             default=None, description=""
         )  # relationship
         quick_sight_analyses: Optional[List[QuickSightAnalysis]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "QuickSightFolder.Attributes" = Field(
+    attributes: QuickSightFolder.Attributes = Field(
         default_factory=lambda: QuickSightFolder.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .quick_sight_analysis import QuickSightAnalysis  # noqa
 from .quick_sight_dashboard import QuickSightDashboard  # noqa
 from .quick_sight_dataset import QuickSightDataset  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/readme.py` & `pyatlan-2.1.2/pyatlan/model/assets/readme.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,18 @@
             return Readme.Attributes(
                 qualified_name=f"{asset.guid}/readme",
                 name=f"{asset_name} Readme",
                 asset=asset,
                 description=quote(content),
             )
 
-    attributes: "Readme.Attributes" = Field(
+    attributes: Readme.Attributes = Field(
         default_factory=lambda: Readme.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .asset import Asset  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/readme_template.py` & `pyatlan-2.1.2/pyatlan/model/assets/readme_template.py`

 * *Files 10% similar despite different names*

```diff
@@ -64,12 +64,15 @@
             self.attributes = self.Attributes()
         self.attributes.icon_type = icon_type
 
     class Attributes(Resource.Attributes):
         icon: Optional[str] = Field(default=None, description="")
         icon_type: Optional[IconType] = Field(default=None, description="")
 
-    attributes: "ReadmeTemplate.Attributes" = Field(
+    attributes: ReadmeTemplate.Attributes = Field(
         default_factory=lambda: ReadmeTemplate.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/redash.py` & `pyatlan-2.1.2/pyatlan/model/assets/redash.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,12 +49,15 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.redash_is_published = redash_is_published
 
     class Attributes(BI.Attributes):
         redash_is_published: Optional[bool] = Field(default=None, description="")
 
-    attributes: "Redash.Attributes" = Field(
+    attributes: Redash.Attributes = Field(
         default_factory=lambda: Redash.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/redash_dashboard.py` & `pyatlan-2.1.2/pyatlan/model/assets/redash_dashboard.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,12 +57,15 @@
         self.attributes.redash_dashboard_widget_count = redash_dashboard_widget_count
 
     class Attributes(Redash.Attributes):
         redash_dashboard_widget_count: Optional[int] = Field(
             default=None, description=""
         )
 
-    attributes: "RedashDashboard.Attributes" = Field(
+    attributes: RedashDashboard.Attributes = Field(
         default_factory=lambda: RedashDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/redash_query.py` & `pyatlan-2.1.2/pyatlan/model/assets/redash_query.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,18 @@
         redash_query_schedule_humanized: Optional[str] = Field(
             default=None, description=""
         )
         redash_visualizations: Optional[List[RedashVisualization]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "RedashQuery.Attributes" = Field(
+    attributes: RedashQuery.Attributes = Field(
         default_factory=lambda: RedashQuery.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .redash_visualization import RedashVisualization  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/redash_visualization.py` & `pyatlan-2.1.2/pyatlan/model/assets/redash_visualization.py`

 * *Files 3% similar despite different names*

```diff
@@ -118,15 +118,18 @@
         redash_visualization_type: Optional[str] = Field(default=None, description="")
         redash_query_name: Optional[str] = Field(default=None, description="")
         redash_query_qualified_name: Optional[str] = Field(default=None, description="")
         redash_query: Optional[RedashQuery] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "RedashVisualization.Attributes" = Field(
+    attributes: RedashVisualization.Attributes = Field(
         default_factory=lambda: RedashVisualization.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .redash_query import RedashQuery  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/referenceable.py` & `pyatlan-2.1.2/pyatlan/model/assets/referenceable.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/resource.py` & `pyatlan-2.1.2/pyatlan/model/assets/resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,12 +99,15 @@
         link: Optional[str] = Field(default=None, description="")
         is_global: Optional[bool] = Field(default=None, description="")
         reference: Optional[str] = Field(default=None, description="")
         resource_metadata: Optional[Dict[str, str]] = Field(
             default=None, description=""
         )
 
-    attributes: "Resource.Attributes" = Field(
+    attributes: Resource.Attributes = Field(
         default_factory=lambda: Resource.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/s3.py` & `pyatlan-2.1.2/pyatlan/model/assets/s3.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,12 +218,15 @@
         aws_region: Optional[str] = Field(default=None, description="")
         aws_account_id: Optional[str] = Field(default=None, description="")
         aws_resource_id: Optional[str] = Field(default=None, description="")
         aws_owner_name: Optional[str] = Field(default=None, description="")
         aws_owner_id: Optional[str] = Field(default=None, description="")
         aws_tags: Optional[List[AwsTag]] = Field(default=None, description="")
 
-    attributes: "S3.Attributes" = Field(
+    attributes: S3.Attributes = Field(
         default_factory=lambda: S3.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/s3_bucket.py` & `pyatlan-2.1.2/pyatlan/model/assets/s3_bucket.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,15 +208,18 @@
                 aws_arn=aws_arn,
                 name=name,
                 connection_qualified_name=connection_qualified_name,
                 qualified_name=f"{connection_qualified_name}/{aws_arn if aws_arn else name}",
                 connector_name=connector_type.value,
             )
 
-    attributes: "S3Bucket.Attributes" = Field(
+    attributes: S3Bucket.Attributes = Field(
         default_factory=lambda: S3Bucket.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .s3_object import S3Object  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/s3_object.py` & `pyatlan-2.1.2/pyatlan/model/assets/s3_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -401,15 +401,18 @@
                 connection_qualified_name=connection_qualified_name,
                 qualified_name=f"{connection_qualified_name}/{object_key}",
                 connector_name=connector_type.value,
                 s3_bucket_qualified_name=s3_bucket_qualified_name,
                 bucket=S3Bucket.ref_by_qualified_name(s3_bucket_qualified_name),
             )
 
-    attributes: "S3Object.Attributes" = Field(
+    attributes: S3Object.Attributes = Field(
         default_factory=lambda: S3Object.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .s3_bucket import S3Bucket  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/s_q_l.py` & `pyatlan-2.1.2/pyatlan/model/assets/s_q_l.py`

 * *Files 1% similar despite different names*

```diff
@@ -431,17 +431,20 @@
         dbt_models: Optional[List[DbtModel]] = Field(
             default=None, description=""
         )  # relationship
         dbt_tests: Optional[List[DbtTest]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SQL.Attributes" = Field(
+    attributes: SQL.Attributes = Field(
         default_factory=lambda: SQL.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .dbt_model import DbtModel  # noqa
 from .dbt_source import DbtSource  # noqa
 from .dbt_test import DbtTest  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/saa_s.py` & `pyatlan-2.1.2/pyatlan/model/assets/saa_s.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/salesforce.py` & `pyatlan-2.1.2/pyatlan/model/assets/salesforce.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,12 +71,15 @@
             self.attributes = self.Attributes()
         self.attributes.api_name = api_name
 
     class Attributes(SaaS.Attributes):
         organization_qualified_name: Optional[str] = Field(default=None, description="")
         api_name: Optional[str] = Field(default=None, description="")
 
-    attributes: "Salesforce.Attributes" = Field(
+    attributes: Salesforce.Attributes = Field(
         default_factory=lambda: Salesforce.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/salesforce_dashboard.py` & `pyatlan-2.1.2/pyatlan/model/assets/salesforce_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,16 +118,19 @@
         reports: Optional[List[SalesforceReport]] = Field(
             default=None, description=""
         )  # relationship
         organization: Optional[SalesforceOrganization] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SalesforceDashboard.Attributes" = Field(
+    attributes: SalesforceDashboard.Attributes = Field(
         default_factory=lambda: SalesforceDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .salesforce_organization import SalesforceOrganization  # noqa
 from .salesforce_report import SalesforceReport  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/salesforce_field.py` & `pyatlan-2.1.2/pyatlan/model/assets/salesforce_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -353,15 +353,18 @@
         lookup_objects: Optional[List[SalesforceObject]] = Field(
             default=None, description=""
         )  # relationship
         object: Optional[SalesforceObject] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SalesforceField.Attributes" = Field(
+    attributes: SalesforceField.Attributes = Field(
         default_factory=lambda: SalesforceField.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .salesforce_object import SalesforceObject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/salesforce_object.py` & `pyatlan-2.1.2/pyatlan/model/assets/salesforce_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,16 +150,19 @@
         organization: Optional[SalesforceOrganization] = Field(
             default=None, description=""
         )  # relationship
         fields: Optional[List[SalesforceField]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SalesforceObject.Attributes" = Field(
+    attributes: SalesforceObject.Attributes = Field(
         default_factory=lambda: SalesforceObject.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .salesforce_field import SalesforceField  # noqa
 from .salesforce_organization import SalesforceOrganization  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/salesforce_organization.py` & `pyatlan-2.1.2/pyatlan/model/assets/salesforce_organization.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,17 +102,20 @@
         objects: Optional[List[SalesforceObject]] = Field(
             default=None, description=""
         )  # relationship
         dashboards: Optional[List[SalesforceDashboard]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SalesforceOrganization.Attributes" = Field(
+    attributes: SalesforceOrganization.Attributes = Field(
         default_factory=lambda: SalesforceOrganization.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .salesforce_dashboard import SalesforceDashboard  # noqa
 from .salesforce_object import SalesforceObject  # noqa
 from .salesforce_report import SalesforceReport  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/salesforce_report.py` & `pyatlan-2.1.2/pyatlan/model/assets/salesforce_report.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,16 +118,19 @@
         dashboards: Optional[List[SalesforceDashboard]] = Field(
             default=None, description=""
         )  # relationship
         organization: Optional[SalesforceOrganization] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SalesforceReport.Attributes" = Field(
+    attributes: SalesforceReport.Attributes = Field(
         default_factory=lambda: SalesforceReport.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .salesforce_dashboard import SalesforceDashboard  # noqa
 from .salesforce_organization import SalesforceOrganization  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/schema.py` & `pyatlan-2.1.2/pyatlan/model/assets/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from typing import ClassVar, List, Optional
 from warnings import warn
 
 from pydantic.v1 import Field, validator
 
 from pyatlan.model.enums import AtlanConnectorType
-from pyatlan.model.fields.atlan_fields import NumericField, RelationField
+from pyatlan.model.fields.atlan_fields import KeywordField, NumericField, RelationField
 from pyatlan.utils import init_guid, validate_required_fields
 
 from .s_q_l import SQL
 
 
 class Schema(SQL):
     """Description"""
@@ -63,14 +63,20 @@
     """
     Number of tables in this schema.
     """
     VIEWS_COUNT: ClassVar[NumericField] = NumericField("viewsCount", "viewsCount")
     """
     Number of views in this schema.
     """
+    LINKED_SCHEMA_QUALIFIED_NAME: ClassVar[KeywordField] = KeywordField(
+        "linkedSchemaQualifiedName", "linkedSchemaQualifiedName"
+    )
+    """
+    Unique name of the Linked Schema on which this Schema is dependent. This concept is mostly applicable for linked datasets/datasource in Google BigQuery via Analytics Hub Listing
+    """  # noqa: E501
 
     SNOWFLAKE_TAGS: ClassVar[RelationField] = RelationField("snowflakeTags")
     """
     TBC
     """
     FUNCTIONS: ClassVar[RelationField] = RelationField("functions")
     """
@@ -114,14 +120,15 @@
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
         "table_count",
         "views_count",
+        "linked_schema_qualified_name",
         "snowflake_tags",
         "functions",
         "tables",
         "database",
         "procedures",
         "views",
         "materialised_views",
@@ -148,14 +155,28 @@
     @views_count.setter
     def views_count(self, views_count: Optional[int]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.views_count = views_count
 
     @property
+    def linked_schema_qualified_name(self) -> Optional[str]:
+        return (
+            None
+            if self.attributes is None
+            else self.attributes.linked_schema_qualified_name
+        )
+
+    @linked_schema_qualified_name.setter
+    def linked_schema_qualified_name(self, linked_schema_qualified_name: Optional[str]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.linked_schema_qualified_name = linked_schema_qualified_name
+
+    @property
     def snowflake_tags(self) -> Optional[List[SnowflakeTag]]:
         return None if self.attributes is None else self.attributes.snowflake_tags
 
     @snowflake_tags.setter
     def snowflake_tags(self, snowflake_tags: Optional[List[SnowflakeTag]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -266,14 +287,17 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.calculation_views = calculation_views
 
     class Attributes(SQL.Attributes):
         table_count: Optional[int] = Field(default=None, description="")
         views_count: Optional[int] = Field(default=None, description="")
+        linked_schema_qualified_name: Optional[str] = Field(
+            default=None, description=""
+        )
         snowflake_tags: Optional[List[SnowflakeTag]] = Field(
             default=None, description=""
         )  # relationship
         functions: Optional[List[Function]] = Field(
             default=None, description=""
         )  # relationship
         tables: Optional[List[Table]] = Field(
@@ -327,18 +351,21 @@
                 connection_qualified_name=f"{fields[0]}/{fields[1]}/{fields[2]}",
                 database_qualified_name=database_qualified_name,
                 qualified_name=f"{database_qualified_name}/{name}",
                 connector_name=connector_type.value,
                 database=Database.ref_by_qualified_name(database_qualified_name),
             )
 
-    attributes: "Schema.Attributes" = Field(
+    attributes: Schema.Attributes = Field(
         default_factory=lambda: Schema.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .calculation_view import CalculationView  # noqa
 from .database import Database  # noqa
 from .function import Function  # noqa
 from .materialised_view import MaterialisedView  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/schema_registry.py` & `pyatlan-2.1.2/pyatlan/model/assets/schema_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,12 +80,15 @@
 
     class Attributes(Catalog.Attributes):
         schema_registry_schema_type: Optional[SchemaRegistrySchemaType] = Field(
             default=None, description=""
         )
         schema_registry_schema_id: Optional[str] = Field(default=None, description="")
 
-    attributes: "SchemaRegistry.Attributes" = Field(
+    attributes: SchemaRegistry.Attributes = Field(
         default_factory=lambda: SchemaRegistry.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/schema_registry_subject.py` & `pyatlan-2.1.2/pyatlan/model/assets/schema_registry_subject.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,18 @@
         schema_registry_subject_governing_asset_qualified_names: Optional[Set[str]] = (
             Field(default=None, description="")
         )
         assets: Optional[List[Asset]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SchemaRegistrySubject.Attributes" = Field(
+    attributes: SchemaRegistrySubject.Attributes = Field(
         default_factory=lambda: SchemaRegistrySubject.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .asset import Asset  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sigma.py` & `pyatlan-2.1.2/pyatlan/model/assets/sigma.py`

 * *Files 6% similar despite different names*

```diff
@@ -169,12 +169,15 @@
         sigma_page_qualified_name: Optional[str] = Field(default=None, description="")
         sigma_page_name: Optional[str] = Field(default=None, description="")
         sigma_data_element_qualified_name: Optional[str] = Field(
             default=None, description=""
         )
         sigma_data_element_name: Optional[str] = Field(default=None, description="")
 
-    attributes: "Sigma.Attributes" = Field(
+    attributes: Sigma.Attributes = Field(
         default_factory=lambda: Sigma.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sigma_data_element.py` & `pyatlan-2.1.2/pyatlan/model/assets/sigma_data_element.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,16 +144,19 @@
         sigma_page: Optional[SigmaPage] = Field(
             default=None, description=""
         )  # relationship
         sigma_data_element_fields: Optional[List[SigmaDataElementField]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SigmaDataElement.Attributes" = Field(
+    attributes: SigmaDataElement.Attributes = Field(
         default_factory=lambda: SigmaDataElement.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .sigma_data_element_field import SigmaDataElementField  # noqa
 from .sigma_page import SigmaPage  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sigma_data_element_field.py` & `pyatlan-2.1.2/pyatlan/model/assets/sigma_data_element_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,18 @@
         sigma_data_element_field_formula: Optional[str] = Field(
             default=None, description=""
         )
         sigma_data_element: Optional[SigmaDataElement] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SigmaDataElementField.Attributes" = Field(
+    attributes: SigmaDataElementField.Attributes = Field(
         default_factory=lambda: SigmaDataElementField.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .sigma_data_element import SigmaDataElement  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sigma_dataset.py` & `pyatlan-2.1.2/pyatlan/model/assets/sigma_dataset.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,15 +78,18 @@
 
     class Attributes(Sigma.Attributes):
         sigma_dataset_column_count: Optional[int] = Field(default=None, description="")
         sigma_dataset_columns: Optional[List[SigmaDatasetColumn]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SigmaDataset.Attributes" = Field(
+    attributes: SigmaDataset.Attributes = Field(
         default_factory=lambda: SigmaDataset.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .sigma_dataset_column import SigmaDatasetColumn  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sigma_dataset_column.py` & `pyatlan-2.1.2/pyatlan/model/assets/sigma_dataset_column.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,18 @@
             default=None, description=""
         )
         sigma_dataset_name: Optional[str] = Field(default=None, description="")
         sigma_dataset: Optional[SigmaDataset] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SigmaDatasetColumn.Attributes" = Field(
+    attributes: SigmaDatasetColumn.Attributes = Field(
         default_factory=lambda: SigmaDatasetColumn.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .sigma_dataset import SigmaDataset  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sigma_page.py` & `pyatlan-2.1.2/pyatlan/model/assets/sigma_page.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,16 +92,19 @@
         sigma_data_elements: Optional[List[SigmaDataElement]] = Field(
             default=None, description=""
         )  # relationship
         sigma_workbook: Optional[SigmaWorkbook] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SigmaPage.Attributes" = Field(
+    attributes: SigmaPage.Attributes = Field(
         default_factory=lambda: SigmaPage.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .sigma_data_element import SigmaDataElement  # noqa
 from .sigma_workbook import SigmaWorkbook  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sigma_workbook.py` & `pyatlan-2.1.2/pyatlan/model/assets/sigma_workbook.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,18 @@
 
     class Attributes(Sigma.Attributes):
         sigma_page_count: Optional[int] = Field(default=None, description="")
         sigma_pages: Optional[List[SigmaPage]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SigmaWorkbook.Attributes" = Field(
+    attributes: SigmaWorkbook.Attributes = Field(
         default_factory=lambda: SigmaWorkbook.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .sigma_page import SigmaPage  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sisense.py` & `pyatlan-2.1.2/pyatlan/model/assets/sisense.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sisense_dashboard.py` & `pyatlan-2.1.2/pyatlan/model/assets/sisense_dashboard.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,17 +148,20 @@
         sisense_widgets: Optional[List[SisenseWidget]] = Field(
             default=None, description=""
         )  # relationship
         sisense_folder: Optional[SisenseFolder] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SisenseDashboard.Attributes" = Field(
+    attributes: SisenseDashboard.Attributes = Field(
         default_factory=lambda: SisenseDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .sisense_datamodel import SisenseDatamodel  # noqa
 from .sisense_folder import SisenseFolder  # noqa
 from .sisense_widget import SisenseWidget  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sisense_datamodel.py` & `pyatlan-2.1.2/pyatlan/model/assets/sisense_datamodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -280,16 +280,19 @@
         sisense_datamodel_tables: Optional[List[SisenseDatamodelTable]] = Field(
             default=None, description=""
         )  # relationship
         sisense_dashboards: Optional[List[SisenseDashboard]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SisenseDatamodel.Attributes" = Field(
+    attributes: SisenseDatamodel.Attributes = Field(
         default_factory=lambda: SisenseDatamodel.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .sisense_dashboard import SisenseDashboard  # noqa
 from .sisense_datamodel_table import SisenseDatamodelTable  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sisense_datamodel_table.py` & `pyatlan-2.1.2/pyatlan/model/assets/sisense_datamodel_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -297,16 +297,19 @@
         sisense_datamodel: Optional[SisenseDatamodel] = Field(
             default=None, description=""
         )  # relationship
         sisense_widgets: Optional[List[SisenseWidget]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SisenseDatamodelTable.Attributes" = Field(
+    attributes: SisenseDatamodelTable.Attributes = Field(
         default_factory=lambda: SisenseDatamodelTable.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .sisense_datamodel import SisenseDatamodel  # noqa
 from .sisense_widget import SisenseWidget  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sisense_folder.py` & `pyatlan-2.1.2/pyatlan/model/assets/sisense_folder.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,16 +146,19 @@
         sisense_dashboards: Optional[List[SisenseDashboard]] = Field(
             default=None, description=""
         )  # relationship
         sisense_parent_folder: Optional[SisenseFolder] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SisenseFolder.Attributes" = Field(
+    attributes: SisenseFolder.Attributes = Field(
         default_factory=lambda: SisenseFolder.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .sisense_dashboard import SisenseDashboard  # noqa
 from .sisense_widget import SisenseWidget  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/sisense_widget.py` & `pyatlan-2.1.2/pyatlan/model/assets/sisense_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,17 +221,20 @@
         sisense_folder: Optional[SisenseFolder] = Field(
             default=None, description=""
         )  # relationship
         sisense_dashboard: Optional[SisenseDashboard] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SisenseWidget.Attributes" = Field(
+    attributes: SisenseWidget.Attributes = Field(
         default_factory=lambda: SisenseWidget.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .sisense_dashboard import SisenseDashboard  # noqa
 from .sisense_datamodel_table import SisenseDatamodelTable  # noqa
 from .sisense_folder import SisenseFolder  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/snowflake_dynamic_table.py` & `pyatlan-2.1.2/pyatlan/model/assets/snowflake_dynamic_table.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,12 +47,15 @@
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.definition = definition
 
     class Attributes(Table.Attributes):
         definition: Optional[str] = Field(default=None, description="")
 
-    attributes: "SnowflakeDynamicTable.Attributes" = Field(
+    attributes: SnowflakeDynamicTable.Attributes = Field(
         default_factory=lambda: SnowflakeDynamicTable.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/snowflake_stream.py` & `pyatlan-2.1.2/pyatlan/model/assets/snowflake_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,18 @@
         snowflake_stream_stale_after: Optional[datetime] = Field(
             default=None, description=""
         )
         atlan_schema: Optional[Schema] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SnowflakeStream.Attributes" = Field(
+    attributes: SnowflakeStream.Attributes = Field(
         default_factory=lambda: SnowflakeStream.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .schema import Schema  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/snowflake_tag.py` & `pyatlan-2.1.2/pyatlan/model/assets/snowflake_tag.py`

 * *Files 0% similar despite different names*

```diff
@@ -524,18 +524,21 @@
         dbt_tests: Optional[List[DbtTest]] = Field(
             default=None, description=""
         )  # relationship
         atlan_schema: Optional[Schema] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SnowflakeTag.Attributes" = Field(
+    attributes: SnowflakeTag.Attributes = Field(
         default_factory=lambda: SnowflakeTag.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .dbt_model import DbtModel  # noqa
 from .dbt_source import DbtSource  # noqa
 from .dbt_test import DbtTest  # noqa
 from .schema import Schema  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/soda.py` & `pyatlan-2.1.2/pyatlan/model/assets/soda.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/soda_check.py` & `pyatlan-2.1.2/pyatlan/model/assets/soda_check.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,16 +173,19 @@
         soda_check_columns: Optional[List[Column]] = Field(
             default=None, description=""
         )  # relationship
         soda_check_assets: Optional[List[Asset]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "SodaCheck.Attributes" = Field(
+    attributes: SodaCheck.Attributes = Field(
         default_factory=lambda: SodaCheck.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .asset import Asset  # noqa
 from .column import Column  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/table.py` & `pyatlan-2.1.2/pyatlan/model/assets/table.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,18 @@
     """
     PARTITION_LIST: ClassVar[KeywordField] = KeywordField(
         "partitionList", "partitionList"
     )
     """
     List of partitions in this table.
     """
+    IS_SHARDED: ClassVar[BooleanField] = BooleanField("isSharded", "isSharded")
+    """
+    Whether this table is a sharded table (true) or not (false).
+    """
 
     COLUMNS: ClassVar[RelationField] = RelationField("columns")
     """
     TBC
     """
     FACTS: ClassVar[RelationField] = RelationField("facts")
     """
@@ -175,14 +179,15 @@
         "external_location",
         "external_location_region",
         "external_location_format",
         "is_partitioned",
         "partition_strategy",
         "partition_count",
         "partition_list",
+        "is_sharded",
         "columns",
         "facts",
         "atlan_schema",
         "partitions",
         "queries",
         "dimensions",
     ]
@@ -332,14 +337,24 @@
     @partition_list.setter
     def partition_list(self, partition_list: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_list = partition_list
 
     @property
+    def is_sharded(self) -> Optional[bool]:
+        return None if self.attributes is None else self.attributes.is_sharded
+
+    @is_sharded.setter
+    def is_sharded(self, is_sharded: Optional[bool]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.is_sharded = is_sharded
+
+    @property
     def columns(self) -> Optional[List[Column]]:
         return None if self.attributes is None else self.attributes.columns
 
     @columns.setter
     def columns(self, columns: Optional[List[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
@@ -408,14 +423,15 @@
         external_location: Optional[str] = Field(default=None, description="")
         external_location_region: Optional[str] = Field(default=None, description="")
         external_location_format: Optional[str] = Field(default=None, description="")
         is_partitioned: Optional[bool] = Field(default=None, description="")
         partition_strategy: Optional[str] = Field(default=None, description="")
         partition_count: Optional[int] = Field(default=None, description="")
         partition_list: Optional[str] = Field(default=None, description="")
+        is_sharded: Optional[bool] = Field(default=None, description="")
         columns: Optional[List[Column]] = Field(
             default=None, description=""
         )  # relationship
         facts: Optional[List[Table]] = Field(
             default=None, description=""
         )  # relationship
         atlan_schema: Optional[Schema] = Field(
@@ -452,18 +468,21 @@
                 qualified_name=f"{schema_qualified_name}/{name}",
                 schema_qualified_name=schema_qualified_name,
                 schema_name=fields[4],
                 connector_name=connector_type.value,
                 atlan_schema=Schema.ref_by_qualified_name(schema_qualified_name),
             )
 
-    attributes: "Table.Attributes" = Field(
+    attributes: Table.Attributes = Field(
         default_factory=lambda: Table.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .column import Column  # noqa
 from .query import Query  # noqa
 from .schema import Schema  # noqa
 from .table_partition import TablePartition  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/table_partition.py` & `pyatlan-2.1.2/pyatlan/model/assets/table_partition.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,31 +109,31 @@
     PARTITION_LIST: ClassVar[KeywordField] = KeywordField(
         "partitionList", "partitionList"
     )
     """
     List of sub-partitions in this partition.
     """
 
-    CHILD_TABLE_PARTITIONS: ClassVar[RelationField] = RelationField(
-        "childTablePartitions"
-    )
+    COLUMNS: ClassVar[RelationField] = RelationField("columns")
     """
     TBC
     """
-    COLUMNS: ClassVar[RelationField] = RelationField("columns")
+    PARENT_TABLE: ClassVar[RelationField] = RelationField("parentTable")
     """
     TBC
     """
-    PARENT_TABLE_PARTITION: ClassVar[RelationField] = RelationField(
-        "parentTablePartition"
+    CHILD_TABLE_PARTITIONS: ClassVar[RelationField] = RelationField(
+        "childTablePartitions"
     )
     """
     TBC
     """
-    PARENT_TABLE: ClassVar[RelationField] = RelationField("parentTable")
+    PARENT_TABLE_PARTITION: ClassVar[RelationField] = RelationField(
+        "parentTablePartition"
+    )
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
         "constraint",
         "column_count",
@@ -146,18 +146,18 @@
         "external_location",
         "external_location_region",
         "external_location_format",
         "is_partitioned",
         "partition_strategy",
         "partition_count",
         "partition_list",
-        "child_table_partitions",
         "columns",
-        "parent_table_partition",
         "parent_table",
+        "child_table_partitions",
+        "parent_table_partition",
     ]
 
     @property
     def constraint(self) -> Optional[str]:
         return None if self.attributes is None else self.attributes.constraint
 
     @constraint.setter
@@ -311,59 +311,59 @@
     @partition_list.setter
     def partition_list(self, partition_list: Optional[str]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.partition_list = partition_list
 
     @property
+    def columns(self) -> Optional[List[Column]]:
+        return None if self.attributes is None else self.attributes.columns
+
+    @columns.setter
+    def columns(self, columns: Optional[List[Column]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.columns = columns
+
+    @property
+    def parent_table(self) -> Optional[Table]:
+        return None if self.attributes is None else self.attributes.parent_table
+
+    @parent_table.setter
+    def parent_table(self, parent_table: Optional[Table]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.parent_table = parent_table
+
+    @property
     def child_table_partitions(self) -> Optional[List[TablePartition]]:
         return (
             None if self.attributes is None else self.attributes.child_table_partitions
         )
 
     @child_table_partitions.setter
     def child_table_partitions(
         self, child_table_partitions: Optional[List[TablePartition]]
     ):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.child_table_partitions = child_table_partitions
 
     @property
-    def columns(self) -> Optional[List[Column]]:
-        return None if self.attributes is None else self.attributes.columns
-
-    @columns.setter
-    def columns(self, columns: Optional[List[Column]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.columns = columns
-
-    @property
     def parent_table_partition(self) -> Optional[TablePartition]:
         return (
             None if self.attributes is None else self.attributes.parent_table_partition
         )
 
     @parent_table_partition.setter
     def parent_table_partition(self, parent_table_partition: Optional[TablePartition]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.parent_table_partition = parent_table_partition
 
-    @property
-    def parent_table(self) -> Optional[Table]:
-        return None if self.attributes is None else self.attributes.parent_table
-
-    @parent_table.setter
-    def parent_table(self, parent_table: Optional[Table]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.parent_table = parent_table
-
     class Attributes(SQL.Attributes):
         constraint: Optional[str] = Field(default=None, description="")
         column_count: Optional[int] = Field(default=None, description="")
         row_count: Optional[int] = Field(default=None, description="")
         size_bytes: Optional[int] = Field(default=None, description="")
         alias: Optional[str] = Field(default=None, description="")
         is_temporary: Optional[bool] = Field(default=None, description="")
@@ -374,29 +374,32 @@
         external_location: Optional[str] = Field(default=None, description="")
         external_location_region: Optional[str] = Field(default=None, description="")
         external_location_format: Optional[str] = Field(default=None, description="")
         is_partitioned: Optional[bool] = Field(default=None, description="")
         partition_strategy: Optional[str] = Field(default=None, description="")
         partition_count: Optional[int] = Field(default=None, description="")
         partition_list: Optional[str] = Field(default=None, description="")
-        child_table_partitions: Optional[List[TablePartition]] = Field(
+        columns: Optional[List[Column]] = Field(
             default=None, description=""
         )  # relationship
-        columns: Optional[List[Column]] = Field(
+        parent_table: Optional[Table] = Field(
             default=None, description=""
         )  # relationship
-        parent_table_partition: Optional[TablePartition] = Field(
+        child_table_partitions: Optional[List[TablePartition]] = Field(
             default=None, description=""
         )  # relationship
-        parent_table: Optional[Table] = Field(
+        parent_table_partition: Optional[TablePartition] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "TablePartition.Attributes" = Field(
+    attributes: TablePartition.Attributes = Field(
         default_factory=lambda: TablePartition.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .column import Column  # noqa
 from .table import Table  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tableau.py` & `pyatlan-2.1.2/pyatlan/model/assets/tableau.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tableau_calculated_field.py` & `pyatlan-2.1.2/pyatlan/model/assets/tableau_calculated_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,16 +286,19 @@
         worksheets: Optional[List[TableauWorksheet]] = Field(
             default=None, description=""
         )  # relationship
         datasource: Optional[TableauDatasource] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "TableauCalculatedField.Attributes" = Field(
+    attributes: TableauCalculatedField.Attributes = Field(
         default_factory=lambda: TableauCalculatedField.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .tableau_datasource import TableauDatasource  # noqa
 from .tableau_worksheet import TableauWorksheet  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tableau_dashboard.py` & `pyatlan-2.1.2/pyatlan/model/assets/tableau_dashboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -174,16 +174,19 @@
         workbook: Optional[TableauWorkbook] = Field(
             default=None, description=""
         )  # relationship
         worksheets: Optional[List[TableauWorksheet]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "TableauDashboard.Attributes" = Field(
+    attributes: TableauDashboard.Attributes = Field(
         default_factory=lambda: TableauDashboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .tableau_workbook import TableauWorkbook  # noqa
 from .tableau_worksheet import TableauWorksheet  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tableau_datasource.py` & `pyatlan-2.1.2/pyatlan/model/assets/tableau_datasource.py`

 * *Files 0% similar despite different names*

```diff
@@ -336,17 +336,20 @@
         project: Optional[TableauProject] = Field(
             default=None, description=""
         )  # relationship
         fields: Optional[List[TableauDatasourceField]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "TableauDatasource.Attributes" = Field(
+    attributes: TableauDatasource.Attributes = Field(
         default_factory=lambda: TableauDatasource.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .tableau_datasource_field import TableauDatasourceField  # noqa
 from .tableau_project import TableauProject  # noqa
 from .tableau_workbook import TableauWorkbook  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tableau_datasource_field.py` & `pyatlan-2.1.2/pyatlan/model/assets/tableau_datasource_field.py`

 * *Files 0% similar despite different names*

```diff
@@ -438,16 +438,19 @@
         worksheets: Optional[List[TableauWorksheet]] = Field(
             default=None, description=""
         )  # relationship
         datasource: Optional[TableauDatasource] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "TableauDatasourceField.Attributes" = Field(
+    attributes: TableauDatasourceField.Attributes = Field(
         default_factory=lambda: TableauDatasourceField.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .tableau_datasource import TableauDatasource  # noqa
 from .tableau_worksheet import TableauWorksheet  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tableau_flow.py` & `pyatlan-2.1.2/pyatlan/model/assets/tableau_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -190,15 +190,18 @@
         output_steps: Optional[List[Dict[str, str]]] = Field(
             default=None, description=""
         )
         project: Optional[TableauProject] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "TableauFlow.Attributes" = Field(
+    attributes: TableauFlow.Attributes = Field(
         default_factory=lambda: TableauFlow.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .tableau_project import TableauProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tableau_metric.py` & `pyatlan-2.1.2/pyatlan/model/assets/tableau_metric.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,15 +136,18 @@
         project_hierarchy: Optional[List[Dict[str, str]]] = Field(
             default=None, description=""
         )
         project: Optional[TableauProject] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "TableauMetric.Attributes" = Field(
+    attributes: TableauMetric.Attributes = Field(
         default_factory=lambda: TableauMetric.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .tableau_project import TableauProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tableau_project.py` & `pyatlan-2.1.2/pyatlan/model/assets/tableau_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,18 +224,21 @@
         flows: Optional[List[TableauFlow]] = Field(
             default=None, description=""
         )  # relationship
         child_projects: Optional[List[TableauProject]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "TableauProject.Attributes" = Field(
+    attributes: TableauProject.Attributes = Field(
         default_factory=lambda: TableauProject.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .tableau_datasource import TableauDatasource  # noqa
 from .tableau_flow import TableauFlow  # noqa
 from .tableau_site import TableauSite  # noqa
 from .tableau_workbook import TableauWorkbook  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tableau_site.py` & `pyatlan-2.1.2/pyatlan/model/assets/tableau_site.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,15 +49,18 @@
         self.attributes.projects = projects
 
     class Attributes(Tableau.Attributes):
         projects: Optional[List[TableauProject]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "TableauSite.Attributes" = Field(
+    attributes: TableauSite.Attributes = Field(
         default_factory=lambda: TableauSite.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .tableau_project import TableauProject  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tableau_workbook.py` & `pyatlan-2.1.2/pyatlan/model/assets/tableau_workbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,18 +210,21 @@
         worksheets: Optional[List[TableauWorksheet]] = Field(
             default=None, description=""
         )  # relationship
         datasources: Optional[List[TableauDatasource]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "TableauWorkbook.Attributes" = Field(
+    attributes: TableauWorkbook.Attributes = Field(
         default_factory=lambda: TableauWorkbook.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .tableau_dashboard import TableauDashboard  # noqa
 from .tableau_datasource import TableauDatasource  # noqa
 from .tableau_project import TableauProject  # noqa
 from .tableau_worksheet import TableauWorksheet  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tableau_worksheet.py` & `pyatlan-2.1.2/pyatlan/model/assets/tableau_worksheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,18 +214,21 @@
         calculated_fields: Optional[List[TableauCalculatedField]] = Field(
             default=None, description=""
         )  # relationship
         dashboards: Optional[List[TableauDashboard]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "TableauWorksheet.Attributes" = Field(
+    attributes: TableauWorksheet.Attributes = Field(
         default_factory=lambda: TableauWorksheet.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .tableau_calculated_field import TableauCalculatedField  # noqa
 from .tableau_dashboard import TableauDashboard  # noqa
 from .tableau_datasource_field import TableauDatasourceField  # noqa
 from .tableau_workbook import TableauWorkbook  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tag.py` & `pyatlan-2.1.2/pyatlan/model/assets/tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,12 +106,15 @@
         tag_id: Optional[str] = Field(default=None, description="")
         tag_attributes: Optional[List[SourceTagAttribute]] = Field(
             default=None, description=""
         )
         tag_allowed_values: Optional[Set[str]] = Field(default=None, description="")
         mapped_atlan_tag_name: Optional[str] = Field(default=None, description="")
 
-    attributes: "Tag.Attributes" = Field(
+    attributes: Tag.Attributes = Field(
         default_factory=lambda: Tag.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/tag_attachment.py` & `pyatlan-2.1.2/pyatlan/model/assets/tag_attachment.py`

 * *Files 12% similar despite different names*

```diff
@@ -73,12 +73,15 @@
             self.attributes = self.Attributes()
         self.attributes.tag_attachment_string_value = tag_attachment_string_value
 
     class Attributes(Asset.Attributes):
         tag_qualified_name: Optional[str] = Field(default=None, description="")
         tag_attachment_string_value: Optional[str] = Field(default=None, description="")
 
-    attributes: "TagAttachment.Attributes" = Field(
+    attributes: TagAttachment.Attributes = Field(
         default_factory=lambda: TagAttachment.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/thoughtspot.py` & `pyatlan-2.1.2/pyatlan/model/assets/thoughtspot.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,12 +115,15 @@
 
     class Attributes(BI.Attributes):
         thoughtspot_chart_type: Optional[str] = Field(default=None, description="")
         thoughtspot_question_text: Optional[str] = Field(default=None, description="")
         thoughtspot_join_count: Optional[int] = Field(default=None, description="")
         thoughtspot_column_count: Optional[int] = Field(default=None, description="")
 
-    attributes: "Thoughtspot.Attributes" = Field(
+    attributes: Thoughtspot.Attributes = Field(
         default_factory=lambda: Thoughtspot.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_answer.py` & `pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_answer.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_column.py` & `pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_column.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,17 +230,20 @@
         thoughtspot_view: Optional[ThoughtspotView] = Field(
             default=None, description=""
         )  # relationship
         thoughtspot_worksheet: Optional[ThoughtspotWorksheet] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "ThoughtspotColumn.Attributes" = Field(
+    attributes: ThoughtspotColumn.Attributes = Field(
         default_factory=lambda: ThoughtspotColumn.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .thoughtspot_table import ThoughtspotTable  # noqa
 from .thoughtspot_view import ThoughtspotView  # noqa
 from .thoughtspot_worksheet import ThoughtspotWorksheet  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_dashlet.py` & `pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_dashlet.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,18 @@
         thoughtspot_liveboard_qualified_name: Optional[str] = Field(
             default=None, description=""
         )
         thoughtspot_liveboard: Optional[ThoughtspotLiveboard] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "ThoughtspotDashlet.Attributes" = Field(
+    attributes: ThoughtspotDashlet.Attributes = Field(
         default_factory=lambda: ThoughtspotDashlet.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .thoughtspot_liveboard import ThoughtspotLiveboard  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_liveboard.py` & `pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_liveboard.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,18 @@
         self.attributes.thoughtspot_dashlets = thoughtspot_dashlets
 
     class Attributes(Thoughtspot.Attributes):
         thoughtspot_dashlets: Optional[List[ThoughtspotDashlet]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "ThoughtspotLiveboard.Attributes" = Field(
+    attributes: ThoughtspotLiveboard.Attributes = Field(
         default_factory=lambda: ThoughtspotLiveboard.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .thoughtspot_dashlet import ThoughtspotDashlet  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_table.py` & `pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_table.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,18 @@
         self.attributes.thoughtspot_columns = thoughtspot_columns
 
     class Attributes(Thoughtspot.Attributes):
         thoughtspot_columns: Optional[List[ThoughtspotColumn]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "ThoughtspotTable.Attributes" = Field(
+    attributes: ThoughtspotTable.Attributes = Field(
         default_factory=lambda: ThoughtspotTable.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .thoughtspot_column import ThoughtspotColumn  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_view.py` & `pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_view.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,15 +51,18 @@
         self.attributes.thoughtspot_columns = thoughtspot_columns
 
     class Attributes(Thoughtspot.Attributes):
         thoughtspot_columns: Optional[List[ThoughtspotColumn]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "ThoughtspotView.Attributes" = Field(
+    attributes: ThoughtspotView.Attributes = Field(
         default_factory=lambda: ThoughtspotView.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .thoughtspot_column import ThoughtspotColumn  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/thoughtspot_worksheet.py` & `pyatlan-2.1.2/pyatlan/model/assets/thoughtspot_worksheet.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,18 @@
         self.attributes.thoughtspot_columns = thoughtspot_columns
 
     class Attributes(Thoughtspot.Attributes):
         thoughtspot_columns: Optional[List[ThoughtspotColumn]] = Field(
             default=None, description=""
         )  # relationship
 
-    attributes: "ThoughtspotWorksheet.Attributes" = Field(
+    attributes: ThoughtspotWorksheet.Attributes = Field(
         default_factory=lambda: ThoughtspotWorksheet.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .thoughtspot_column import ThoughtspotColumn  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/assets/view.py` & `pyatlan-2.1.2/pyatlan/model/assets/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,35 +101,35 @@
     SQL definition of this view.
     """
 
     COLUMNS: ClassVar[RelationField] = RelationField("columns")
     """
     TBC
     """
-    QUERIES: ClassVar[RelationField] = RelationField("queries")
+    ATLAN_SCHEMA: ClassVar[RelationField] = RelationField("atlanSchema")
     """
     TBC
     """
-    ATLAN_SCHEMA: ClassVar[RelationField] = RelationField("atlanSchema")
+    QUERIES: ClassVar[RelationField] = RelationField("queries")
     """
     TBC
     """
 
     _convenience_properties: ClassVar[List[str]] = [
         "column_count",
         "row_count",
         "size_bytes",
         "is_query_preview",
         "query_preview_config",
         "alias",
         "is_temporary",
         "definition",
         "columns",
-        "queries",
         "atlan_schema",
+        "queries",
     ]
 
     @property
     def column_count(self) -> Optional[int]:
         return None if self.attributes is None else self.attributes.column_count
 
     @column_count.setter
@@ -215,51 +215,51 @@
     @columns.setter
     def columns(self, columns: Optional[List[Column]]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.columns = columns
 
     @property
-    def queries(self) -> Optional[List[Query]]:
-        return None if self.attributes is None else self.attributes.queries
-
-    @queries.setter
-    def queries(self, queries: Optional[List[Query]]):
-        if self.attributes is None:
-            self.attributes = self.Attributes()
-        self.attributes.queries = queries
-
-    @property
     def atlan_schema(self) -> Optional[Schema]:
         return None if self.attributes is None else self.attributes.atlan_schema
 
     @atlan_schema.setter
     def atlan_schema(self, atlan_schema: Optional[Schema]):
         if self.attributes is None:
             self.attributes = self.Attributes()
         self.attributes.atlan_schema = atlan_schema
 
+    @property
+    def queries(self) -> Optional[List[Query]]:
+        return None if self.attributes is None else self.attributes.queries
+
+    @queries.setter
+    def queries(self, queries: Optional[List[Query]]):
+        if self.attributes is None:
+            self.attributes = self.Attributes()
+        self.attributes.queries = queries
+
     class Attributes(SQL.Attributes):
         column_count: Optional[int] = Field(default=None, description="")
         row_count: Optional[int] = Field(default=None, description="")
         size_bytes: Optional[int] = Field(default=None, description="")
         is_query_preview: Optional[bool] = Field(default=None, description="")
         query_preview_config: Optional[Dict[str, str]] = Field(
             default=None, description=""
         )
         alias: Optional[str] = Field(default=None, description="")
         is_temporary: Optional[bool] = Field(default=None, description="")
         definition: Optional[str] = Field(default=None, description="")
         columns: Optional[List[Column]] = Field(
             default=None, description=""
         )  # relationship
-        queries: Optional[List[Query]] = Field(
+        atlan_schema: Optional[Schema] = Field(
             default=None, description=""
         )  # relationship
-        atlan_schema: Optional[Schema] = Field(
+        queries: Optional[List[Query]] = Field(
             default=None, description=""
         )  # relationship
 
         @classmethod
         @init_guid
         def create(cls, *, name: str, schema_qualified_name: str) -> View.Attributes:
             if not name:
@@ -280,17 +280,20 @@
                 qualified_name=f"{schema_qualified_name}/{name}",
                 schema_qualified_name=schema_qualified_name,
                 schema_name=fields[4],
                 connector_name=connector_type.value,
                 atlan_schema=Schema.ref_by_qualified_name(schema_qualified_name),
             )
 
-    attributes: "View.Attributes" = Field(
+    attributes: View.Attributes = Field(
         default_factory=lambda: View.Attributes(),
-        description="Map of attributes in the instance and their values. The specific keys of this map will vary by "
-        "type, so are described in the sub-types of this schema.\n",
+        description=(
+            "Map of attributes in the instance and their values. "
+            "The specific keys of this map will vary by type, "
+            "so are described in the sub-types of this schema."
+        ),
     )
 
 
 from .column import Column  # noqa
 from .query import Query  # noqa
 from .schema import Schema  # noqa
```

### Comparing `pyatlan-2.1.1/pyatlan/model/atlan_image.py` & `pyatlan-2.1.2/pyatlan/model/atlan_image.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/audit.py` & `pyatlan-2.1.2/pyatlan/model/audit.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/core.py` & `pyatlan-2.1.2/pyatlan/model/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,21 +170,21 @@
     propagate: Optional[bool] = Field(default=None, description="")
     remove_propagations_on_entity_delete: Optional[bool] = Field(
         default=None, description="", alias="removePropagationsOnEntityDelete"
     )
     restrict_propagation_through_lineage: Optional[bool] = Field(
         default=None, description="", alias="restrictPropagationThroughLineage"
     )
-    propagation_only_through_lineage: Optional[bool] = Field(
+    restrict_propagation_through_hierarchy: Optional[bool] = Field(
         default=None,
         description=(
-            "If specified as `True`, propagation will only "
-            "occur downstream lineage and not within hierarchy."
+            "Whether to prevent this Atlan tag from propagating through "
+            "hierarchy (True) or allow it to propagate through hierarchy (False)"
         ),
-        alias="propagationOnlyThroughLineage",
+        alias="restrictPropagationThroughHierachy",
     )
     validity_periods: Optional[List[str]] = Field(default=None, alias="validityPeriods")
     _source_tag_attachements: List[SourceTagAttachment] = PrivateAttr(
         default_factory=list
     )
 
     attributes: Optional[Dict[str, Any]] = None
```

### Comparing `pyatlan-2.1.1/pyatlan/model/credential.py` & `pyatlan-2.1.2/pyatlan/model/credential.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/custom_metadata.py` & `pyatlan-2.1.2/pyatlan/model/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/data_mesh.py` & `pyatlan-2.1.2/pyatlan/model/data_mesh.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/enums.py` & `pyatlan-2.1.2/pyatlan/model/enums.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,14 +276,15 @@
     SOFT = "SOFT"
     PURGE = "PURGE"
 
 
 class AtlanIcon(str, Enum):
     ATLAN_TAG = "atlanTags"
     ATLAN_SHIELD = "atlanShield"
+    ATLAN_METADATA = "atlanMetadata"
     ADDRESS_BOOK = "PhAddressBook"
     AIR_TRAFFIC_CONTROL = "PhAirTrafficControl"
     AIRPLANE = "PhAirplane"
     AIRPLANE_IN_FLIGHT = "PhAirplaneInFlight"
     AIRPLANE_LANDING = "PhAirplaneLanding"
     AIRPLANE_TAKEOFF = "PhAirplaneTakeoff"
     AIRPLANE_TILT = "PhAirplaneTilt"
```

### Comparing `pyatlan-2.1.1/pyatlan/model/events.py` & `pyatlan-2.1.2/pyatlan/model/events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/fields/atlan_fields.py` & `pyatlan-2.1.2/pyatlan/model/fields/atlan_fields.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/fluent_search.py` & `pyatlan-2.1.2/pyatlan/model/fluent_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/fluent_tasks.py` & `pyatlan-2.1.2/pyatlan/model/fluent_tasks.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/group.py` & `pyatlan-2.1.2/pyatlan/model/group.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/keycloak_events.py` & `pyatlan-2.1.2/pyatlan/model/keycloak_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/lineage.py` & `pyatlan-2.1.2/pyatlan/model/lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/packages/base/crawler.py` & `pyatlan-2.1.2/pyatlan/model/packages/base/crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/packages/base/package.py` & `pyatlan-2.1.2/pyatlan/model/packages/base/package.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/packages/confluent_kafka_crawler.py` & `pyatlan-2.1.2/pyatlan/model/packages/confluent_kafka_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/packages/dbt_crawler.py` & `pyatlan-2.1.2/pyatlan/model/packages/dbt_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/packages/glue_crawler.py` & `pyatlan-2.1.2/pyatlan/model/packages/glue_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/packages/powerbi_crawler.py` & `pyatlan-2.1.2/pyatlan/model/packages/powerbi_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/packages/sigma_crawler.py` & `pyatlan-2.1.2/pyatlan/model/packages/sigma_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/packages/snowflake_crawler.py` & `pyatlan-2.1.2/pyatlan/model/packages/snowflake_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/packages/sql_server_crawler.py` & `pyatlan-2.1.2/pyatlan/model/packages/sql_server_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/packages/tableau_crawler.py` & `pyatlan-2.1.2/pyatlan/model/packages/tableau_crawler.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/query.py` & `pyatlan-2.1.2/pyatlan/model/query.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/response.py` & `pyatlan-2.1.2/pyatlan/model/response.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/role.py` & `pyatlan-2.1.2/pyatlan/model/role.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/search.py` & `pyatlan-2.1.2/pyatlan/model/search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/search_log.py` & `pyatlan-2.1.2/pyatlan/model/search_log.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/structs.py` & `pyatlan-2.1.2/pyatlan/model/structs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-# Copyright 2022 Atlan Pte. Ltd.
+# SPDX-License-Identifier: Apache-2.0
+# Copyright 2024 Atlan Pte. Ltd.
+
 from __future__ import annotations
 
 from datetime import datetime
-from typing import Dict, List, Optional, Set, Union
+from typing import Any, Dict, List, Optional, Set, Union
 
-from pydantic.v1 import BaseModel, Extra, Field
+from pydantic.v1 import BaseModel, Extra, Field, root_validator
 
 from pyatlan.model.enums import (
     BadgeComparisonOperator,
     BadgeConditionColor,
     SourceCostUnitType,
 )
 from pyatlan.model.utils import to_camel_case
@@ -19,14 +21,26 @@
     class Config:
         allow_population_by_field_name = True
         alias_generator = to_camel_case
         extra = Extra.ignore
         json_encoders = {datetime: lambda v: int(v.timestamp() * 1000)}
         validate_assignment = True
 
+    @root_validator(pre=True)
+    def flatten_structs_attributes(cls, values: Dict[str, Any]) -> Dict[str, Any]:
+        """
+        Flatten the 'attributes' of the struct models.
+
+        :param values: dictionary containing the attributes.
+        :returns: modified dictionary with attributes flattened.
+        """
+        attributes = values.pop("attributes", {})
+        values = {**values, **attributes}
+        return values
+
 
 class MCRuleSchedule(AtlanObject):
     """Description"""
 
     mc_rule_schedule_type: Optional[str] = Field(default=None, description="")
     mc_rule_schedule_interval_in_minutes: Optional[int] = Field(
         default=None, description=""
```

### Comparing `pyatlan-2.1.1/pyatlan/model/task.py` & `pyatlan-2.1.2/pyatlan/model/task.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/typedef.py` & `pyatlan-2.1.2/pyatlan/model/typedef.py`

 * *Files 0% similar despite different names*

```diff
@@ -708,14 +708,19 @@
 
     @staticmethod
     def create(
         display_name: str,
         attribute_type: AtlanCustomAttributePrimitiveType,
         multi_valued: bool = False,
         options_name: Optional[str] = None,
+        applicable_connections: Optional[Set[str]] = None,
+        applicable_asset_types: Optional[Set[str]] = None,
+        applicable_glossaries: Optional[Set[str]] = None,
+        applicable_glossary_types: Optional[Set[str]] = None,
+        applicable_other_asset_types: Optional[Set[str]] = None,
     ) -> AttributeDef:
         from pyatlan.utils import validate_required_fields
 
         validate_required_fields(
             ["display_name", "attribute_type"],
             [display_name, attribute_type],
         )
@@ -756,19 +761,28 @@
         if add_enum_values:
             from pyatlan.cache.enum_cache import EnumCache
 
             if enum_def := EnumCache.get_by_name(str(options_name)):
                 attr_def.enum_values = enum_def.get_valid_values()
             else:
                 attr_def.enum_values = []
-        attr_def.applicable_asset_types = _complete_type_list
-        attr_def.applicable_glossary_types = _all_glossary_types
-        attr_def.applicable_other_asset_types = _all_other_types
-        attr_def.applicable_connections = _get_all_qualified_names("Connection")
-        attr_def.applicable_glossaries = _get_all_qualified_names("AtlasGlossary")
+
+        attr_def.applicable_asset_types = applicable_asset_types or _complete_type_list
+        attr_def.applicable_glossary_types = (
+            applicable_glossary_types or _all_glossary_types
+        )
+        attr_def.applicable_other_asset_types = (
+            applicable_other_asset_types or _all_other_types
+        )
+        attr_def.applicable_connections = (
+            applicable_connections or _get_all_qualified_names("Connection")
+        )
+        attr_def.applicable_glossaries = (
+            applicable_glossaries or _get_all_qualified_names("AtlasGlossary")
+        )
         return attr_def
 
     def is_archived(self) -> bool:
         return bool(opt.is_archived) if (opt := self.options) else False
 
     def archive(self, by: str) -> AttributeDef:
         if self.options:
```

### Comparing `pyatlan-2.1.1/pyatlan/model/user.py` & `pyatlan-2.1.2/pyatlan/model/user.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/utils.py` & `pyatlan-2.1.2/pyatlan/model/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/model/workflow.py` & `pyatlan-2.1.2/pyatlan/model/workflow.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/multipart_data_generator.py` & `pyatlan-2.1.2/pyatlan/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/pkg/create_package_files.py` & `pyatlan-2.1.2/pyatlan/pkg/create_package_files.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/pkg/models.py` & `pyatlan-2.1.2/pyatlan/pkg/models.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/pkg/templates/default_configmap.jinja2` & `pyatlan-2.1.2/pyatlan/pkg/templates/default_configmap.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/pkg/templates/default_template.jinja2` & `pyatlan-2.1.2/pyatlan/pkg/templates/default_template.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/pkg/templates/package_config.jinja2` & `pyatlan-2.1.2/pyatlan/pkg/templates/package_config.jinja2`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/pkg/ui.py` & `pyatlan-2.1.2/pyatlan/pkg/ui.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/pkg/utils.py` & `pyatlan-2.1.2/pyatlan/pkg/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/pkg/widgets.py` & `pyatlan-2.1.2/pyatlan/pkg/widgets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/pyatlan/utils.py` & `pyatlan-2.1.2/pyatlan/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -322,51 +322,14 @@
         if isinstance(_type, tuple)
         else _type.__name__
     )
 
     raise ErrorCode.INVALID_PARAMETER_TYPE.exception_with_parameters(name, type_name)
 
 
-def move_struct(data):
-    struct_names = {
-        "sourceQueryComputeCostRecordList",
-        "sourceReadExpensiveQueryRecordList",
-        "sourceReadPopularQueryRecordList",
-        "sourceReadRecentUserRecordList",
-        "sourceReadSlowQueryRecordList",
-        "sourceReadTopUserRecordList",
-        "mcMonitorRuleScheduleConfig",
-        "columnHistogram",
-        "kafkaConsumerGroupTopicConsumptionProperties",
-        "columnTopValues",
-        "badgeConditions",
-        "azureTags",
-        "starredDetailsList",
-        "policyConditions",
-        "awsTags",
-        "dbtMetricFilters",
-        "google_tags",
-        "policyValiditySchedule",
-        "mcMonitorRuleComparisons",
-        "googleLabels",
-        "tagAttributes",
-    }
-    for struct_name in struct_names:
-        if (a := data.get("attributes", None)) and (s := a.get(struct_name, None)):
-            if isinstance(s, list):
-                records = [
-                    record if "attributes" not in record else record["attributes"]
-                    for record in s
-                ]
-                a[struct_name] = records
-            elif isinstance(s, dict):
-                if "attributes" in s:
-                    a[struct_name] = s["attributes"]
-
-
 class AuthorizationFilter(logging.Filter):
     """
     A Filter that will replace the authorization header with the text '***REDACTED***'
     """
 
     def filter(self, record: logging.LogRecord) -> bool:
         if record.args and hasattr(record.args, "__iter__"):
```

### Comparing `pyatlan-2.1.1/pyatlan.egg-info/PKG-INFO` & `pyatlan-2.1.2/pyatlan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyatlan
-Version: 2.1.1
+Version: 2.1.2
 Summary: Atlan Python Client
 Home-page: https://github.com/atlanhq/atlan-python
 Author: Atlan Technologies Pvt Ltd
 Author-email: engineering@atlan.com
 License: Apache LICENSE 2.0
 Keywords: atlan client
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `pyatlan-2.1.1/pyatlan.egg-info/SOURCES.txt` & `pyatlan-2.1.2/pyatlan.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -113,18 +113,29 @@
 pyatlan/model/assets/azure_event_hub_consumer_group.py
 pyatlan/model/assets/b_i.py
 pyatlan/model/assets/b_i_process.py
 pyatlan/model/assets/badge.py
 pyatlan/model/assets/calculation_view.py
 pyatlan/model/assets/catalog.py
 pyatlan/model/assets/cloud.py
+pyatlan/model/assets/cognite.py
+pyatlan/model/assets/cognite3_d_model.py
+pyatlan/model/assets/cognite_asset.py
+pyatlan/model/assets/cognite_event.py
+pyatlan/model/assets/cognite_file.py
+pyatlan/model/assets/cognite_sequence.py
+pyatlan/model/assets/cognite_time_series.py
 pyatlan/model/assets/collection.py
 pyatlan/model/assets/column.py
 pyatlan/model/assets/column_process.py
 pyatlan/model/assets/connection.py
+pyatlan/model/assets/cube.py
+pyatlan/model/assets/cube_dimension.py
+pyatlan/model/assets/cube_field.py
+pyatlan/model/assets/cube_hierarchy.py
 pyatlan/model/assets/data_domain.py
 pyatlan/model/assets/data_mesh.py
 pyatlan/model/assets/data_product.py
 pyatlan/model/assets/data_quality.py
 pyatlan/model/assets/data_set.py
 pyatlan/model/assets/data_studio.py
 pyatlan/model/assets/data_studio_asset.py
@@ -202,14 +213,15 @@
 pyatlan/model/assets/mode_query.py
 pyatlan/model/assets/mode_report.py
 pyatlan/model/assets/mode_workspace.py
 pyatlan/model/assets/mongo_d_b.py
 pyatlan/model/assets/mongo_d_b_collection.py
 pyatlan/model/assets/mongo_d_b_database.py
 pyatlan/model/assets/monte_carlo.py
+pyatlan/model/assets/multi_dimensional_dataset.py
 pyatlan/model/assets/namespace.py
 pyatlan/model/assets/no_s_q_l.py
 pyatlan/model/assets/object_store.py
 pyatlan/model/assets/persona.py
 pyatlan/model/assets/power_b_i.py
 pyatlan/model/assets/power_b_i_column.py
 pyatlan/model/assets/power_b_i_dashboard.py
@@ -284,14 +296,16 @@
 pyatlan/model/assets/sisense_widget.py
 pyatlan/model/assets/snowflake_dynamic_table.py
 pyatlan/model/assets/snowflake_pipe.py
 pyatlan/model/assets/snowflake_stream.py
 pyatlan/model/assets/snowflake_tag.py
 pyatlan/model/assets/soda.py
 pyatlan/model/assets/soda_check.py
+pyatlan/model/assets/spark.py
+pyatlan/model/assets/spark_job.py
 pyatlan/model/assets/table.py
 pyatlan/model/assets/table_partition.py
 pyatlan/model/assets/tableau.py
 pyatlan/model/assets/tableau_calculated_field.py
 pyatlan/model/assets/tableau_dashboard.py
 pyatlan/model/assets/tableau_datasource.py
 pyatlan/model/assets/tableau_datasource_field.py
@@ -377,14 +391,15 @@
 tests/unit/test_events.py
 tests/unit/test_glossary_term.py
 tests/unit/test_lineage.py
 tests/unit/test_model.py
 tests/unit/test_packages.py
 tests/unit/test_query_client.py
 tests/unit/test_search_model.py
+tests/unit/test_structs.py
 tests/unit/test_task_client.py
 tests/unit/test_typedef_model.py
 tests/unit/test_utils.py
 tests/unit/test_workflow_client.py
 tests/unit/model/__init__.py
 tests/unit/model/a_d_l_s_account_test.py
 tests/unit/model/a_d_l_s_container_test.py
```

### Comparing `pyatlan-2.1.1/setup.py` & `pyatlan-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/adls_asset_test.py` & `pyatlan-2.1.2/tests/integration/adls_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/admin_test.py` & `pyatlan-2.1.2/tests/integration/admin_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/api_asset_test.py` & `pyatlan-2.1.2/tests/integration/api_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/atlan_tag_test.py` & `pyatlan-2.1.2/tests/integration/atlan_tag_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/client.py` & `pyatlan-2.1.2/tests/integration/client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/connection_test.py` & `pyatlan-2.1.2/tests/integration/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/custom_metadata_test.py` & `pyatlan-2.1.2/tests/integration/custom_metadata_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 # SPDX-License-Identifier: Apache-2.0
 # Copyright 2022 Atlan Pte. Ltd.
+import json
 import time
 from typing import Generator, List, Optional, Tuple
 
 import pytest
 
 from pyatlan.cache.custom_metadata_cache import CustomMetadataCache
 from pyatlan.client.atlan import AtlanClient
-from pyatlan.model.assets import Asset, AtlasGlossary, AtlasGlossaryTerm, Badge
+from pyatlan.model.assets import (
+    Asset,
+    AtlasGlossary,
+    AtlasGlossaryTerm,
+    Badge,
+    Connection,
+)
 from pyatlan.model.custom_metadata import CustomMetadataDict
 from pyatlan.model.enums import (
     AtlanCustomAttributePrimitiveType,
     AtlanIcon,
     AtlanTagColor,
     AtlanTypeCategory,
     BadgeComparisonOperator,
@@ -108,21 +115,35 @@
         name=name, values=values, replace_existing=replace_existing
     )
     r = client.typedef.update(enum_def)
     return r.enum_defs[0]
 
 
 @pytest.fixture(scope="module")
+def limit_attribute_applicability_kwargs(
+    glossary: AtlasGlossary, connection: Connection
+):
+    return dict(
+        applicable_asset_types={"Link"},
+        applicable_other_asset_types={"File"},
+        applicable_glossaries={glossary.qualified_name},
+        applicable_glossary_types={"AtlasGlossary", "AtlasGlossaryTerm"},
+        applicable_connections={connection.qualified_name},
+    )
+
+
+@pytest.fixture(scope="module")
 def cm_ipr(
-    client: AtlanClient,
+    client: AtlanClient, limit_attribute_applicability_kwargs
 ) -> Generator[CustomMetadataDef, None, None]:
     attribute_defs = [
         AttributeDef.create(
             display_name=CM_ATTR_IPR_LICENSE,
             attribute_type=AtlanCustomAttributePrimitiveType.STRING,
+            **limit_attribute_applicability_kwargs,
         ),
         AttributeDef.create(
             display_name=CM_ATTR_IPR_VERSION,
             attribute_type=AtlanCustomAttributePrimitiveType.DECIMAL,
         ),
         AttributeDef.create(
             display_name=CM_ATTR_IPR_MANDATORY,
@@ -140,33 +161,39 @@
     cm = create_custom_metadata(
         client, name=CM_IPR, attribute_defs=attribute_defs, logo="⚖️", locked=True
     )
     yield cm
     client.typedef.purge(CM_IPR, CustomMetadataDef)
 
 
-def test_cm_ipr(
-    cm_ipr: CustomMetadataDef,
-):
+def test_cm_ipr(cm_ipr: CustomMetadataDef, limit_attribute_applicability_kwargs):
     cm_name = CM_IPR
     assert cm_ipr.category == AtlanTypeCategory.CUSTOM_METADATA
     assert cm_ipr.guid
     assert cm_ipr.name != cm_name
     assert cm_ipr.display_name == cm_name
     attributes = cm_ipr.attribute_defs
     assert attributes
     assert len(attributes) == 5
-    one = attributes[0]
-    assert one
-    assert one.display_name == CM_ATTR_IPR_LICENSE
-    assert one.name
-    assert one.name != CM_ATTR_IPR_LICENSE
-    assert one.type_name == AtlanCustomAttributePrimitiveType.STRING.value
-    assert one.options
-    assert not one.options.multi_value_select
+    one_with_limited = attributes[0]
+    assert one_with_limited
+    assert one_with_limited.options
+    assert one_with_limited.display_name == CM_ATTR_IPR_LICENSE
+    assert one_with_limited.name
+    assert one_with_limited.name != CM_ATTR_IPR_LICENSE
+    assert one_with_limited.type_name == AtlanCustomAttributePrimitiveType.STRING.value
+    assert not one_with_limited.options.multi_value_select
+    options = one_with_limited.options
+    for attribute in limit_attribute_applicability_kwargs.keys():
+        assert getattr(
+            one_with_limited, attribute
+        ) == limit_attribute_applicability_kwargs.get(attribute)
+        assert getattr(options, attribute) == json.dumps(
+            list(limit_attribute_applicability_kwargs.get(attribute))
+        )
     one = attributes[1]
     assert one.display_name == CM_ATTR_IPR_VERSION
     assert one.name != CM_ATTR_IPR_VERSION
     assert one.type_name == AtlanCustomAttributePrimitiveType.DECIMAL.value
     assert one.options
     assert not one.options.multi_value_select
     one = attributes[2]
```

### Comparing `pyatlan-2.1.1/tests/integration/custom_package_test.py` & `pyatlan-2.1.2/tests/integration/custom_package_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/data_mesh_test.py` & `pyatlan-2.1.2/tests/integration/data_mesh_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/data_studio_asset_test.py` & `pyatlan-2.1.2/tests/integration/data_studio_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/file_test.py` & `pyatlan-2.1.2/tests/integration/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/gcs_asset_test.py` & `pyatlan-2.1.2/tests/integration/gcs_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/glossary_test.py` & `pyatlan-2.1.2/tests/integration/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/lineage_test.py` & `pyatlan-2.1.2/tests/integration/lineage_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/owner_propagator_cfg.py` & `pyatlan-2.1.2/tests/integration/owner_propagator_cfg.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/persona_test.py` & `pyatlan-2.1.2/tests/integration/persona_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/preset_asset_test.py` & `pyatlan-2.1.2/tests/integration/preset_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/purpose_test.py` & `pyatlan-2.1.2/tests/integration/purpose_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/query_parser_test.py` & `pyatlan-2.1.2/tests/integration/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/requests_test.py` & `pyatlan-2.1.2/tests/integration/requests_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/s3_asset_test.py` & `pyatlan-2.1.2/tests/integration/s3_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/test_client.py` & `pyatlan-2.1.2/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/test_index_search.py` & `pyatlan-2.1.2/tests/integration/test_index_search.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/test_sql_assets.py` & `pyatlan-2.1.2/tests/integration/test_sql_assets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/test_task_client.py` & `pyatlan-2.1.2/tests/integration/test_task_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/integration/utils.py` & `pyatlan-2.1.2/tests/integration/utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/conftest.py` & `pyatlan-2.1.2/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/constants.py` & `pyatlan-2.1.2/tests/unit/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/a_d_l_s_account_test.py` & `pyatlan-2.1.2/tests/unit/model/a_d_l_s_account_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/a_d_l_s_container_test.py` & `pyatlan-2.1.2/tests/unit/model/a_d_l_s_container_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/a_d_l_s_object_test.py` & `pyatlan-2.1.2/tests/unit/model/a_d_l_s_object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/a_p_i_path_test.py` & `pyatlan-2.1.2/tests/unit/model/a_p_i_path_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/a_p_i_spec_test.py` & `pyatlan-2.1.2/tests/unit/model/a_p_i_spec_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/badge_condition_test.py` & `pyatlan-2.1.2/tests/unit/model/badge_condition_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/badge_test.py` & `pyatlan-2.1.2/tests/unit/model/badge_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/column_process_test.py` & `pyatlan-2.1.2/tests/unit/model/column_process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/column_test.py` & `pyatlan-2.1.2/tests/unit/model/column_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/connection_test.py` & `pyatlan-2.1.2/tests/unit/model/connection_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/constants.py` & `pyatlan-2.1.2/tests/unit/model/constants.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/data_domain_test.py` & `pyatlan-2.1.2/tests/unit/model/data_domain_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/data_product_test.py` & `pyatlan-2.1.2/tests/unit/model/data_product_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/data_studio_asset_test.py` & `pyatlan-2.1.2/tests/unit/model/data_studio_asset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/database_test.py` & `pyatlan-2.1.2/tests/unit/model/database_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/fields/atlan_fields_test.py` & `pyatlan-2.1.2/tests/unit/model/fields/atlan_fields_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/file_test.py` & `pyatlan-2.1.2/tests/unit/model/file_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/gcs_bucket_test.py` & `pyatlan-2.1.2/tests/unit/model/gcs_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/gcs_object_test.py` & `pyatlan-2.1.2/tests/unit/model/gcs_object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/glossary_category_test.py` & `pyatlan-2.1.2/tests/unit/model/glossary_category_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/glossary_term_test.py` & `pyatlan-2.1.2/tests/unit/model/glossary_term_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/glossary_test.py` & `pyatlan-2.1.2/tests/unit/model/glossary_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/materialised_view_test.py` & `pyatlan-2.1.2/tests/unit/model/materialised_view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/preset_chart_test.py` & `pyatlan-2.1.2/tests/unit/model/preset_chart_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/preset_dashboard_test.py` & `pyatlan-2.1.2/tests/unit/model/preset_dashboard_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/preset_dataset_test.py` & `pyatlan-2.1.2/tests/unit/model/preset_dataset_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/preset_workspace_test.py` & `pyatlan-2.1.2/tests/unit/model/preset_workspace_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/process_test.py` & `pyatlan-2.1.2/tests/unit/model/process_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/readme_test.py` & `pyatlan-2.1.2/tests/unit/model/readme_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/s3_bucket_test.py` & `pyatlan-2.1.2/tests/unit/model/s3_bucket_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/s3object_test.py` & `pyatlan-2.1.2/tests/unit/model/s3object_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/schema_test.py` & `pyatlan-2.1.2/tests/unit/model/schema_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/table_test.py` & `pyatlan-2.1.2/tests/unit/model/table_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/model/view_test.py` & `pyatlan-2.1.2/tests/unit/model/view_test.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/pkg/conftest.py` & `pyatlan-2.1.2/tests/unit/pkg/conftest.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/pkg/test_models.py` & `pyatlan-2.1.2/tests/unit/pkg/test_models.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/pkg/test_ui.py` & `pyatlan-2.1.2/tests/unit/pkg/test_ui.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/pkg/test_utils.py` & `pyatlan-2.1.2/tests/unit/pkg/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/pkg/test_widgets.py` & `pyatlan-2.1.2/tests/unit/pkg/test_widgets.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_atlan_tag_name.py` & `pyatlan-2.1.2/tests/unit/test_atlan_tag_name.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_client.py` & `pyatlan-2.1.2/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_core.py` & `pyatlan-2.1.2/tests/unit/test_core.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_credential_client.py` & `pyatlan-2.1.2/tests/unit/test_credential_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_custom_metadata.py` & `pyatlan-2.1.2/tests/unit/test_custom_metadata.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_deprecated.py` & `pyatlan-2.1.2/tests/unit/test_deprecated.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,15 +469,15 @@
             {
                 "asset_type": AtlasGlossary,
                 "qualified_name": "qname",
                 "atlan_tag_names": ["Something"],
                 "propagate": False,
                 "remove_propagation_on_delete": False,
                 "restrict_lineage_propagation": False,
-                "propagation_only_through_lineage": False,
+                "restrict_propagation_through_hierarchy": False,
             },
         ),
         (
             "remove_atlan_tag",
             "remove_atlan_tag",
             {
                 "asset_type": AtlasGlossary,
```

### Comparing `pyatlan-2.1.1/tests/unit/test_events.py` & `pyatlan-2.1.2/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_glossary_term.py` & `pyatlan-2.1.2/tests/unit/test_glossary_term.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_lineage.py` & `pyatlan-2.1.2/tests/unit/test_lineage.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_model.py` & `pyatlan-2.1.2/tests/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_packages.py` & `pyatlan-2.1.2/tests/unit/test_packages.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_query_client.py` & `pyatlan-2.1.2/tests/unit/test_query_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_search_model.py` & `pyatlan-2.1.2/tests/unit/test_search_model.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_task_client.py` & `pyatlan-2.1.2/tests/unit/test_task_client.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_typedef_model.py` & `pyatlan-2.1.2/tests/unit/test_typedef_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -384,7 +384,37 @@
     def test_applicable_types_with_valid_value(
         self, attribute, value, sut: AttributeDef
     ):
         setattr(sut, attribute, value)
         assert getattr(sut, attribute) == value
         options = sut.options
         assert getattr(options, attribute) == json.dumps(list(value))
+
+    def test_attribute_create_with_limited_applicability(self):
+        applicable_kwargs = dict(
+            applicable_asset_types={"Link"},
+            applicable_other_asset_types={"File"},
+            applicable_glossaries={"8Jdg4PdxcURBBNDt2RZD3"},
+            applicable_glossary_types={"AtlasGlossaryTerm", "AtlasGlossaryCategory"},
+            applicable_connections={
+                "default/snowflake/1699268171",
+                "default/snowflake/16992681799",
+            },
+        )
+        attribute_def_with_limited = AttributeDef.create(
+            display_name="test-attr-def",
+            attribute_type=AtlanCustomAttributePrimitiveType.STRING,
+            # Optional kwargs that allow limiting
+            # the applicability of an attribute within Atlan
+            **applicable_kwargs
+        )
+
+        assert attribute_def_with_limited
+        assert attribute_def_with_limited.options
+        options = attribute_def_with_limited.options
+        for attribute in applicable_kwargs.keys():
+            assert getattr(
+                attribute_def_with_limited, attribute
+            ) == applicable_kwargs.get(attribute)
+            assert getattr(options, attribute) == json.dumps(
+                list(applicable_kwargs.get(attribute))
+            )
```

### Comparing `pyatlan-2.1.1/tests/unit/test_utils.py` & `pyatlan-2.1.2/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyatlan-2.1.1/tests/unit/test_workflow_client.py` & `pyatlan-2.1.2/tests/unit/test_workflow_client.py`

 * *Files identical despite different names*

