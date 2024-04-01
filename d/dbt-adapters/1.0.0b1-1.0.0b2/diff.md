# Comparing `tmp/dbt_adapters-1.0.0b1.tar.gz` & `tmp/dbt_adapters-1.0.0b2.tar.gz`

## Comparing `dbt_adapters-1.0.0b1.tar` & `dbt_adapters-1.0.0b2.tar`

### file list

```diff
@@ -1,154 +1,154 @@
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/__init__.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/__about__.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/__init__.py
--rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/cache.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/capability.py
--rw-r--r--   0        0        0     9043 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/factory.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/protocol.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/py.typed
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/reference_keys.py
--rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/utils.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/base/README.md
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/base/__init__.py
--rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/base/column.py
--rw-r--r--   0        0        0    16907 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/base/connections.py
--rw-r--r--   0        0        0    63791 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/base/impl.py
--rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/base/meta.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/base/plugin.py
--rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/base/query_headers.py
--rw-r--r--   0        0        0    15582 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/base/relation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/clients/__init__.py
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/clients/jinja.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/contracts/__init__.py
--rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/contracts/connection.py
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/contracts/macros.py
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/contracts/relation.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/events/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/events/__init__.py
--rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/events/adapter_types.proto
--rw-r--r--   0        0        0    26048 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/events/adapter_types_pb2.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/events/base_types.py
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/events/logging.py
--rw-r--r--   0        0        0    11726 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/events/types.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/exceptions/__init__.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/exceptions/alias.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/exceptions/cache.py
--rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/exceptions/compilation.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/exceptions/connection.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/exceptions/database.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/relation_configs/README.md
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/relation_configs/__init__.py
--rw-r--r--   0        0        0     1714 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/relation_configs/config_base.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/relation_configs/config_change.py
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/relation_configs/config_validation.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/sql/__init__.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/sql/connections.py
--rw-r--r--   0        0        0    10648 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/adapters/sql/impl.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/py.typed
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/__init__.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/dbt_project.yml
--rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/docs/overview.md
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/show.sql
--rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/timestamps.sql
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/validate_sql.sql
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/etc/statement.sql
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/generic_test_sql/unique.sql
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/hooks.sql
--rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/materialized_view.sql
--rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/table.sql
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/view.sql
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
--rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/clone/clone.sql
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
--rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/seeds/seed.sql
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/tests/unit.sql
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/python_model/python.sql
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/create.sql
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/create_backup.sql
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/create_intermediate.sql
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/drop.sql
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/drop_backup.sql
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/rename.sql
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/rename_intermediate.sql
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/replace.sql
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/schema.sql
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql
--rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/materialized_view/alter.sql
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/materialized_view/create.sql
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/materialized_view/drop.sql
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/materialized_view/refresh.sql
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/materialized_view/rename.sql
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/materialized_view/replace.sql
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/table/create.sql
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/table/drop.sql
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/table/rename.sql
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/table/replace.sql
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/view/create.sql
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/view/drop.sql
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/view/rename.sql
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/view/replace.sql
--rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/cast.sql
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/date_spine.sql
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/generate_series.sql
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/split_part.sql
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/.gitignore
--rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/LICENSE
--rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/README.md
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/__init__.py
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/__about__.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/__init__.py
+-rw-r--r--   0        0        0    20084 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/cache.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/capability.py
+-rw-r--r--   0        0        0     9021 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/factory.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/protocol.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/py.typed
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/reference_keys.py
+-rw-r--r--   0        0        0     2414 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/utils.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/README.md
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/__init__.py
+-rw-r--r--   0        0        0     5450 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/column.py
+-rw-r--r--   0        0        0    16921 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/connections.py
+-rw-r--r--   0        0        0    64403 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/impl.py
+-rw-r--r--   0        0        0     4644 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/meta.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/plugin.py
+-rw-r--r--   0        0        0     3496 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/query_headers.py
+-rw-r--r--   0        0        0    15642 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/base/relation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/clients/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/clients/jinja.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/contracts/__init__.py
+-rw-r--r--   0        0        0     6860 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/contracts/connection.py
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/contracts/macros.py
+-rw-r--r--   0        0        0     4652 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/contracts/relation.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/__init__.py
+-rw-r--r--   0        0        0     9484 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/adapter_types.proto
+-rw-r--r--   0        0        0    26048 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/adapter_types_pb2.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/base_types.py
+-rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/logging.py
+-rw-r--r--   0        0        0    11726 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/events/types.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/exceptions/__init__.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/exceptions/alias.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/exceptions/cache.py
+-rw-r--r--   0        0        0     8586 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/exceptions/compilation.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/exceptions/connection.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/exceptions/database.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/README.md
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/__init__.py
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/config_base.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/config_change.py
+-rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/config_validation.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/sql/__init__.py
+-rw-r--r--   0        0        0     6565 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/sql/connections.py
+-rw-r--r--   0        0        0    10722 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/adapters/sql/impl.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/py.typed
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/__init__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/dbt_project.yml
+-rw-r--r--   0        0        0     1824 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/docs/overview.md
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0        0        0     5438 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/show.sql
+-rw-r--r--   0        0        0     1482 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/timestamps.sql
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/validate_sql.sql
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/etc/statement.sql
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/generic_test_sql/unique.sql
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/hooks.sql
+-rw-r--r--   0        0        0     5011 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/materialized_view.sql
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/table.sql
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/view.sql
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/clone/can_clone_table.sql
+-rw-r--r--   0        0        0     2698 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/clone/clone.sql
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/clone/create_or_replace_clone.sql
+-rw-r--r--   0        0        0     2577 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0        0        0     4235 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0        0        0     5197 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/seeds/seed.sql
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0        0        0     3680 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/unit.sql
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/python_model/python.sql
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/create.sql
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/create_backup.sql
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/create_intermediate.sql
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/drop.sql
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/drop_backup.sql
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/rename.sql
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/rename_intermediate.sql
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/replace.sql
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/schema.sql
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql
+-rw-r--r--   0        0        0     1806 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/alter.sql
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/create.sql
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/drop.sql
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/refresh.sql
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/rename.sql
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/replace.sql
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/table/create.sql
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/table/drop.sql
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/table/rename.sql
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/table/replace.sql
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/view/create.sql
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/view/drop.sql
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/view/rename.sql
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/view/replace.sql
+-rw-r--r--   0        0        0     3841 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/cast.sql
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0        0        0     4416 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/date_spine.sql
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/generate_series.sql
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/split_part.sql
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0        0        0     2716 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/.gitignore
+-rw-r--r--   0        0        0    11344 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/README.md
+-rw-r--r--   0        0        0     4233 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 dbt_adapters-1.0.0b2/PKG-INFO
```

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/cache.py` & `dbt_adapters-1.0.0b2/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/capability.py` & `dbt_adapters-1.0.0b2/dbt/adapters/capability.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/factory.py` & `dbt_adapters-1.0.0b2/dbt/adapters/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,17 +96,15 @@
 
         return plugin.credentials
 
     def register_adapter(self, config: AdapterRequiredConfig, mp_context: SpawnContext) -> None:
         adapter_name = config.credentials.type
         adapter_type = self.get_adapter_class_by_name(adapter_name)
         adapter_version = self._adapter_version(adapter_name)
