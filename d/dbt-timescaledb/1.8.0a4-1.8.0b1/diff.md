# Comparing `tmp/dbt_timescaledb-1.8.0a4.tar.gz` & `tmp/dbt_timescaledb-1.8.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_timescaledb-1.8.0a4.tar", last modified: Mon Apr  1 22:01:50 2024, max compression
+gzip compressed data, was "dbt_timescaledb-1.8.0b1.tar", last modified: Tue Apr  2 21:43:11 2024, max compression
```

## Comparing `dbt_timescaledb-1.8.0a4.tar` & `dbt_timescaledb-1.8.0b1.tar`

### file list

```diff
@@ -1,46 +1,49 @@
--rw-r--r--   0        0        0     1068 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/LICENSE
--rw-r--r--   0        0        0     3128 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/README.md
--rw-r--r--   0        0        0       76 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/__init__.py
--rw-r--r--   0        0        0      413 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/__init__.py
--rw-r--r--   0        0        0       19 2024-04-01 22:01:50.454325 dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/__version__.py
--rw-r--r--   0        0        0      701 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_adapter.py
--rw-r--r--   0        0        0     1684 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_connection_manager.py
--rw-r--r--   0        0        0      224 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_credentials.py
--rw-r--r--   0        0        0      791 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_index_config.py
--rw-r--r--   0        0        0       52 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/__init__.py
--rw-r--r--   0        0        0       55 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/dbt_project.yml
--rw-r--r--   0        0        0     2585 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/adapters.sql
--rw-r--r--   0        0        0     3143 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/materializations/models/continuous_aggregate.sql
--rw-r--r--   0        0        0     4088 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/materializations/models/hypertable.sql
--rw-r--r--   0        0        0     2105 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/materializations/models/virtual_hypertable.sql
--rw-r--r--   0        0        0     1784 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/compression.sql
--rw-r--r--   0        0        0     1551 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/continuous_aggregate.sql
--rw-r--r--   0        0        0     1724 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/dimensions.sql
--rw-r--r--   0        0        0      628 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/hypertable.sql
--rw-r--r--   0        0        0      459 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/integer_now_func.sql
--rw-r--r--   0        0        0      846 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/reorder_policy.sql
--rw-r--r--   0        0        0      706 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/retention_policy.sql
--rw-r--r--   0        0        0      307 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/profile_template.yml
--rw-r--r--   0        0        0     2041 2024-04-01 22:01:50.458325 dbt_timescaledb-1.8.0a4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/__init__.py
--rw-r--r--   0        0        0      714 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/conftest.py
--rw-r--r--   0        0        0     2425 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate.py
--rw-r--r--   0        0        0     2573 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_compression.py
--rw-r--r--   0        0        0     1351 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_index.py
--rw-r--r--   0        0        0     2109 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_refresh_policy.py
--rw-r--r--   0        0        0     2407 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_retention_policy.py
--rw-r--r--   0        0        0     1821 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable.py
--rw-r--r--   0        0        0     4858 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_compression.py
--rw-r--r--   0        0        0     3071 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_dimension.py
--rw-r--r--   0        0        0     1277 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_index.py
--rw-r--r--   0        0        0     1933 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_integer_now_func.py
--rw-r--r--   0        0        0     1859 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_reorder_policy.py
--rw-r--r--   0        0        0     1429 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/test_basic.py
--rw-r--r--   0        0        0     3510 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/test_retention_policy.py
--rw-r--r--   0        0        0     3174 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable.py
--rw-r--r--   0        0        0     1855 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_compression.py
--rw-r--r--   0        0        0     2074 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_integer_now_func.py
--rw-r--r--   0        0        0     2324 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_reorder_policy.py
--rw-r--r--   0        0        0     2254 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_retention_policy.py
--rw-r--r--   0        0        0      177 2024-04-01 22:01:35.006186 dbt_timescaledb-1.8.0a4/tests/utils.py
--rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 dbt_timescaledb-1.8.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/LICENSE
+-rw-r--r--   0        0        0     3128 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/README.md
+-rw-r--r--   0        0        0       76 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/__init__.py
+-rw-r--r--   0        0        0      413 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/adapters/timescaledb/__init__.py
+-rw-r--r--   0        0        0       19 2024-04-02 21:43:11.139517 dbt_timescaledb-1.8.0b1/dbt/adapters/timescaledb/__version__.py
+-rw-r--r--   0        0        0      814 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/adapters/timescaledb/timescaledb_adapter.py
+-rw-r--r--   0        0        0      515 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/adapters/timescaledb/timescaledb_change_collection.py
+-rw-r--r--   0        0        0     1684 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/adapters/timescaledb/timescaledb_connection_manager.py
+-rw-r--r--   0        0        0      224 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/adapters/timescaledb/timescaledb_credentials.py
+-rw-r--r--   0        0        0      791 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/adapters/timescaledb/timescaledb_index_config.py
+-rw-r--r--   0        0        0     1965 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/adapters/timescaledb/timescaledb_relation.py
+-rw-r--r--   0        0        0       52 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/__init__.py
+-rw-r--r--   0        0        0       55 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/dbt_project.yml
+-rw-r--r--   0        0        0     2585 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/adapters.sql
+-rw-r--r--   0        0        0     3143 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/materializations/models/continuous_aggregate.sql
+-rw-r--r--   0        0        0     4088 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/materializations/models/hypertable.sql
+-rw-r--r--   0        0        0     2150 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/materializations/models/virtual_hypertable.sql
+-rw-r--r--   0        0        0     1784 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/relations/compression.sql
+-rw-r--r--   0        0        0     1551 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/relations/continuous_aggregate.sql
+-rw-r--r--   0        0        0     1724 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/relations/dimensions.sql
+-rw-r--r--   0        0        0     1653 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/relations/hypertable.sql
+-rw-r--r--   0        0        0      459 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/relations/integer_now_func.sql
+-rw-r--r--   0        0        0      846 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/relations/reorder_policy.sql
+-rw-r--r--   0        0        0      706 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/relations/retention_policy.sql
+-rw-r--r--   0        0        0      307 2024-04-02 21:42:50.579264 dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/profile_template.yml
+-rw-r--r--   0        0        0     2041 2024-04-02 21:43:11.143517 dbt_timescaledb-1.8.0b1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/__init__.py
+-rw-r--r--   0        0        0      714 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/conftest.py
+-rw-r--r--   0        0        0     2425 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate.py
+-rw-r--r--   0        0        0     2573 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_compression.py
+-rw-r--r--   0        0        0     1351 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_index.py
+-rw-r--r--   0        0        0     2109 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_refresh_policy.py
+-rw-r--r--   0        0        0     2407 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_retention_policy.py
+-rw-r--r--   0        0        0     1821 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/hypertable/test_hypertable.py
+-rw-r--r--   0        0        0     4858 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/hypertable/test_hypertable_compression.py
+-rw-r--r--   0        0        0     3071 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/hypertable/test_hypertable_dimension.py
+-rw-r--r--   0        0        0     1277 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/hypertable/test_hypertable_index.py
+-rw-r--r--   0        0        0     1933 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/hypertable/test_hypertable_integer_now_func.py
+-rw-r--r--   0        0        0     1859 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/hypertable/test_reorder_policy.py
+-rw-r--r--   0        0        0     1429 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/test_basic.py
+-rw-r--r--   0        0        0     3510 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/test_retention_policy.py
+-rw-r--r--   0        0        0     3174 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable.py
+-rw-r--r--   0        0        0     1855 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_compression.py
+-rw-r--r--   0        0        0     2116 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_index_updates.py
+-rw-r--r--   0        0        0     2074 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_integer_now_func.py
+-rw-r--r--   0        0        0     2324 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_reorder_policy.py
+-rw-r--r--   0        0        0     2254 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_retention_policy.py
+-rw-r--r--   0        0        0      177 2024-04-02 21:42:50.583264 dbt_timescaledb-1.8.0b1/tests/utils.py
+-rw-r--r--   0        0        0     3992 1970-01-01 00:00:00.000000 dbt_timescaledb-1.8.0b1/PKG-INFO
```

### Comparing `dbt_timescaledb-1.8.0a4/LICENSE` & `dbt_timescaledb-1.8.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/README.md` & `dbt_timescaledb-1.8.0b1/README.md`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_adapter.py` & `dbt_timescaledb-1.8.0b1/dbt/adapters/timescaledb/timescaledb_adapter.py`

 * *Files 26% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from dbt.adapters.base.meta import available
 from dbt.adapters.postgres import PostgresAdapter
 from dbt.adapters.timescaledb.timescaledb_connection_manager import (
     NO_TRANSACTION_MARKER,
     TimescaleDBConnectionManager,
 )
 from dbt.adapters.timescaledb.timescaledb_index_config import TimescaleDBIndexConfig
