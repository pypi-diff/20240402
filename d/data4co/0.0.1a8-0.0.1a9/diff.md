# Comparing `tmp/data4co-0.0.1a8.tar.gz` & `tmp/data4co-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data4co-0.0.1a8.tar", last modified: Sun Feb 11 16:13:56 2024, max compression
+gzip compressed data, was "data4co-0.0.1a9.tar", last modified: Sun Feb 11 16:18:44 2024, max compression
```

## Comparing `data4co-0.0.1a8.tar` & `data4co-0.0.1a9.tar`

### file list

```diff
@@ -1,724 +1,724 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.599282 data4co-0.0.1a8/
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-02-11 16:13:56.599282 data4co-0.0.1a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-11 16:13:49.000000 data4co-0.0.1a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.479282 data4co-0.0.1a8/data4co/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.479282 data4co-0.0.1a8/data4co/eva/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/eva/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/eva/tsp_eva.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.479282 data4co-0.0.1a8/data4co/generator/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/generator/mis_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/generator/tsp_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.479282 data4co-0.0.1a8/data4co/solver/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.483282 data4co-0.0.1a8/data4co/solver/mis/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/gurobi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.483282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/
--rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)   101393 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/Doxyfile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.483282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/
--rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/configuration_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/graphchecker.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/online_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/parse_parameters.h
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/parse_parameters_omis.h
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/reduction_evomis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/sort_adjacencies.cpp
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/cleanup.sh
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/compile_withcmake.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.467282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.463282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.483282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/app/
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/app/balance_configuration.h
--rw-r--r--   0 runner    (1001) docker     (127)    18484 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/app/configuration.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.483282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/interface/
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/interface/SConscript
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/interface/SConstruct
--rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.483282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.487282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)    16717 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.h
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.h
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.h
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.487282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/flow_graph.h
--rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_access.h
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.487282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.487282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/union_find.h
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/definitions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.487282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/io/
--rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.491282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/diversifyer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.491282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.491282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h
--rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.491282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.491282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.495282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h
--rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h
--rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.h
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.495282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/
--rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.495282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.495282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h
--rw-r--r--   0 runner    (1001) docker     (127)    14090 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.h
--rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.495282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h
--rw-r--r--   0 runner    (1001) docker     (127)    10512 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.499282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h
--rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.499282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/partition_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.499282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.499282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.503282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h
--rw-r--r--   0 runner    (1001) docker     (127)    24993 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18912 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.503282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h
--rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h
--rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.503282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     7702 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.507282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.507282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)    18924 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    25414 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.507282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.507282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/
--rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.507282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h
--rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.511282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.511282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/
--rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.511282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/
--rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.511282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/
--rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.515282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.h
--rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_partition_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.h
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.h
--rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.h
--rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.h
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/timer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.515282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   156123 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.c
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.519282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/echo.c
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/ls.c
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/multisyntax.c
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/mv.c
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog.c
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog_C89.c
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/testargtable3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/uname.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.519282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.c
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.h
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testall.c
--rw-r--r--   0 runner    (1001) docker     (127)    15949 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdate.c
--rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdbl.c
--rw-r--r--   0 runner    (1001) docker     (127)    26632 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargfile.c
--rw-r--r--   0 runner    (1001) docker     (127)    81374 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargint.c
--rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testarglit.c
--rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargrex.c
--rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargstr.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.471282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.523282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/array_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list.h
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list_online.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list_online.h
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation.h
--rw-r--r--   0 runner    (1001) docker     (127)    17497 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.h
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/operation_log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/operation_log.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.523282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/sparse_array_set.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.523282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.523282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.527282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/combine.h
--rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/diversifier.h
--rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.h
--rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.527282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/hopcroft/
--rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.527282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/ils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/ils.h
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/local_search.h
--rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/local_search_online.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/local_search_online.h
--rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/online_ils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/online_ils.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.531282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.h
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.h
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.531282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.471282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.471282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.531282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/
--rw-r--r--   0 runner    (1001) docker     (127)    70067 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.h
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.471282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.471282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.471282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.531282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.531282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/graph_access.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.531282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/definitions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.531282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/
--rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.535282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/timer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.535282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/
--rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ArraySet.h
--rw-r--r--   0 runner    (1001) docker     (127)    36218 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.h
--rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ProfilingHelper.h
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/Reduction.h
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SimpleSet.h
--rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SparseArraySet.h
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/bucket_pq.h
--rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/configuration_mis.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.535282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/array_set.h
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/fast_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.h
--rw-r--r--   0 runner    (1001) docker     (127)    67592 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.h
--rw-r--r--   0 runner    (1001) docker     (127)    67473 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/fast_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/modified.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/modified.h
--rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/mis_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.535282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/tools/mis_log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7978 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/tools/mis_log.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.539282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/misc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.539282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/misc/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/misc/conversion/dimacs_to_metis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/misc/conversion/metis_to_dimacs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/misc/conversion/sort_metis.py
--rw-r--r--   0 runner    (1001) docker     (127)    16853 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/misc/cpp.vim
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.539282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.539282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/app/
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/app/branch_reduce.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/app/configuration_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/app/merge_graph_weights.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/app/parse_parameters.h
--rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/app/weighted_ls.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.475282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.539282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.539282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/
--rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConscript
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConstruct
--rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.539282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.543282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.h
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.h
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.h
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.543282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/flow_graph.h
--rw-r--r--   0 runner    (1001) docker     (127)    15794 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_access.h
--rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.543282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/online_distance_matrix.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.543282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h
--rw-r--r--   0 runner    (1001) docker     (127)     9902 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
--rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/union_find.h
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/definitions.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.543282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/
--rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.547282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/
--rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.h
--rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.h
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.h
--rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.h
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.h
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.h
--rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.h
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.547282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/diversifyer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.547282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/
--rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.547282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/
--rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h
--rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h
--rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h
--rw-r--r--   0 runner    (1001) docker     (127)    16784 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.551282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.551282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.551282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h
--rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.h
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h
--rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.551282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/
--rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.551282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.555282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h
--rw-r--r--   0 runner    (1001) docker     (127)    14144 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.h
--rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.555282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h
--rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.555282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.h
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h
--rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.555282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/partition_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.555282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.555282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.559282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/
--rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h
--rw-r--r--   0 runner    (1001) docker     (127)    25053 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h
--rw-r--r--   0 runner    (1001) docker     (127)    10193 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.559282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h
--rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.563282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.563282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/
--rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.h
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.h
--rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.563282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.563282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h
--rw-r--r--   0 runner    (1001) docker     (127)    18978 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    25468 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.567282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.567282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/
--rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.567282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/
--rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h
--rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.567282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.567282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h
--rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.571282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.h
--rw-r--r--   0 runner    (1001) docker     (127)    31427 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h
--rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.571282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/
--rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.571282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/
--rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.575282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.h
--rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.h
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_partition_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_assertions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_common.h
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.h
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.h
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.h
--rw-r--r--   0 runner    (1001) docker     (127)    13611 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.h
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.h
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/timer.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.575282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)   156123 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.c
--rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.575282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/echo.c
--rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/ls.c
--rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/multisyntax.c
--rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/mv.c
--rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog.c
--rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog_C89.c
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/testargtable3.c
--rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/uname.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.579282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.c
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.h
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile.nmake
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testall.c
--rw-r--r--   0 runner    (1001) docker     (127)    15949 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdate.c
--rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdbl.c
--rw-r--r--   0 runner    (1001) docker     (127)    26632 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargfile.c
--rw-r--r--   0 runner    (1001) docker     (127)    81374 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargint.c
--rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testarglit.c
--rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargrex.c
--rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargstr.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.479282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.579282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/
--rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/array_set.h
--rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.h
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/dynamic_graph.h
--rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.h
--rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.579282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.h
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/sized_vector.h
--rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/sparse_array_set.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.583282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.583282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/
--rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/ils.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/ils.h
--rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.583282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/
--rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.h
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.h
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.583282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/
--rw-r--r--   0 runner    (1001) docker     (127)    25450 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.h
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/fast_set.h
--rw-r--r--   0 runner    (1001) docker     (127)    31140 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.h
--rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/mis_config.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.583282 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/tools/mis_log.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/tools/mis_log.h
--rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/mis/kamis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.587282 data4co-0.0.1a8/data4co/solver/tsp/
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/concorde.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/lkh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.587282 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.587282 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1200353 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/_concorde.c
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/_concorde.pyx
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/concorde.py
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/problem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/solution.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/tsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.599282 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/data/
--rw-r--r--   0 runner    (1001) docker     (127)  7630518 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/data/concorde.a
--rw-r--r--   0 runner    (1001) docker     (127)   248168 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/data/concorde.h
--rw-r--r--   0 runner    (1001) docker     (127)   854866 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/data/qsopt.a
--rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/data/qsopt.h
--rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.599282 data4co-0.0.1a8/data4co/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-02-11 16:13:49.000000 data4co-0.0.1a8/data4co/utils/tsp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.599282 data4co-0.0.1a8/data4co.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-02-11 16:13:56.000000 data4co-0.0.1a8/data4co.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    53704 2024-02-11 16:13:56.000000 data4co-0.0.1a8/data4co.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 16:13:56.000000 data4co-0.0.1a8/data4co.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-11 16:13:56.000000 data4co-0.0.1a8/data4co.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-11 16:13:56.000000 data4co-0.0.1a8/data4co.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-11 16:13:56.599282 data4co-0.0.1a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-02-11 16:13:49.000000 data4co-0.0.1a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:13:56.599282 data4co-0.0.1a8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-02-11 16:13:49.000000 data4co-0.0.1a8/tests/test_data4co.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.440405 data4co-0.0.1a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-02-11 16:18:44.440405 data4co-0.0.1a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2473 2024-02-11 16:18:34.000000 data4co-0.0.1a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.324405 data4co-0.0.1a9/data4co/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.328405 data4co-0.0.1a9/data4co/eva/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/eva/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/eva/tsp_eva.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.328405 data4co-0.0.1a9/data4co/generator/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8532 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/generator/mis_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9290 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/generator/tsp_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.328405 data4co-0.0.1a9/data4co/solver/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.328405 data4co-0.0.1a9/data4co/solver/mis/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/gurobi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.328405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/
+-rw-r--r--   0 runner    (1001) docker     (127)    11020 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   101393 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/Doxyfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.328405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     5294 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/configuration_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10626 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/graphchecker.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/online_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/parse_parameters.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/parse_parameters_omis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/reduction_evomis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/sort_adjacencies.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/cleanup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/compile_withcmake.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.316405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.312405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.332405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/app/balance_configuration.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18484 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/app/configuration.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.332405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/interface/SConscript
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/interface/SConstruct
+-rw-r--r--   0 runner    (1001) docker     (127)     9613 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.332405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.332405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)    16717 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.h
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9555 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.332405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     3691 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/flow_graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_access.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.336405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.336405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/union_find.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/definitions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.336405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     8825 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.336405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/diversifyer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.336405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)     9984 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.336405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12929 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16545 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.336405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.340405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.340405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11270 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3751 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.340405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/
+-rw-r--r--   0 runner    (1001) docker     (127)     7323 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.340405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.344405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14090 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5311 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.344405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10512 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.344405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5118 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.344405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8121 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/partition_config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.344405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.344405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.348405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30385 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    24993 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18912 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12415 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.348405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7173 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.352405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     7702 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2460 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.352405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.352405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8879 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18924 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6176 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25414 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.352405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.356405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)    10283 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.356405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/
+-rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3643 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13791 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.356405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.356405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     6417 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11539 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.356405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/
+-rw-r--r--   0 runner    (1001) docker     (127)     7158 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5432 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1542 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.356405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.360405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8316 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_partition_assertions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_assertions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7612 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.h
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7687 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/timer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.364405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   156123 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.364405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/echo.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/ls.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/multisyntax.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/mv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog_C89.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/testargtable3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/uname.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.368405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testall.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15949 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdbl.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26632 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargfile.c
+-rw-r--r--   0 runner    (1001) docker     (127)    81374 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargint.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testarglit.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargrex.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargstr.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.316405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.368405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/array_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list_online.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list_online.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7858 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17497 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8265 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/operation_log.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/operation_log.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.368405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/priority_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/sparse_array_set.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.368405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.372405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.372405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/combine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/combine.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13072 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5153 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9666 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5635 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.h
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/diversifier.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13116 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9147 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14632 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9045 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16938 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.372405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/hopcroft/
+-rw-r--r--   0 runner    (1001) docker     (127)     7813 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3321 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.372405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/
+-rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/ils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/ils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/local_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4962 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/local_search.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/local_search_online.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4893 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/local_search_online.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12821 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/online_ils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2854 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/online_ils.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.376405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.h
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.376405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.316405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.316405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.376405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/
+-rw-r--r--   0 runner    (1001) docker     (127)    70067 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.316405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.316405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.316405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.376405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.376405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/graph_access.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.376405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/definitions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.376405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/
+-rw-r--r--   0 runner    (1001) docker     (127)     8809 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.380405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_assertions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/timer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.380405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     8559 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ArraySet.h
+-rw-r--r--   0 runner    (1001) docker     (127)    36218 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12654 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ProfilingHelper.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/Reduction.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SimpleSet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8615 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SparseArraySet.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/bucket_pq.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2276 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/configuration_mis.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.380405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/array_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/fast_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7239 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    67592 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    67473 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/fast_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/modified.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3103 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/modified.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3575 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/mis_config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.380405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)    24348 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/tools/mis_log.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7978 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/tools/mis_log.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.380405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/misc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.380405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/misc/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/misc/conversion/dimacs_to_metis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/misc/conversion/metis_to_dimacs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/misc/conversion/sort_metis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16853 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/misc/cpp.vim
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.380405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.384405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/app/
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/app/branch_reduce.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/app/configuration_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/app/merge_graph_weights.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/app/parse_parameters.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6803 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/app/weighted_ls.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.324405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.384405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.384405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/
+-rw-r--r--   0 runner    (1001) docker     (127)     6659 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConscript
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConstruct
+-rw-r--r--   0 runner    (1001) docker     (127)    11971 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.384405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.384405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)    16771 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.h
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.384405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/flow_graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15794 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_access.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.388405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/online_distance_matrix.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.388405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     4807 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9902 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/union_find.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/definitions.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.388405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/
+-rw-r--r--   0 runner    (1001) docker     (127)    11170 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2982 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.388405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)     3657 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.h
+-rw-r--r--   0 runner    (1001) docker     (127)      509 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6735 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.h
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4917 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.392405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/diversifyer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.392405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/
+-rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.392405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14215 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h
+-rw-r--r--   0 runner    (1001) docker     (127)    16784 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.392405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.392405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.392405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1934 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11324 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9074 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.392405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/
+-rw-r--r--   0 runner    (1001) docker     (127)    14597 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.396405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.396405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h
+-rw-r--r--   0 runner    (1001) docker     (127)    14144 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9392 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.396405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11654 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.396405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5559 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.396405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)     9534 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/partition_config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.396405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.400405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.400405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/
+-rw-r--r--   0 runner    (1001) docker     (127)     9057 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    30439 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10666 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    25053 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10193 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    12325 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.404405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7233 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10044 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7225 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.404405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     7756 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.404405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/
+-rw-r--r--   0 runner    (1001) docker     (127)    10834 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3779 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13928 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     9130 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.404405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.404405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     7768 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8933 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h
+-rw-r--r--   0 runner    (1001) docker     (127)    18978 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6230 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    25468 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.408405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/
+-rw-r--r--   0 runner    (1001) docker     (127)     2618 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.408405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)    10337 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.408405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/
+-rw-r--r--   0 runner    (1001) docker     (127)     8648 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13845 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.408405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3555 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.408405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h
+-rw-r--r--   0 runner    (1001) docker     (127)    11593 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.408405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31427 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13781 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.408405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.412405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/
+-rw-r--r--   0 runner    (1001) docker     (127)     8151 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.412405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8370 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_partition_assertions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_assertions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_common.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.h
+-rw-r--r--   0 runner    (1001) docker     (127)    13611 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.h
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8622 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/timer.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.416405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5383 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)   156123 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11087 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.416405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3893 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/echo.c
+-rw-r--r--   0 runner    (1001) docker     (127)    16761 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/ls.c
+-rw-r--r--   0 runner    (1001) docker     (127)    10404 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/multisyntax.c
+-rw-r--r--   0 runner    (1001) docker     (127)     8779 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/mv.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6858 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog_C89.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/testargtable3.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5974 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/uname.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.420405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8103 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile.nmake
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testall.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15949 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    18636 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdbl.c
+-rw-r--r--   0 runner    (1001) docker     (127)    26632 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargfile.c
+-rw-r--r--   0 runner    (1001) docker     (127)    81374 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargint.c
+-rw-r--r--   0 runner    (1001) docker     (127)    21822 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testarglit.c
+-rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargrex.c
+-rw-r--r--   0 runner    (1001) docker     (127)    22381 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargstr.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.324405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.420405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/
+-rw-r--r--   0 runner    (1001) docker     (127)     6859 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/array_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2464 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/dynamic_graph.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10625 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1611 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.420405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/sized_vector.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/sparse_array_set.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.420405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.420405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/
+-rw-r--r--   0 runner    (1001) docker     (127)    11571 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/ils.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/ils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    12974 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7109 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.424405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/
+-rw-r--r--   0 runner    (1001) docker     (127)     2334 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.h
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.424405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/
+-rw-r--r--   0 runner    (1001) docker     (127)    25450 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     6065 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.h
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/fast_set.h
+-rw-r--r--   0 runner    (1001) docker     (127)    31140 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    10796 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/mis_config.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.424405 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     6968 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/tools/mis_log.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/tools/mis_log.h
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/mis/kamis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.424405 data4co-0.0.1a9/data4co/solver/tsp/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/concorde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/lkh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.424405 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.428405 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1200353 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/_concorde.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/_concorde.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/concorde.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/problem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/solution.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-02-11 16:18:34.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.436405 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  7630518 2024-02-11 16:18:35.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/data/concorde.a
+-rw-r--r--   0 runner    (1001) docker     (127)   248168 2024-02-11 16:18:35.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/data/concorde.h
+-rw-r--r--   0 runner    (1001) docker     (127)   854866 2024-02-11 16:18:35.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/data/qsopt.a
+-rw-r--r--   0 runner    (1001) docker     (127)    14871 2024-02-11 16:18:35.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/data/qsopt.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5644 2024-02-11 16:18:35.000000 data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.440405 data4co-0.0.1a9/data4co/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7719 2024-02-11 16:18:35.000000 data4co-0.0.1a9/data4co/utils/tsp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.440405 data4co-0.0.1a9/data4co.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3769 2024-02-11 16:18:44.000000 data4co-0.0.1a9/data4co.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    53704 2024-02-11 16:18:44.000000 data4co-0.0.1a9/data4co.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-11 16:18:44.000000 data4co-0.0.1a9/data4co.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-11 16:18:44.000000 data4co-0.0.1a9/data4co.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-11 16:18:44.000000 data4co-0.0.1a9/data4co.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-11 16:18:44.440405 data4co-0.0.1a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-02-11 16:18:35.000000 data4co-0.0.1a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-11 16:18:44.440405 data4co-0.0.1a9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-02-11 16:18:35.000000 data4co-0.0.1a9/tests/test_data4co.py
```

### Comparing `data4co-0.0.1a8/PKG-INFO` & `data4co-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data4co
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: data4co provides convenient dataset generators for the combinatorial optimization problem
 Home-page: https://github.com/heatingma/Data4CO
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -65,16 +65,16 @@
 Python >= 3.8
 numpy>=1.24.4
 networkx==2.8.8
 lkh>=1.1.1
 tsplib95==0.7.1
 tqdm>=4.66.1
 pulp>=2.8.0, 
