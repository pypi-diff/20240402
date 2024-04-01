# Comparing `tmp/dbt_timescaledb-1.8.0a3.tar.gz` & `tmp/dbt_timescaledb-1.8.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_timescaledb-1.8.0a3.tar", last modified: Thu Mar 28 23:18:27 2024, max compression
+gzip compressed data, was "dbt_timescaledb-1.8.0a4.tar", last modified: Mon Apr  1 22:01:50 2024, max compression
```

## Comparing `dbt_timescaledb-1.8.0a3.tar` & `dbt_timescaledb-1.8.0a4.tar`

### file list

```diff
@@ -1,40 +1,46 @@
--rw-r--r--   0        0        0     1068 2024-03-28 23:18:11.859500 dbt_timescaledb-1.8.0a3/LICENSE
--rw-r--r--   0        0        0     3128 2024-03-28 23:18:11.859500 dbt_timescaledb-1.8.0a3/README.md
--rw-r--r--   0        0        0       76 2024-03-28 23:18:11.859500 dbt_timescaledb-1.8.0a3/dbt/__init__.py
--rw-r--r--   0        0        0      413 2024-03-28 23:18:11.859500 dbt_timescaledb-1.8.0a3/dbt/adapters/timescaledb/__init__.py
--rw-r--r--   0        0        0       19 2024-03-28 23:18:27.655541 dbt_timescaledb-1.8.0a3/dbt/adapters/timescaledb/__version__.py
--rw-r--r--   0        0        0      701 2024-03-28 23:18:11.859500 dbt_timescaledb-1.8.0a3/dbt/adapters/timescaledb/timescaledb_adapter.py
--rw-r--r--   0        0        0     1684 2024-03-28 23:18:11.859500 dbt_timescaledb-1.8.0a3/dbt/adapters/timescaledb/timescaledb_connection_manager.py
--rw-r--r--   0        0        0      224 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/adapters/timescaledb/timescaledb_credentials.py
--rw-r--r--   0        0        0      791 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/adapters/timescaledb/timescaledb_index_config.py
--rw-r--r--   0        0        0       52 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/__init__.py
--rw-r--r--   0        0        0       55 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/dbt_project.yml
--rw-r--r--   0        0        0     1024 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/adapters.sql
--rw-r--r--   0        0        0     4752 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/materializations/models/continuous_aggregate.sql
--rw-r--r--   0        0        0     4093 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/materializations/models/hypertable.sql
--rw-r--r--   0        0        0     1814 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/materializations/models/virtual_hypertable.sql
--rw-r--r--   0        0        0     1501 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/relations/compression.sql
--rw-r--r--   0        0        0     1410 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/relations/continuous_aggregate.sql
--rw-r--r--   0        0        0     1724 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/relations/dimensions.sql
--rw-r--r--   0        0        0     1715 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/relations/hypertable.sql
--rw-r--r--   0        0        0      574 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/relations/retention_policy.sql
--rw-r--r--   0        0        0      307 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/profile_template.yml
--rw-r--r--   0        0        0     1999 2024-03-28 23:18:27.659541 dbt_timescaledb-1.8.0a3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/tests/__init__.py
--rw-r--r--   0        0        0      546 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/tests/conftest.py
--rw-r--r--   0        0        0     2038 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate.py
--rw-r--r--   0        0        0     2523 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_compression.py
--rw-r--r--   0        0        0     1290 2024-03-28 23:18:11.863499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_index.py
--rw-r--r--   0        0        0     2059 2024-03-28 23:18:11.867499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_refresh_policy.py
--rw-r--r--   0        0        0     1771 2024-03-28 23:18:11.867499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/hypertable/test_hypertable.py
--rw-r--r--   0        0        0     4808 2024-03-28 23:18:11.867499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/hypertable/test_hypertable_compression.py
--rw-r--r--   0        0        0     3001 2024-03-28 23:18:11.867499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/hypertable/test_hypertable_dimension.py
--rw-r--r--   0        0        0     1216 2024-03-28 23:18:11.867499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/hypertable/test_hypertable_index.py
--rw-r--r--   0        0        0     1835 2024-03-28 23:18:11.867499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/hypertable/test_hypertable_integer_now_func.py
--rw-r--r--   0        0        0     1798 2024-03-28 23:18:11.867499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/hypertable/test_reorder_policy.py
--rw-r--r--   0        0        0     1429 2024-03-28 23:18:11.867499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/test_basic.py
--rw-r--r--   0        0        0     3440 2024-03-28 23:18:11.867499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/test_retention_policy.py
--rw-r--r--   0        0        0     3118 2024-03-28 23:18:11.867499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable.py
--rw-r--r--   0        0        0     1995 2024-03-28 23:18:11.867499 dbt_timescaledb-1.8.0a3/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_integer_now_func.py
--rw-r--r--   0        0        0      177 2024-03-28 23:18:11.867499 dbt_timescaledb-1.8.0a3/tests/utils.py
--rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 dbt_timescaledb-1.8.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/LICENSE
+-rw-r--r--   0        0        0     3128 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/README.md
+-rw-r--r--   0        0        0       76 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/__init__.py
+-rw-r--r--   0        0        0      413 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/__init__.py
+-rw-r--r--   0        0        0       19 2024-04-01 22:01:50.454325 dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/__version__.py
+-rw-r--r--   0        0        0      701 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_adapter.py
+-rw-r--r--   0        0        0     1684 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_connection_manager.py
+-rw-r--r--   0        0        0      224 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_credentials.py
+-rw-r--r--   0        0        0      791 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_index_config.py
+-rw-r--r--   0        0        0       52 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/dbt_project.yml
+-rw-r--r--   0        0        0     2585 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/adapters.sql
+-rw-r--r--   0        0        0     3143 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/materializations/models/continuous_aggregate.sql
+-rw-r--r--   0        0        0     4088 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/materializations/models/hypertable.sql
+-rw-r--r--   0        0        0     2105 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/materializations/models/virtual_hypertable.sql
+-rw-r--r--   0        0        0     1784 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/compression.sql
+-rw-r--r--   0        0        0     1551 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/continuous_aggregate.sql
+-rw-r--r--   0        0        0     1724 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/dimensions.sql
+-rw-r--r--   0        0        0      628 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/hypertable.sql
+-rw-r--r--   0        0        0      459 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/integer_now_func.sql
+-rw-r--r--   0        0        0      846 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/reorder_policy.sql
+-rw-r--r--   0        0        0      706 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/retention_policy.sql
+-rw-r--r--   0        0        0      307 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/profile_template.yml
+-rw-r--r--   0        0        0     2041 2024-04-01 22:01:50.458325 dbt_timescaledb-1.8.0a4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/__init__.py
+-rw-r--r--   0        0        0      714 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/conftest.py
+-rw-r--r--   0        0        0     2425 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate.py
+-rw-r--r--   0        0        0     2573 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_compression.py
+-rw-r--r--   0        0        0     1351 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_index.py
+-rw-r--r--   0        0        0     2109 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_refresh_policy.py
+-rw-r--r--   0        0        0     2407 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_retention_policy.py
+-rw-r--r--   0        0        0     1821 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable.py
+-rw-r--r--   0        0        0     4858 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_compression.py
+-rw-r--r--   0        0        0     3071 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_dimension.py
+-rw-r--r--   0        0        0     1277 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_index.py
+-rw-r--r--   0        0        0     1933 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_integer_now_func.py
+-rw-r--r--   0        0        0     1859 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_reorder_policy.py
+-rw-r--r--   0        0        0     1429 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/test_basic.py
+-rw-r--r--   0        0        0     3510 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/test_retention_policy.py
+-rw-r--r--   0        0        0     3174 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable.py
+-rw-r--r--   0        0        0     1855 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_compression.py
+-rw-r--r--   0        0        0     2074 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_integer_now_func.py
+-rw-r--r--   0        0        0     2324 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_reorder_policy.py
+-rw-r--r--   0        0        0     2254 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_retention_policy.py
+-rw-r--r--   0        0        0      177 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/utils.py
+-rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 dbt_timescaledb-1.8.0a4/PKG-INFO
```

### Comparing `dbt_timescaledb-1.8.0a3/LICENSE` & `dbt_timescaledb-1.8.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a3/README.md` & `dbt_timescaledb-1.8.0a4/README.md`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a3/dbt/adapters/timescaledb/timescaledb_adapter.py` & `dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_adapter.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a3/dbt/adapters/timescaledb/timescaledb_connection_manager.py` & `dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_connection_manager.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a3/dbt/adapters/timescaledb/timescaledb_index_config.py` & `dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_index_config.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/materializations/models/hypertable.sql` & `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/materializations/models/hypertable.sql`

 * *Files 6% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 
     {%- if should_truncate %}
       truncate {{ intermediate_relation }};
     {% endif -%}
 
     {{- get_create_hypertable_as_sql(intermediate_relation) }}
 