-        fire_event(
-            AdapterRegistered(adapter_name=adapter_name, adapter_version=adapter_version)
-        )
+        fire_event(AdapterRegistered(adapter_name=adapter_name, adapter_version=adapter_version))
         with self.lock:
             if adapter_name in self.adapters:
                 # this shouldn't really happen...
                 return
 
             adapter: Adapter = adapter_type(config, mp_context)  # type: ignore
             self.adapters[adapter_name] = adapter
```

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/protocol.py` & `dbt_adapters-1.0.0b2/dbt/adapters/protocol.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,29 +6,32 @@
     Generic,
     Hashable,
     List,
     Optional,
     Type,
     TypeVar,
     Tuple,
+    TYPE_CHECKING,
 )
 from typing_extensions import Protocol
 
-import agate
 from dbt_common.clients.jinja import MacroProtocol
 from dbt_common.contracts.config.base import BaseConfig
 
 from dbt.adapters.contracts.connection import (
     AdapterRequiredConfig,
     AdapterResponse,
     Connection,
 )
 from dbt.adapters.contracts.macros import MacroResolverProtocol
 from dbt.adapters.contracts.relation import HasQuoting, Policy, RelationConfig
 
+if TYPE_CHECKING:
+    import agate
+
 
 @dataclass
 class AdapterConfig(BaseConfig):
     pass
 
 
 class ConnectionManagerProtocol(Protocol):
@@ -165,9 +168,9 @@
         ...
 
     def commit_if_has_connection(self) -> None:
         ...
 
     def execute(
         self, sql: str, auto_begin: bool = False, fetch: bool = False
-    ) -> Tuple[AdapterResponse, agate.Table]:
+    ) -> Tuple[AdapterResponse, "agate.Table"]:
         ...
```

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/reference_keys.py` & `dbt_adapters-1.0.0b2/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/utils.py` & `dbt_adapters-1.0.0b2/dbt/adapters/utils.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/base/README.md` & `dbt_adapters-1.0.0b2/dbt/adapters/base/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/base/column.py` & `dbt_adapters-1.0.0b2/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/base/connections.py` & `dbt_adapters-1.0.0b2/dbt/adapters/base/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     Hashable,
     Iterable,
     List,
     Optional,
     Tuple,
     Type,
     Union,
+    TYPE_CHECKING,
 )
 
-import agate
 from dbt_common.events.contextvars import get_node_info
 from dbt_common.events.functions import fire_event
 from dbt_common.exceptions import DbtInternalError, NotImplementedError
 from dbt_common.utils import cast_to_str
 
 from dbt.adapters.base.query_headers import MacroQueryStringSetter
 from dbt.adapters.contracts.connection import (
@@ -44,14 +44,17 @@
     ConnectionReused,
     NewConnection,
     Rollback,
     RollbackFailed,
 )
 from dbt.adapters.exceptions import FailedToConnectError, InvalidConnectionError
 
+if TYPE_CHECKING:
+    import agate
+
 
 SleepTime = Union[int, float]  # As taken by time.sleep.
 AdapterHandle = Any  # Adapter connection handle objects can be any class.
 
 
 class BaseConnectionManager(metaclass=abc.ABCMeta):
     """Methods to implement:
@@ -158,17 +161,15 @@
                 transaction_open=False,
                 handle=None,
                 credentials=self.profile.credentials,
             )
             conn.handle = LazyHandle(self.open)
             # Add the connection to thread_connections for this thread
             self.set_thread_connection(conn)
-            fire_event(
-                NewConnection(conn_name=conn_name, conn_type=self.TYPE, node_info=get_node_info())
-            )
+            fire_event(NewConnection(conn_name=conn_name, conn_type=self.TYPE, node_info=get_node_info()))
         else:  # existing connection either wasn't open or didn't have the right name
             if conn.state != "open":
                 conn.handle = LazyHandle(self.open)
             if conn.name != conn_name:
                 orig_conn_name: str = conn.name or ""
                 conn.name = conn_name
                 fire_event(ConnectionReused(orig_conn_name=orig_conn_name, conn_name=conn_name))
@@ -392,15 +393,15 @@
     @abc.abstractmethod
     def execute(
         self,
         sql: str,
         auto_begin: bool = False,
         fetch: bool = False,
         limit: Optional[int] = None,
-    ) -> Tuple[AdapterResponse, agate.Table]:
+    ) -> Tuple[AdapterResponse, "agate.Table"]:
         """Execute the given SQL.
 
         :param str sql: The sql to execute.
         :param bool auto_begin: If set, and dbt is not currently inside a
             transaction, automatically begin one.
         :param bool fetch: If set, fetch results.
         :param int limit: If set, limits the result set