+from dbt.adapters.timescaledb.timescaledb_relation import TimescaleDBRelation
 
 
 class TimescaleDBAdapter(PostgresAdapter):
     ConnectionManager = TimescaleDBConnectionManager
+    Relation = TimescaleDBRelation
 
     @available
     def parse_index(self, raw_index: Any) -> Optional[TimescaleDBIndexConfig]:
         return TimescaleDBIndexConfig.parse(raw_index)
 
     @available
     def marker_run_outside_transaction(self) -> str:
```

### Comparing `dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_connection_manager.py` & `dbt_timescaledb-1.8.0b1/dbt/adapters/timescaledb/timescaledb_connection_manager.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/dbt/adapters/timescaledb/timescaledb_index_config.py` & `dbt_timescaledb-1.8.0b1/dbt/adapters/timescaledb/timescaledb_index_config.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/adapters.sql` & `dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/materializations/models/continuous_aggregate.sql` & `dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/materializations/models/continuous_aggregate.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/materializations/models/hypertable.sql` & `dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/materializations/models/hypertable.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/materializations/models/virtual_hypertable.sql` & `dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/materializations/models/virtual_hypertable.sql`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 {% materialization virtual_hypertable, adapter="timescaledb" %}
 
     {%- set target_relation = this.incorporate(type=this.Table) -%}
-
+    {%- set existing_relation = load_cached_relation(target_relation) -%}
+    {%- set change_collection = get_virtual_hypertable_change_collection(existing_relation, config) -%}
     {%- set grant_config = config.get('grants') -%}
     {{ run_hooks(pre_hooks, inside_transaction=False) }}
 
     -- `BEGIN` happens here:
     {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
     -- build model
@@ -18,35 +19,29 @@
             {{ add_compression_policy(target_relation, config.get("compression")) }}
         {% endif -%}
 
         {%- if config.get("integer_now_func") %}
             {{ set_integer_now_func(target_relation, config.get("integer_now_func"), config.get("integer_now_func_sql")) }}
         {% endif -%}
 
-    {%- endcall %}
-
-    {% do create_indexes(target_relation) %}
+        {%- if change_collection %}
+            {{ timescaledb__update_indexes_on_virtual_hypertable(target_relation, change_collection.indexes) }}
+        {%- endif %}
+
+        {{ clear_reorder_policy(target_relation) }}
+        {%- if config.get("reorder_policy") %}
+                {{ add_reorder_policy(target_relation, config.get("reorder_policy")) }}
+        {% endif -%}
 
-    {%- call statement("clear_reorder_policy") %}
-      {{ clear_reorder_policy(target_relation) }}
-    {% endcall -%}
-    {%- if config.get("reorder_policy") %}
-        {% call statement("reorder_policy") %}
-            {{ add_reorder_policy(target_relation, config.get("reorder_policy")) }}
-        {% endcall %}
-    {% endif -%}
-
-    {%- call statement("clear_retention_policy") %}
-      {{ clear_retention_policy(target_relation) }}
-    {% endcall -%}
-    {%- if config.get("retention_policy") %}
-        {% call statement("retention_policy") %}
+        {{ clear_retention_policy(target_relation) }}
+        {%- if config.get("retention_policy") %}
             {{ add_retention_policy(target_relation, config.get("retention_policy")) }}
-        {% endcall %}
-    {% endif -%}
+        {% endif -%}
+
+    {%- endcall %}
 
     {{ run_hooks(post_hooks, inside_transaction=True) }}
 
     {% set should_revoke = should_revoke(target_relation, full_refresh_mode=True) %}
     {% do apply_grants(target_relation, grant_config, should_revoke=should_revoke) %}
 
     {% do persist_docs(target_relation, model) %}
```

