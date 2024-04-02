# Comparing `tmp/mlcroissant-1.0.3.tar.gz` & `tmp/mlcroissant-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcroissant-1.0.3.tar", last modified: Wed Mar 13 13:43:53 2024, max compression
+gzip compressed data, was "mlcroissant-1.0.4.tar", last modified: Tue Apr  2 07:25:14 2024, max compression
```

## Comparing `mlcroissant-1.0.3.tar` & `mlcroissant-1.0.4.tar`

### file list

```diff
@@ -1,140 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.759872 mlcroissant-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-03-13 13:43:53.755872 mlcroissant-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7220 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.739872 mlcroissant-1.0.3/mlcroissant/
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.739872 mlcroissant-1.0.3/mlcroissant/_src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.743872 mlcroissant-1.0.3/mlcroissant/_src/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/constants_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/dataclasses_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/dates_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/git_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.743872 mlcroissant-1.0.3/mlcroissant/_src/core/graphs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/graphs/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/issues.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/issues_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10679 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/json_ld.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/json_ld_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.743872 mlcroissant-1.0.3/mlcroissant/_src/core/ml/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/ml/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/ml/bounding_box_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/optional.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/optional_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     5013 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/rdf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/rdf_test.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/core/uuid_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6578 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/nodes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.743872 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/base_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/execute_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.747872 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/concatenate.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/concatenate_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/data.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/data_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/download_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/extract_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/field_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/filter_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/init.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/init_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/join.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/join_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/local_directory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/parse_json.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/parse_json_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/read_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.747872 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18581 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/base_node_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/graph_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.751872 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/creative_work.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/croissant_version_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/field.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/field_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/file_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/file_object_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/file_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/file_set_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18322 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/person.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/record_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/record_set_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/source_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.751872 mlcroissant-1.0.3/mlcroissant/_src/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/tests/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/tests/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/tests/records.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/tests/records_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/tests/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.751872 mlcroissant-1.0.3/mlcroissant/_src/torch/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.751872 mlcroissant-1.0.3/mlcroissant/_src/torch/torch_adapter/
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/torch/torch_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/torch/torch_adapter/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/_src/torch/torch_adapter/dataloader_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.751872 mlcroissant-1.0.3/mlcroissant/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/load_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.755872 mlcroissant-1.0.3/mlcroissant/scripts/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/migrate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.755872 mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202302061400.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202307171508.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202307201041.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202308312000.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202309061700.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202312062353.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202402011100.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202402020202.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202402051000.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202402201330.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202429011700.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/mlcroissant/scripts/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 13:43:53.755872 mlcroissant-1.0.3/mlcroissant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8656 2024-03-13 13:43:53.000000 mlcroissant-1.0.3/mlcroissant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5395 2024-03-13 13:43:53.000000 mlcroissant-1.0.3/mlcroissant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 13:43:53.000000 mlcroissant-1.0.3/mlcroissant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-13 13:43:53.000000 mlcroissant-1.0.3/mlcroissant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-03-13 13:43:53.000000 mlcroissant-1.0.3/mlcroissant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-13 13:43:53.000000 mlcroissant-1.0.3/mlcroissant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-03-13 13:43:41.000000 mlcroissant-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 13:43:53.759872 mlcroissant-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.406834 mlcroissant-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-02 07:25:14.406834 mlcroissant-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.386834 mlcroissant-1.0.4/mlcroissant/
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.390834 mlcroissant-1.0.4/mlcroissant/_src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.390834 mlcroissant-1.0.4/mlcroissant/_src/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9718 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/constants_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8416 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/dataclasses_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/dates_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/git_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.394834 mlcroissant-1.0.4/mlcroissant/_src/core/graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/graphs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/issues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/issues_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/json_ld.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/json_ld_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.394834 mlcroissant-1.0.4/mlcroissant/_src/core/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/ml/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/ml/bounding_box_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/optional.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/optional_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/rdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/rdf_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/uuid_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/core/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.394834 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/base_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5254 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/execute_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8512 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.398834 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/concatenate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/concatenate_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/data_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8870 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/download_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1998 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/extract_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6751 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7022 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/field_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/filter_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/init_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/join_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/local_directory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/parse_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/parse_json_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7283 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/read_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.398834 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8715 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/base_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5820 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/graph_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.402834 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/creative_work.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/croissant_version_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/field_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3978 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_set_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16621 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6291 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6975 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/record_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/record_set_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/source_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.402834 mlcroissant-1.0.4/mlcroissant/_src/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3136 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/tests/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/tests/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/tests/records.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/tests/records_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/tests/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.402834 mlcroissant-1.0.4/mlcroissant/_src/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.402834 mlcroissant-1.0.4/mlcroissant/_src/torch/torch_adapter/
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/torch/torch_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/torch/torch_adapter/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/_src/torch/torch_adapter/dataloader_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.402834 mlcroissant-1.0.4/mlcroissant/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2997 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/load_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.402834 mlcroissant-1.0.4/mlcroissant/scripts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/migrate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.406834 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202302061400.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202307171508.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202307201041.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202308312000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202309061700.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202312062353.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202402011100.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202402020202.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202402051000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202402201330.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202403270859.py
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202403271030.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202429011700.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/mlcroissant/scripts/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 07:25:14.406834 mlcroissant-1.0.4/mlcroissant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-04-02 07:25:14.000000 mlcroissant-1.0.4/mlcroissant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-02 07:25:14.000000 mlcroissant-1.0.4/mlcroissant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 07:25:14.000000 mlcroissant-1.0.4/mlcroissant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 07:25:14.000000 mlcroissant-1.0.4/mlcroissant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-02 07:25:14.000000 mlcroissant-1.0.4/mlcroissant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-02 07:25:14.000000 mlcroissant-1.0.4/mlcroissant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-02 07:24:58.000000 mlcroissant-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 07:25:14.406834 mlcroissant-1.0.4/setup.cfg
```

### Comparing `mlcroissant-1.0.3/PKG-INFO` & `mlcroissant-1.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcroissant
-Version: 1.0.3
+Version: 1.0.4
 Summary: MLCommons datasets format.
 Author: Joaquin Vanschoren, Jos van der Velde, Monjish Bhattacharyya, Omar Benjelloun, Peter Mattson, Pieter Gijsbers, Pierre Marcenac, Pierre Ruyssen, Prabhant Singh
 Description-Content-Type: text/markdown
 Requires-Dist: absl-py
 Requires-Dist: etils[epath]>=1.7.0
 Requires-Dist: jsonpath-rw
 Requires-Dist: networkx
@@ -123,14 +123,67 @@
 import mlcroissant as mlc
 metadata=mlc.nodes.Metadata(
   name="...",
 )
 metadata.to_json()  # this returns the JSON-LD file.
 ```
 
+## Add new properties to the standard
+
+Nodes (Metadata, RecordSets, etc) implement [PEP 681](https://peps.python.org/pep-0681/). So you can declare RDF triplets using the [dataclass](https://docs.python.org/3/library/dataclasses.html) syntax.
+
+**Example 1**: implement [CreativeWork](https://schema.org/CreativeWork):
+
+```python
+@mlc_dataclasses.dataclass
+class CreativeWork(Node):
+
+    JSONLD_TYPE = SDO.CreativeWork           # https://schema.org/CreativeWork
+
+    name: str | None = mlc_dataclasses.jsonld_field(
+        cardinality="ONE",                   # Cardinality can be ONE or MANY
+        default=None,                        # Specify the default value in Python
+        description="The name of the item.", # The full description
+        input_types=[SDO.Text],              # The schema.org type
+        url=SDO.name,                        # The URL of the property
+    )
+```
+
+**Example 2**: implement [RecordSet](https://mlcommons.github.io/croissant/docs/croissant-spec.html#recordset):
+
+```python
+@mlc_dataclasses.dataclass
+class RecordSet(Node):
+    JSONLD_TYPE = constants.ML_COMMONS_RECORD_SET_TYPE
+
+    fields: list[Field] = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",                  # Example with cardinality=="MANY"
+        default_factory=list,
+        description=(
+            "A data element that appears in the records of the RecordSet (e.g., one"
+            " column of a table)."
+        ),
+        input_types=[Field],                 # Types can also be other nodes (here `Field`)
+        url=constants.ML_COMMONS_FIELD,
+    )
+```
+
+**Example 3**: specify a version (by default all versions):
+
+```python
+@mlc_dataclasses.dataclass
+class Field(Node):
+    is_enumeration: bool | None = mlc_dataclasses.jsonld_field(
+        default=None,
+        input_types=[SDO.Boolean],
+        url=constants.ML_COMMONS_IS_ENUMERATION,
+        versions=[CroissantVersion.V_0_8],   # `is_enumeration` is only valid for v0.8, not v1.0
+    )
+```
+
 ## Run tests
 
 All tests can be run from the Makefile:
 
 ```bash
 make tests
 ```
```

### Comparing `mlcroissant-1.0.3/README.md` & `mlcroissant-1.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -83,14 +83,67 @@
 import mlcroissant as mlc
 metadata=mlc.nodes.Metadata(
   name="...",
 )
 metadata.to_json()  # this returns the JSON-LD file.
 ```
 
+## Add new properties to the standard
+
+Nodes (Metadata, RecordSets, etc) implement [PEP 681](https://peps.python.org/pep-0681/). So you can declare RDF triplets using the [dataclass](https://docs.python.org/3/library/dataclasses.html) syntax.
+
+**Example 1**: implement [CreativeWork](https://schema.org/CreativeWork):
+
+```python
+@mlc_dataclasses.dataclass
+class CreativeWork(Node):
+
+    JSONLD_TYPE = SDO.CreativeWork           # https://schema.org/CreativeWork
+
+    name: str | None = mlc_dataclasses.jsonld_field(
+        cardinality="ONE",                   # Cardinality can be ONE or MANY
+        default=None,                        # Specify the default value in Python
+        description="The name of the item.", # The full description
+        input_types=[SDO.Text],              # The schema.org type
+        url=SDO.name,                        # The URL of the property
+    )
+```
+
+**Example 2**: implement [RecordSet](https://mlcommons.github.io/croissant/docs/croissant-spec.html#recordset):
+
+```python
+@mlc_dataclasses.dataclass
+class RecordSet(Node):
+    JSONLD_TYPE = constants.ML_COMMONS_RECORD_SET_TYPE
+
+    fields: list[Field] = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",                  # Example with cardinality=="MANY"
+        default_factory=list,
+        description=(
+            "A data element that appears in the records of the RecordSet (e.g., one"
+            " column of a table)."
+        ),
+        input_types=[Field],                 # Types can also be other nodes (here `Field`)
+        url=constants.ML_COMMONS_FIELD,
+    )
+```
+
+**Example 3**: specify a version (by default all versions):
+
+```python
+@mlc_dataclasses.dataclass
+class Field(Node):
+    is_enumeration: bool | None = mlc_dataclasses.jsonld_field(
+        default=None,
+        input_types=[SDO.Boolean],
+        url=constants.ML_COMMONS_IS_ENUMERATION,
+        versions=[CroissantVersion.V_0_8],   # `is_enumeration` is only valid for v0.8, not v1.0
+    )
+```
+
 ## Run tests
 
 All tests can be run from the Makefile:
 
 ```bash
 make tests
 ```
```