```

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/base/impl.py` & `dbt_adapters-1.0.0b2/dbt/adapters/base/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,24 +16,17 @@
     Mapping,
     Optional,
     Set,
     Tuple,
     Type,
     TypedDict,
     Union,
+    TYPE_CHECKING,
 )
 
-import agate
-from dbt_common.clients.agate_helper import (
-    Integer,
-    empty_table,
-    get_column_value_uncased,
-    merge_tables,
-    table_from_rows,
-)
 from dbt_common.clients.jinja import CallableMacroGenerator
 from dbt_common.contracts.constraints import (
     ColumnLevelConstraint,
     ConstraintType,
     ModelLevelConstraint,
 )
 from dbt_common.exceptions import (
@@ -90,44 +83,54 @@
     RenameToNoneAttemptedError,
     SnapshotTargetIncompleteError,
     SnapshotTargetNotSnapshotTableError,
     UnexpectedNonTimestampError,
 )
 from dbt.adapters.protocol import AdapterConfig, MacroContextGeneratorCallable
 
+if TYPE_CHECKING:
+    import agate
+
 
 GET_CATALOG_MACRO_NAME = "get_catalog"
 GET_CATALOG_RELATIONS_MACRO_NAME = "get_catalog_relations"
 FRESHNESS_MACRO_NAME = "collect_freshness"
 GET_RELATION_LAST_MODIFIED_MACRO_NAME = "get_relation_last_modified"
 
 
 class ConstraintSupport(str, Enum):
     ENFORCED = "enforced"
     NOT_ENFORCED = "not_enforced"
     NOT_SUPPORTED = "not_supported"
 
 
-def _expect_row_value(key: str, row: agate.Row):
+def _parse_callback_empty_table(*args, **kwargs) -> Tuple[str, "agate.Table"]:
+    # Lazy load agate_helper to avoid importing agate when it is not necessary.
+    from dbt_common.clients.agate_helper import empty_table
+
+    return "", empty_table()
+
+
+def _expect_row_value(key: str, row: "agate.Row"):
     if key not in row.keys():
         raise DbtInternalError(
             'Got a row without "{}" column, columns: {}'.format(key, row.keys())
         )
     return row[key]
 
 
 def _catalog_filter_schemas(
     used_schemas: FrozenSet[Tuple[str, str]]
-) -> Callable[[agate.Row], bool]:
+) -> Callable[["agate.Row"], bool]:
     """Return a function that takes a row and decides if the row should be
     included in the catalog output.
     """
     schemas = frozenset((d.lower(), s.lower()) for d, s in used_schemas)
 
-    def test(row: agate.Row) -> bool:
+    def test(row: "agate.Row") -> bool:
         table_database = _expect_row_value("table_database", row)
         table_schema = _expect_row_value("table_schema", row)
         # the schema may be present but None, which is not an error and should
         # be filtered out
         if table_schema is None:
             return False
         return (table_database.lower(), table_schema.lower()) in schemas
@@ -250,14 +253,16 @@
         ConstraintType.check: ConstraintSupport.NOT_SUPPORTED,
         ConstraintType.not_null: ConstraintSupport.ENFORCED,
         ConstraintType.unique: ConstraintSupport.NOT_ENFORCED,
         ConstraintType.primary_key: ConstraintSupport.NOT_ENFORCED,
         ConstraintType.foreign_key: ConstraintSupport.ENFORCED,
     }
 
+    MAX_SCHEMA_METADATA_RELATIONS = 100
+
     # This static member variable can be overriden in concrete adapter
     # implementations to indicate adapter support for optional capabilities.
     _capabilities = CapabilityDict({})
 
     def __init__(self, config, mp_context: SpawnContext) -> None:
         self.config = config
         self.cache = RelationsCache(log_cache_events=config.log_cache_events)
@@ -319,32 +324,32 @@
             self.acquire_connection(name)
             yield
         finally:
             self.release_connection()
             if self.connections.query_header is not None:
                 self.connections.query_header.reset()
 
-    @available.parse(lambda *a, **k: ("", empty_table()))
+    @available.parse(_parse_callback_empty_table)
     def execute(
         self,
         sql: str,
         auto_begin: bool = False,
         fetch: bool = False,
         limit: Optional[int] = None,
-    ) -> Tuple[AdapterResponse, agate.Table]:
+    ) -> Tuple[AdapterResponse, "agate.Table"]:
         """Execute the given SQL. This is a thin wrapper around
         ConnectionManager.execute.
 
         :param str sql: The sql to execute.
         :param bool auto_begin: If set, and dbt is not currently inside a
             transaction, automatically begin one.
         :param bool fetch: If set, fetch results.
         :param Optional[int] limit: If set, only fetch n number of rows
         :return: A tuple of the query status and results (empty if fetch=False).
-        :rtype: Tuple[AdapterResponse, agate.Table]
+        :rtype: Tuple[AdapterResponse, "agate.Table"]
         """
         return self.connections.execute(sql=sql, auto_begin=auto_begin, fetch=fetch, limit=limit)
 
     def validate_sql(self, sql: str) -> AdapterResponse:
         """Submit the given SQL to the engine for validation, but not execution.
 
         This should throw an appropriate exception if the input SQL is invalid, although
@@ -364,24 +369,24 @@
                 column_name, self.connections.data_type_code_to_name(column_type_code)
             )
             # https://peps.python.org/pep-0249/#description
             for column_name, column_type_code, *_ in cursor.description
         ]
         return columns
 
-    @available.parse(lambda *a, **k: ("", empty_table()))
-    def get_partitions_metadata(self, table: str) -> Tuple[agate.Table]:
+    @available.parse(_parse_callback_empty_table)
+    def get_partitions_metadata(self, table: str) -> Tuple["agate.Table"]:
         """
         TODO: Can we move this to dbt-bigquery?
         Obtain partitions metadata for a BigQuery partitioned table.
 
         :param str table: a partitioned table id, in standard SQL format.
         :return: a partition metadata tuple, as described in
             https://cloud.google.com/bigquery/docs/creating-partitioned-tables#getting_partition_metadata_using_meta_tables.
-        :rtype: agate.Table
+        :rtype: "agate.Table"
         """
         if hasattr(self.connections, "get_partitions_metadata"):
             return self.connections.get_partitions_metadata(table=table)
         else:
             raise NotImplementedError(
                 "`get_partitions_metadata` is not implemented for this adapter!"
             )
@@ -417,15 +422,17 @@
             return True
 
     def _get_cache_schemas(self, relation_configs: Iterable[RelationConfig]) -> Set[BaseRelation]:
         """Get the set of schema relations that the cache logic needs to
         populate.
         """
         return {
-            self.Relation.create_from(quoting=self.config, relation_config=relation_config).without_identifier()
+            self.Relation.create_from(
+                quoting=self.config, relation_config=relation_config
+            ).without_identifier()
             for relation_config in relation_configs
         }
 
     def _get_catalog_schemas(self, relation_configs: Iterable[RelationConfig]) -> SchemaSearchMap:
         """Get a mapping of each node's "information_schema" relations to a
         set of all schemas expected in that information_schema.
 
@@ -659,15 +666,15 @@
             "`list_relations_without_caching` is not implemented for this adapter!"
         )
 
     ###
     # Methods about grants
     ###
     @available
-    def standardize_grants_dict(self, grants_table: agate.Table) -> dict:
+    def standardize_grants_dict(self, grants_table: "agate.Table") -> dict:
         """Translate the result of `show grants` (or equivalent) to match the
         grants which a user would configure in their project.
 
         Ideally, the SQL to show grants should also be filtering:
         filter OUT any grants TO the current user/role (e.g. OWNERSHIP).
         If that's not possible in SQL, it can be done in this method instead.
 
@@ -934,102 +941,105 @@
 
     ###
     # Conversions: These must be implemented by concrete implementations, for
     # converting agate types into their sql equivalents.
     ###
     @classmethod
     @abc.abstractmethod
-    def convert_text_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_text_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         """Return the type in the database that best maps to the agate.Text
         type for the given agate table and column index.
 
         :param agate_table: The table
         :param col_idx: The index into the agate table for the column.
         :return: The name of the type in the database
         """
         raise NotImplementedError("`convert_text_type` is not implemented for this adapter!")
 
     @classmethod
     @abc.abstractmethod
-    def convert_number_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_number_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         """Return the type in the database that best maps to the agate.Number
         type for the given agate table and column index.
 
         :param agate_table: The table
         :param col_idx: The index into the agate table for the column.
         :return: The name of the type in the database
         """
         raise NotImplementedError("`convert_number_type` is not implemented for this adapter!")
 
     @classmethod
-    def convert_integer_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_integer_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         """Return the type in the database that best maps to the agate.Number
         type for the given agate table and column index.
 
         :param agate_table: The table
         :param col_idx: The index into the agate table for the column.
         :return: The name of the type in the database
         """
         return "integer"
 
     @classmethod
     @abc.abstractmethod
-    def convert_boolean_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_boolean_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         """Return the type in the database that best maps to the agate.Boolean
         type for the given agate table and column index.
 
         :param agate_table: The table
         :param col_idx: The index into the agate table for the column.
         :return: The name of the type in the database
         """
         raise NotImplementedError("`convert_boolean_type` is not implemented for this adapter!")
 
     @classmethod
     @abc.abstractmethod
-    def convert_datetime_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_datetime_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         """Return the type in the database that best maps to the agate.DateTime
         type for the given agate table and column index.
 
         :param agate_table: The table
         :param col_idx: The index into the agate table for the column.
         :return: The name of the type in the database
         """
         raise NotImplementedError("`convert_datetime_type` is not implemented for this adapter!")
 
     @classmethod
     @abc.abstractmethod
-    def convert_date_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_date_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         """Return the type in the database that best maps to the agate.Date
         type for the given agate table and column index.
 
         :param agate_table: The table
         :param col_idx: The index into the agate table for the column.
         :return: The name of the type in the database
         """
         raise NotImplementedError("`convert_date_type` is not implemented for this adapter!")
 
     @classmethod
     @abc.abstractmethod
-    def convert_time_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_time_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         """Return the type in the database that best maps to the
         agate.TimeDelta type for the given agate table and column index.
 
         :param agate_table: The table
         :param col_idx: The index into the agate table for the column.
         :return: The name of the type in the database
         """
         raise NotImplementedError("`convert_time_type` is not implemented for this adapter!")
 
     @available
     @classmethod
-    def convert_type(cls, agate_table: agate.Table, col_idx: int) -> Optional[str]:
+    def convert_type(cls, agate_table: "agate.Table", col_idx: int) -> Optional[str]:
         return cls.convert_agate_type(agate_table, col_idx)
 
     @classmethod
-    def convert_agate_type(cls, agate_table: agate.Table, col_idx: int) -> Optional[str]:
+    def convert_agate_type(cls, agate_table: "agate.Table", col_idx: int) -> Optional[str]:
+        import agate
+        from dbt_common.clients.agate_helper import Integer
+
         agate_type: Type = agate_table.column_types[col_idx]
         conversions: List[Tuple[Type, Callable[..., str]]] = [
             (Integer, cls.convert_integer_type),
             (agate.Text, cls.convert_text_type),
             (agate.Number, cls.convert_number_type),
             (agate.Boolean, cls.convert_boolean_type),
             (agate.DateTime, cls.convert_datetime_type),
@@ -1098,45 +1108,47 @@
 
         with self.connections.exception_handler(f"macro {macro_name}"):
             result = macro_function(**kwargs)
         return result
 
     @classmethod
     def _catalog_filter_table(
-        cls, table: agate.Table, used_schemas: FrozenSet[Tuple[str, str]]
-    ) -> agate.Table:
+        cls, table: "agate.Table", used_schemas: FrozenSet[Tuple[str, str]]
+    ) -> "agate.Table":
         """Filter the table as appropriate for catalog entries. Subclasses can
         override this to change filtering rules on a per-adapter basis.
         """
+        from dbt_common.clients.agate_helper import table_from_rows
+
         # force database + schema to be strings
         table = table_from_rows(
             table.rows,
             table.column_names,
             text_only_columns=["table_database", "table_schema", "table_name"],
         )
         return table.where(_catalog_filter_schemas(used_schemas))
 
     def _get_one_catalog(
         self,
         information_schema: InformationSchema,
         schemas: Set[str],
         used_schemas: FrozenSet[Tuple[str, str]],
-    ) -> agate.Table:
+    ) -> "agate.Table":
         kwargs = {"information_schema": information_schema, "schemas": schemas}
         table = self.execute_macro(GET_CATALOG_MACRO_NAME, kwargs=kwargs)
 
         results = self._catalog_filter_table(table, used_schemas)  # type: ignore[arg-type]
         return results
 
     def _get_one_catalog_by_relations(
         self,
         information_schema: InformationSchema,
         relations: List[BaseRelation],
         used_schemas: FrozenSet[Tuple[str, str]],
-    ) -> agate.Table:
+    ) -> "agate.Table":
         kwargs = {
             "information_schema": information_schema,
             "relations": relations,
         }
         table = self.execute_macro(GET_CATALOG_RELATIONS_MACRO_NAME, kwargs=kwargs)
 
         results = self._catalog_filter_table(table, used_schemas)  # type: ignore[arg-type]
@@ -1144,18 +1156,18 @@
 
     def get_filtered_catalog(
         self,
         relation_configs: Iterable[RelationConfig],
         used_schemas: FrozenSet[Tuple[str, str]],
         relations: Optional[Set[BaseRelation]] = None,
     ):
-        catalogs: agate.Table
+        catalogs: "agate.Table"
         if (
             relations is None
-            or len(relations) > 100
+            or len(relations) > self.MAX_SCHEMA_METADATA_RELATIONS
             or not self.supports(Capability.SchemaMetadataByRelations)
         ):
             # Do it the traditional way. We get the full catalog.
             catalogs, exceptions = self.get_catalog(relation_configs, used_schemas)
         else:
             # Do it the new way. We try to save time by selecting information
             # only for the exact set of relations we are interested in.
@@ -1167,37 +1179,37 @@
                     r.database.casefold() if r.database else None,
                     r.schema.casefold() if r.schema else None,
                     r.identifier.casefold() if r.identifier else None,
                 )
                 for r in relations
             }
 
-            def in_map(row: agate.Row):
+            def in_map(row: "agate.Row"):
                 d = _expect_row_value("table_database", row)
                 s = _expect_row_value("table_schema", row)
                 i = _expect_row_value("table_name", row)
                 d = d.casefold() if d is not None else None
                 s = s.casefold() if s is not None else None
                 i = i.casefold() if i is not None else None
                 return (d, s, i) in relation_map
 
             catalogs = catalogs.where(in_map)
 
         return catalogs, exceptions
 
-    def row_matches_relation(self, row: agate.Row, relations: Set[BaseRelation]):
+    def row_matches_relation(self, row: "agate.Row", relations: Set[BaseRelation]):
         pass
 
     def get_catalog(
         self,
         relation_configs: Iterable[RelationConfig],
         used_schemas: FrozenSet[Tuple[str, str]],
-    ) -> Tuple[agate.Table, List[Exception]]:
+    ) -> Tuple["agate.Table", List[Exception]]:
         with executor(self.config) as tpe:
-            futures: List[Future[agate.Table]] = []
+            futures: List[Future["agate.Table"]] = []
             schema_map: SchemaSearchMap = self._get_catalog_schemas(relation_configs)
             for info, schemas in schema_map.items():
                 if len(schemas) == 0:
                     continue
                 name = ".".join([str(info.database), "information_schema"])
                 fut = tpe.submit_connected(
                     self, name, self._get_one_catalog, info, schemas, used_schemas
@@ -1205,17 +1217,17 @@
                 futures.append(fut)
 
         catalogs, exceptions = catch_as_completed(futures)
         return catalogs, exceptions
 
     def get_catalog_by_relations(
         self, used_schemas: FrozenSet[Tuple[str, str]], relations: Set[BaseRelation]
-    ) -> Tuple[agate.Table, List[Exception]]:
+    ) -> Tuple["agate.Table", List[Exception]]:
         with executor(self.config) as tpe:
-            futures: List[Future[agate.Table]] = []
+            futures: List[Future["agate.Table"]] = []
             relations_by_schema = self._get_catalog_relations_by_info_schema(relations)
             for info_schema in relations_by_schema:
                 name = ".".join([str(info_schema.database), "information_schema"])
                 relations = set(relations_by_schema[info_schema])
                 fut = tpe.submit_connected(
                     self,
                     name,
@@ -1237,26 +1249,28 @@
         self,
         source: BaseRelation,
         loaded_at_field: str,
         filter: Optional[str],
         macro_resolver: Optional[MacroResolverProtocol] = None,
     ) -> Tuple[Optional[AdapterResponse], FreshnessResponse]:
         """Calculate the freshness of sources in dbt, and return it"""
+        import agate
+
         kwargs: Dict[str, Any] = {
             "source": source,
             "loaded_at_field": loaded_at_field,
             "filter": filter,
         }
 
         # run the macro
         # in older versions of dbt-core, the 'collect_freshness' macro returned the table of results directly
         # starting in v1.5, by default, we return both the table and the adapter response (metadata about the query)
         result: Union[
-            AttrDict,  # current: contains AdapterResponse + agate.Table
-            agate.Table,  # previous: just table
+            AttrDict,  # current: contains AdapterResponse + "agate.Table"
+            "agate.Table",  # previous: just table
         ]
         result = self.execute_macro(
             FRESHNESS_MACRO_NAME, kwargs=kwargs, macro_resolver=macro_resolver
         )
         if isinstance(result, agate.Table):
             warn_or_error(CollectFreshnessReturnSignature())
             adapter_response = None
@@ -1296,14 +1310,16 @@
             GET_RELATION_LAST_MODIFIED_MACRO_NAME,
             kwargs=kwargs,
             macro_resolver=macro_resolver,
         )
         adapter_response, table = result.response, result.table  # type: ignore[attr-defined]
 
         try:
+            from dbt_common.clients.agate_helper import get_column_value_uncased
+
             row = table[0]
             last_modified_val = get_column_value_uncased("last_modified", row)
             snapshotted_at_val = get_column_value_uncased("snapshotted_at", row)
         except Exception:
             raise MacroResultError(GET_RELATION_LAST_MODIFIED_MACRO_NAME, table)
 
         if last_modified_val is None:
@@ -1632,18 +1648,20 @@
     diff_count.num_missing as num_mismatched
 from row_count_diff
 join diff_count using (id)
 """.strip()
 
 
 def catch_as_completed(
-    futures,  # typing: List[Future[agate.Table]]
-) -> Tuple[agate.Table, List[Exception]]:
-    # catalogs: agate.Table = agate.Table(rows=[])
-    tables: List[agate.Table] = []
+    futures,  # typing: List[Future["agate.Table"]]
+) -> Tuple["agate.Table", List[Exception]]:
+    from dbt_common.clients.agate_helper import merge_tables
+
+    # catalogs: "agate.Table" =".Table(rows=[])
+    tables: List["agate.Table"] = []
     exceptions: List[Exception] = []
 
     for future in as_completed(futures):
         exc = future.exception()
         # we want to re-raise on ctrl+c and BaseException
         if exc is None:
             catalog = future.result()
```

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/base/meta.py` & `dbt_adapters-1.0.0b2/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/base/plugin.py` & `dbt_adapters-1.0.0b2/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/base/query_headers.py` & `dbt_adapters-1.0.0b2/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/base/relation.py` & `dbt_adapters-1.0.0b2/dbt/adapters/base/relation.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,21 +48,21 @@
     dbt_created: bool = False
     limit: Optional[int] = None
 
     # register relation types that can be renamed for the purpose of replacing relations using stages and backups
     # adding a relation type here also requires defining the associated rename macro
     # e.g. adding RelationType.View in dbt-postgres requires that you define:
     # include/postgres/macros/relations/view/rename.sql::postgres__get_rename_view_sql()
