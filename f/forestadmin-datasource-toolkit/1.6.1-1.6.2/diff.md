# Comparing `tmp/forestadmin_datasource_toolkit-1.6.1.tar.gz` & `tmp/forestadmin_datasource_toolkit-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forestadmin_datasource_toolkit-1.6.1.tar", max compression
+gzip compressed data, was "forestadmin_datasource_toolkit-1.6.2.tar", max compression
```

## Comparing `forestadmin_datasource_toolkit-1.6.1.tar` & `forestadmin_datasource_toolkit-1.6.2.tar`

### file list

```diff
@@ -1,147 +1,147 @@
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/README.md
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/__init__.py
--rw-r--r--   0        0        0     3538 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/collections.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/context/__init__.py
--rw-r--r--   0        0        0      678 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/context/agent_context.py
--rw-r--r--   0        0        0      658 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/context/collection_context.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
--rw-r--r--   0        0        0     7190 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
--rw-r--r--   0        0        0    29444 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py
--rw-r--r--   0        0        0     5335 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py
--rw-r--r--   0        0        0      320 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/datasource_customizer/types.py
--rw-r--r--   0        0        0     1658 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/datasources.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/__init__.py
--rw-r--r--   0        0        0     5941 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/collections.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
--rw-r--r--   0        0        0     2251 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/context/base.py
--rw-r--r--   0        0        0      591 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
--rw-r--r--   0        0        0      950 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/context/single.py
--rw-r--r--   0        0        0     4758 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/result_builder.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
--rw-r--r--   0        0        0     1360 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/types/actions.py
--rw-r--r--   0        0        0    22687 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/types/fields.py
--rw-r--r--   0        0        0     6215 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/types/widgets.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/binary/__init__.py
--rw-r--r--   0        0        0     9653 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/binary/collection.py
--rw-r--r--   0        0        0      295 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/binary/utils.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/chart/__init__.py
--rw-r--r--   0        0        0     1963 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py
--rw-r--r--   0        0        0     2133 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py
--rw-r--r--   0        0        0     1549 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py
--rw-r--r--   0        0        0     7673 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/chart/result_builder.py
--rw-r--r--   0        0        0      728 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/chart/types.py
--rw-r--r--   0        0        0     5355 2024-03-22 10:40:32.423445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/collection_decorator.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/computed/__init__.py
--rw-r--r--   0        0        0     5310 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/computed/collections.py
--rw-r--r--   0        0        0      154 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
--rw-r--r--   0        0        0     3916 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/computed/helpers.py
--rw-r--r--   0        0        0      748 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/computed/types.py
--rw-r--r--   0        0        0     2812 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/computed/utils.py
--rw-r--r--   0        0        0     1666 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/datasource_decorator.py
--rw-r--r--   0        0        0     5079 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/decorator_stack.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/empty/__init__.py
--rw-r--r--   0        0        0     4495 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/empty/collection.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/__init__.py
--rw-r--r--   0        0        0     4841 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/collections.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/__init__.py
--rw-r--r--   0        0        0     1233 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/aggregate.py
--rw-r--r--   0        0        0      870 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/create.py
--rw-r--r--   0        0        0      599 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/delete.py
--rw-r--r--   0        0        0      525 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/hooks.py
--rw-r--r--   0        0        0     1153 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/list.py
--rw-r--r--   0        0        0      777 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/update.py
--rw-r--r--   0        0        0      852 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/hooks.py
--rw-r--r--   0        0        0      392 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/types.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/operators_emulate/__init__.py
--rw-r--r--   0        0        0     6521 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py
--rw-r--r--   0        0        0      371 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/operators_emulate/types.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/operators_equivalence/__init__.py
--rw-r--r--   0        0        0     3855 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/publication/__init__.py
--rw-r--r--   0        0        0     3866 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/publication/collections.py
--rw-r--r--   0        0        0     2421 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/publication/datasource.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/relation/__init__.py
--rw-r--r--   0        0        0    12558 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/relation/collections.py
--rw-r--r--   0        0        0     1125 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/relation/types.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/rename_collection/__init__.py
--rw-r--r--   0        0        0     1041 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/rename_collection/collection.py
--rw-r--r--   0        0        0     2897 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/rename_collection/datasource.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/rename_field/__init__.py
--rw-r--r--   0        0        0    10161 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/rename_field/collections.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/schema/__init__.py
--rw-r--r--   0        0        0      671 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/schema/collection.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/search/__init__.py
--rw-r--r--   0        0        0     6164 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/search/collections.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/segments/__init__.py
--rw-r--r--   0        0        0     2627 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/segments/collections.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/sort_emulate/__init__.py
--rw-r--r--   0        0        0     6009 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/sort_emulate/collections.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/validation/__init__.py
--rw-r--r--   0        0        0     4019 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/validation/collection.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/create_relations/__init__.py
--rw-r--r--   0        0        0     4987 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/update_relations/__init__.py
--rw-r--r--   0        0        0     4845 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py
--rw-r--r--   0        0        0     1020 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/write_replace/__init__.py
--rw-r--r--   0        0        0      420 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/write_replace/types.py
--rw-r--r--   0        0        0      932 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py
--rw-r--r--   0        0        0     6436 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py
--rw-r--r--   0        0        0     2331 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/exceptions.py
--rw-r--r--   0        0        0     6148 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/__init__.py
--rw-r--r--   0        0        0     3364 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/actions.py
--rw-r--r--   0        0        0     1141 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/chart.py
--rw-r--r--   0        0        0     2463 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/collections.py
--rw-r--r--   0        0        0     5160 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/fields.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/models/__init__.py
--rw-r--r--   0        0        0     1304 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/models/collections.py
--rw-r--r--   0        0        0     6148 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/__init__.py
--rw-r--r--   0        0        0     7885 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
--rw-r--r--   0        0        0     6148 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
--rw-r--r--   0        0        0     4505 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
--rw-r--r--   0        0        0     5340 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
--rw-r--r--   0        0        0     2696 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
--rw-r--r--   0        0        0     4745 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
--rw-r--r--   0        0        0     9753 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
--rw-r--r--   0        0        0     1270 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
--rw-r--r--   0        0        0     3836 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
--rw-r--r--   0        0        0     1688 2024-03-22 10:40:32.427445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
--rw-r--r--   0        0        0     7643 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
--rw-r--r--   0        0        0     8081 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
--rw-r--r--   0        0        0     2889 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
--rw-r--r--   0        0        0     3110 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
--rw-r--r--   0        0        0      759 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/page.py
--rw-r--r--   0        0        0     4442 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
--rw-r--r--   0        0        0      902 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
--rw-r--r--   0        0        0     2455 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
--rw-r--r--   0        0        0      595 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
--rw-r--r--   0        0        0      118 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/records.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/plugins/__init__.py
--rw-r--r--   0        0        0     2514 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/plugins/add_external_relation.py
--rw-r--r--   0        0        0     4353 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/plugins/import_field.py
--rw-r--r--   0        0        0      395 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/plugins/plugin.py
--rw-r--r--   0        0        0       73 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/utils/__init__.py
--rw-r--r--   0        0        0     8601 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/utils/collections.py
--rw-r--r--   0        0        0     2559 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/utils/operators.py
--rw-r--r--   0        0        0     1169 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/utils/records.py
--rw-r--r--   0        0        0     1878 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/utils/schema.py
--rw-r--r--   0        0        0      449 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/utils/user_callable.py
--rw-r--r--   0        0        0        0 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/__init__.py
--rw-r--r--   0        0        0     4790 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/condition_tree.py
--rw-r--r--   0        0        0     4231 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/field.py
--rw-r--r--   0        0        0      393 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/projection.py
--rw-r--r--   0        0        0     1542 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/records.py
--rw-r--r--   0        0        0     4573 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/rules.py
--rw-r--r--   0        0        0      469 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/sort.py
--rw-r--r--   0        0        0     4649 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/type_getter.py
--rw-r--r--   0        0        0      372 2024-03-22 10:40:32.431445 forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/types.py
--rw-r--r--   0        0        0     1567 2024-03-22 10:40:48.735492 forestadmin_datasource_toolkit-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      966 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/__init__.py
+-rw-r--r--   0        0        0     3538 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/collections.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/__init__.py
+-rw-r--r--   0        0        0      678 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/agent_context.py
+-rw-r--r--   0        0        0      658 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/collection_context.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/relaxed_wrappers/__init__.py
+-rw-r--r--   0        0        0     7240 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py
+-rw-r--r--   0        0        0    29444 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py
+-rw-r--r--   0        0        0     5404 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py
+-rw-r--r--   0        0        0      279 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasource_customizer/types.py
+-rw-r--r--   0        0        0     1658 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasources.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/__init__.py
+-rw-r--r--   0        0        0     5983 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/collections.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/__init__.py
+-rw-r--r--   0        0        0     2276 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/base.py
+-rw-r--r--   0        0        0      591 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/bulk.py
+-rw-r--r--   0        0        0      974 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/single.py
+-rw-r--r--   0        0        0     4677 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/result_builder.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/__init__.py
+-rw-r--r--   0        0        0     1360 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/actions.py
+-rw-r--r--   0        0        0    22709 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/fields.py
+-rw-r--r--   0        0        0     6215 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/widgets.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/binary/__init__.py
+-rw-r--r--   0        0        0     9653 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/binary/collection.py
+-rw-r--r--   0        0        0      295 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/binary/utils.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/__init__.py
+-rw-r--r--   0        0        0     2216 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py
+-rw-r--r--   0        0        0     2362 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py
+-rw-r--r--   0        0        0     1567 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py
+-rw-r--r--   0        0        0     7890 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/result_builder.py
+-rw-r--r--   0        0        0      728 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/types.py
+-rw-r--r--   0        0        0     5355 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/collection_decorator.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/__init__.py
+-rw-r--r--   0        0        0     5310 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/collections.py
+-rw-r--r--   0        0        0      154 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/exceptions.py
+-rw-r--r--   0        0        0     3916 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/helpers.py
+-rw-r--r--   0        0        0      748 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/types.py
+-rw-r--r--   0        0        0     2812 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/utils.py
+-rw-r--r--   0        0        0     1666 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/datasource_decorator.py
+-rw-r--r--   0        0        0     5079 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/decorator_stack.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/empty/__init__.py
+-rw-r--r--   0        0        0     4495 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/empty/collection.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/__init__.py
+-rw-r--r--   0        0        0     4841 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/collections.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/__init__.py
+-rw-r--r--   0        0        0     1233 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/aggregate.py
+-rw-r--r--   0        0        0      870 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/create.py
+-rw-r--r--   0        0        0      599 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/delete.py
+-rw-r--r--   0        0        0      525 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/hooks.py
+-rw-r--r--   0        0        0     1153 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/list.py
+-rw-r--r--   0        0        0      777 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/update.py
+-rw-r--r--   0        0        0      852 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/hooks.py
+-rw-r--r--   0        0        0      392 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/types.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_emulate/__init__.py
+-rw-r--r--   0        0        0     6521 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py
+-rw-r--r--   0        0        0      371 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_emulate/types.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_equivalence/__init__.py
+-rw-r--r--   0        0        0     3855 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/publication/__init__.py
+-rw-r--r--   0        0        0     3866 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/publication/collections.py
+-rw-r--r--   0        0        0     2421 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/publication/datasource.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/relation/__init__.py
+-rw-r--r--   0        0        0    12558 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/relation/collections.py
+-rw-r--r--   0        0        0     1125 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/relation/types.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_collection/__init__.py
+-rw-r--r--   0        0        0     1041 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_collection/collection.py
+-rw-r--r--   0        0        0     2897 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_collection/datasource.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_field/__init__.py
+-rw-r--r--   0        0        0    10161 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_field/collections.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.650600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/schema/__init__.py
+-rw-r--r--   0        0        0      671 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/schema/collection.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/search/__init__.py
+-rw-r--r--   0        0        0     6164 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/search/collections.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/segments/__init__.py
+-rw-r--r--   0        0        0     2627 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/segments/collections.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/sort_emulate/__init__.py
+-rw-r--r--   0        0        0     6009 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/sort_emulate/collections.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/validation/__init__.py
+-rw-r--r--   0        0        0     4019 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/validation/collection.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/create_relations/__init__.py
+-rw-r--r--   0        0        0     4987 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/update_relations/__init__.py
+-rw-r--r--   0        0        0     4845 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py
+-rw-r--r--   0        0        0     1020 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_replace/__init__.py
+-rw-r--r--   0        0        0      420 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_replace/types.py
+-rw-r--r--   0        0        0      932 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py
+-rw-r--r--   0        0        0     6436 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py
+-rw-r--r--   0        0        0     2331 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/exceptions.py
+-rw-r--r--   0        0        0     6148 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/__init__.py
+-rw-r--r--   0        0        0     3551 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/actions.py
+-rw-r--r--   0        0        0     1141 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/chart.py
+-rw-r--r--   0        0        0     2463 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/collections.py
+-rw-r--r--   0        0        0     5160 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/fields.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/models/__init__.py
+-rw-r--r--   0        0        0     1346 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/models/collections.py
+-rw-r--r--   0        0        0     6148 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/__init__.py
+-rw-r--r--   0        0        0     7998 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/aggregation.py
+-rw-r--r--   0        0        0     6148 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/__init__.py
+-rw-r--r--   0        0        0     4505 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py
+-rw-r--r--   0        0        0     5340 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/__init__.py
+-rw-r--r--   0        0        0     2696 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py
+-rw-r--r--   0        0        0     4844 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py
+-rw-r--r--   0        0        0     9918 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py
+-rw-r--r--   0        0        0     1270 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/__init__.py
+-rw-r--r--   0        0        0     3836 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py
+-rw-r--r--   0        0        0     1688 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py
+-rw-r--r--   0        0        0     7643 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/__init__.py
+-rw-r--r--   0        0        0     8081 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py
+-rw-r--r--   0        0        0     2889 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py
+-rw-r--r--   0        0        0     3110 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py
+-rw-r--r--   0        0        0      759 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/page.py
+-rw-r--r--   0        0        0     4442 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py
+-rw-r--r--   0        0        0      902 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py
+-rw-r--r--   0        0        0     2455 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py
+-rw-r--r--   0        0        0      595 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py
+-rw-r--r--   0        0        0      118 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/records.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/plugins/__init__.py
+-rw-r--r--   0        0        0     2514 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/plugins/add_external_relation.py
+-rw-r--r--   0        0        0     4353 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/plugins/import_field.py
+-rw-r--r--   0        0        0      395 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/plugins/plugin.py
+-rw-r--r--   0        0        0       73 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/__init__.py
+-rw-r--r--   0        0        0     8601 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/collections.py
+-rw-r--r--   0        0        0     2559 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/operators.py
+-rw-r--r--   0        0        0     1169 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/records.py
+-rw-r--r--   0        0        0     1878 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/schema.py
+-rw-r--r--   0        0        0      449 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/user_callable.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/__init__.py
+-rw-r--r--   0        0        0     4790 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/condition_tree.py
+-rw-r--r--   0        0        0     4231 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/field.py
+-rw-r--r--   0        0        0      393 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/projection.py
+-rw-r--r--   0        0        0     1542 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/records.py
+-rw-r--r--   0        0        0     4573 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/rules.py
+-rw-r--r--   0        0        0      469 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/sort.py
+-rw-r--r--   0        0        0     4649 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/type_getter.py
+-rw-r--r--   0        0        0      372 2024-04-02 07:31:20.654600 forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/types.py
+-rw-r--r--   0        0        0     1567 2024-04-02 07:31:36.310502 forestadmin_datasource_toolkit-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0      966 1970-01-01 00:00:00.000000 forestadmin_datasource_toolkit-1.6.2/PKG-INFO
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/context/agent_context.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/agent_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/context/collection_context.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/collection_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/context/relaxed_wrappers/collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         raise RelaxedDatasourceException("Cannot modify existing datasources")
 
 
 class RelaxedCollection(Collection):
     def __init__(self, collection: Collection):
         self.collection = collection
 