+    {{ set_compression(intermediate_relation, config.get("compression")) }}
     {%- if config.get('compression') %}
-      {{ enable_compression(intermediate_relation, config.get("compression")) }}
       {{ add_compression_policy(intermediate_relation, config.get("compression")) }}
     {% endif -%}
 
     {%- if config.get("integer_now_func") %}
       {{ set_integer_now_func(intermediate_relation, config.get("integer_now_func"), config.get("integer_now_func_sql")) }}
     {% endif -%}
```

### Comparing `dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/materializations/models/virtual_hypertable.sql` & `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/materializations/models/virtual_hypertable.sql`

 * *Files 7% similar despite different names*

```diff
@@ -8,33 +8,40 @@
     -- `BEGIN` happens here:
     {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
     -- build model
     {% call statement('main') -%}
         select 1 as dummy;
 
+        {{ set_compression(target_relation, config.get("compression")) }}
+        {{ clear_compression_policy(target_relation) }}
         {%- if config.get('compression') %}
-            {{ enable_compression(target_relation, config.get("compression")) }}
             {{ add_compression_policy(target_relation, config.get("compression")) }}
         {% endif -%}
 
         {%- if config.get("integer_now_func") %}
             {{ set_integer_now_func(target_relation, config.get("integer_now_func"), config.get("integer_now_func_sql")) }}
         {% endif -%}
 
     {%- endcall %}
 
     {% do create_indexes(target_relation) %}
 
+    {%- call statement("clear_reorder_policy") %}
+      {{ clear_reorder_policy(target_relation) }}
+    {% endcall -%}
     {%- if config.get("reorder_policy") %}
         {% call statement("reorder_policy") %}
             {{ add_reorder_policy(target_relation, config.get("reorder_policy")) }}
         {% endcall %}
     {% endif -%}
 
+    {%- call statement("clear_retention_policy") %}
+      {{ clear_retention_policy(target_relation) }}
+    {% endcall -%}
     {%- if config.get("retention_policy") %}
         {% call statement("retention_policy") %}
             {{ add_retention_policy(target_relation, config.get("retention_policy")) }}
         {% endcall %}
     {% endif -%}
 
     {{ run_hooks(post_hooks, inside_transaction=True) }}
```

### Comparing `dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/relations/compression.sql` & `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/compression.sql`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-{% macro enable_compression(relation, compression_config) %}
+{% macro set_compression(relation, compression_config) %}
   {%- if relation.is_materialized_view -%}
     {%- set relation_type = "materialized view" -%}
   {%- elif relation.is_table -%}
     {%- set relation_type = "table" -%}
   {%- else -%}
     {{ exceptions.raise_compiler_error("Cannot enable compression on a " ~ relation.type) }}
   {%- endif -%}
 
+  {% set bool_compression = compression_config is not none %}
+
   alter {{ relation_type }} {{ relation }} set (
-    timescaledb.compress = true
+    timescaledb.compress = {{ bool_compression }}
 
-    {%- if compression_config.orderby %}
+    {%- if compression_config and compression_config.orderby %}
         ,timescaledb.compress_orderby = '{{ compression_config.orderby }}'
     {% endif -%}
 
-    {%- if compression_config.segmentby %}
+    {%- if compression_config and compression_config.segmentby %}
         ,timescaledb.compress_segmentby = '{{ compression_config.segmentby | join(",") }}'
     {% endif -%}
 
-    {%- if compression_config.chunk_time_interval %}
+    {%- if compression_config and compression_config.chunk_time_interval %}
         ,timescaledb.compress_chunk_time_interval = '{{ compression_config.chunk_time_interval }}'
     {% endif -%}
   );
 {% endmacro %}
 
 {% macro add_compression_policy(relation, compression_config) %}
   select add_compression_policy(
@@ -39,7 +41,11 @@
 
     {%- if compression_config.timezone %}
         timezone => '{{ compression_config.timezone }}',
     {% endif -%}
 
     if_not_exists => true);
 {% endmacro %}
+
+{% macro clear_compression_policy(relation) %}
+  select remove_compression_policy('{{ relation }}', if_exists => true);
+{% endmacro %}
```

### Comparing `dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/relations/continuous_aggregate.sql` & `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/continuous_aggregate.sql`

 * *Files 7% similar despite different names*

```diff
@@ -37,7 +37,11 @@
 
     {%- if refresh_config.timezone %}
         timezone => '{{ refresh_config.timezone }}',
     {% endif -%}
 
     if_not_exists => true);
 {% endmacro %}
+
+{% macro clear_refresh_policy(relation) %}
+  select remove_continuous_aggregate_policy('{{ relation }}', if_exists => true);
+{% endmacro %}
```

### Comparing `dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/relations/dimensions.sql` & `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/dimensions.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a3/dbt/include/timescaledb/macros/relations/retention_policy.sql` & `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/retention_policy.sql`

 * *Files 9% similar despite different names*

```diff
@@ -13,7 +13,11 @@
 
     {%- if retention_config.timezone %}
         timezone => '{{ retention_config.timezone }}',
     {% endif -%}
 
     if_not_exists => true);
 {% endmacro %}
+
+{% macro clear_retention_policy(relation) %}
+  select remove_retention_policy('{{ relation }}', if_exists => true);
+{% endmacro %}
```

### Comparing `dbt_timescaledb-1.8.0a3/pyproject.toml` & `dbt_timescaledb-1.8.0a4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.11",
 ]