-    renameable_relations: SerializableIterable = ()
+    renameable_relations: SerializableIterable = field(default_factory=frozenset)
 
     # register relation types that are atomically replaceable, e.g. they have "create or replace" syntax
     # adding a relation type here also requires defining the associated replace macro
     # e.g. adding RelationType.View in dbt-postgres requires that you define:
     # include/postgres/macros/relations/view/replace.sql::postgres__get_replace_view_sql()
-    replaceable_relations: SerializableIterable = ()
+    replaceable_relations: SerializableIterable = field(default_factory=frozenset)
 
     def _is_exactish_match(self, field: ComponentName, value: str) -> bool:
         if self.dbt_created and self.quote_policy.get_part(field) is False:
             return self.path.get_lowered_part(field) == value.lower()
         else:
             return self.path.get_part(field) == value
```

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/clients/jinja.py` & `dbt_adapters-1.0.0b2/dbt/adapters/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/contracts/connection.py` & `dbt_adapters-1.0.0b2/dbt/adapters/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/contracts/relation.py` & `dbt_adapters-1.0.0b2/dbt/adapters/contracts/relation.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,19 +44,23 @@
         ...
 
     def __delitem__(self, key):
         ...
 
 
 class RelationConfig(Protocol):
+    resource_type: str
     name: str
+    description: str
     database: str
     schema: str
     identifier: str
     compiled_code: Optional[str]
+    meta: Dict[str, Any]
+    tags: List[str]
     quoting_dict: Dict[str, bool]
     config: Optional[MaterializationConfig]
 
 
 class ComponentName(StrEnum):
     Database = "database"
     Schema = "schema"
```

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/events/README.md` & `dbt_adapters-1.0.0b2/dbt/adapters/events/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/events/adapter_types.proto` & `dbt_adapters-1.0.0b2/dbt/adapters/events/adapter_types.proto`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/events/adapter_types_pb2.py` & `dbt_adapters-1.0.0b2/dbt/adapters/events/adapter_types_pb2.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/events/base_types.py` & `dbt_adapters-1.0.0b2/dbt/adapters/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/events/logging.py` & `dbt_adapters-1.0.0b2/dbt/adapters/events/logging.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/events/types.py` & `dbt_adapters-1.0.0b2/dbt/adapters/events/types.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/exceptions/__init__.py` & `dbt_adapters-1.0.0b2/dbt/adapters/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/exceptions/alias.py` & `dbt_adapters-1.0.0b2/dbt/adapters/exceptions/alias.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/exceptions/cache.py` & `dbt_adapters-1.0.0b2/dbt/adapters/exceptions/cache.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/exceptions/compilation.py` & `dbt_adapters-1.0.0b2/dbt/adapters/exceptions/compilation.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/exceptions/database.py` & `dbt_adapters-1.0.0b2/dbt/adapters/exceptions/database.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/relation_configs/README.md` & `dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/relation_configs/config_base.py` & `dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/config_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from dataclasses import dataclass
-from typing import Dict, Union
+from typing import Dict, Union, TYPE_CHECKING
 
-import agate
 from dbt_common.utils import filter_null_values
 
+if TYPE_CHECKING:
+    import agate
+
 
 """
 This is what relation metadata from the database looks like. It's a dictionary because there will be
 multiple grains of data for a single object. For example, a materialized view in Postgres has base level information,
 like name. But it also can have multiple indexes, which needs to be a separate query. It might look like this:
 
 {
     "base": agate.Row({"table_name": "table_abc", "query": "select * from table_def"})
     "indexes": agate.Table("rows": [
         agate.Row({"name": "index_a", "columns": ["column_a"], "type": "hash", "unique": False}),
         agate.Row({"name": "index_b", "columns": ["time_dim_a"], "type": "btree", "unique": False}),
     ])
 }
 """
-RelationResults = Dict[str, Union[agate.Row, agate.Table]]
+RelationResults = Dict[str, Union["agate.Row", "agate.Table"]]
 
 
 @dataclass(frozen=True)
 class RelationConfigBase:
     @classmethod
     def from_dict(cls, kwargs_dict) -> "RelationConfigBase":
         """
```

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/relation_configs/config_change.py` & `dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/config_change.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/relation_configs/config_validation.py` & `dbt_adapters-1.0.0b2/dbt/adapters/relation_configs/config_validation.py`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/sql/connections.py` & `dbt_adapters-1.0.0b2/dbt/adapters/sql/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import abc
 import time
-from typing import Any, Dict, Iterable, List, Optional, Tuple
+from typing import Any, Dict, Iterable, List, Optional, Tuple, TYPE_CHECKING
 
-import agate
-from dbt_common.clients.agate_helper import empty_table, table_from_data_flat
 from dbt_common.events.contextvars import get_node_info
 from dbt_common.events.functions import fire_event
 from dbt_common.exceptions import DbtInternalError, NotImplementedError
 from dbt_common.utils import cast_to_str
 
 from dbt.adapters.base import BaseConnectionManager
 from dbt.adapters.contracts.connection import (
@@ -18,14 +16,17 @@
 from dbt.adapters.events.types import (
     ConnectionUsed,
     SQLCommit,
     SQLQuery,
     SQLQueryStatus,
 )
 
+if TYPE_CHECKING:
+    import agate
+
 
 class SQLConnectionManager(BaseConnectionManager):
     """The default connection manager with some common SQL methods implemented.
 
     Methods to implement:
         - exception_handler
         - cancel
@@ -122,15 +123,17 @@
                 column_names[idx] = f"{col_name}_{unique_col_names[col_name]}"  # type: ignore[index] # noqa
             else:
                 # TODO CT-211
                 unique_col_names[column_names[idx]] = 1  # type: ignore[index]
         return [dict(zip(column_names, row)) for row in rows]
 
     @classmethod
-    def get_result_from_cursor(cls, cursor: Any, limit: Optional[int]) -> agate.Table:
+    def get_result_from_cursor(cls, cursor: Any, limit: Optional[int]) -> "agate.Table":
+        from dbt_common.clients.agate_helper import table_from_data_flat
+
         data: List[Any] = []
         column_names: List[str] = []
 
         if cursor.description is not None:
             column_names = [col[0] for col in cursor.description]
             if limit:
                 rows = cursor.fetchmany(limit)
@@ -142,15 +145,17 @@
 
     def execute(
         self,
         sql: str,
         auto_begin: bool = False,
         fetch: bool = False,
         limit: Optional[int] = None,
-    ) -> Tuple[AdapterResponse, agate.Table]:
+    ) -> Tuple[AdapterResponse, "agate.Table"]:
+        from dbt_common.clients.agate_helper import empty_table
+
         sql = self._add_query_comment(sql)
         _, cursor = self.add_query(sql, auto_begin)
         response = self.get_response(cursor)
         if fetch:
             table = self.get_result_from_cursor(cursor, limit)
         else:
             table = empty_table()
```