-    def get_native_driver(self):
+    def get_native_driver(self) -> Any:
         return self.collection.get_native_driver()
 
     @property
     def datasource(self) -> Datasource[Self]:
         self.collection.datasource
         return RelaxedDatasource(self.collection.datasource)
 
@@ -127,15 +127,18 @@
     def _build_aggregation(self, aggregation: Union[Aggregation, PlainAggregation]) -> Aggregation:
         if is_aggregation(aggregation):
             return aggregation
         aggregation = cast(PlainAggregation, aggregation)
         return Aggregation(aggregation)
 
     async def list(
-        self, caller: User, filter_: Union[PaginatedFilter, PlainPaginatedFilter], projection: Projection
+        self,
+        caller: User,
+        filter_: Union[PaginatedFilter, PlainPaginatedFilter],
+        projection: Union[Projection, List[str]],
     ) -> List[RecordsDataAlias]:
         filter_instance = self._build_paginated_filter(filter_)
         projection_instance = self._build_projection(projection)
 
         return await self.collection.list(caller, filter_instance, projection_instance)
 
     async def update(
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasource_customizer/collection_customizer.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasource_customizer/datasource_customizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Optional
+from typing import Dict, Optional
 
 from forestadmin.datasource_toolkit.datasource_customizer.collection_customizer import CollectionCustomizer
 from forestadmin.datasource_toolkit.datasource_customizer.types import DataSourceOptions
 from forestadmin.datasource_toolkit.datasources import Datasource
 from forestadmin.datasource_toolkit.decorators.chart.types import DataSourceChartDefinition
 from forestadmin.datasource_toolkit.decorators.decorator_stack import DecoratorStack
 from forestadmin.datasource_toolkit.decorators.publication.datasource import PublicationDataSourceDecorator
@@ -32,27 +32,28 @@
     def add_datasource(self, datasource: Datasource, options: Optional[DataSourceOptions] = None) -> Self:
         """Add a datasource
 
         Args:
             datasource (Datasource): the datasource to add
             options (DataSourceOptions, optional): the options
         """
-        if options is None:
-            options = {}
+        _options: DataSourceOptions = DataSourceOptions() if options is None else options
 
         async def _add_datasource():
             nonlocal datasource
-            if "include" in options or "exclude" in options:
+            if "include" in _options or "exclude" in _options:
                 publication_decorator = PublicationDataSourceDecorator(datasource)
-                publication_decorator.keep_collections_matching(options.get("include", []), options.get("exclude", []))
+                publication_decorator.keep_collections_matching(
+                    _options.get("include", []), _options.get("exclude", [])
+                )
                 datasource = publication_decorator
 
-            if "rename" in options:
+            if "rename" in _options:
                 rename_decorator = RenameCollectionDataSourceDecorator(datasource)
-                rename_decorator.rename_collections(options.get("rename", {}))
+                rename_decorator.rename_collections(_options.get("rename", {}))
                 datasource = rename_decorator
 
             for collection in datasource.collections:
                 self.composite_datasource.add_collection(collection)
 
         self.stack.queue_customization(_add_datasource)
         return self
@@ -98,15 +99,15 @@
 
         async def _add_chart():
             self.stack.chart.add_chart(name, definition)
 
         self.stack.queue_customization(_add_chart)
         return self
 
-    def remove_collections(self, *names: List[str]) -> Self:
+    def remove_collections(self, *names: str) -> Self:
         """Remove collections from the exported schema (they will still be usable within the agent).
 
         Args:
             names (List[str]): the collections to remove
 
         Documentation:
             https://docs.forestadmin.com/developer-guide-agents-python/agent-customization/agent-customization#removing-collections
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/datasources.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/datasources.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,17 @@
         action = self._actions.get(name)
         if not action:
             return await super().execute(caller, name, data, filter_)  # type: ignore
 
         context = self._get_context(caller, action, data, filter_, None)
         response_builder = ResultBuilder()
         result = await call_user_function(action["execute"], context, response_builder)  # type: ignore
-        return result or {"type": "Success", "invalidated": set(), "format": "text", "message": "Success"}
+        return cast(
+            ActionResult, result or {"type": "Success", "invalidated": set(), "format": "text", "message": "Success"}
+        )
 
     async def get_form(
         self,
         caller: User,
         name: str,
         data: Optional[RecordsDataAlias],
         filter_: Optional[Filter] = None,
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/context/base.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, List, Optional, Set
+from typing import Any, Dict, List, Optional, Set, Union
 
 from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.collections import Collection
 from forestadmin.datasource_toolkit.context.collection_context import CollectionCustomizationContext
 from forestadmin.datasource_toolkit.interfaces.query.filter.paginated import PaginatedFilter
 from forestadmin.datasource_toolkit.interfaces.query.filter.unpaginated import Filter
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
@@ -43,14 +43,14 @@
         self.filter = filter
         self._changed_field = changed_field
 
     def has_field_changed(self, field_name):
         self.form_values._used.add(field_name)
         return field_name == self._changed_field
 
-    async def get_records(self, fields: Projection) -> List[RecordsDataAlias]:
+    async def get_records(self, fields: Union[Projection, List[str]]) -> List[RecordsDataAlias]:
         ProjectionValidator.validate(self.collection, fields)
         projection = Projection(*fields)
         return await self._run_query(projection)
 
     async def _run_query(self, projection: Projection) -> List[RecordsDataAlias]:
         return await self.collection.list(self._caller, PaginatedFilter.from_base_filter(self.filter), projection)
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/context/bulk.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/bulk.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/context/single.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/context/single.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Union
+from typing import List, Optional, Union
 
 from forestadmin.datasource_toolkit.decorators.action.context.base import ActionContext
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
 from forestadmin.datasource_toolkit.utils.records import RecordUtils
 
 
@@ -11,10 +11,10 @@
         projection = Projection().with_pks(self.collection)
         records = await self.get_records(projection)
         if len(records) == 0:
             return None
         ret = RecordUtils.get_primary_key(self.collection.schema, records[0])
         return ret[0] if len(ret) > 0 else None
 
-    async def get_record(self, fields: Projection) -> RecordsDataAlias:
+    async def get_record(self, fields: Union[Projection, List[str]]) -> RecordsDataAlias:
         records = await self.get_records(fields)
         return records[0] if len(records) > 0 else None  # type: ignore
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/result_builder.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/result_builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from io import IOBase
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import Any, Dict, List, Literal, Optional
 
 from forestadmin.datasource_toolkit.interfaces.actions import ActionResult
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
 from typing_extensions import NotRequired, Self, TypedDict
 
-OptionTypeAlias = Union[Literal["html"], Literal["text"]]
-WebhookMethod = Union[Literal["GET"], Literal["POST"]]
+OptionTypeAlias = Literal["html", "text"]
+WebhookMethod = Literal["GET", "POST"]
 
 
 class OptionAlias(TypedDict):
     type: NotRequired[OptionTypeAlias]
     invalidated: NotRequired[List[str]]
 
 
@@ -45,15 +45,15 @@
         """Returns a success response from the action
 
         Args:
             message (str, optional): the success message to return. Defaults to None.
             options (dict, optional): available options to return. Defaults to None.
 
         Example:
-            .success("Success", {"html": "<blinkee>Success!</blinkee>"})
+            .success("Success", {"type": "html"})
         """
         if not options:
             options = {}
 
         return {
             "type": self.SUCCESS,
             "message": message or self.SUCCESS,
@@ -66,15 +66,15 @@
         """Returns an error response from the action
 
         Args:
             message (str, optional): the error message to return. Defaults to None.
             options (dict, optional): available options to return. Defaults to None.
 
         Example:
-            .error("Failed to refund the customer!", {"html": "<strong>Error!</strong>"})
+            .error("Failed to refund the customer!", {"type": "html"})
         """
         if not options:
             options = {}
         return {
             "type": self.ERROR,
             "message": message or self.ERROR,
             "format": options.get("type", "text"),
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/types/actions.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/actions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/types/fields.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     def dynamic_fields(self):
         ret = [getattr(self, f"_{field}") for field in BaseDynamicField.ATTR_TO_EVALUATE]
         if len(self._widget_fields) > 0:
             ret.extend(self._widget_fields.get(widget_attr) for widget_attr in BaseDynamicField.WIDGET_ATTR_TO_EVALUATE)
         return ret
 
     @property
-    def is_dynamic(self):
+    def is_dynamic(self) -> bool:
         return any(map(lambda x: isinstance(x, Callable), self.dynamic_fields))
 
     async def to_action_field(
         self, context: Context, default_value: Result, search_value: Optional[str] = None
     ) -> ActionField:
         field = ActionField(
             type=self.TYPE,
@@ -146,15 +146,15 @@
         if self._widget_fields.get("search", "") == "dynamic":
             return await call_user_function(self._widget_fields["options"], context, search_value)
         else:
             return await self._evaluate(context, attribute)
 
 
 class PlainCollectionDynamicField(PlainField):
-    type: Literal[ActionFieldType.COLLECTION]
+    type: Literal[ActionFieldType.COLLECTION, "Collection"]
     collection_name: ValueOrHandler[str]
     value: NotRequired[ValueOrHandler[CompositeIdAlias]]
     default_value: NotRequired[ValueOrHandler[CompositeIdAlias]]
 
 
 # collection
 class CollectionDynamicField(BaseDynamicField[CompositeIdAlias]):
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/action/types/widgets.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/action/types/widgets.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/binary/collection.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/binary/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/chart_collection_decorator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Any, Dict, List
+from urllib.parse import quote
 
+from forestadmin.agent_toolkit.forest_logger import ForestLogger
 from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.collections import CollectionException
 from forestadmin.datasource_toolkit.decorators.chart.collection_chart_context import CollectionChartContext
 from forestadmin.datasource_toolkit.decorators.chart.result_builder import ResultBuilder
 from forestadmin.datasource_toolkit.decorators.chart.types import CollectionChartDefinition
 from forestadmin.datasource_toolkit.decorators.collection_decorator import CollectionDecorator
 from forestadmin.datasource_toolkit.interfaces.chart import Chart
@@ -17,14 +19,16 @@
         super().__init__(*args, **kwargs)
 
     def add_chart(self, name: str, definition: CollectionChartDefinition):
         if name in self.schema["charts"].keys():
             raise CollectionException(f"Chart {name} already exists.")
 
         self._charts[name] = definition
+        chart_url = quote(f"/forest/_charts/{self.name}/{name}")
+        ForestLogger.log("info", f"Chart {self.name}.{name} added with url: '{chart_url}'")
         self.mark_schema_as_dirty()
 
     async def render_chart(self, caller: User, name: str, record_id: List) -> Chart:
         if self._charts.get(name) is not None:
             context = CollectionChartContext(caller, self, record_id)
             result_builder = ResultBuilder()
             ret = await call_user_function(self._charts[name], context, result_builder, record_id)
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/chart_datasource_decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from typing import Dict, Union
+from urllib.parse import quote
 
+from forestadmin.agent_toolkit.forest_logger import ForestLogger
 from forestadmin.agent_toolkit.utils.context import User
 from forestadmin.datasource_toolkit.context.agent_context import AgentCustomizationContext
 from forestadmin.datasource_toolkit.datasources import Datasource
 from forestadmin.datasource_toolkit.decorators.chart.chart_collection_decorator import ChartCollectionDecorator
 from forestadmin.datasource_toolkit.decorators.chart.result_builder import ResultBuilder
 from forestadmin.datasource_toolkit.decorators.chart.types import DataSourceChartDefinition
 from forestadmin.datasource_toolkit.decorators.datasource_decorator import DatasourceDecorator
@@ -17,14 +19,16 @@
         super().__init__(child_datasource, ChartCollectionDecorator)
         self.charts: Dict[str, DataSourceChartDefinition] = dict()
 
     def add_chart(self, name: str, chart_definition: DataSourceChartDefinition):
         if name in self.schema["charts"]:
             raise DatasourceToolkitException(f"Chart {name} already exists.")
         self.charts[name] = chart_definition
+        chart_url = quote(f"/forest/_charts/{name}")
+        ForestLogger.log("info", f"Chart {name} added with url: '{chart_url}'")
 
     async def render_chart(self, caller: User, name: str) -> Chart:
         chart_definition = self.charts.get(name)
 
         if chart_definition is not None:
             return await call_user_function(chart_definition, AgentCustomizationContext(self, caller), ResultBuilder)
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/collection_chart_context.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 
     async def get_record_id(self) -> Union[str, int]:
         if len(self.composite_record_id) > 1:
             raise DatasourceToolkitException("Collection is using a composite pk: use 'context.composite_record_id'.")
 
         return self.composite_record_id[0]
 
-    async def get_record(self, fields: Projection) -> RecordsDataAlias:
+    async def get_record(self, fields: Union[Projection, List[str]]) -> RecordsDataAlias:
         condition_tree = ConditionTreeFactory.match_ids(self.collection.schema, [self.composite_record_id])
 
         records = await self.collection.list(self._caller, PaginatedFilter({"condition_tree": condition_tree}), fields)
         return records[0]
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/chart/result_builder.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/result_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MultipleTimeBasedChart,
     ObjectiveChart,
     PercentageChart,
     SmartChart,
     TimeBasedChart,
     ValueChart,
 )
-from forestadmin.datasource_toolkit.interfaces.query.aggregation import DateOperation
+from forestadmin.datasource_toolkit.interfaces.query.aggregation import DateOperation, DateOperationLiteral
 from forestadmin.datasource_toolkit.interfaces.query.condition_tree.transforms.time import Frequency
 
 
 class _DateRangeFrequency(enum.Enum):
     Day: str = "days"
     Week: str = "weeks"
     Month: str = "months"
@@ -66,15 +66,17 @@
 
     @staticmethod
     def distribution(obj: Dict[str, Union[int, float]]) -> DistributionChart:
         return [{"key": key, "value": value} for key, value in obj.items()]
 
     @classmethod
     def time_based(
-        cls, time_range: DateOperation, values: Dict[Union[str, date, datetime], Union[int, float]]
+        cls,
+        time_range: Union[DateOperation, DateOperationLiteral],
+        values: Dict[Union[str, date, datetime], Union[int, float]],
     ) -> TimeBasedChart:
         """Add a TimeBasedChart based on a time range and a set of values
 
         Args:
             time_range (DateOperation): The time range for the chart, specified as a DateOperation
             values (Dict[Union[str, date, datetime], Union[int, float]]): This can be an array of objects with 'date'
                 and 'value' properties, or a record (object) with date-value pairs
@@ -89,20 +91,20 @@
                 {"date": datetime(2023, 1, 3), "value": None},
             ])
         """
         formatted = []
         for _date, value in values.items():
             formatted.append({"date": _date, "value": value})
 
-        return ResultBuilder._build_time_base_chart_result(time_range, formatted)
+        return ResultBuilder._build_time_base_chart_result(DateOperation(time_range), formatted)
 
     @classmethod
     def multiple_time_based(
         cls,
-        time_range: DateOperation,
+        time_range: Union[DateOperation, DateOperationLiteral],
         dates: List[Union[str, date, datetime]],
         lines: MultipleTimeBasedLines,
     ) -> MultipleTimeBasedChart:
         """Add a MultipleTimeBasedChart based on a time range, an array of dates, and multiple lines of data.
 
         Args:
             time_range (DateOperation): The time range for the chart, specified as a DateOperation