### Comparing `mlcroissant-1.0.3/mlcroissant/__init__.py` & `mlcroissant-1.0.4/mlcroissant/__init__.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/constants.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,34 +71,32 @@
 
 # Croissant RAI extension
 # V1.0 namespace
 RAI = rdflib.Namespace("http://mlcommons.org/croissant/RAI/")
 # Attributes
 ML_COMMONS_RAI_DATA_COLLECTION = RAI.dataCollection
 ML_COMMONS_RAI_DATA_COLLECTION_TYPE = RAI.dataCollectionType
-ML_COMMONS_RAI_DATA_COLLECTION_TYPE_OTHERS = RAI.dataCollectionTypeOthers
-ML_COMMONS_RAI_DATA_COLLECTION_MISSING = RAI.dataCollectionMissing
-ML_COMMONS_RAI_DATA_COLLECTION_RAW = RAI.dataCollectionRaw
-ML_COMMONS_RAI_DATA_COLLECTION_TIMEFRAME_START = RAI.dataCollectionTimeFrameStart
-ML_COMMONS_RAI_DATA_COLLECTION_TIMEFRAME_END = RAI.dataCollectionTimeFrameEnd
-ML_COMMONS_RAI_DATA_PREPROCESSING_IMPUTATION = RAI.dataPreprocessingImputation
-ML_COMMONS_RAI_DATA_PREPROCESSING_PROTOCOL = RAI.dataPeprocessingProtocol
-ML_COMMONS_RAI_DATA_PREPROCESSING_MANIPULATION = RAI.dataPreprocessingManipulation
+ML_COMMONS_RAI_DATA_COLLECTION_MISSING_DATA = RAI.dataCollectionMissingData
+ML_COMMONS_RAI_DATA_COLLECTION_RAW_DATA = RAI.dataCollectionRawData
+ML_COMMONS_RAI_DATA_COLLECTION_TIME_FRAME = RAI.dataCollectionTimeFrame
+ML_COMMONS_RAI_DATA_IMPUTATION_PROTOCOL = RAI.dataImputationProtocol
+ML_COMMONS_RAI_DATA_PREPROCESSING_PROTOCOL = RAI.dataPreprocessingProtocol
+ML_COMMONS_RAI_DATA_DATA_MANIPULATION_PROTOCOL = RAI.dataDataManipulationProtocol
 ML_COMMONS_RAI_DATA_ANNOTATION_PROTOCOL = RAI.dataAnnotationProtocol
 ML_COMMONS_RAI_DATA_ANNOTATION_PLATFORM = RAI.dataAnnotationPlatform
 ML_COMMONS_RAI_DATA_ANNOTATION_ANALYSIS = RAI.dataAnnotationAnalysis
-ML_COMMONS_RAI_DATA_ANNOTATION_PER_ITEM = RAI.dataAnnotationPerItem
-ML_COMMONS_RAI_DATA_ANNOTATION_DEMOGRAPHICS = RAI.dataAnnotationDemographics
-ML_COMMONS_RAI_DATA_ANNOTATION_TOOLS = RAI.dataAnnotationTools
+ML_COMMONS_RAI_ANNOTATIONS_PER_ITEM = RAI.annotationsPerItem
+ML_COMMONS_RAI_ANNOTATOR_DEMOGRAPHICS = RAI.annotatorDemographics
+ML_COMMONS_RAI_MACHINE_ANNOTATION_TOOLS = RAI.machineAnnotationTools
 ML_COMMONS_RAI_DATA_USE_CASES = RAI.dataUseCases
 ML_COMMONS_RAI_DATA_BIASES = RAI.dataBiases
-ML_COMMONS_RAI_DATA_LIMITATION = RAI.dataLimitation
+ML_COMMONS_RAI_DATA_LIMITATIONS = RAI.dataLimitations
 ML_COMMONS_RAI_DATA_SOCIAL_IMPACT = RAI.dataSocialImpact
-ML_COMMONS_RAI_DATA_SENSITIVE = RAI.dataSensitive
-ML_COMMONS_RAI_DATA_MAINTENANCE = RAI.dataMaintenance
+ML_COMMONS_RAI_PERSONAL_SENSITIVE_INFORMATION = RAI.personalSensitiveInformation
+ML_COMMONS_RAI_DATA_RELEASE_MAINTENANCE_PLAN = RAI.dataReleaseMaintenancePlan
 
 # RDF standard URIs.
 # For "@type" key:
 RDF_TYPE = namespace.RDF.type
 
 # Dublin Core terms standard URIs.
 DCTERMS = "http://purl.org/dc/terms/"
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/constants_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/constants_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/context.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,21 @@
 """Global context."""
 
 from __future__ import annotations
 
 import dataclasses
 import enum
-import typing
 from typing import Any, Mapping
 
 from etils import epath
 import networkx as nx
 
 from mlcroissant._src.core.issues import Issues
 from mlcroissant._src.core.rdf import Rdf
 
-if typing.TYPE_CHECKING:
-    from mlcroissant._src.structure_graph.base_node import Node
-
 
 class CroissantVersion(enum.Enum):
     """Major and minor versions of the Croissant standard."""
 
     V_0_8 = "http://mlcommons.org/croissant/0.8"
     V_1_0 = "http://mlcommons.org/croissant/1.0"
 
@@ -87,14 +83,7 @@
     def copy(self, **changes) -> Context:
         """Copies and replaces all changes."""
         return dataclasses.replace(self, **changes)
 
     def is_v0(self):
         """Whether the JSON-LD conforms to Croissant v0.8 or lower."""
         return self.conforms_to < CroissantVersion.V_1_0
-
-    def node_by_uuid(self, uuid: str | None) -> Node | None:
-        """Retrieves a node in the graph by its UID."""
-        for node in self.graph.nodes():
-            if node.uuid == uuid:  # pytype: disable=attribute-error
-                return node  # pytype: disable=bad-return-type
-        return None
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/data_types.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/data_types.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/dataclasses_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/dataclasses_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """dataclasses_test module."""
 
+import pytest
 from rdflib.namespace import SDO
 
 from mlcroissant._src.core import dataclasses as mlc_dataclasses
 from mlcroissant._src.core.context import Context
 from mlcroissant._src.core.context import CroissantVersion
 from mlcroissant._src.structure_graph.base_node import Node
 
@@ -13,44 +14,41 @@
 
     @mlc_dataclasses.dataclass
     class SomeNode:
         field1: int = mlc_dataclasses.jsonld_field(
             description="The first field",
             input_types=[SDO.Integer],
         )