### Comparing `dbt_adapters-1.0.0b1/dbt/adapters/sql/impl.py` & `dbt_adapters-1.0.0b2/dbt/adapters/sql/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from typing import Any, List, Optional, Tuple, Type
+from typing import Any, List, Optional, Tuple, Type, TYPE_CHECKING
 
-import agate
 from dbt_common.events.functions import fire_event
 
 from dbt.adapters.base import BaseAdapter, BaseRelation, available
 from dbt.adapters.cache import _make_ref_key_dict
 from dbt.adapters.contracts.connection import AdapterResponse, Connection
 from dbt.adapters.events.types import ColTypeChange, SchemaCreation, SchemaDrop
 from dbt.adapters.exceptions import RelationTypeNullError
@@ -19,14 +18,17 @@
 DROP_SCHEMA_MACRO_NAME = "drop_schema"
 RENAME_RELATION_MACRO_NAME = "rename_relation"
 TRUNCATE_RELATION_MACRO_NAME = "truncate_relation"
 DROP_RELATION_MACRO_NAME = "drop_relation"
 ALTER_COLUMN_TYPE_MACRO_NAME = "alter_column_type"
 VALIDATE_SQL_MACRO_NAME = "validate_sql"
 
+if TYPE_CHECKING:
+    import agate
+
 
 class SQLAdapter(BaseAdapter):
     """The default adapter with the common agate conversions and some SQL
     methods was implemented. This adapter has a different much shorter list of
     methods to implement, but some more macros that must be implemented.
 
     To implement a macro, implement "${adapter_type}__${macro_name}". in the
@@ -61,41 +63,43 @@
         :param bindings: An optional list of bindings for the query.
         :param abridge_sql_log: If set, limit the raw sql logged to 512
             characters
         """
         return self.connections.add_query(sql, auto_begin, bindings, abridge_sql_log)
 
     @classmethod