-pandas>=2.2.0,
-scipy>=1.12.0
+pandas>=2.0.0,
+scipy>=1.10.1
 ```
 
 **PyPI**
 It is very convenient to directly use the following commands
 ```
 pip install data4co
 ```
```

### Comparing `data4co-0.0.1a8/README.md` & `data4co-0.0.1a9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 Python >= 3.8
 numpy>=1.24.4
 networkx==2.8.8
 lkh>=1.1.1
 tsplib95==0.7.1
 tqdm>=4.66.1
 pulp>=2.8.0, 
-pandas>=2.2.0,
-scipy>=1.12.0
+pandas>=2.0.0,
+scipy>=1.10.1
 ```
 
 **PyPI**
 It is very convenient to directly use the following commands
 ```
 pip install data4co
 ```
```

### Comparing `data4co-0.0.1a8/data4co/generator/mis_data.py` & `data4co-0.0.1a9/data4co/generator/mis_data.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/generator/tsp_data.py` & `data4co-0.0.1a9/data4co/generator/tsp_data.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/base.py` & `data4co-0.0.1a9/data4co/solver/mis/base.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/gurobi.py` & `data4co-0.0.1a9/data4co/solver/mis/gurobi.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/CMakeLists.txt` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/Doxyfile` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/Doxyfile`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/configuration_mis.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/configuration_mis.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/graphchecker.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/graphchecker.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/online_mis.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/online_mis.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/parse_parameters.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/parse_parameters.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/parse_parameters_omis.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/parse_parameters_omis.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/reduction_evomis.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/reduction_evomis.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/app/sort_adjacencies.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/app/sort_adjacencies.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/compile_withcmake.sh` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/compile_withcmake.sh`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/app/balance_configuration.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/app/balance_configuration.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/app/configuration.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/app/configuration.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/interface/SConscript` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/interface/SConscript`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/interface/SConstruct` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/interface/SConstruct`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/interface/kaHIP_interface.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/cycle_search.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/push_relabel.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/strongly_connected_components.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/algorithms/topological_sort.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/flow_graph.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/flow_graph.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_access.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_access.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/graph_hierarchy.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/matrix.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/matrix.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/union_find.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/data_structure/union_find.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/definitions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/definitions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/io/graph_io.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/diversifyer.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/diversifyer.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/parallel_mh/population.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/contraction.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/matching.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/graph_partitioner.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/partition_config.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/partition_config.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_communication.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_extractor.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_partition_assertions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/graph_partition_assertions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_assertions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_assertions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_common.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/macros_common.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/misc.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/mpi_tools.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/partition_snapshooter.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/quality_metrics.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/random_functions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/timer.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/KaHIP/lib/tools/timer.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/CMakeLists.txt` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/LICENSE` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile.nmake` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/README.md` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/argtable3.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/CMakeLists.txt` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile.nmake` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/echo.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/echo.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/ls.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/ls.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/multisyntax.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/multisyntax.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/mv.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/mv.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog_C89.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/myprog_C89.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/testargtable3.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/testargtable3.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/uname.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/examples/uname.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CMakeLists.txt` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/CuTest.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile.nmake` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testall.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testall.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdate.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdate.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdbl.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargdbl.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargfile.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargfile.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargint.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargint.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testarglit.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testarglit.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargrex.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargrex.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargstr.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/extern/argtable3-3.0.3/tests/testargstr.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/array_set.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/array_set.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list_online.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list_online.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list_online.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/candidate_list_online.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/mis_permutation_online.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/operation_log.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/operation_log.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/operation_log.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/operation_log.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/priority_queues/bucket_array.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/data_structure/sparse_array_set.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/data_structure/sparse_array_set.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/cover_combine.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/multiway_combine.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/combine/separator_combine.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/diversifier.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/diversifier.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/population_mis.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/reduction_evolution.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/evolutionary/separator_pool.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/hopcroft/bipartite_vertex_cover.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/ils.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/ils.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/ils.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/ils.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/local_search.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/local_search.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/local_search.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/local_search.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/local_search_online.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/local_search_online.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/local_search_online.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/local_search_online.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/online_ils.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/online_ils.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/ils/online_ils.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/ils/online_ils.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_mis_online.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/greedy_vertex.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/initial_mis.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/initial_mis/random_mis.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Graph.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/LinearTime/MIS_sigmod_pub/Utility.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/graph_access.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/graph_access.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/definitions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/definitions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/io/graph_io.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_assertions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_assertions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_common.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/macros_common.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/timer.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/extern/KaHIP/lib/tools/timer.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ArraySet.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ArraySet.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/MaximumMatching.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ProfilingHelper.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/ProfilingHelper.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/Reduction.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/Reduction.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SimpleSet.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SimpleSet.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SparseArraySet.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/SparseArraySet.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/bucket_pq.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/bucket_pq.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/configuration_mis.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/configuration_mis.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/array_set.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/data_structures/array_set.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/fast_set.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/fast_set.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/full_reductions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/ParFastKer/fast_reductions/src/parallel_reductions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/branch_and_reduce_algorithm.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/fast_set.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/fast_set.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/modified.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/modified.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/kernel/modified.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/kernel/modified.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/mis/mis_config.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/mis/mis_config.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/tools/mis_log.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/tools/mis_log.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/lib/tools/mis_log.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/lib/tools/mis_log.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/misc/conversion/dimacs_to_metis.py` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/misc/conversion/dimacs_to_metis.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/misc/conversion/metis_to_dimacs.py` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/misc/conversion/metis_to_dimacs.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/misc/conversion/sort_metis.py` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/misc/conversion/sort_metis.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/misc/cpp.vim` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/misc/cpp.vim`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/CMakeLists.txt` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/app/branch_reduce.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/app/branch_reduce.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/app/configuration_mis.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/app/configuration_mis.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/app/merge_graph_weights.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/app/merge_graph_weights.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/app/parse_parameters.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/app/parse_parameters.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/app/weighted_ls.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/app/weighted_ls.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/LICENSE` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/LICENSE`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConscript` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConscript`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConstruct` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/SConstruct`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/interface/kaHIP_interface.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/cycle_search.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/push_relabel.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/strongly_connected_components.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/algorithms/topological_sort.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/flow_graph.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/flow_graph.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_access.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_access.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/graph_hierarchy.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/matrix.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/matrix.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/normal_matrix.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/online_distance_matrix.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/matrix/online_distance_matrix.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/bucket_pq.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/maxNodeHeap.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/priority_queues/priority_queue_interface.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/union_find.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/data_structure/union_find.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/definitions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/definitions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/io/graph_io.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/communication_graph_search_space.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_distance_matrix.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/construct_mapping.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/fast_construct_mapping.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/full_search_space_pruned.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/local_search_mapping.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/mapping/mapping_algorithms.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/diversifyer.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/diversifyer.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/exchange/exchanger.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/construct_partition.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/galinier_combine/gal_combine.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/parallel_mh_async.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/parallel_mh/population.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/node_ordering.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/clustering/size_constraint_label_propagation.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/coarsening_configurator.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/contraction.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/edge_rating/edge_ratings.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/compare_degrees.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/compare_rating.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/gpa_matching.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/gpa/path_set.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/matching.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/matching/random_matching.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/coarsening/stop_rules/stop_rules.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/graph_partitioner.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/bipartition.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_node_separator.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partition_bipartition.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioner.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_partitioning.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/initial_partitioning/initial_refinement/initial_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/partition_config.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/partition_config.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/advanced_models.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/augmented_Qgraph_fabric.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_definitions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/cycle_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/greedy_neg_cycle.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/cycle_improvements/problem_factory.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_commons.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_graph_refinement_core.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/kway_stop_rule.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/kway_graph_refinement/multitry_kway_fm.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/label_propagation_refinement/label_propagation_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/mixed_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/fm_ns_local_search.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/greedy_ns_local_search.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/node_separators/localized_fm_ns_local_search.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/partition_accept_rule.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/queue_selection_strategie.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/search_stop_rule.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/two_way_fm.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/2way_fm_refinement/vertex_moved_hashtable.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/boundary_lookup.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/complete_boundary.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/boundary_bfs.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/flow_solving_kernel/cut_flow_problem_solver.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/most_balanced_minimum_cuts/most_balanced_minimum_cuts.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/flow_refinement/two_way_flow_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/partial_boundary.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/active_block_quotient_graph_scheduler.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/quotient_graph_scheduling.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/quotient_graph_scheduling/simple_quotient_graph_scheduler.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/quotient_graph_refinement/two_way_refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/refinement.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_bucket_queue.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_moves_queue.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/refinement/tabu_search/tabu_search.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/area_bfs.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_algorithm.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/separator/vertex_separator_flow_solver.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/uncoarsening/uncoarsening.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/partition/w_cycles/wcycle_partitioner.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/spac/spac.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_communication.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_extractor.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_partition_assertions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/graph_partition_assertions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_assertions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_assertions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_common.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/macros_common.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/misc.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/mpi_tools.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/partition_snapshooter.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/quality_metrics.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/random_functions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/timer.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/KaHIP/lib/tools/timer.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/CMakeLists.txt` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/LICENSE` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile.nmake` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/README.md` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/README.md`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/argtable3.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/CMakeLists.txt` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile.nmake` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/echo.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/echo.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/ls.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/ls.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/multisyntax.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/multisyntax.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/mv.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/mv.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog_C89.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/myprog_C89.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/testargtable3.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/testargtable3.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/uname.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/examples/uname.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CMakeLists.txt` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/CuTest.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile.nmake` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/Makefile.nmake`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testall.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testall.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdate.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdate.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdbl.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargdbl.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargfile.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargfile.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargint.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargint.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testarglit.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testarglit.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargrex.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargrex.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargstr.c` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/extern/argtable3-3.0.3/tests/testargstr.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/array_set.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/array_set.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/candidate_list.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/dynamic_graph.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/dynamic_graph.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/mis_permutation.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/operation_log.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/priority_queues/bucket_array.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/sized_vector.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/sized_vector.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/data_structure/sparse_array_set.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/data_structure/sparse_array_set.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/ils.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/ils.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/ils.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/ils.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/ils/local_search.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_mis.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/greedy_vertex.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/initial_mis.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/initial_mis/random_mis.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/branch_and_reduce_algorithm.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/fast_set.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/fast_set.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/kernel/reductions.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/mis/mis_config.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/mis/mis_config.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/tools/mis_log.cpp` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/tools/mis_log.cpp`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis-source/wmis/lib/tools/mis_log.h` & `data4co-0.0.1a9/data4co/solver/mis/kamis-source/wmis/lib/tools/mis_log.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/mis/kamis.py` & `data4co-0.0.1a9/data4co/solver/mis/kamis.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/base.py` & `data4co-0.0.1a9/data4co/solver/tsp/base.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/concorde.py` & `data4co-0.0.1a9/data4co/solver/tsp/concorde.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/lkh.py` & `data4co-0.0.1a9/data4co/solver/tsp/lkh.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/_concorde.c` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/_concorde.c`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/_concorde.pyx` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/_concorde.pyx`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/concorde.py` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/concorde.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/problem.py` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/problem.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/solution.py` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/solution.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/testing.py` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/testing.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/tsp.py` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/tsp.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/concorde/util.py` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/concorde/util.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/data/concorde.a` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/data/concorde.a`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/data/concorde.h` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/data/concorde.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/data/qsopt.a` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/data/qsopt.a`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/data/qsopt.h` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/data/qsopt.h`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/solver/tsp/pyconcorde/setup.py` & `data4co-0.0.1a9/data4co/solver/tsp/pyconcorde/setup.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co/utils/tsp_utils.py` & `data4co-0.0.1a9/data4co/utils/tsp_utils.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/data4co.egg-info/PKG-INFO` & `data4co-0.0.1a9/data4co.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data4co
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: data4co provides convenient dataset generators for the combinatorial optimization problem
 Home-page: https://github.com/heatingma/Data4CO
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -65,16 +65,16 @@
 Python >= 3.8
 numpy>=1.24.4
 networkx==2.8.8
 lkh>=1.1.1
 tsplib95==0.7.1
 tqdm>=4.66.1
 pulp>=2.8.0, 
-pandas>=2.2.0,
-scipy>=1.12.0
+pandas>=2.0.0,
+scipy>=1.10.1
 ```
 
 **PyPI**
 It is very convenient to directly use the following commands
 ```
 pip install data4co
 ```
```

### Comparing `data4co-0.0.1a8/data4co.egg-info/SOURCES.txt` & `data4co-0.0.1a9/data4co.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/setup.py` & `data4co-0.0.1a9/setup.py`

 * *Files identical despite different names*

### Comparing `data4co-0.0.1a8/tests/test_data4co.py` & `data4co-0.0.1a9/tests/test_data4co.py`

 * *Files identical despite different names*