### Comparing `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/compression.sql` & `dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/relations/compression.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/continuous_aggregate.sql` & `dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/relations/continuous_aggregate.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/dimensions.sql` & `dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/relations/dimensions.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/reorder_policy.sql` & `dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/relations/reorder_policy.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/dbt/include/timescaledb/macros/relations/retention_policy.sql` & `dbt_timescaledb-1.8.0b1/dbt/include/timescaledb/macros/relations/retention_policy.sql`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/pyproject.toml` & `dbt_timescaledb-1.8.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Microsoft :: Windows",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
     "Programming Language :: Python :: 3.11",
 ]
-version = "1.8.0a4"
+version = "1.8.0b1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://dbt-timescaledb.debruyn.dev"
 Repository = "https://github.com/sdebruyn/dbt-timescaledb"
```

### Comparing `dbt_timescaledb-1.8.0a4/tests/conftest.py` & `dbt_timescaledb-1.8.0b1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_compression.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_compression.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_index.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_index.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_refresh_policy.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_refresh_policy.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_retention_policy.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/continuous_aggregate/test_continuous_aggregate_retention_policy.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/hypertable/test_hypertable.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_compression.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/hypertable/test_hypertable_compression.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_dimension.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/hypertable/test_hypertable_dimension.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_index.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/hypertable/test_hypertable_index.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_hypertable_integer_now_func.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/hypertable/test_hypertable_integer_now_func.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/hypertable/test_reorder_policy.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/hypertable/test_reorder_policy.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/test_basic.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/test_basic.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/test_retention_policy.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/test_retention_policy.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_compression.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_compression.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_integer_now_func.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_integer_now_func.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_reorder_policy.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_reorder_policy.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_retention_policy.py` & `dbt_timescaledb-1.8.0b1/tests/functional/adapter/virtual_hypertable/test_virtual_hypertable_retention_policy.py`

 * *Files identical despite different names*

### Comparing `dbt_timescaledb-1.8.0a4/PKG-INFO` & `dbt_timescaledb-1.8.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-timescaledb
-Version: 1.8.0a4
+Version: 1.8.0b1
 Summary: The TimescaleDB adapter plugin for dbt
 Keywords: dbt timescaledb
 Author-Email: Sam Debruyn <dbt.sam@debruyn.dev>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
```