-    def convert_text_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_text_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         return "text"
 
     @classmethod
-    def convert_number_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_number_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
+        import agate
+
         # TODO CT-211
         decimals = agate_table.aggregate(agate.MaxPrecision(col_idx))  # type: ignore[attr-defined]
         return "float8" if decimals else "integer"
 
     @classmethod
-    def convert_integer_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_integer_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         return "integer"
 
     @classmethod
-    def convert_boolean_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_boolean_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         return "boolean"
 
     @classmethod
-    def convert_datetime_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_datetime_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         return "timestamp without time zone"
 
     @classmethod
-    def convert_date_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_date_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         return "date"
 
     @classmethod
-    def convert_time_type(cls, agate_table: agate.Table, col_idx: int) -> str:
+    def convert_time_type(cls, agate_table: "agate.Table", col_idx: int) -> str:
         return "time"
 
     @classmethod
     def is_cancelable(cls) -> bool:
         return True
 
     def expand_column_types(self, goal, current):
```

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/docs/overview.md` & `dbt_adapters-1.0.0b2/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/columns.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/indexes.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/relation.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/schema.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/show.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/show.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/etc/datetime.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/etc/statement.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/configs.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/materialized_view.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/materialized_view.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/table.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/table.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/view.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/view.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/clone/clone.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/clone/clone.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/materializations/tests/unit.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/materializations/tests/unit.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/python_model/python.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/create.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/create_backup.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/create_backup.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/create_intermediate.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/create_intermediate.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/drop.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/drop.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/rename.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/rename.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/replace.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/column/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/materialized_view/alter.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/alter.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/materialized_view/drop.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/materialized_view/drop.sql`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {# /*
 This was already implemented. Instead of creating a new macro that aligns with the standard,
 this was reused and the default was maintained. This gets called by `drop_relation`, which
 actually executes the drop, and `get_drop_sql`, which returns the template.
 */ #}
 
 {% macro drop_materialized_view(relation) -%}
-    {{ return(adapter.dispatch('drop_materialized_view', 'dbt')(relation)) }}
+    {{- adapter.dispatch('drop_materialized_view', 'dbt')(relation) -}}
 {%- endmacro %}
 
 
 {% macro default__drop_materialized_view(relation) -%}
     drop materialized view if exists {{ relation }} cascade
 {%- endmacro %}
```

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/table/create.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/table/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/view/create.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/view/create.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/relations/view/replace.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/relations/view/replace.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/unit_test_sql/get_fixture_sql.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/data_types.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/date_spine.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/date_spine.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/generate_series.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/generate_series.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/listagg.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/macros/utils/split_part.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/dbt/include/global_project/tests/generic/builtin.sql` & `dbt_adapters-1.0.0b2/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/.gitignore` & `dbt_adapters-1.0.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/LICENSE` & `dbt_adapters-1.0.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/README.md` & `dbt_adapters-1.0.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt_adapters-1.0.0b1/pyproject.toml` & `dbt_adapters-1.0.0b2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -138,14 +138,15 @@
 mypy_path = "third-party-stubs/"
 files = [
     "dbt",
     "tests/unit",
 ]
 exclude = [
     "dbt/adapters/events/adapter_types_pb2.py",
+    "dbt-tests-adapter/dbt/__init__.py",  # overlaps with `dbt/__init__.py` as expected for namespaces
     "venv",
 ]
 [[tool.mypy.overrides]]
 module = ["dbt.adapters.events.adapter_types_pb2"]
 follow_imports = "skip"
 
 [tool.pytest]
```

### Comparing `dbt_adapters-1.0.0b1/PKG-INFO` & `dbt_adapters-1.0.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dbt-adapters
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: The set of adapter protocols and base functionality that supports integration with dbt-core
 Project-URL: Homepage, https://github.com/dbt-labs/dbt-adapters
 Project-URL: Documentation, https://docs.getdbt.com
 Project-URL: Repository, https://github.com/dbt-labs/dbt-adapters.git
 Project-URL: Issues, https://github.com/dbt-labs/dbt-adapters/issues
 Project-URL: Changelog, https://github.com/dbt-labs/dbt-adapters/blob/main/CHANGELOG.md
 Author-email: dbt Labs <info@dbtlabs.com>
```