-version = "1.8.0a3"
+version = "1.8.0a4"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://dbt-timescaledb.debruyn.dev"
 Repository = "https://github.com/sdebruyn/dbt-timescaledb"
@@ -99,8 +99,8 @@
 [tool.pytest.ini_options]
 env_files = [
     "test.env",
 ]
 testpaths = [
     "tests",
 ]
-addopts = "-v -n auto --cov-report=xml"
+addopts = "-W ignore::pytest.PytestCollectionWarning -v -n auto --cov-report=xml"
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/conftest.py` & `dbt_timescaledb-1.8.0a4/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,7 +12,13 @@
         "type": "timescaledb",
         "host": os.getenv("TIMESCALEDB_TEST_HOST", "localhost"),
         "port": int(os.getenv("TIMESCALEDB_TEST_PORT", "5432")),
         "user": os.getenv("POSTGRES_USER", "timescaledb"),
         "pass": os.getenv("POSTGRES_PASSWORD", "timescaledb"),
         "dbname": os.getenv("POSTGRES_DB", "timescaledb"),
     }
+
+
+@pytest.fixture(scope="class")
+def unique_schema(unique_schema: str) -> str:
+    # The schema name must be less than 64 characters long
+    return unique_schema[:63]
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import (
     check_result_nodes_by_name,
     run_dbt,
 )
 
 
 class TestContinuousAggregate:
@@ -19,43 +20,51 @@
         ],
     )
     def project_config_update(self, request) -> dict[str, Any]:  # noqa: ANN001
         return {
             "name": "continuous_aggregate_tests",
             "models": {
                 "continuous_aggregate_tests": {
-                    "base": {"+materialized": "hypertable", "+main_dimension": "time_column"},
+                    "vht": {"+materialized": "virtual_hypertable"},
                     "test_model": {"+materialized": "continuous_aggregate"} | request.param,
                 }
             },
         }
 
     @pytest.fixture(scope="class")
     def models(self) -> dict[str, Any]:
         return {
-            "base.sql": "select current_timestamp as time_column",
+            "vht.sql": "--",
             "test_model.sql": """
 select
     count(*),
     time_bucket(interval '1 day', time_column) as bucket
-from {{ ref('base') }}
+from {{ ref('vht') }}
 group by 2
 """,
         }
 
-    def test_continuous_aggregate(self, project, unique_schema: str) -> None:  # noqa: ANN001
+    def test_continuous_aggregate(self, project: TestProjInfo, unique_schema: str) -> None:
+        project.run_sql(f"""
+create table if not exists {unique_schema}.vht (time_column timestamp);
+select create_hypertable('{unique_schema}.vht', by_range('time_column'), if_not_exists => true);""")
+
         results = run_dbt(["run"])
         assert len(results) == 2  # noqa