@@ -127,15 +129,15 @@
 
         formatted_lines = []
         formatted_times = None
         for line in lines:
             values = []
             for idx, _date in enumerate(dates):
                 values.append({"date": _date, "value": line["values"][idx]})
-            build_time_base = ResultBuilder._build_time_base_chart_result(time_range, values)
+            build_time_base = ResultBuilder._build_time_base_chart_result(DateOperation(time_range), values)
 
             if formatted_times is None:
                 formatted_times = [time_based["label"] for time_based in build_time_base]
 
             formatted_lines.append(
                 {"key": line["label"], "values": [time_base["values"]["value"] for time_base in build_time_base]}
             )
@@ -155,15 +157,16 @@
 
     @staticmethod
     def smart(data) -> SmartChart:
         return data
 
     @staticmethod
     def _build_time_base_chart_result(
-        time_range: DateOperation, points: List[Dict[Union[date, datetime, str], Union[int, float, None]]]
+        time_range: Union[DateOperation, DateOperationLiteral],
+        points: List[Dict[Union[date, datetime, str], Union[int, float, None]]],
     ) -> TimeBasedChart:
         """Normalize the time based chart result to have a value for each time range.
         For example, if the time range is 'Month' and the values are:
             [
                 # YYYY-MM-DD
                 { "date": date('2022-01-07'), "value": 1 }, # Jan 22
                 { "date": date('2022-02-02'), "value": 2 }, # Feb 22
@@ -175,22 +178,24 @@
                 { "label": 'Jan 22', "values": { "value": 4 } },
                 { "label": 'Feb 22', "values": { "value": 6 } },
             ]
         """
         if len(points) == 0:
             return []
         points_in_date_time = [{"date": _parse_date(point["date"]), "value": point["value"]} for point in points]