-        field2: str = mlc_dataclasses.jsonld_field(
+        field2: list[str] = mlc_dataclasses.jsonld_field(
             cardinality="MANY",
             description="The second field",
             input_types=[SDO.Text],
-            required=True,
             url=url,
         )
 
-    node = SomeNode(field1=42, field2="foo")
+    node = SomeNode(field1=42, field2=["foo"])
     for cls_or_instance in [node, SomeNode]:
         field1, field2 = list(mlc_dataclasses.jsonld_fields(cls_or_instance))
 
         # Field #1
         assert field1.name == "field1"
         assert field1.cardinality == "ONE"
         assert field1.description == "The first field"
         assert field1.from_jsonld == None
         assert field1.input_types == [SDO.Integer]
         assert field1.to_jsonld == None
-        assert field1.required == False
         assert field1.url == None
 
         # Field #2
         assert field2.name == "field2"
         assert field2.cardinality == "MANY"
         assert field2.description == "The second field"
         assert field2.from_jsonld == None
         assert field2.input_types == [SDO.Text]
         assert field2.to_jsonld == None
-        assert field2.required == True
         assert field2.url == url
         assert (
             field2.call_url(Context(conforms_to=CroissantVersion.V_0_8))
             == "http://foo.org"
         )
         assert (
             field2.call_url(Context(conforms_to=CroissantVersion.V_1_0))
@@ -73,7 +71,63 @@
             input_types=[SDO.Text],
         )
 
     node = SomeNode(ctx=Context(conforms_to=CroissantVersion.V_1_0))
     fields = list(mlc_dataclasses.jsonld_fields(node))
     assert len(fields) == 1
     assert fields[0].name == "field2"
+
+
+@pytest.mark.parametrize(
+    "accessor",
+    [
+        # Access class
+        lambda cls: cls,
+        # Access instance of class
+        lambda cls: cls(),
+    ],
+)
+def test_types_of_fields(accessor):
+    @mlc_dataclasses.dataclass
+    class SubNode(Node):
+        field: int | None = mlc_dataclasses.jsonld_field(
+            default=None,
+            input_types=[SDO.Text],  # this is incompatible with `int`
+        )
+
+    with pytest.raises(TypeError, match='Field "SubNode.field" should have type'):
+        list(mlc_dataclasses.jsonld_fields(accessor(SubNode)))
+
+    @mlc_dataclasses.dataclass
+    class SubNode(Node):
+        field: int = mlc_dataclasses.jsonld_field(
+            default=None,  # this is incompatible with `int` (expect int | None)
+            input_types=[SDO.Integer],
+        )
+
+    with pytest.raises(TypeError, match='Field "SubNode.field" should have type'):
+        list(mlc_dataclasses.jsonld_fields(accessor(SubNode)))
+
+    @mlc_dataclasses.dataclass
+    class SubNode(Node):
+        field: str = mlc_dataclasses.jsonld_field(
+            default_factory=Node,  # this is incompatible with str
+            input_types=[Node],
+        )
+
+    with pytest.raises(TypeError, match='Field "SubNode.field" should have type'):
+        list(mlc_dataclasses.jsonld_fields(accessor(SubNode)))
+
+    def cast_fn(value: Node) -> int:  # int is incompatible with Node
+        del value
+        return 0
+
+    @mlc_dataclasses.dataclass
+    class SubNode(Node):
+        field: Node = mlc_dataclasses.jsonld_field(
+            cast_fn=cast_fn,
+            default_factory=Node,
+            input_types=[Node],
+        )
+
+    with pytest.raises(TypeError, match='Field "SubNode.field" .* should have type'):
+        list(mlc_dataclasses.jsonld_fields(accessor(SubNode)))
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/dates_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/dates_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/git.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/git.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/git_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/git_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/graphs/utils.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/graphs/utils.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/issues.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/issues.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,22 @@
     """Error during the validation of the format."""
 
 
 class GenerationError(Exception):
     """Error during the generation of the dataset."""
 
 
+class WarningException(Exception):
+    """Exception triggering a warning."""
+
+
+class ErrorException(Exception):
+    """Exception triggering an error."""
+
+
 @dataclasses.dataclass(frozen=True)
 class Issues:
     """Issues during the validation of the format.
 
     Issues can either be errors (blocking) or warnings (informative).
 
     We use sets to represent errors and warnings to avoid repeated strings.
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/issues_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/issues_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/json_ld.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/json_ld.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,33 +77,41 @@
     """Sorts items from dict.items().
 
     For human readability, we want "@type"/"name"/"description/conformsTo" to be
     at the beginning of the JSON, while long lists (""distribution"/"recordSet")
     are at the end.
     """
     items = sorted(jsonld.items())
-    start_keys = ["@context", "@type", "name", "description", "conformsTo"]
-    end_keys = ["distribution", "field", "data", "recordSet", "subField"]
+    start_keys = ["@context", "@type", "@id", "name", "description", "conformsTo"]
+    end_keys = [
+        "distribution",
+        "field",
+        "data",
+        "recordSet",
+        "subField",
+        "extract",
+        "transform",
+    ]
     sorted_items = []
     for key in start_keys:
         if key in jsonld:
             sorted_items.append((key, jsonld[key]))
     for item in items:
         if item[0] not in start_keys and item[0] not in end_keys:
             sorted_items.append(item)
     for key in end_keys:
         if key in jsonld:
             sorted_items.append((key, jsonld[key]))
     return sorted_items
 
 
-def _sort_dict(d: Json):
+def sort_dict(d: Json):
     """Sorts the keys of a nested dict."""
     return {
-        k: _sort_dict(v) if isinstance(v, dict) and k != "@context" else v
+        k: sort_dict(v) if isinstance(v, dict) and k != "@context" else v
         for k, v in _sort_items(d)
     }
 
 
 def remove_empty_values(d: Json) -> Json:
     """Removes empty values in a JSON."""
     # Either v exists or v is a bool (to account for False values)
@@ -272,8 +280,8 @@
             new_key = key.replace(constants.ML_COMMONS_V_1_0, "")
             json_[new_key] = new_value
         elif _DCTERMS_PREFIX in key:
             new_key = key.replace(_DCTERMS_PREFIX, "")
             json_[new_key] = value
         else:
             json_[key] = new_value
-    return _sort_dict(json_)
+    return sort_dict(json_)
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/json_ld_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/json_ld_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/ml/bounding_box.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/ml/bounding_box.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/ml/bounding_box_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/ml/bounding_box_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/optional.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/optional.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/optional_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/optional_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/path.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/path.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/rdf.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/rdf.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from __future__ import annotations
 
 import dataclasses
 import functools
 from typing import Any
 
+from absl import logging
 from rdflib import term
 
 from mlcroissant._src.core.types import Json
 
 
 def get_context(json_: Json) -> Json:
     """Returns the context and raises an error if it is not a dictionary as expected."""
@@ -67,14 +68,23 @@
 
     context: Json = dataclasses.field(default_factory=make_context)
 
     @classmethod
     def from_json(cls, ctx, json: Json) -> Rdf:
         """Creates a `Rdf` from JSON."""
         context = get_context(json)
+        # Keys that are in the standard @context, but not in the current @context.
+        different_keys = make_context(ctx).keys() - context.keys()
+        if different_keys:
+            logging.warning(
+                "WARNING: The JSON-LD `@context` is not standard. Refer to the"
+                " official @context (e.g., from the example datasets in"
+                " https://github.com/mlcommons/croissant/tree/main/datasets/1.0). The"
+                f" different keys are: {different_keys}"
+            )
         return cls(context=context)
 
     @functools.cache
     def reverse_context(self) -> Json:
         """Reverses the context dictionary.
 
         - context = "ml"->"http://mlcommons.org/schema"
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/uuid.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/uuid.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/core/uuid_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/core/uuid_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/datasets.py` & `mlcroissant-1.0.4/mlcroissant/_src/datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,14 @@
         ctx = Context(mapping=_expand_mapping(self.mapping))
         if isinstance(self.jsonld, dict):
             self.metadata = Metadata.from_json(ctx=ctx, json_=self.jsonld)
         elif self.jsonld is not None:
             self.metadata = Metadata.from_file(ctx=ctx, file=self.jsonld)
         else:
             return
-        ctx.is_live_dataset = self.metadata.is_live_dataset
         # Draw the structure graph for debugging purposes.
         if self.debug:
             graphs_utils.pretty_print_graph(ctx.graph, simplify=True)
         self.operations = get_operations(ctx, self.metadata)
         # Draw the operations graph for debugging purposes.
         if self.debug:
             graphs_utils.pretty_print_graph(self.operations.operations, simplify=False)
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/datasets_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/datasets_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,16 +177,16 @@
 
 @pytest.mark.nonhermetic
 def test_load_from_huggingface():
     url = "https://datasets-server.huggingface.co/croissant?dataset=mnist&full=true"
     dataset = datasets.Dataset(url)
     has_one_record = False
     for record in dataset.records(record_set="record_set_mnist"):
-        assert record["label"] == 7
-        assert isinstance(record["image"], deps.PIL_Image.Image)
+        assert record["record_set_mnist/label"] == 7
+        assert isinstance(record["record_set_mnist/image"], deps.PIL_Image.Image)
         has_one_record = True
         break
     assert has_one_record, (
         "mlc.Dataset.records() didn't yield any record. Warning: this test is"
         " non-hermetic and makes an API call to Hugging Face, so it's prone to network"
         " failure."
     )
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/nodes.py` & `mlcroissant-1.0.4/mlcroissant/_src/nodes.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/base_operation.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/base_operation.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/execute.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/execute.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/execute_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/execute_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/graph.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from mlcroissant._src.operation_graph.operations import InitOperation
 from mlcroissant._src.operation_graph.operations import Join
 from mlcroissant._src.operation_graph.operations import LocalDirectory
 from mlcroissant._src.operation_graph.operations import Read
 from mlcroissant._src.operation_graph.operations import ReadFields
 from mlcroissant._src.operation_graph.operations.extract import should_extract
 from mlcroissant._src.structure_graph.base_node import Node
+from mlcroissant._src.structure_graph.base_node import node_by_uuid
 from mlcroissant._src.structure_graph.nodes.field import Field
 from mlcroissant._src.structure_graph.nodes.file_object import FileObject
 from mlcroissant._src.structure_graph.nodes.file_set import FileSet
 from mlcroissant._src.structure_graph.nodes.record_set import RecordSet
 
 
 def _find_record_set(node: Node) -> RecordSet:
@@ -158,16 +159,16 @@
     record_set = _find_record_set(node)
     joins = [
         operation
         for operation in operations.nodes
         if isinstance(operation, Join) and operation.node == record_set
     ]
     for join in joins:
-        left_node = node.ctx.node_by_uuid(node.source.uuid)
-        right_node = node.ctx.node_by_uuid(node.references.uuid)
+        left_node = node_by_uuid(node.ctx, node.source.uuid)
+        right_node = node_by_uuid(node.ctx, node.references.uuid)
         if left_node and right_node:
             join.connect_to_last_operation(left_node)
             join.connect_to_last_operation(right_node)
 
 
 @dataclasses.dataclass(frozen=True)
 class OperationGraph:
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/__init__.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/concatenate.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/concatenate.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/data.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/data.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/download.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/download.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/download_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/download_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/extract.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/extract.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/extract_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/extract_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/field.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/field.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/field_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/field_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/filter.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/filter.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/filter_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/filter_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/join.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/join.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/local_directory.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/local_directory.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/parse_json.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/parse_json.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/parse_json_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/parse_json_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/read.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/read.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/operation_graph/operations/read_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/operation_graph/operations/read_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/base_node.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/base_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,47 @@
 """Base node module."""
 
-from __future__ import annotations
-
 import dataclasses
 import inspect
 import re
 from typing import Any, Callable
 
 from rdflib import term
 from rdflib.namespace import SDO
 
 from mlcroissant._src.core import constants
 from mlcroissant._src.core import dataclasses as mlc_dataclasses
 from mlcroissant._src.core.context import Context
 from mlcroissant._src.core.context import CroissantVersion
 from mlcroissant._src.core.data_types import check_expected_type
 from mlcroissant._src.core.issues import Issues
+from mlcroissant._src.core.issues import WarningException
 from mlcroissant._src.core.json_ld import box_singleton_list
 from mlcroissant._src.core.json_ld import remove_empty_values
+from mlcroissant._src.core.json_ld import sort_dict
 from mlcroissant._src.core.json_ld import unbox_singleton_list
 from mlcroissant._src.core.types import Json
 from mlcroissant._src.core.uuid import generate_uuid
 from mlcroissant._src.core.uuid import uuid_from_jsonld
 
 NAME_REGEX = "[a-zA-Z0-9\\-_\\.]+"
 _MAX_NAME_LENGTH = 255
 # This could also be an attribute of JsonldField:
 _LIST_FIELDS = {"distribution", "fields", "record_sets"}
 _MISSING_JSONLD_TYPE = "__MISSING_JSONLD_TYPE__"
+MATCHING_TYPES = {
+    SDO.Boolean: bool,
+    SDO.Date: str,
+    SDO.DateTime: str,
+    SDO.Integer: int,
+    SDO.Number: float,
+    SDO.Text: str,
+    SDO.Time: str,
+    SDO.URL: str,
+}
 
 
 @dataclasses.dataclass(eq=False, repr=False)
 class Node:
     """Structure node in Croissant.
 
     This generic class will be inherited by the actual Croissant nodes:
@@ -49,21 +59,35 @@
         name: The name of the node.
         parents: The parent nodes in the Croissant JSON-LD as a tuple.
     """
 
     ctx: Context = dataclasses.field(default_factory=Context)
     id: str = dataclasses.field(default_factory=generate_uuid)
     name: str | None = None
-    parents: list[Node] = dataclasses.field(default_factory=list)
+    parents: list["Node"] = dataclasses.field(default_factory=list)
     jsonld: Any = None
 
     def __post_init__(self):
         """Checks exclusive properties."""
+        self._cast_fields()
         self._check_exclusive_properties()
 
+    def _cast_fields(self):
+        """Applies all `field.cast_fn`."""
+        for field in mlc_dataclasses.jsonld_fields(self):
+            if field.cast_fn:
+                try:
+                    value = getattr(self, field.name)
+                    new_value = field.cast_fn(value)
+                    setattr(self, field.name, new_value)
+                except WarningException as e:
+                    self.add_warning(repr(e))
+                except Exception as e:
+                    self.add_error(repr(e))
+
     def assert_has_mandatory_properties(self, *mandatory_properties: str):
         """Checks a node in the graph for existing properties with constraints.
 
         Args:
             mandatory_properties: A list of mandatory properties for the current node.
                 If the node doesn't have one, it triggers an error.
         """
@@ -177,63 +201,63 @@
             if len(self.parents) <= 1:
                 return self.name or ""
             return f"{self.parents[-1].uuid}/{self.name}"
         else:
             return self.id
 
     @property
-    def parent(self) -> Node | None:
+    def parent(self) -> "Node | None":
         """Direct parent of the node or None if no parent."""
         if not self.parents:
             return None
         return self.parents[-1]
 
     @property
-    def predecessors(self) -> set[Node]:
+    def predecessors(self) -> set["Node"]:
         """Predecessors in the structure graph."""
         return set(self.ctx.graph.predecessors(self))  # pytype: disable=bad-return-type
 
     @property
-    def recursive_predecessors(self) -> set[Node]:
+    def recursive_predecessors(self) -> set["Node"]:
         """Predecessors and predecessors of predecessors in the structure graph."""
         predecessors = set()
         for predecessor in self.predecessors:
             predecessors.add(predecessor)
             predecessors.update(predecessor.recursive_predecessors)
         return predecessors
 
     @property
-    def predecessor(self) -> Node | None:
+    def predecessor(self) -> "Node | None":
         """First predecessor in the structure graph."""
         if not self.ctx.graph.has_node(self):
             return None
         return next(
             self.ctx.graph.predecessors(self), None
         )  # pytype: disable=bad-return-type
 
     @property
-    def successors(self) -> tuple[Node, ...]:
+    def successors(self) -> tuple["Node", ...]:
         """Successors in the structure graph."""
         if self not in self.ctx.graph:
             return ()
         # We use tuples in order to have a hashable data structure to be put in input of
         # operations.
         return tuple(self.ctx.graph.successors(self))  # pytype: disable=bad-return-type
 
     @property
-    def recursive_successors(self) -> set[Node]:
+    def recursive_successors(self) -> set["Node"]:
         """Successors and successors of successors in the structure graph."""
         successors = set()
         for successor in self.successors:
             successors.add(successor)
             successors.update(successor.recursive_successors)
         return successors
 
     @property
-    def successor(self) -> Node | None:
+    def successor(self) -> "Node | None":
         """Direct successor in the structure graph."""
         if not self.ctx.graph.has_node(self):
             return None
         return next(
             self.ctx.graph.successors(self), None
         )  # pytype: disable=bad-return-type
 
@@ -320,28 +344,30 @@
                     value = [_value_to_jsonld(v) for v in value]
                 else:
                     value = _value_to_jsonld(value)
             # fields in _LIST_FIELDS are always lists, so we don't unbox them.
             if field.cardinality == "MANY" and field.name not in _LIST_FIELDS:
                 value = unbox_singleton_list(value)
             jsonld[key] = value
-        return remove_empty_values(jsonld)
+        jsonld = remove_empty_values(jsonld)
+        return sort_dict(jsonld)
 
     @classmethod
     def from_jsonld(cls, ctx: Context, jsonld: Json):
         """Creates a Python class from JSON-LD."""
         if not isinstance(jsonld, list) and not isinstance(jsonld, dict):
             name = cls._jsonld_type(ctx) or cls.__name__
             ctx.issues.add_error(f'{name} should be a dict with keys. Got "{jsonld}"')
             return None
         if cls._jsonld_type(ctx) == constants.SCHEMA_ORG_DATASET:
-            # For `Metadata` node, insert the conforms_to in the context:
+            # For `Metadata` node, insert conforms_to/is_live_dataset in the context:
             ctx.conforms_to = CroissantVersion.from_jsonld(
                 ctx, jsonld.get(constants.DCTERMS_CONFORMS_TO)
             )
+            ctx.is_live_dataset = jsonld.get(constants.ML_COMMONS_IS_LIVE_DATASET(ctx))
         if isinstance(jsonld, list):
             return [cls.from_jsonld(ctx, el) for el in jsonld]
         check_expected_type(ctx.issues, jsonld, cls._jsonld_type(ctx))
         kwargs = {}
         for field in mlc_dataclasses.jsonld_fields(cls):
             url = field.call_url(ctx)
             value = jsonld.get(url)
@@ -357,18 +383,15 @@
                     value = _value_from_input_types(ctx, value, field)
             if field.cardinality == "MANY" and value:
                 value = box_singleton_list(value) if value else []
             elif field.cardinality == "ONE" and isinstance(value, list):
                 value = value[0] if value else None
                 warning = f"`{field.name}` has cardinality `ONE`, but got a list"
                 ctx.issues.add_warning(warning)
-            if value is None:
-                if field.required:
-                    ctx.issues.add_warning(f"`{field.name}` is required, but got None")
-            else:
+            if value is not None:
                 kwargs[field.name] = value
         return cls(
             ctx=ctx,
             id=uuid_from_jsonld(jsonld),
             jsonld=jsonld,
             **kwargs,
         )
@@ -411,25 +434,15 @@
         if isinstance(value, dict) and _is_a_node(input_type):
             jsonld_type = input_type._jsonld_type(ctx)
             actual_jsonld_type = value.get("@type")
             if actual_jsonld_type == jsonld_type:
                 return input_type.from_jsonld(ctx, value)
         # ...or it's a basic int/str/bool/etc type
         else:
-            matching_types = {
-                SDO.Boolean: bool,
-                SDO.Date: str,
-                SDO.DateTime: str,
-                SDO.Integer: int,
-                SDO.Number: float,
-                SDO.Text: str,
-                SDO.Time: str,
-                SDO.URL: str,
-            }
-            matching_type = matching_types.get(input_type)
+            matching_type = MATCHING_TYPES.get(input_type)
             if type(value) is matching_type:
                 return value
     types = [
         input_type._jsonld_type(ctx) if _is_a_node(input_type) else str(input_type)
         for input_type in input_types
     ]
     if isinstance(value, dict):
@@ -456,7 +469,15 @@
         # For lists, we don't return field.default_factory() to not produce [[]]:
         return dataclasses.MISSING
     raise ValueError(f"{field.name} specifies neither default, nor default_factory")
 
 
 def _is_a_node(input_type: Any) -> bool:
     return inspect.isclass(input_type) and issubclass(input_type, Node)
+
+
+def node_by_uuid(ctx: Context, uuid: str | None) -> Node | None:
+    """Retrieves a node in the graph by its UID."""
+    for node in ctx.graph.nodes():
+        if node.uuid == uuid:  # pytype: disable=attribute-error
+            return node  # pytype: disable=bad-return-type
+    return None
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/base_node_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/base_node_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """base_node_test module."""
 
-from __future__ import annotations
-
 import dataclasses
 
 import pytest
 from rdflib.namespace import SDO
 
 from mlcroissant._src.core import dataclasses as mlc_dataclasses
 from mlcroissant._src.core.context import Context
@@ -183,44 +181,14 @@
     assert node.to_json() == {
         "@id": "foo",
         "@type": "foo.org/CustomNode",
         "foo.org/property1": 42,
     }
 
 
-def test_custom_node_with_required():
-    @mlc_dataclasses.dataclass
-    class CustomNode(base_node.Node):
-        JSONLD_TYPE = "foo.org/CustomNode"
-
-        property1: str | None = mlc_dataclasses.jsonld_field(
-            default="default property1",
-            input_types=[SDO.Text],
-            required=True,
-            url="foo.org/property1",
-        )
-        property2: str | None = mlc_dataclasses.jsonld_field(
-            default="default property2",
-            input_types=[SDO.Text],
-            required=False,
-            url="foo.org/property2",
-        )
-
-    node = CustomNode.from_jsonld(
-        Context(),
-        {
-            "@type": "foo.org/CustomNode",
-            "@id": "foo",
-        },
-    )
-    assert node.property1 == "default property1"
-    assert node.property2 == "default property2"
-    assert_contain_warning(node.ctx.issues, "`property1` is required, but got None")
-
-
 def test_custom_node_with_input_types():
     @mlc_dataclasses.dataclass
     class ChildNode(base_node.Node):
         JSONLD_TYPE = "foo.org/ChildNode"
 
         child: str | None = mlc_dataclasses.jsonld_field(
             default=None,
@@ -294,7 +262,38 @@
     assert_contain_error(
         node.ctx.issues,
         "`property1` should have type https://schema.org/Integer, but got str",
     )
     assert_contain_error(
         node.ctx.issues, "`property2` should have type foo.org/ChildNode, but got str"
     )
+
+
+def test_cast_fn():
+    def node(cast_fn):
+        @mlc_dataclasses.dataclass
+        class Node(base_node.Node):
+            JSONLD_TYPE = None
+
+            field: int | None = mlc_dataclasses.jsonld_field(
+                default=None,
+                cast_fn=cast_fn,
+                input_types=[SDO.Text],
+                url="foo.org/property1",
+            )
+
+        return Node
+
+    def cast_fn(value) -> int | None:
+        del value
+        return 42
+
+    Node = node(cast_fn)
+    assert Node(field="field").field == 42
+
+    def cast_fn(value) -> int | None:
+        del value
+        raise ValueError("bad value")
+
+    Node = node(cast_fn)
+    assert Node(field="field").field == "field"
+    assert_contain_error(Node(field="field").issues, "bad value")
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/graph.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/graph.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/graph_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/graph_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/creative_work.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/creative_work.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/croissant_version_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/croissant_version_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/field.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/field.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Field module."""
 
-from __future__ import annotations
-
 from rdflib import term
 from rdflib.namespace import SDO
+from typing_extensions import Self
 
 from mlcroissant._src.core import constants
 from mlcroissant._src.core import dataclasses as mlc_dataclasses
 from mlcroissant._src.core.constants import DataType
 from mlcroissant._src.core.context import CroissantVersion
 from mlcroissant._src.core.data_types import data_types_from_jsonld
 from mlcroissant._src.core.data_types import data_types_to_jsonld
 from mlcroissant._src.core.data_types import EXPECTED_DATA_TYPES
 from mlcroissant._src.structure_graph.base_node import Node
+from mlcroissant._src.structure_graph.base_node import node_by_uuid
 from mlcroissant._src.structure_graph.nodes.source import Source
 
 
 @mlc_dataclasses.dataclass
 class ParentField(Node):
     """Class for the `parentField` property."""
 
@@ -34,14 +34,16 @@
     )
 
 
 @mlc_dataclasses.dataclass
 class Field(Node):
     """Nodes to describe a dataset Field."""
 
+    JSONLD_TYPE = constants.ML_COMMONS_FIELD_TYPE
+
     description: str | None = mlc_dataclasses.jsonld_field(
         default=None,
         input_types=[SDO.Text],
         url=constants.SCHEMA_ORG_DESCRIPTION,
     )
     # `data_types` is different than `node.data_type`. See `data_type`'s docstring.
     data_types: list[term.URIRef] | None = mlc_dataclasses.jsonld_field(
@@ -108,33 +110,31 @@
         description=(
             "The data source of the field. This will generally reference a `FileObject`"
             " or `FileSet`'s contents (e.g., a specific column of a table)."
         ),
         input_types=[Source],
         url=constants.ML_COMMONS_SOURCE,
     )
-    sub_fields: list[Field] = mlc_dataclasses.jsonld_field(
+    sub_fields: list[Self] = mlc_dataclasses.jsonld_field(
         cardinality="MANY",
         default_factory=list,
         description="Another `Field` that is nested inside this one.",
         from_jsonld=lambda ctx, fields: Field.from_jsonld(ctx, fields),
         url=constants.ML_COMMONS_SUB_FIELD,
     )
 
     def __post_init__(self):
         """Checks arguments of the node."""
+        Node.__post_init__(self)
         uuid_field = "name" if self.ctx.is_v0() else "id"
         self.validate_name()
         self.assert_has_mandatory_properties(uuid_field)
-        self.assert_has_optional_properties("description")
         self.source.check_source(self.add_error)
         self._standardize_data_types()
 
-    JSONLD_TYPE = constants.ML_COMMONS_FIELD_TYPE
-
     def _standardize_data_types(self):
         """Converts data_types to a list of rdflib.URIRef."""
         data_types = self.data_types
         if data_types is None:
             data_types = []
         if not isinstance(data_types, list):
             data_types = [data_types]
@@ -162,15 +162,15 @@
                 DataType.IMAGE_OBJECT,
                 # For some reasons, pytype cannot infer `Any` on ctx:
                 DataType.BOUNDING_BOX(self.ctx),  # pytype: disable=wrong-arg-types
                 DataType.AUDIO_OBJECT,
             ]:
                 return term.URIRef(data_type)
         # The data_type has to be found on the source:
-        source = self.ctx.node_by_uuid(self.source.uuid)
+        source = node_by_uuid(self.ctx, self.source.uuid)
         if not isinstance(source, Field):
             self.add_error(
                 "The field does not specify a valid"
                 f" {constants.ML_COMMONS_DATA_TYPE(self.ctx)}, neither does any of"
                 f" its predecessor. Got: {self.data_types}"
             )
             return None
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/field_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/field_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -17,23 +17,18 @@
 @pytest.mark.parametrize(
     ["conforms_to", "field_uuid"],
     [[CroissantVersion.V_0_8, "name"], [CroissantVersion.V_1_0, "id"]],
 )
 def test_checks_are_performed(conforms_to, field_uuid):
     with mock.patch.object(
         Node, "assert_has_mandatory_properties"
-    ) as mandatory_mock, mock.patch.object(
-        Node, "assert_has_optional_properties"
-    ) as optional_mock, mock.patch.object(
-        Node, "validate_name"
-    ) as validate_name_mock:
+    ) as mandatory_mock, mock.patch.object(Node, "validate_name") as validate_name_mock:
         ctx = Context(conforms_to=conforms_to)
         create_test_node(Field, ctx=ctx)
         mandatory_mock.assert_called_once_with(field_uuid)
-        optional_mock.assert_called_once_with("description")
         validate_name_mock.assert_called_once()
 
 
 def test_data_type():
     # data_types can be a string:
     assert create_test_field(data_types=DataType.BOOL).data_types == [DataType.BOOL]
     # ...or a list of strings:
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/file_object.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_object.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """FileObject module."""
 
-from __future__ import annotations
-
 from rdflib.namespace import SDO
 
 from mlcroissant._src.core import constants
 from mlcroissant._src.core import dataclasses as mlc_dataclasses
 from mlcroissant._src.core.constants import ML_COMMONS
 from mlcroissant._src.core.uuid import formatted_uuid_to_json
 from mlcroissant._src.core.uuid import uuid_from_jsonld
@@ -74,15 +72,15 @@
             ' "images.zip".'
         ),
         input_types=[SDO.Text],
         url=SDO.name,
     )
     same_as: list[str] | None = mlc_dataclasses.jsonld_field(
         cardinality="MANY",
-        default_factory=list,
+        default=None,
         description=(
             "URL (or local name) of a FileObject with the same content, but in a"
             " different format."
         ),
         input_types=[SDO.URL],
         url=SDO.sameAs,
     )
@@ -97,17 +95,18 @@
         default_factory=Source,
         input_types=[Source],
         url=lambda ctx: ML_COMMONS(ctx).source,
     )
 
     def __post_init__(self):
         """Checks arguments of the node."""
+        Node.__post_init__(self)
         self.validate_name()
         uuid_field = "name" if self.ctx.is_v0() else "id"
         self.assert_has_mandatory_properties("encoding_format", uuid_field)
 
         if not self.contained_in:
             self.assert_has_mandatory_properties("content_url")
-            if self.ctx and not self.ctx.is_live_dataset:
+            if not self.ctx.is_live_dataset:
                 self.assert_has_exclusive_properties(["md5", "sha256"])
 
     JSONLD_TYPE = constants.SCHEMA_ORG_FILE_OBJECT
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/file_object_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_object_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/file_set.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """FileSet module."""
 
-from __future__ import annotations
-
 from rdflib.namespace import SDO
 
 from mlcroissant._src.core import constants
 from mlcroissant._src.core import dataclasses as mlc_dataclasses
 from mlcroissant._src.core.uuid import formatted_uuid_to_json
 from mlcroissant._src.core.uuid import uuid_from_jsonld
 from mlcroissant._src.structure_graph.base_node import Node
 
 
 @mlc_dataclasses.dataclass
 class FileSet(Node):
     """Nodes to describe a dataset FileSet (distribution)."""
 
+    JSONLD_TYPE = constants.SCHEMA_ORG_FILE_SET
+
     contained_in: list[str] | None = mlc_dataclasses.jsonld_field(
         cardinality="MANY",
         default_factory=list,
         description=(
             "Another FileObject or FileSet that this one is contained in, e.g., in the"
             " case of a file extracted from an archive. When this property is present,"
             " the contentUrl is evaluated as a relative path within the container"
@@ -64,12 +64,11 @@
         ),
         input_types=[SDO.Text],
         url=SDO.name,
     )
 
     def __post_init__(self):
         """Checks arguments of the node."""
+        Node.__post_init__(self)
         uuid_field = "name" if self.ctx.is_v0() else "id"
         self.validate_name()
         self.assert_has_mandatory_properties("includes", "encoding_format", uuid_field)
-
-    JSONLD_TYPE = constants.SCHEMA_ORG_FILE_SET
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/file_set_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/file_set_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/metadata.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """Metadata module."""
 
-from __future__ import annotations
-
 import datetime
-from typing import Any
 
 from etils import epath
 from rdflib.namespace import SDO
 import requests
+from typing_extensions import Self
 
 from mlcroissant._src.core import constants
 from mlcroissant._src.core import dataclasses as mlc_dataclasses
 from mlcroissant._src.core.context import Context
 from mlcroissant._src.core.context import CroissantVersion
-from mlcroissant._src.core.dates import from_str_to_datetime
+from mlcroissant._src.core.dates import cast_date
+from mlcroissant._src.core.dates import cast_dates
 from mlcroissant._src.core.issues import ValidationError
 from mlcroissant._src.core.json_ld import expand_jsonld
 from mlcroissant._src.core.json_ld import remove_empty_values
+from mlcroissant._src.core.json_ld import sort_dict
 from mlcroissant._src.core.rdf import Rdf
 from mlcroissant._src.core.types import Json
 from mlcroissant._src.core.url import is_url
+from mlcroissant._src.core.versions import cast_version
 from mlcroissant._src.structure_graph.base_node import Node
 from mlcroissant._src.structure_graph.graph import from_file_to_json
 from mlcroissant._src.structure_graph.graph import from_nodes_to_graph
 from mlcroissant._src.structure_graph.nodes.creative_work import CreativeWork
 from mlcroissant._src.structure_graph.nodes.field import Field
 from mlcroissant._src.structure_graph.nodes.file_object import FileObject
 from mlcroissant._src.structure_graph.nodes.file_set import FileSet
@@ -32,14 +33,16 @@
 from mlcroissant._src.structure_graph.nodes.record_set import RecordSet
 
 
 @mlc_dataclasses.dataclass
 class Metadata(Node):
     """Nodes to describe a dataset metadata."""
 
+    JSONLD_TYPE = constants.SCHEMA_ORG_DATASET
+
     cite_as: str | None = mlc_dataclasses.jsonld_field(
         default=None,
         description=(
             "A citation for a publication that describes the dataset. Ideally,"
             " citations should be expressed using the bibtex format. Note that this is"
             " different from schema.org/citation, which is used to make a citation to"
             " another publication from this dataset."
@@ -51,46 +54,43 @@
         cardinality="MANY",
         default_factory=list,
         description="The creator(s) of the dataset.",
         input_types=[Organization, Person],
         url=constants.SCHEMA_ORG_CREATOR,
     )
     date_created: datetime.datetime | None = mlc_dataclasses.jsonld_field(
+        cast_fn=cast_date,
         default=None,
         description="The date the dataset was initially created.",
         input_types=[SDO.Date, SDO.DateTime],
         url=constants.SCHEMA_ORG_DATE_CREATED,
     )
     date_modified: datetime.datetime | None = mlc_dataclasses.jsonld_field(
+        cast_fn=cast_date,
         default=None,
         description="The date the dataset was last modified.",
         input_types=[SDO.Date, SDO.DateTime],
         url=constants.SCHEMA_ORG_DATE_MODIFIED,
     )
     date_published: datetime.datetime | None = mlc_dataclasses.jsonld_field(
+        cast_fn=cast_date,
         default=None,
         description="The date the dataset was published.",
         input_types=[SDO.Date, SDO.DateTime],
         url=constants.SCHEMA_ORG_DATE_PUBLISHED,
     )
     description: str | None = mlc_dataclasses.jsonld_field(
         default=None,
         description="Description of the dataset.",
         input_types=[SDO.Text],
         url=constants.SCHEMA_ORG_DESCRIPTION,
     )
-    is_live_dataset: bool | None = mlc_dataclasses.jsonld_field(
-        default=None,
-        description="Whether the dataset is a live dataset.",
-        input_types=[SDO.Boolean],
-        url=constants.ML_COMMONS_IS_LIVE_DATASET,
-    )
     keywords: list[str] | None = mlc_dataclasses.jsonld_field(
         cardinality="MANY",
-        default_factory=list,
+        default=None,
         description=(
             "A set of keywords associated with the dataset, either as free text, or"
             " a DefinedTerm with a formal definition."
         ),
         input_types=[SDO.Text],
         url=constants.SCHEMA_ORG_KEYWORDS,
     )
@@ -125,15 +125,15 @@
             "The publisher of the dataset, which may be distinct from its creator."
         ),
         input_types=[Organization, Person],
         url=constants.SCHEMA_ORG_PUBLISHER,
     )
     same_as: list[str] | None = mlc_dataclasses.jsonld_field(
         cardinality="MANY",
-        default_factory=list,
+        default=None,
         description=(
             "The URL of another Web resource that represents the same dataset as this"
             " one."
         ),
         input_types=[SDO.URL],
         url=constants.SCHEMA_ORG_SAME_AS,
     )
@@ -153,14 +153,15 @@
             "The URL of the dataset. This generally corresponds to the Web page for"
             " the dataset."
         ),
         input_types=[SDO.URL],
         url=constants.SCHEMA_ORG_URL,
     )
     version: str | None = mlc_dataclasses.jsonld_field(
+        cast_fn=cast_version,
         default=None,
         description="The version of the dataset following the requirements below.",
         input_types=[SDO.Integer, SDO.Number, SDO.Text],
         url=constants.SCHEMA_ORG_VERSION,
     )
     distribution: list[FileObject | FileSet] = mlc_dataclasses.jsonld_field(
         cardinality="MANY",
@@ -171,131 +172,140 @@
     record_sets: list[RecordSet] = mlc_dataclasses.jsonld_field(
         cardinality="MANY",
         default_factory=list,
         input_types=[RecordSet],
         url=constants.ML_COMMONS_RECORD_SET,
     )
     data_collection: str | None = mlc_dataclasses.jsonld_field(
+        cardinality="ONE",
         default=None,
         input_types=[SDO.Text],
         url=constants.ML_COMMONS_RAI_DATA_COLLECTION,
     )
-    data_collection_type: str | None = mlc_dataclasses.jsonld_field(
+    data_collection_type: list[str] | None = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",
         default=None,
         input_types=[SDO.Text],
         url=constants.ML_COMMONS_RAI_DATA_COLLECTION_TYPE,
     )
-    data_collection_type_others: str | None = mlc_dataclasses.jsonld_field(
+    data_collection_missing_data: str | None = mlc_dataclasses.jsonld_field(
+        cardinality="ONE",
         default=None,
         input_types=[SDO.Text],
-        url=constants.ML_COMMONS_RAI_DATA_COLLECTION_TYPE_OTHERS,
+        url=constants.ML_COMMONS_RAI_DATA_COLLECTION_MISSING_DATA,
     )
-    data_collection_missing: str | None = mlc_dataclasses.jsonld_field(
+    data_collection_raw_data: str | None = mlc_dataclasses.jsonld_field(
+        cardinality="ONE",
         default=None,
         input_types=[SDO.Text],
-        url=constants.ML_COMMONS_RAI_DATA_COLLECTION_MISSING,
+        url=constants.ML_COMMONS_RAI_DATA_COLLECTION_RAW_DATA,
     )
-    data_collection_raw: str | None = mlc_dataclasses.jsonld_field(
-        default=None,
-        input_types=[SDO.Text],
-        url=constants.ML_COMMONS_RAI_DATA_COLLECTION_RAW,
-    )
-    data_collection_timeframe_start: datetime.datetime | None = (
-        mlc_dataclasses.jsonld_field(
-            default=None,
-            input_types=[SDO.Date, SDO.DateTime],
-            url=constants.ML_COMMONS_RAI_DATA_COLLECTION_TIMEFRAME_START,
-        )
-    )
-    data_collection_timeframe_end: datetime.datetime | None = (
+    data_collection_timeframe: list[datetime.datetime] | None = (
         mlc_dataclasses.jsonld_field(
+            cardinality="MANY",
+            cast_fn=cast_dates,
             default=None,
             input_types=[SDO.Date, SDO.DateTime],
-            url=constants.ML_COMMONS_RAI_DATA_COLLECTION_TIMEFRAME_END,
+            url=constants.ML_COMMONS_RAI_DATA_COLLECTION_TIME_FRAME,
         )
     )
-    data_preprocessing_imputation: str | None = mlc_dataclasses.jsonld_field(
+    data_imputation_protocol: str | None = mlc_dataclasses.jsonld_field(
+        cardinality="ONE",
         default=None,
         input_types=[SDO.Text],
-        url=constants.ML_COMMONS_RAI_DATA_PREPROCESSING_IMPUTATION,
+        url=constants.ML_COMMONS_RAI_DATA_IMPUTATION_PROTOCOL,
     )
-    data_preprocessing_protocol: str | None = mlc_dataclasses.jsonld_field(
+    data_preprocessing_protocol: list[str] | None = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",
         default=None,
         input_types=[SDO.Text],
         url=constants.ML_COMMONS_RAI_DATA_PREPROCESSING_PROTOCOL,
     )
-    data_preprocessing_manipulation: str | None = mlc_dataclasses.jsonld_field(
+    data_manipulation_protocol: str | None = mlc_dataclasses.jsonld_field(
+        cardinality="ONE",
         default=None,
         input_types=[SDO.Text],
-        url=constants.ML_COMMONS_RAI_DATA_PREPROCESSING_MANIPULATION,
+        url=constants.ML_COMMONS_RAI_DATA_DATA_MANIPULATION_PROTOCOL,
     )
-    data_annotation_protocol: str | None = mlc_dataclasses.jsonld_field(
+    data_annotation_protocol: list[str] | None = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",
         default=None,
         input_types=[SDO.Text],
         url=constants.ML_COMMONS_RAI_DATA_ANNOTATION_PROTOCOL,
     )
-    data_annotation_platform: str | None = mlc_dataclasses.jsonld_field(
+    data_annotation_platform: list[str] | None = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",
         default=None,
         input_types=[SDO.Text],
         url=constants.ML_COMMONS_RAI_DATA_ANNOTATION_PLATFORM,
     )
-    data_annotation_analysis: str | None = mlc_dataclasses.jsonld_field(
+    data_annotation_analysis: list[str] | None = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",
         default=None,
         input_types=[SDO.Text],
         url=constants.ML_COMMONS_RAI_DATA_ANNOTATION_ANALYSIS,
     )
-    data_annotation_peritem: str | None = mlc_dataclasses.jsonld_field(
+    annotations_per_item: str | None = mlc_dataclasses.jsonld_field(
+        cardinality="ONE",
         default=None,
         input_types=[SDO.Text],
-        url=constants.ML_COMMONS_RAI_DATA_ANNOTATION_PER_ITEM,
+        url=constants.ML_COMMONS_RAI_ANNOTATIONS_PER_ITEM,
     )
-    data_annotation_demographics: str | None = mlc_dataclasses.jsonld_field(
+    annotator_demographics: list[str] | None = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",
         default=None,
         input_types=[SDO.Text],
-        url=constants.ML_COMMONS_RAI_DATA_ANNOTATION_DEMOGRAPHICS,
+        url=constants.ML_COMMONS_RAI_ANNOTATOR_DEMOGRAPHICS,
     )
-    data_annotation_tools: str | None = mlc_dataclasses.jsonld_field(
+    machine_annotation_tools: list[str] | None = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",
         default=None,
         input_types=[SDO.Text],
-        url=constants.ML_COMMONS_RAI_DATA_ANNOTATION_TOOLS,
+        url=constants.ML_COMMONS_RAI_MACHINE_ANNOTATION_TOOLS,
     )
     data_biases: list[str] | None = mlc_dataclasses.jsonld_field(
         cardinality="MANY",
         default=None,
         input_types=[SDO.Text],
         url=constants.ML_COMMONS_RAI_DATA_BIASES,
     )
-    data_usecases: str | None = mlc_dataclasses.jsonld_field(
+    data_use_cases: list[str] | None = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",
         default=None,
         input_types=[SDO.Text],
         url=constants.ML_COMMONS_RAI_DATA_USE_CASES,
     )
-    data_limitation: str | None = mlc_dataclasses.jsonld_field(
+    data_limitations: list[str] | None = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",
         default=None,
         input_types=[SDO.Text],
-        url=constants.ML_COMMONS_RAI_DATA_LIMITATION,
+        url=constants.ML_COMMONS_RAI_DATA_LIMITATIONS,
     )
     data_social_impact: str | None = mlc_dataclasses.jsonld_field(
+        cardinality="ONE",
         default=None,
         input_types=[SDO.Text],
         url=constants.ML_COMMONS_RAI_DATA_SOCIAL_IMPACT,
     )
-    data_sensitive: str | None = mlc_dataclasses.jsonld_field(
+    personal_sensitive_information: list[str] | None = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",
         default=None,
         input_types=[SDO.Text],
-        url=constants.ML_COMMONS_RAI_DATA_SENSITIVE,
+        url=constants.ML_COMMONS_RAI_PERSONAL_SENSITIVE_INFORMATION,
     )
-    data_maintenance: str | None = mlc_dataclasses.jsonld_field(
+    data_release_maintenance_plan: str | None = mlc_dataclasses.jsonld_field(
+        cardinality="ONE",
         default=None,
         input_types=[SDO.Text],
-        url=constants.ML_COMMONS_RAI_DATA_MAINTENANCE,
+        url=constants.ML_COMMONS_RAI_DATA_RELEASE_MAINTENANCE_PLAN,
     )
 
     def __post_init__(self):
         """Checks arguments of the node and setup ID."""
+        Node.__post_init__(self)
         # Define parents.
         for node in self.distribution:
             node.parents = [self]
         for record_set in self.record_sets:
             record_set.parents = [self]
             for field in record_set.fields:
                 field.parents = [self, record_set]
@@ -304,19 +314,15 @@
 
         # Back-fill the graph in every node.
         self.ctx.graph = from_nodes_to_graph(self)
         self.check_graph()
 
         # Check properties.
         self.validate_name()
-        self.version = self.validate_version()
         self.license = self.validate_license()
-        self.date_created = self.validate_date(self.date_created)
-        self.date_modified = self.validate_date(self.date_modified)
-        self.date_published = self.validate_date(self.date_published)
         if self.ctx.is_v0():
             self.assert_has_mandatory_properties("name")
         self.assert_has_optional_properties(
             "cite_as", "date_published", "license", "version"
         )
 
         # Raise exception if there are errors.
@@ -324,28 +330,29 @@
             if node.ctx.issues.errors:
                 raise ValidationError(node.ctx.issues.report())
 
         self.ctx.conforms_to = CroissantVersion.from_jsonld(
             self.ctx, self.ctx.conforms_to
         )
 
-    JSONLD_TYPE = constants.SCHEMA_ORG_DATASET
-
     def to_json(self) -> Json:
         """Converts the `Metadata` to JSON."""
         context = self.ctx.rdf.context
         if "@base" in context:
             if context["@base"] == constants.BASE_IRI:
                 context.pop("@base")
         jsonld = super().to_json()
         jsonld.pop("@id", None)
         jsonld["@context"] = context
         conforms_to = self.ctx.conforms_to.to_json() if self.ctx.conforms_to else None
         jsonld["conformsTo"] = conforms_to
-        return remove_empty_values(jsonld)
+        if self.ctx.is_live_dataset:
+            jsonld["isLiveDataset"] = self.ctx.is_live_dataset
+        jsonld = remove_empty_values(jsonld)
+        return sort_dict(jsonld)
 
     @property
     def file_objects(self) -> list[FileObject]:
         """Gets `https://schema.org/FileObject` in the distribution."""
         return [
             file_object
             for file_object in self.distribution
@@ -366,45 +373,14 @@
         nodes.extend(self.record_sets)
         for record_set in self.record_sets:
             nodes.extend(record_set.fields)
             for field in record_set.fields:
                 nodes.extend(field.sub_fields)
         return nodes
 
-    def validate_version(self) -> str | None:
-        """Validates the given version and returns a normalized string version.
-
-        A valid version follows Semantic Versioning 2.0.0 `MAJOR.MINOR.PATCH`.
-        For more information: https://semver.org/spec/v2.0.0.html.
-        """
-        version = self.version
-
-        # Version is a recommended but not mandatory attribute.
-        if version is None:
-            return None
-
-        if isinstance(version, str):
-            numbers = version.split(".")
-            are_not_all_numbers = any(not number.isnumeric() for number in numbers)
-            if len(numbers) != 3 or are_not_all_numbers:
-                self.add_warning(
-                    f"Version doesn't follow MAJOR.MINOR.PATCH: {version}. For more"
-                    " information refer to: https://semver.org/spec/v2.0.0.html"
-                )
-            return version
-        elif isinstance(version, int):
-            return f"{version}.0.0"
-        elif isinstance(version, float):
-            return f"{version}.0"
-        else:
-            self.add_error(
-                f"The version should be a string or a number. Got: {type(version)}."
-            )
-            return None
-
     def validate_license(self) -> list[str | CreativeWork] | None:
         """Validates the license as a list of strings."""
         license = self.license
         input_types = (str, CreativeWork)
         if license is None:
             return None
         elif isinstance(license, list):
@@ -418,27 +394,14 @@
             return [license]
         else:
             self.add_error(
                 f"License should be a list of str or CreativeWork. Got: {license}"
             )
             return None
 
-    def validate_date(self, date: Any) -> datetime.datetime | None:
-        """Validates dates as a datetime for any input."""
-        if date is None:
-            return None
-        elif isinstance(date, str):
-            return from_str_to_datetime(self.ctx.issues, date)
-        elif isinstance(date, datetime.datetime):
-            return date
-        elif isinstance(date, datetime.date):
-            return datetime.datetime.combine(date, datetime.time.min)
-        self.add_error(f"Wrong type for a date. Expected Date or Datetime. Got: {date}")
-        return None
-
     def check_graph(self):
         """Checks the integrity of the structure graph.
 
         The rules are the following:
         - The graph is directed.
         - All fields have a data type: either directly specified, or on a parent.
 
@@ -451,27 +414,27 @@
             self.ctx.issues.add_error("The structure graph is not directed.")
         fields = [node for node in self.ctx.graph.nodes if isinstance(node, Field)]
         # Check all fields have a data type: either on the field, on a parent.
         for field in fields:
             field.data_type
 
     @classmethod
-    def from_file(cls, ctx: Context, file: epath.PathLike) -> Metadata:
+    def from_file(cls, ctx: Context, file: epath.PathLike) -> Self:
         """Creates the Metadata from a Croissant file."""
         if is_url(file):
             response = requests.get(file)
             json_ = response.json()
             return cls.from_json(ctx=ctx, json_=json_)
         folder, json_ = from_file_to_json(file)
         ctx.folder = folder
         return cls.from_json(ctx=ctx, json_=json_)
 
     @classmethod
     def from_json(
         cls,
         ctx: Context,
         json_: Json,
-    ) -> Metadata:
+    ) -> Self:
         """Creates a `Metadata` from JSON."""
         ctx.rdf = Rdf.from_json(ctx, json_)
         jsonld = expand_jsonld(json_, ctx=ctx)
         return cls.from_jsonld(ctx=ctx, jsonld=jsonld)
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/metadata_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/metadata_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     assert metadata.date_modified == datetime.datetime(1990, 2, 2, 0, 0)
     assert metadata.date_published == datetime.datetime(1990, 2, 3, 0, 0)
     assert len(metadata.license) == 2
     assert isinstance(metadata.license[0], CreativeWork)
     assert metadata.license[0].name == "U.S. Government Works"
     assert metadata.license[0].url == "https://www.usa.gov/government-works/"
     assert metadata.license[1] == "License"
-    assert metadata.is_live_dataset == False
+    assert metadata.ctx.is_live_dataset == False
     assert metadata.url == "https://mlcommons.org"
     assert metadata.version == "1.0.0"
     assert not ctx.issues.errors
     assert not ctx.issues.warnings
 
 
 @pytest.mark.parametrize(
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/organization.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/organization.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/person.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/person.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/record_set.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/record_set.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """RecordSet module."""
 
-from __future__ import annotations
-
 import itertools
 import json
 
 from rdflib import term
 from rdflib.namespace import SDO
 
 from mlcroissant._src.core import constants
 from mlcroissant._src.core import dataclasses as mlc_dataclasses
 from mlcroissant._src.core.context import Context
 from mlcroissant._src.core.data_types import data_types_from_jsonld
 from mlcroissant._src.core.data_types import data_types_to_jsonld
 from mlcroissant._src.core.types import Json
 from mlcroissant._src.structure_graph.base_node import Node
+from mlcroissant._src.structure_graph.base_node import node_by_uuid
 from mlcroissant._src.structure_graph.nodes.field import Field
 
 
 def json_from_jsonld(ctx: Context, data) -> Json | None:
     """Creates `data` from a JSON-LD fragment."""
     if isinstance(data, str):
         try:
@@ -30,14 +29,16 @@
     return None
 
 
 @mlc_dataclasses.dataclass
 class RecordSet(Node):
     """Nodes to describe a dataset RecordSet."""
 
+    JSONLD_TYPE = constants.ML_COMMONS_RECORD_SET_TYPE
+
     data: list[Json] | None = mlc_dataclasses.jsonld_field(
         cardinality="MANY",
         default=None,
         description="One or more records that constitute the data of the `RecordSet`.",
         from_jsonld=json_from_jsonld,
         url=constants.ML_COMMONS_DATA,
     )
@@ -67,15 +68,15 @@
         url=constants.ML_COMMONS_EXAMPLES,
     )
     is_enumeration: bool | None = mlc_dataclasses.jsonld_field(
         default=None,
         input_types=[SDO.Boolean],
         url=constants.ML_COMMONS_IS_ENUMERATION,
     )
-    key: str | list[str] | None = mlc_dataclasses.jsonld_field(
+    key: list[str] | None = mlc_dataclasses.jsonld_field(
         cardinality="MANY",
         default=None,
         description=(
             "One or more fields whose values uniquely identify each record in the"
             " `RecordSet`."
         ),
         input_types=[SDO.Text],
@@ -96,18 +97,18 @@
         ),
         input_types=[Field],
         url=constants.ML_COMMONS_FIELD,
     )
 
     def __post_init__(self):
         """Checks arguments of the node."""
+        Node.__post_init__(self)
         uuid_field = "name" if self.ctx.is_v0() else "id"
         self.validate_name()
         self.assert_has_mandatory_properties(uuid_field)
-        self.assert_has_optional_properties("description")
 
         if self.data is not None:
             data = self.data
             if not isinstance(data, list):
                 self.add_error(
                     f"{constants.ML_COMMONS_DATA(self.ctx)} should declare a list. Got:"
                     f" {type(data)}."
@@ -164,20 +165,18 @@
                 self.add_error(
                     f"You try to use the sources with names {ordered_combination} as"
                     " sources, but you didn't declare a join between them. Use"
                     " `ml:references` to declare a join. Please, refer to the"
                     " documentation for more information."
                 )
 
-    JSONLD_TYPE = constants.ML_COMMONS_RECORD_SET_TYPE
-
 
 def get_parent_uuid(ctx: Context, uuid: str) -> str | None:
     """Retrieves the UID of the parent, e.g. `file/column` -> `file`."""
-    node = ctx.node_by_uuid(uuid)
+    node = node_by_uuid(ctx, uuid)
     if node is None:
         ctx.issues.add_error(
             f"Node with uuid={uuid} does not exist. This error might have been found"
             " during a Join operation."
         )
         return None
     if isinstance(node, Field):
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/record_set_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/record_set_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -64,23 +64,18 @@
 @pytest.mark.parametrize(
     ["conforms_to", "field_uuid"],
     [[CroissantVersion.V_0_8, "name"], [CroissantVersion.V_1_0, "id"]],
 )
 def test_checks_are_performed(conforms_to, field_uuid):
     with mock.patch.object(
         Node, "assert_has_mandatory_properties"
-    ) as mandatory_mock, mock.patch.object(
-        Node, "assert_has_optional_properties"
-    ) as optional_mock, mock.patch.object(
-        Node, "validate_name"
-    ) as validate_name_mock:
+    ) as mandatory_mock, mock.patch.object(Node, "validate_name") as validate_name_mock:
         ctx = Context(conforms_to=conforms_to)
         create_test_node(RecordSet, ctx=ctx)
         mandatory_mock.assert_called_once_with(field_uuid)
-        optional_mock.assert_called_once_with("description")
         validate_name_mock.assert_called_once()
 
 
 @parametrize_conforms_to()
 def test_from_jsonld(conforms_to: CroissantVersion):
     ctx = Context(conforms_to=conforms_to)
     jsonld = {
@@ -110,16 +105,16 @@
     }
 
 
 @pytest.mark.parametrize(
     ["node_type", "uuid", "parent_uuid", "input", "output"],
     [
         [RecordSet, "foo", "other", "foo", "foo"],
-        [Field, "foo/bar", "foo", "bar", "foo"],
+        [Field, "foo/bar", "foo", "foo/bar", "foo"],
     ],
 )
 def test_get_parent_uuid(node_type, uuid, parent_uuid, input, output):
     mocked_node = mock.Mock(uuid=uuid, spec_set=node_type)
     mocked_node.parent.uuid = parent_uuid
     mocked_ctx = Context()
-    mocked_ctx.node_by_uuid = mock.Mock(return_value=mocked_node)
+    mocked_ctx.graph.nodes = lambda: [mocked_node]
     assert get_parent_uuid(mocked_ctx, input) == output
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/source.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 """Source module."""
 
-from __future__ import annotations
-
 import enum
 from typing import Any
 
 import jsonpath_rw
 from jsonpath_rw import lexer
 from rdflib.namespace import SDO
 
@@ -45,56 +43,56 @@
     """Checks if a string is a FileProperty (e.g., "content"->FileProperty.content)."""
     for possible_file_property in FileProperty:
         if possible_file_property.name == file_property:
             return True
     return False
 
 
+def _cast_file_property(file_property: Any) -> FileProperty | None:
+    if file_property is None:
+        return None
+    elif isinstance(file_property, str) and is_file_property(file_property):
+        return FileProperty[file_property]
+    raise ValueError(
+        "Property fileProperty can only have values in `fullpath`, `filepath` and"
+        f" `content`. Got: {file_property}"
+    )
+
+
 @mlc_dataclasses.dataclass
 class Extract(Node):
     """Container for possible ways of extracting the data.
 
     Args:
         column: The column in a columnar format (e.g., CSV).
         file_property: The property of a file to extract.
         json_path: The JSON path if the source is a JSON.
     """
 
     JSONLD_TYPE = None
 
     column: str | None = mlc_dataclasses.jsonld_field(
         default=None,
-        exclusive_with=["json_path"],
+        exclusive_with=["file_property", "json_path"],
         input_types=[SDO.Text],
         url=constants.ML_COMMONS_COLUMN,
     )
     file_property: FileProperty | None = mlc_dataclasses.jsonld_field(
+        cast_fn=_cast_file_property,
         default=None,
         input_types=[SDO.Text],
         to_jsonld=lambda ctx, fp: fp.name if isinstance(fp, FileProperty) else fp,
         url=constants.ML_COMMONS_FILE_PROPERTY,
     )
     json_path: str | None = mlc_dataclasses.jsonld_field(
         default=None,
         input_types=[SDO.Text],
         url=constants.ML_COMMONS_JSON_PATH,
     )
 
-    def __post_init__(self):
-        """Standardizes `self.file_property: FileProperty`."""
-        ctx = self.ctx
-        if isinstance(self.file_property, str) and is_file_property(self.file_property):
-            self.file_property = FileProperty[self.file_property]
-        elif self.file_property is not None:
-            ctx.issues.add_error(
-                f"Property {constants.ML_COMMONS_FILE_PROPERTY(ctx)} can only"
-                " have values in `fullpath`, `filepath` and `content`. Got:"
-                f" {self.file_property}"
-            )
-
 
 @mlc_dataclasses.dataclass
 class Transform(Node):
     """Container for transformation.
 
     Args:
         format: The format for a date (e.g. "%Y-%m-%d %H:%M:%S.%f") or for a bounding
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/structure_graph/nodes/source_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/structure_graph/nodes/source_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             constants.ML_COMMONS_COLUMN(ctx): "csv_column",
             constants.ML_COMMONS_JSON_PATH(ctx): "json_path",
         },
     }
     assert Source.from_jsonld(ctx, json_ld) == Source(
         extract=Extract(column="csv_column", json_path="json_path"),
     )
-    assert len(ctx.issues.errors) == 1
+    assert len(ctx.issues.errors) == 2
     assert_contain_error(
         ctx.issues, "Source should have one of the following properties"
     )
 
 
 @parametrize_conforms_to()
 def test_declaring_wrong_file_property(conforms_to):
```

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/tests/nodes.py` & `mlcroissant-1.0.4/mlcroissant/_src/tests/nodes.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/tests/records.py` & `mlcroissant-1.0.4/mlcroissant/_src/tests/records.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/tests/records_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/tests/records_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/torch/torch_adapter/dataloader.py` & `mlcroissant-1.0.4/mlcroissant/_src/torch/torch_adapter/dataloader.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/_src/torch/torch_adapter/dataloader_test.py` & `mlcroissant-1.0.4/mlcroissant/_src/torch/torch_adapter/dataloader_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/cli.py` & `mlcroissant-1.0.4/mlcroissant/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/documentation.py` & `mlcroissant-1.0.4/mlcroissant/scripts/documentation.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/load.py` & `mlcroissant-1.0.4/mlcroissant/scripts/load.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/load_test.py` & `mlcroissant-1.0.4/mlcroissant/scripts/load_test.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/migrations/migrate.py` & `mlcroissant-1.0.4/mlcroissant/scripts/migrations/migrate.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,15 @@
 
 from absl import app
 from absl import flags
 from etils import epath
 
 import mlcroissant as mlc
 from mlcroissant._src.core.context import Context
-from mlcroissant._src.core.json_ld import compact_jsonld
-from mlcroissant._src.core.json_ld import expand_jsonld
+from mlcroissant._src.core.rdf import make_context
 
 _PREVIOUS_MIGRATIONS_FOLDER = "previous"
 
 flags.DEFINE_string(
     "migration",
     None,
     "The name of the Python file with the migration.",
@@ -91,23 +90,43 @@
 
 
 def migrate_test_dataset(dataset: epath.Path, json_ld):
     """Migrates a test Croissant files.
 
     Cannot use mlc.Metadata as test Croissant files may contain errors.
     """
-    json_ld = compact_jsonld(expand_jsonld(json_ld, ctx=Context()))
+    # Here you can process json_ld as such:
+    # ```
+    # from mlcroissant._src.core.json_ld import compact_jsonld
+    # from mlcroissant._src.core.json_ld import expand_jsonld
+    # try:
+    #     json_ld = compact_jsonld(expand_jsonld(json_ld, ctx=Context()))
+    # except mlc.ValidationError:
+    #     pass
+    # ```
+    # But this behaviour is still bugged, so for now you have to perform all
+    # transformations in the up migration function.
+    if "@base" in json_ld["@context"]:
+        del json_ld["@context"]["@base"]
     # Special cases for test datasets without @context
     if "recordset_missing_context_for_datatype" in os.fspath(dataset):
         del json_ld["@context"]["dataType"]
     if "mlfield_missing_source" in os.fspath(dataset):
         del json_ld["@context"]["source"]
     return json_ld
 
 
+def standardize_context(json_ld):
+    """Standardizes the @context by merging it with the actual context."""
+    existing_context = json_ld["@context"]
+    context = make_context() | existing_context
+    json_ld["@context"] = context
+    return json_ld
+
+
 def main(argv):
     """Main function launched for the migration."""
     del argv
     version = FLAGS.version
     # Datasets in croissant/datasets
     datasets_path = (
         epath.Path(__file__).parent.parent.parent.parent.parent.parent
@@ -124,30 +143,31 @@
     )
     test_datasets = [
         p
         for p in test_path.glob("*/*.json")
         if not os.fspath(p).endswith("recordset_bad_type/metadata.json")
     ]
     assert test_datasets, f"No dataset found in {test_path}"
+    up = get_migration_fn(FLAGS.migration)
     for dataset in datasets:
         print(f"Converting {dataset}...")
         with dataset.open("r") as f:
             json_ld = json.load(f)
-            up = get_migration_fn(FLAGS.migration)
             json_ld = up(json_ld)
         json_ld = migrate_dataset(json_ld)
+        json_ld = standardize_context(json_ld)
         with dataset.open("w") as f:
             json.dump(json_ld, f, indent="  ")
             f.write("\n")
     for dataset in test_datasets:
         print(f"Converting test dataset {dataset}...")
         with dataset.open("r") as f:
             json_ld = json.load(f)
-            up = get_migration_fn(FLAGS.migration)
             json_ld = up(json_ld)
+        json_ld = standardize_context(json_ld)
         json_ld = migrate_test_dataset(dataset, json_ld)
         with dataset.open("w") as f:
             json.dump(json_ld, f, indent="  ")
             f.write("\n")
     print("Done.")
```

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202307171508.py` & `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202307171508.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202307201041.py` & `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202307201041.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202308312000.py` & `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202308312000.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202309061700.py` & `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202309061700.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202312062353.py` & `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202312062353.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202402051000.py` & `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202402051000.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202402201330.py` & `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202402201330.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/migrations/previous/202429011700.py` & `mlcroissant-1.0.4/mlcroissant/scripts/migrations/previous/202429011700.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant/scripts/validate.py` & `mlcroissant-1.0.4/mlcroissant/scripts/validate.py`

 * *Files identical despite different names*

### Comparing `mlcroissant-1.0.3/mlcroissant.egg-info/PKG-INFO` & `mlcroissant-1.0.4/mlcroissant.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcroissant
-Version: 1.0.3
+Version: 1.0.4
 Summary: MLCommons datasets format.
 Author: Joaquin Vanschoren, Jos van der Velde, Monjish Bhattacharyya, Omar Benjelloun, Peter Mattson, Pieter Gijsbers, Pierre Marcenac, Pierre Ruyssen, Prabhant Singh
 Description-Content-Type: text/markdown
 Requires-Dist: absl-py
 Requires-Dist: etils[epath]>=1.7.0
 Requires-Dist: jsonpath-rw
 Requires-Dist: networkx
@@ -123,14 +123,67 @@
 import mlcroissant as mlc
 metadata=mlc.nodes.Metadata(
   name="...",
 )
 metadata.to_json()  # this returns the JSON-LD file.
 ```
 
+## Add new properties to the standard
+
+Nodes (Metadata, RecordSets, etc) implement [PEP 681](https://peps.python.org/pep-0681/). So you can declare RDF triplets using the [dataclass](https://docs.python.org/3/library/dataclasses.html) syntax.
+
+**Example 1**: implement [CreativeWork](https://schema.org/CreativeWork):
+
+```python
+@mlc_dataclasses.dataclass
+class CreativeWork(Node):
+
+    JSONLD_TYPE = SDO.CreativeWork           # https://schema.org/CreativeWork
+
+    name: str | None = mlc_dataclasses.jsonld_field(
+        cardinality="ONE",                   # Cardinality can be ONE or MANY
+        default=None,                        # Specify the default value in Python
+        description="The name of the item.", # The full description
+        input_types=[SDO.Text],              # The schema.org type
+        url=SDO.name,                        # The URL of the property
+    )
+```
+
+**Example 2**: implement [RecordSet](https://mlcommons.github.io/croissant/docs/croissant-spec.html#recordset):
+
+```python
+@mlc_dataclasses.dataclass
+class RecordSet(Node):
+    JSONLD_TYPE = constants.ML_COMMONS_RECORD_SET_TYPE
+
+    fields: list[Field] = mlc_dataclasses.jsonld_field(
+        cardinality="MANY",                  # Example with cardinality=="MANY"
+        default_factory=list,
+        description=(
+            "A data element that appears in the records of the RecordSet (e.g., one"
+            " column of a table)."
+        ),
+        input_types=[Field],                 # Types can also be other nodes (here `Field`)
+        url=constants.ML_COMMONS_FIELD,
+    )
+```
+
+**Example 3**: specify a version (by default all versions):
+
+```python
+@mlc_dataclasses.dataclass
+class Field(Node):
+    is_enumeration: bool | None = mlc_dataclasses.jsonld_field(
+        default=None,
+        input_types=[SDO.Boolean],
+        url=constants.ML_COMMONS_IS_ENUMERATION,
+        versions=[CroissantVersion.V_0_8],   # `is_enumeration` is only valid for v0.8, not v1.0
+    )
+```
+
 ## Run tests
 
 All tests can be run from the Makefile:
 
 ```bash
 make tests
 ```
```

### Comparing `mlcroissant-1.0.3/mlcroissant.egg-info/SOURCES.txt` & `mlcroissant-1.0.4/mlcroissant.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 mlcroissant/_src/core/path.py
 mlcroissant/_src/core/rdf.py
 mlcroissant/_src/core/rdf_test.py
 mlcroissant/_src/core/types.py
 mlcroissant/_src/core/url.py
 mlcroissant/_src/core/uuid.py
 mlcroissant/_src/core/uuid_test.py
+mlcroissant/_src/core/versions.py
 mlcroissant/_src/core/graphs/__init__.py
 mlcroissant/_src/core/graphs/utils.py
 mlcroissant/_src/core/ml/__init__.py
 mlcroissant/_src/core/ml/bounding_box.py
 mlcroissant/_src/core/ml/bounding_box_test.py
 mlcroissant/_src/operation_graph/__init__.py
 mlcroissant/_src/operation_graph/base_operation.py
@@ -114,8 +115,10 @@
 mlcroissant/scripts/migrations/previous/202308312000.py
 mlcroissant/scripts/migrations/previous/202309061700.py
 mlcroissant/scripts/migrations/previous/202312062353.py
 mlcroissant/scripts/migrations/previous/202402011100.py
 mlcroissant/scripts/migrations/previous/202402020202.py
 mlcroissant/scripts/migrations/previous/202402051000.py
 mlcroissant/scripts/migrations/previous/202402201330.py
+mlcroissant/scripts/migrations/previous/202403270859.py
+mlcroissant/scripts/migrations/previous/202403271030.py
 mlcroissant/scripts/migrations/previous/202429011700.py
```

### Comparing `mlcroissant-1.0.3/pyproject.toml` & `mlcroissant-1.0.4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 # Project metadata. Available keys are documented at:
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 name = "mlcroissant"
 description = "MLCommons datasets format."
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name = "Joaquin Vanschoren" },
   { name = "Jos van der Velde" },
   { name = "Monjish Bhattacharyya" },
   { name = "Omar Benjelloun" },
   { name = "Peter Mattson" },
   { name = "Pieter Gijsbers" },
```