-        check_result_nodes_by_name(results, ["base", "test_model"])
+        check_result_nodes_by_name(results, ["vht", "test_model"])
         nodes = [r.node for r in results]
         test_model = next(n for n in nodes if n.name == "test_model")
         assert test_model.node_info["materialized"] == "continuous_aggregate"
 
         continuous_aggregate_results = project.run_sql(
             f"""
 select *
 from timescaledb_information.continuous_aggregates
 where view_schema = '{unique_schema}'
 and view_name = 'test_model'""",
             fetch="all",
         )
         assert len(continuous_aggregate_results) == 1
+
+    def test_continuous_aggregate_multiple_runs(self, project: TestProjInfo, unique_schema: str) -> None:
+        for _ in range(5):
+            self.test_continuous_aggregate(project, unique_schema)
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_compression.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_compression.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import check_result_nodes_by_name, run_dbt
 
 
 class TestContinuousAggregateCompression:
     @pytest.fixture(scope="class")
     def project_config_update(self) -> dict[str, Any]:
         return {
@@ -41,15 +42,15 @@
     count(*),
     time_bucket(interval '1 day', time_column) as bucket
 from {{ ref('base') }}
 group by 2
 """,
         }
 
-    def test_continuous_aggregate(self, project, unique_schema: str) -> None:  # noqa: ANN001
+    def test_continuous_aggregate(self, project: TestProjInfo, unique_schema: str) -> None:
         results = run_dbt(["run"])
         assert len(results) == 2
         check_result_nodes_by_name(results, ["base", "test_model"])
 
         continuous_aggregate_results = project.run_sql(
             f"""
 select *
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_index.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_index.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import run_dbt
 
 
 class TestContinuousAggregateIndex:
     def _model_sql(self, create_group_indexes: bool) -> str:
         return f"""
 {{{{
@@ -40,10 +41,10 @@
     def models(self) -> dict[str, Any]:
         return {
             "base.sql": "select current_timestamp as time_column",
             "with_default.sql": self._model_sql(True),
             "without_default.sql": self._model_sql(False),
         }
 
-    def test_continuous_aggregate(self, project: Any) -> None:
+    def test_continuous_aggregate(self, project: TestProjInfo) -> None:
         results = run_dbt(["run"])
         assert len(results) == 3
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_refresh_policy.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_refresh_policy.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import (
     check_result_nodes_by_name,
     run_dbt,
 )
 
 
 class TestContinuousAggregateRefreshPolicy:
@@ -37,15 +38,15 @@
     count(*),
     time_bucket(interval '1 day', time_column) as bucket
 from {{ ref('base') }}
 group by 2
 """,
         }
 