-        format_ = ResultBuilder.FORMATS[time_range]
+        format_ = ResultBuilder.FORMATS[DateOperation(time_range)]
 
         formatted = {}
         for point in points_in_date_time:
             label = point["date"].strftime(format_)
             if point["value"] is not None:
                 formatted[label] = formatted.get(label, 0) + point["value"]
 
         data_points = []
         dates = sorted([p["date"] for p in points_in_date_time])
         first = dates[0]
         last = dates[-1]
-        for label in _make_formatted_date_range(first, last, _DateRangeFrequency[time_range.value], format_):
+        for label in _make_formatted_date_range(
+            first, last, _DateRangeFrequency[DateOperation(time_range).value], format_
+        ):
             data_points.append({"label": label, "values": {"value": formatted.get(label, 0)}})
         return data_points
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/chart/types.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/chart/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/collection_decorator.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/collection_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/computed/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/computed/helpers.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/helpers.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/computed/types.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/computed/utils.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/computed/utils.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/datasource_decorator.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/decorator_stack.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/decorator_stack.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/empty/collection.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/empty/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/aggregate.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/aggregate.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/create.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/create.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/delete.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/delete.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/hooks.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/hooks.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/list.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/list.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/context/update.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/context/update.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/hook/hooks.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/hook/hooks.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_emulate/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/operators_equivalence/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/publication/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/publication/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/publication/datasource.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/publication/datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/relation/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/relation/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/relation/types.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/relation/types.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/rename_collection/collection.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_collection/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/rename_collection/datasource.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_collection/datasource.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/rename_field/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/rename_field/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/schema/collection.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/schema/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/search/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/search/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/segments/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/segments/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/sort_emulate/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/sort_emulate/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/validation/collection.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/validation/collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/create_relations/create_relations_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/update_relations/update_relations_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_datasource_decorator.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_customization_context.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/decorators/write/write_replace/write_replace_collection.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/exceptions.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/.DS_Store` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/actions.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/actions.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 from typing_extensions import NotRequired, TypedDict
 
 Number = Union[int, float]
 
 
 class ActionsScope(enum.Enum):
-    SINGLE = "single"
-    BULK = "bulk"
-    GLOBAL = "global"
+    SINGLE = "Single"
+    BULK = "Bulk"
+    GLOBAL = "Global"
 
 
-ActionScopeLiteral = Literal["single", "bulk", "global"]
+ActionScopeLiteral = Literal["Single", "Bulk", "Global"]
 
 
 @dataclass
 class File:
     mime_type: str
     buffer: bytes
     name: str
@@ -119,38 +119,43 @@
     search: NotRequired[Any]
     allow_empty_values: NotRequired[bool]
 
 
 class SuccessResult(TypedDict):
     type: Literal["Success"]
     message: str
-    format: Union[Literal["html"], Literal["text"]]
+    format: Literal["html", "text"]
     invalidated: Set[str]
+    response_headers: Optional[Dict[str, str]]
 
 
 class ErrorResult(TypedDict):
     type: Literal["Error"]
     message: str
-    format: Union[Literal["html"], Literal["text"]]
+    format: Literal["html", "text"]
+    response_headers: Optional[Dict[str, str]]
 
 
 class WebHookResult(TypedDict):
     type: Literal["Webhook"]
     url: str
-    method: Union[Literal["GET"], Literal["POST"]]
+    method: Literal["GET", "POST"]
     headers: Dict[str, str]
     body: Any
+    response_headers: Optional[Dict[str, str]]
 
 
 class FileResult(TypedDict):
     type: Literal["File"]
     mimeType: str
     name: str
     stream: Any
+    response_headers: Optional[Dict[str, str]]
 
 
 class RedirectResult(TypedDict):
     type: Literal["Redirect"]
     path: str
+    response_headers: Optional[Dict[str, str]]
 
 
 ActionResult = Union[SuccessResult, ErrorResult, WebHookResult, FileResult, RedirectResult]
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/chart.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/chart.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/fields.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     GREATER_THAN = "greater_than"
     IN = "in"
     NOT_IN = "not_in"
     LIKE = "like"
     STARTS_WITH = "starts_with"
     ENDS_WITH = "ends_with"
     CONTAINS = "contains"
-    MATCH = "Match"
+    MATCH = "match"
     # ICONTAINS = "icontains"
     NOT_CONTAINS = "not_contains"
     LONGER_THAN = "longer_than"
     SHORTER_THAN = "shorter_than"
     BEFORE = "before"
     AFTER = "after"
     AFTER_X_HOURS_AGO = "after_x_hours_ago"
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/models/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/models/collections.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import abc
-from typing import Dict, Generic, List, TypedDict, TypeVar
+from typing import Callable, Dict, Generic, List, TypedDict, TypeVar
 
 from forestadmin.datasource_toolkit.interfaces.actions import Action
 from forestadmin.datasource_toolkit.interfaces.fields import FieldAlias
 from typing_extensions import Self
 
 
 class CollectionSchema(TypedDict):
     actions: Dict[str, Action]
     fields: Dict[str, FieldAlias]
     searchable: bool
     segments: List[str]
     countable: bool
+    charts: Dict[str, Callable]
 
 
 class Collection(abc.ABC):
     @abc.abstractproperty
     def datasource(self) -> "Datasource[Self]":
         raise NotImplementedError
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/.DS_Store` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/aggregation.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/aggregation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,60 +1,64 @@
 import enum
 import json
 import sys
 from datetime import datetime, timedelta