-    def test_continuous_aggregate(self, project, unique_schema: str) -> None:  # noqa: ANN001
+    def test_continuous_aggregate(self, project: TestProjInfo, unique_schema: str) -> None:
         results = run_dbt(["run"])
         assert len(results) == 2  # noqa
         check_result_nodes_by_name(results, ["base", "test_model"])
 
         continuous_aggregate_results = project.run_sql(
             f"""
 select *
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/hypertable/test_hypertable.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import (
     check_result_nodes_by_name,
     relation_from_name,
     run_dbt,
 )
 
 _base_model_config: dict[str, str] = {
@@ -36,15 +37,15 @@
             "models": {"hypertable_tests": _models_with_configs},
         }
 
     @pytest.fixture(scope="class")
     def models(self) -> dict[str, Any]:
         return {f"{k}.sql": _model_sql for k in _models_with_configs.keys()}
 
-    def test_hypertable(self, project, unique_schema: str) -> None:  # noqa: ANN001
+    def test_hypertable(self, project: TestProjInfo, unique_schema: str) -> None:
         results = run_dbt(["run"])
         assert len(results) == len(_models_with_configs)
         check_result_nodes_by_name(results, _models_with_configs.keys())
         assert all(result.node.config.materialized == "hypertable" for result in results)
 
         hypertables = project.run_sql(
             f"""
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/hypertable/test_hypertable_compression.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_compression.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import check_result_nodes_by_name, run_dbt
 
 
 class BaseTestHypertableCompression:
     def base_compression_settings(self) -> dict[str, Any]:
         return {"after": "interval '1 day'", "schedule_interval": "interval '6 day'"}
 
@@ -51,15 +52,15 @@
         assert time_column[6]
 
     def validate_jobs(self, timescale_jobs: list) -> None:
         assert len(timescale_jobs) == 1
         job = timescale_jobs[0]
         assert job[9]
 
-    def test_hypertable(self, project, unique_schema: str) -> None:  # noqa: ANN001
+    def test_hypertable(self, project: TestProjInfo, unique_schema: str) -> None:
         results = run_dbt(["run"])
         assert len(results) == 1
         check_result_nodes_by_name(results, ["test_model"])
         assert results[0].node.node_info["materialized"] == "hypertable"
 
         hypertables = project.run_sql(
             f"""
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/hypertable/test_hypertable_dimension.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_dimension.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import check_result_nodes_by_name, run_dbt
 
 
 class TestHypertableDimension:
     @pytest.fixture(scope="class")
     def project_config_update(self) -> dict[str, Any]:
         return {
@@ -27,15 +28,15 @@
 
     @pytest.fixture(scope="class")
     def models(self) -> dict[str, Any]:
         return {
             "test_model.sql": "select current_timestamp as time_column, 1 as id, 2 as col_1",
         }
 
-    def test_hypertable_dimension(self, project: Any, unique_schema: str) -> None:
+    def test_hypertable_dimension(self, project: TestProjInfo, unique_schema: str) -> None:
         results = run_dbt(["run"])
         assert len(results) == 1
         check_result_nodes_by_name(results, ["test_model"])
 
         dimensions_results = project.run_sql(
             f"""
 select *
@@ -77,11 +78,11 @@
                         "+main_dimension": "time_column",
                         "+dimensions": [{"column_name": "id"}],
                     }
                 }
             },
         }
 