-from numbers import Number
 from typing import Any, Callable, Dict, List, Literal, Optional, Union
 
 if sys.version_info >= (3, 9):
     import zoneinfo
 else:
     from backports import zoneinfo
 
 from forestadmin.datasource_toolkit.interfaces.query.projections import Projection
 from forestadmin.datasource_toolkit.interfaces.records import RecordsDataAlias
 from forestadmin.datasource_toolkit.utils.records import RecordUtils
 from typing_extensions import NotRequired, Self, TypedDict, TypeGuard
 
+Number = Union[int, float]
+
 
 class Aggregator(enum.Enum):
     COUNT = "Count"
     SUM = "Sum"
     AVG = "Avg"
     MAX = "Max"
     MIN = "Min"
 
 
-PlainAggregator = Union[Literal["Count"], Literal["Sum"], Literal["Avg"], Literal["Max"], Literal["Min"]]
+PlainAggregator = Literal["Count", "Sum", "Avg", "Max", "Min"]
 
 
 class DateOperation(enum.Enum):
     YEAR = "Year"
     MONTH = "Month"
     WEEK = "Week"
     DAY = "Day"
 
 
+DateOperationLiteral = Literal["Year", "Month", "Week", "Day"]
+
+
 class AggregateResult(TypedDict):
     value: Any
     group: Dict[str, Any]
 
 
 class Summary(TypedDict):
     group: Dict[str, Any]