-    def test_hypertable_dimension_throw_exception(self, project: Any) -> None:
+    def test_hypertable_dimension_throw_exception(self, project: TestProjInfo) -> None:
         results = run_dbt(["run"], expect_pass=False)
         assert len(results) == 1
         assert str(results[0].status) == "error"
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/hypertable/test_hypertable_index.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_index.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import run_dbt
 from tests.utils import get_indexes_sql
 
 
 class TestHypertableIndex:
     def _model_sql(self, create_default_indexes: bool) -> str:
         return f"""
@@ -28,15 +29,15 @@
     @pytest.fixture(scope="class")
     def models(self) -> dict[str, Any]:
         return {
             "with_default.sql": self._model_sql(True),
             "without_default.sql": self._model_sql(False),
         }
 
-    def test_table(self, project: Any, unique_schema: str) -> None:
+    def test_table(self, project: TestProjInfo, unique_schema: str) -> None:
         results = run_dbt(["run"])
         assert len(results) == 2
 
         with_default_results = project.run_sql(get_indexes_sql(unique_schema, "with_default"), fetch="all")
         without_default_results = project.run_sql(
             get_indexes_sql(unique_schema, "without_default"), fetch="all"
         )
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/hypertable/test_hypertable_integer_now_func.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_integer_now_func.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import run_dbt
 
 
 class BaseTestHypertableIntegerNowFunc:
     @pytest.fixture(scope="class")
     def extra_model_config(self) -> dict[str, Any]:
         return {}
@@ -28,28 +29,29 @@
 
     @pytest.fixture(scope="class")
     def models(self) -> dict[str, Any]:
         return {
             "test_model.sql": "select 1::bigint as id",
         }
 
-    def prepare_func(self, project: Any, unique_schema: str) -> None:
+    def prepare_func(self, project: TestProjInfo, unique_schema: str) -> None:
         pass
 
-    def test_integer_now_func(self, project: Any, unique_schema: str) -> None:
+    def test_integer_now_func(self, project: TestProjInfo, unique_schema: str) -> None:
         self.prepare_func(project, unique_schema)
         results = run_dbt(["run"])
         assert len(results) == 1
 
 
 class TestHypertableIntegerNowFuncWithoutSQL(BaseTestHypertableIntegerNowFunc):
-    def prepare_func(self, project: Any, unique_schema: str) -> None:
+    def prepare_func(self, project: TestProjInfo, unique_schema: str) -> None:
         project.run_sql(
             f"""
-create or replace function {unique_schema}.test_model_now() returns bigint language sql immutable as $$
+create or replace function {project.database}.{unique_schema}.test_model_now()
+returns bigint language sql immutable as $$
       select extract(epoch from now())::bigint
     $$;
 """
         )
 
 
 class TestHypertableIntegerNowFuncWithSQL(BaseTestHypertableIntegerNowFunc):
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/hypertable/test_reorder_policy.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_reorder_policy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import run_dbt
 from tests.utils import get_indexes_sql
 
 
 class TestHypertableReorderPolicy:
     def _model_sql(self, create_index: bool) -> str:
         return f"""
@@ -32,15 +33,15 @@
     @pytest.fixture(scope="class")
     def models(self) -> dict[str, Any]:
         return {
             "create_index.sql": self._model_sql(True),
             "sep_index.sql": self._model_sql(False),
         }
 