-    start_count: int
-    Count: int
-    Sum: int
-    Max: Optional[int]
-    Min: Optional[int]
+    start_count: Number
+    Count: Number
+    Sum: Number
+    Max: Optional[Number]
+    Min: Optional[Number]
 
 
 class PlainAggregationGroup(TypedDict):
     field: str
-    operation: NotRequired[Union[str, DateOperation]]
+    operation: NotRequired[Union[DateOperation, DateOperationLiteral]]
 
 
 class AggregationGroup(TypedDict):
     field: str
     operation: NotRequired[DateOperation]
 
 
@@ -73,15 +77,15 @@
             aggregation_group = AggregationGroup(
                 field=plain_aggregation_group["field"],
             )
             if plain_aggregation_group.get("operation"):
                 aggregation_group["operation"] = DateOperation(plain_aggregation_group.get("operation"))
             self.groups.append(aggregation_group)
 
-    def __eq__(self: Self, obj: Self) -> bool:
+    def __eq__(self: Self, obj: Self) -> bool:  # type:ignore
         return (
             self.__class__ == obj.__class__
             and self.field == obj.field
             and self.operation == obj.operation
             and self.groups == obj.groups
         )
 
@@ -101,20 +105,20 @@
 
     def _prefix_handler(self, prefix: str) -> Callable[[str], str]:
         def __prefix(field: str) -> str:
             return f"{prefix}:{field}"
 
         return __prefix
 