-    def test_reorder_policy(self, project: Any, unique_schema: str) -> None:
+    def test_reorder_policy(self, project: TestProjInfo, unique_schema: str) -> None:
         results = run_dbt(["run"])
         assert len(results) == 2
 
         create_index_results = project.run_sql(get_indexes_sql(unique_schema, "create_index"), fetch="all")
         sep_index_results = project.run_sql(get_indexes_sql(unique_schema, "sep_index"), fetch="all")
 
         assert len(create_index_results) == 2, "Expected 2 indexes when index should be created"
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/test_basic.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/test_retention_policy.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/test_retention_policy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import run_dbt
 
 RETENTION_CONFIGS: list = [
     pytest.param(
         {
             "drop_after": "interval '1 day'",
         },
@@ -52,15 +53,15 @@
     @pytest.fixture(scope="class")
     def project_config_update(self, model_configs: dict[str, Any]) -> dict[str, Any]:
         return {
             "name": "retention_policy_tests",
             "models": {"retention_policy_tests": model_configs},
         }
 
-    def test_retention_policy(self, project: Any, model_count: int, unique_schema: str) -> None:
+    def test_retention_policy(self, project: TestProjInfo, model_count: int, unique_schema: str) -> None:
         results = run_dbt(["run"])
         assert len(results) == model_count
 
         hypertable_jobs = project.run_sql(
             f"""
 select *
 from timescaledb_information.jobs
@@ -91,15 +92,15 @@
         return super().base_model_config(retention_config) | {
             "cagg": {
                 "+materialized": "continuous_aggregate",
                 "+retention_policy": retention_config,
             }
         }
 
-    def test_retention_policy(self, project: Any, model_count: int, unique_schema: str) -> None:
+    def test_retention_policy(self, project: TestProjInfo, model_count: int, unique_schema: str) -> None:
         super().test_retention_policy(project, model_count, unique_schema)
 
         cagg_jobs = project.run_sql(
             f"""
 select *
 from timescaledb_information.jobs j
 join timescaledb_information.continuous_aggregates c
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import (
     run_dbt,
 )
 
 
 class BaseTestVirtualHypertable:
     @pytest.fixture(scope="class")
@@ -23,18 +24,18 @@
             },
         }
 
     @pytest.fixture(scope="class")
     def models(self) -> dict[str, Any]:
         return {"vht.sql": "--"}
 
-    def run_assertions(self, project, unique_schema: str, hypertable) -> None:  # noqa: ANN001
+    def run_assertions(self, project: TestProjInfo, unique_schema: str, hypertable: Any) -> None:
         pass
 
-    def test_virtual_hypertable(self, project, unique_schema: str) -> None:  # noqa: ANN001
+    def test_virtual_hypertable(self, project: TestProjInfo, unique_schema: str) -> None:
         project.run_sql(f"""
 create table {unique_schema}.vht (time_column timestamp, col_1 int);
 select create_hypertable('{unique_schema}.vht', by_range('time_column'));""")
         results = run_dbt(["run"])
         assert len(results) == 1
         assert all(result.node.config.materialized == "virtual_hypertable" for result in results)
 
@@ -72,15 +73,15 @@
 
 
 class TestVirtualHypertableCompression(BaseTestVirtualHypertable):
     @pytest.fixture(scope="class")
     def extra_model_config(self) -> dict[str, Any]:
         return {"+compression": {"after": "interval '1 day'", "schedule_interval": "interval '6 day'"}}
 
-    def run_assertions(self, project, unique_schema: str, hypertable) -> None:  # noqa: ANN001
+    def run_assertions(self, project: TestProjInfo, unique_schema: str, hypertable: Any) -> None:
         assert hypertable[5]  # compression_enabled
 
         compression_settings = project.run_sql(
             f"""
 select *
 from timescaledb_information.compression_settings
 where hypertable_name = 'vht'
```

### Comparing `dbt_timescaledb-1.8.0a3/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_integer_now_func.py` & `dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_integer_now_func.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any
 
 import pytest
 
+from dbt.tests.fixtures.project import TestProjInfo
 from dbt.tests.util import run_dbt
 
 
 class BaseTestVirtualHypertableIntegerNowFunc:
     @pytest.fixture(scope="class")
     def extra_model_config(self) -> dict[str, Any]:
         return {}
@@ -27,27 +28,27 @@
 
     @pytest.fixture(scope="class")
     def models(self) -> dict[str, Any]:
         return {
             "vht.sql": "--",
         }
 
-    def prepare_func(self, project: Any, unique_schema: str) -> None:
+    def prepare_func(self, project: TestProjInfo, unique_schema: str) -> None:
         project.run_sql(f"""
 create table {unique_schema}.vht (id bigint);
 select create_hypertable('{unique_schema}.vht', by_range('id'));""")
 
-    def test_integer_now_func(self, project: Any, unique_schema: str) -> None:
+    def test_integer_now_func(self, project: TestProjInfo, unique_schema: str) -> None:
         self.prepare_func(project, unique_schema)
         results = run_dbt(["run"])
         assert len(results) == 1
 
 
 class TestVirtualHypertableIntegerNowFuncWithoutSQL(BaseTestVirtualHypertableIntegerNowFunc):
-    def prepare_func(self, project: Any, unique_schema: str) -> None:
+    def prepare_func(self, project: TestProjInfo, unique_schema: str) -> None:
         super().prepare_func(project, unique_schema)
         project.run_sql(
             f"""
 create or replace function {unique_schema}.test_model_now() returns bigint language sql immutable as $$
       select extract(epoch from now())::bigint
     $$;
 """
```

### Comparing `dbt_timescaledb-1.8.0a3/PKG-INFO` & `dbt_timescaledb-1.8.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-timescaledb
-Version: 1.8.0a3
+Version: 1.8.0a4
 Summary: The TimescaleDB adapter plugin for dbt
 Keywords: dbt timescaledb
 Author-Email: Sam Debruyn <dbt.sam@debruyn.dev>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