-    def nest(self, prefix: str) -> Self:
+    def nest(self, prefix: str) -> "Aggregation":
         if not prefix or (not self.field and not self.groups):
             return self
         return self.replace_fields(self._prefix_handler(prefix))
 
-    def replace_fields(self, handler: Callable[[str], str]) -> Self:
+    def replace_fields(self, handler: Callable[[str], str]) -> "Aggregation":
         result = Aggregation(self._to_plain)
         if result.field:
             result.field = handler(result.field)
         new_groups: List[AggregationGroup] = []
         for group in result.groups:
             new_group: AggregationGroup = {"field": handler(group["field"])}
             if "operation" in group:
@@ -180,15 +184,15 @@
             value = RecordUtils.get_field_value(record, self.field)
             if value is not None:
                 summary["Count"] += 1  #  count(field)
                 if summary["Min"] is None or value < summary["Min"]:
                     summary["Min"] = value
                 if summary["Max"] is None or value > summary["Max"]:
                     summary["Max"] = value
-            if isinstance(value, Number):
+            if isinstance(value, int) or isinstance(value, float):
                 summary["Sum"] += value
         return summary
 
     def _create_group(self, record: RecordsDataAlias, timezone: str) -> RecordsDataAlias:
         group_record: RecordsDataAlias = {}
         for group in self.groups:
             group_value = RecordUtils.get_field_value(record, group["field"])
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/.DS_Store`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/equivalence.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/base.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/branch.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,36 +25,36 @@
 
 
 class Aggregator(enum.Enum):
     OR = "or"
     AND = "and"
 
 
-LiteralAggregator = Union[Literal["or"], Literal["and"]]
+LiteralAggregator = Literal["or", "and"]
 
 
 class BranchComponents(ConditionTreeComponent):
     aggregator: LiteralAggregator
     conditions: List[Union["BranchComponents", LeafComponents]]
 
 
 def is_branch_component(tree: Any) -> TypeGuard[BranchComponents]:
     return isinstance(tree, dict) and "aggregator" in tree.keys() and "conditions" in tree.keys()
 
 
 class ConditionTreeBranch(ConditionTree):
-    def __init__(self, aggregator: Aggregator, conditions: List[ConditionTree]):
+    def __init__(self, aggregator: Union[Aggregator, LiteralAggregator], conditions: List[ConditionTree]):
         super().__init__()
-        self.aggregator = aggregator
+        self.aggregator = Aggregator(aggregator)
         self.conditions = conditions
 
     def __repr__(self):
         return f"{self.aggregator}[{self.conditions}]"
 
-    def __eq__(self: Self, obj: Self) -> bool:
+    def __eq__(self: Self, obj: Self) -> bool:  # type: ignore
         return (
             self.__class__ == obj.__class__ and self.aggregator == obj.aggregator and self.conditions == obj.conditions
         )
 
     @property
     def projection(self) -> Projection:
         def reducer(memo: Projection, condition: ConditionTree):
@@ -72,15 +72,15 @@
         meth = all
         if self.aggregator == Aggregator.OR:
             meth = any
         return meth([condition.match(record, collection, timezone) for condition in self.conditions])
 
     def some_leaf(self, handler: Callable[["ConditionTreeLeaf"], bool]) -> bool:  # noqa:F821
         for condition in self.conditions:
-            handler_res = handler(condition)
+            handler_res = handler(condition)  # type: ignore
             if handler_res is True:
                 return True
         return False
 
     def apply(self, handler: "CallbackAlias") -> None:
         for condition in self.conditions:
             condition.apply(handler)
@@ -121,11 +121,12 @@
 
         return self.replace(__rename)
 
     def unnest(self) -> ConditionTree:
         prefix = self._get_prefix()
         return self._remove_prefix(prefix)
 
-    def to_plain_object(self) -> BranchComponents:
+    def to_plain_object(self) -> BranchComponents:  # type: ignore
         return BranchComponents(
-            aggregator=self.aggregator.value, conditions=[condition.to_plain_object() for condition in self.conditions]
+            aggregator=self.aggregator.value,
+            conditions=[condition.to_plain_object() for condition in self.conditions],  # type: ignore
         )
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/leaf.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,25 +44,25 @@
 class OverrideLeafComponents(ConditionTreeComponent, total=False):
     field: str
     operator: Operator
     value: NotRequired[Optional[Any]]
 
 
 class ConditionTreeLeaf(ConditionTree):
-    def __init__(self, field: str, operator: Operator, value: Optional[Any] = None) -> None:
+    def __init__(self, field: str, operator: Union[Operator, LITERAL_OPERATORS], value: Optional[Any] = None) -> None:
         super().__init__()
         self.field = field
-        self.operator = operator
+        self.operator = Operator(operator)
         self.value = value
 
-    def __eq__(self: Self, obj: Self) -> bool:
+    def __eq__(self: Self, obj: Self) -> bool:  # type: ignore
         return (
             self.__class__ == obj.__class__
             and self.field == obj.field
-            and self.operator == obj.operator
+            and Operator(self.operator) == Operator(obj.operator)
             and self.value == obj.value
         )
 
     def __repr__(self):
         return f"{self.field} {self.operator.value} {self.value}"
 
     @property
@@ -113,18 +113,18 @@
         tree: Union[ConditionTree, ConditionTreeComponent] = await handler(self)
         return ConditionTreeLeaf._handle_replace_tree(tree)
 
     def apply(self, handler: CallbackAlias) -> None:
         return handler(self)
 
     @property
-    def _to_leaf_components(self) -> "LeafComponents":
+    def _to_leaf_components(self) -> LeafComponents:
         return {
             "field": self.field,
-            "operator": self.operator.value,
+            "operator": self.operator.value,  # type: ignore
             "value": self.value,
         }
 
     def override(self, params: "OverrideLeafComponents") -> "ConditionTreeLeaf":
         leaf = cast(LeafComponents, {**self._to_leaf_components, **params})
         return ConditionTreeLeaf.load(leaf)
 
@@ -255,9 +255,13 @@
                 f"^{escaped_pattern}$",
                 value,
                 re.I,
             )
             is not None
         )
 
-    def to_plain_object(self) -> LeafComponents:
-        return LeafComponents(field=self.field, operator=self.operator.value, value=self.value)
+    def to_plain_object(self) -> LeafComponents:  # type: ignore
+        return LeafComponents(
+            field=self.field,
+            operator=self.operator.value,  # type: ignore
+            value=self.value,
+        )
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/nodes/operators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/comparison.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/pattern.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/condition_tree/transforms/time.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/paginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/filter/unpaginated.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/page.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/page.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/projections/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/projections/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/sort/__init__.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/interfaces/query/sort/factory.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/plugins/add_external_relation.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/plugins/add_external_relation.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/plugins/import_field.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/plugins/import_field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/utils/collections.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/collections.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/utils/operators.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/operators.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/utils/records.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/utils/schema.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/utils/schema.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/condition_tree.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/condition_tree.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/field.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/field.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/records.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/records.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/rules.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/rules.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/forestadmin/datasource_toolkit/validations/type_getter.py` & `forestadmin_datasource_toolkit-1.6.2/forestadmin/datasource_toolkit/validations/type_getter.py`

 * *Files identical despite different names*

### Comparing `forestadmin_datasource_toolkit-1.6.1/pyproject.toml` & `forestadmin_datasource_toolkit-1.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "forestadmin-datasource-toolkit"
 description = "datasource toolkit for forestadmin python agent"
-version = "1.6.1"
+version = "1.6.2"
 authors = [ "Valentin Monté <valentinm@forestadmin.com>", "Julien Barreau <julien.barreau@forestadmin.com>",]
 readme = "README.md"
 repository = "https://github.com/ForestAdmin/agent-python"
 documentation = "https://docs.forestadmin.com/developer-guide-agents-python/"
 homepage = "https://www.forestadmin.com"
 [[tool.poetry.packages]]
 include = "forestadmin"
```

### Comparing `forestadmin_datasource_toolkit-1.6.1/PKG-INFO` & `forestadmin_datasource_toolkit-1.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forestadmin-datasource-toolkit
-Version: 1.6.1
+Version: 1.6.2
 Summary: datasource toolkit for forestadmin python agent
 Home-page: https://www.forestadmin.com
 Author: Valentin Monté
 Author-email: valentinm@forestadmin.com
 Requires-Python: >=3.8,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

