# Comparing `tmp/bmtk-1.0.8.tar.gz` & `tmp/bmtk-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmtk-1.0.8.tar", last modified: Sun Jul  2 17:52:21 2023, max compression
+gzip compressed data, was "bmtk-1.1.0.tar", last modified: Mon Apr  1 22:47:51 2024, max compression
```

## Comparing `bmtk-1.0.8.tar` & `bmtk-1.1.0.tar`

### file list

```diff
@@ -1,425 +1,432 @@
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.485474 bmtk-1.0.8/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1482 2019-10-23 23:40:04.000000 bmtk-1.0.8/LICENSE.txt
--rw-rw-r--   0 kael      (1000) kael      (1000)      120 2023-06-21 19:55:18.000000 bmtk-1.0.8/MANIFEST.in
--rw-rw-r--   0 kael      (1000) kael      (1000)     3215 2023-07-02 17:52:21.485474 bmtk-1.0.8/PKG-INFO
--rw-rw-r--   0 kael      (1000) kael      (1000)     2223 2022-10-25 18:55:38.000000 bmtk-1.0.8/README.md
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.433472 bmtk-1.0.8/bmtk/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1543 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/__init__.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.437472 bmtk-1.0.8/bmtk/analyzer/
--rw-rw-r--   0 kael      (1000) kael      (1000)     7931 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/analyzer/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4336 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/analyzer/cell_vars.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9180 2022-06-14 03:21:44.000000 bmtk-1.0.8/bmtk/analyzer/compartment.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3594 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/analyzer/ecp.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3751 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/analyzer/firing_rates.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      391 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/analyzer/io_tools.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17928 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/analyzer/spike_trains.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4787 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/analyzer/spikes_analyzer.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3890 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/analyzer/spikes_loader.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      211 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/analyzer/utils.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.437472 bmtk-1.0.8/bmtk/builder/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1580 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/__init__.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.437472 bmtk-1.0.8/bmtk/builder/auxi/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1520 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/builder/auxi/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2515 2020-07-29 19:00:45.000000 bmtk-1.0.8/bmtk/builder/auxi/edge_connectors.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    40569 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/builder/auxi/node_params.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.437472 bmtk-1.0.8/bmtk/builder/bionet/
--rw-rw-r--   0 kael      (1000) kael      (1000)      750 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/builder/bionet/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    19079 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/builder/bionet/swc_reader.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4784 2023-04-26 15:31:12.000000 bmtk-1.0.8/bmtk/builder/builder_utils.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9773 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/connection_map.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1796 2023-04-26 18:17:06.000000 bmtk-1.0.8/bmtk/builder/connector.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3033 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/edge.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.437472 bmtk-1.0.8/bmtk/builder/edges_sorter/
--rw-rw-r--   0 kael      (1000) kael      (1000)      962 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/edges_sorter/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4007 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/edges_sorter/memory_sorter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    27610 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/edges_sorter/merge_sorter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2504 2023-04-26 18:18:24.000000 bmtk-1.0.8/bmtk/builder/functor_cache.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3089 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/id_generator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17456 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/index_builders.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     5336 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/builder/iterator.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.441473 bmtk-1.0.8/bmtk/builder/network_adaptors/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1632 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    19870 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/dm_network.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    23846 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/dm_network_orig.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    11489 2023-04-26 15:31:12.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/edge_props_table.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    21380 2023-04-26 15:31:12.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/edges_collator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    32560 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/network.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3057 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/network_adaptors/nxnetwork.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    30657 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/builder/network_builder.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      179 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/networks.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3055 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/node.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4202 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/builder/node_pool.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3077 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/builder/node_set.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.441473 bmtk-1.0.8/bmtk/simulator/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1521 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/__init__.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.441473 bmtk-1.0.8/bmtk/simulator/bionet/
--rw-rw-r--   0 kael      (1000) kael      (1000)      153 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/README.md
--rw-rw-r--   0 kael      (1000) kael      (1000)     1844 2023-06-21 19:53:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    20932 2023-02-15 16:38:57.000000 bmtk-1.0.8/bmtk/simulator/bionet/biocell.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17281 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/simulator/bionet/bionetwork.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17779 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/biosimulator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3883 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/cell.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2367 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/config.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.445473 bmtk-1.0.8/bmtk/simulator/bionet/default_setters/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1606 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_setters/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17512 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_setters/cell_models.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6112 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_setters/synapse_models.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2449 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_setters/synaptic_weights.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.445473 bmtk-1.0.8/bmtk/simulator/bionet/default_templates/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1036 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_templates/BioAxonStub.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)      608 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_templates/Biophys1.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)      239 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/default_templates/advance.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)     1110 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/gids.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3125 2023-03-23 01:37:03.000000 bmtk-1.0.8/bmtk/simulator/bionet/iclamp.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.445473 bmtk-1.0.8/bmtk/simulator/bionet/import3d/
--rw-rw-r--   0 kael      (1000) kael      (1000)    28325 2022-01-20 23:00:55.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/import3d_gui.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)    10086 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/import3d_sec.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)     2038 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_morphml.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)    16444 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_nlcda.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)    27594 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_nlcda3.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)     7697 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_nts.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)    12318 2022-01-20 23:00:55.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_swc.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)      335 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/import3d.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)     1905 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/io_tools.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.445473 bmtk-1.0.8/bmtk/simulator/bionet/modules/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1895 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6515 2023-04-26 15:31:12.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/comsol.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1434 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/ecephys_module.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    12928 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/ecp.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     5867 2023-03-23 01:37:03.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/iclamp.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    13828 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/record_cellvars.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4732 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/record_clamp.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9514 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/record_netcons.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4898 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/record_spikes.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17767 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/save_synapses.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3356 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/sim_module.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6994 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/xstim.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4012 2023-02-15 16:42:21.000000 bmtk-1.0.8/bmtk/simulator/bionet/modules/xstim_waveforms.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    23657 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/morphology.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     5482 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/nml_reader.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3537 2022-08-22 22:07:50.000000 bmtk-1.0.8/bmtk/simulator/bionet/nrn.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6924 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/pointprocesscell.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      371 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/pointsomacell.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1679 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/pyfunction_cache.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.449473 bmtk-1.0.8/bmtk/simulator/bionet/schemas/
--rw-rw-r--   0 kael      (1000) kael      (1000)     3335 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/schemas/config_schema.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      536 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/schemas/csv_edge_types.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      170 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/schemas/csv_node_types_external.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      347 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/schemas/csv_node_types_internal.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      162 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/schemas/csv_nodes_external.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      456 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/schemas/csv_nodes_internal.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     2257 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/seclamp.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     8019 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/bionet/sonata_adaptors.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4278 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/bionet/utils.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3596 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/bionet/virtualcell.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.449473 bmtk-1.0.8/bmtk/simulator/core/
--rw-rw-r--   0 kael      (1000) kael      (1000)        0 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/core/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      426 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/core/edge_population.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    15605 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/simulator/core/graph.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4666 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/core/io_tools.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.449473 bmtk-1.0.8/bmtk/simulator/core/modules/
--rw-rw-r--   0 kael      (1000) kael      (1000)        0 2023-03-23 01:37:03.000000 bmtk-1.0.8/bmtk/simulator/core/modules/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17106 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/core/modules/ecephys_module.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6954 2023-03-23 01:37:03.000000 bmtk-1.0.8/bmtk/simulator/core/modules/iclamp.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3186 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/core/modules/ndx-aibs-ecephys.extension.yaml
--rw-rw-r--   0 kael      (1000) kael      (1000)      250 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/core/modules/ndx-aibs-ecephys.namespace.yaml
--rw-rw-r--   0 kael      (1000) kael      (1000)     3355 2023-03-23 01:37:03.000000 bmtk-1.0.8/bmtk/simulator/core/modules/simulator_module.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1772 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/core/network_reader.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      886 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/core/node_population.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1928 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/core/node_sets.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    13708 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/simulator/core/pyfunction_cache.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4610 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/core/simulation_config.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6008 2022-06-14 03:21:34.000000 bmtk-1.0.8/bmtk/simulator/core/simulation_config_validator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      203 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/core/simulator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    10605 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/simulator/core/simulator_network.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.449473 bmtk-1.0.8/bmtk/simulator/core/sonata_reader/
--rw-rw-r--   0 kael      (1000) kael      (1000)      159 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/core/sonata_reader/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     7777 2023-04-26 15:31:12.000000 bmtk-1.0.8/bmtk/simulator/core/sonata_reader/edge_adaptor.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    10541 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/core/sonata_reader/network_reader.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     7783 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/core/sonata_reader/node_adaptor.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.449473 bmtk-1.0.8/bmtk/simulator/core/sonata_schemas/
--rw-rw-r--   0 kael      (1000) kael      (1000)     4394 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/core/sonata_schemas/config_schema.json
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.453473 bmtk-1.0.8/bmtk/simulator/filternet/
--rw-rw-r--   0 kael      (1000) kael      (1000)      234 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1782 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/cell.py
--rw-rw-r--   0 kael      (1000) kael      (1000)       57 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/cell_models.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      691 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/config.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.453473 bmtk-1.0.8/bmtk/simulator/filternet/default_setters/
--rw-rw-r--   0 kael      (1000) kael      (1000)       28 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/default_setters/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9248 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/simulator/filternet/default_setters/cell_loaders.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2046 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/filternetwork.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      185 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/filters.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     7136 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/filternet/filtersimulator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      756 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/io_tools.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.453473 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/
--rw-rw-r--   0 kael      (1000) kael      (1000)      195 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/__init__.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.457473 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/
--rwxrwxr-x   0 kael      (1000) kael      (1000)    15615 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/sOFF_cell_data.csv
--rwxrwxr-x   0 kael      (1000) kael      (1000)    12437 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/sON_cell_data.csv
--rwxrwxr-x   0 kael      (1000) kael      (1000)     4186 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/sus_sus_cells_v3.csv
--rwxrwxr-x   0 kael      (1000) kael      (1000)     9904 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/tOFF_cell_data.csv
--rwxrwxr-x   0 kael      (1000) kael      (1000)     1003 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/tON_cell_data.csv
--rwxrwxr-x   0 kael      (1000) kael      (1000)     2783 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/trans_sus_cells_v3.csv
--rw-rw-r--   0 kael      (1000) kael      (1000)     6361 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cellmetrics.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6596 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cellmodel.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9019 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cursor.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3567 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/fitfuns.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4642 2023-02-15 16:42:21.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/gaborfilter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    16117 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/kernel.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9140 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/lattice_unit_constructor.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2111 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/lgnmodel1.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2567 2022-05-24 19:01:38.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/linearfilter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3995 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/lnunit.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6022 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/make_cell_list.py
--rwxrwxr-x   0 kael      (1000) kael      (1000)    14892 2023-03-15 21:19:10.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/movie.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2528 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/poissongeneration.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      263 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/singleunitcell.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4618 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/spatialfilter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3730 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/temporalfilter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2268 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/transferfunction.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     7390 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/util_fns.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3188 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/utilities.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.457473 bmtk-1.0.8/bmtk/simulator/filternet/modules/
--rw-rw-r--   0 kael      (1000) kael      (1000)       81 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/modules/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      161 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/modules/base.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4678 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/filternet/modules/create_spikes.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6390 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/filternet/modules/record_rates.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4158 2023-02-15 16:42:21.000000 bmtk-1.0.8/bmtk/simulator/filternet/pyfunction_cache.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9152 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/sonata_adaptors.py
--rw-rw-r--   0 kael      (1000) kael      (1000)       64 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/filternet/transfer_functions.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      150 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/filternet/utils.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.457473 bmtk-1.0.8/bmtk/simulator/pointnet/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1733 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/simulator/pointnet/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2208 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/pointnet/config.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.457473 bmtk-1.0.8/bmtk/simulator/pointnet/default_setters/
--rw-rw-r--   0 kael      (1000) kael      (1000)       59 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/pointnet/default_setters/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      471 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/pointnet/default_setters/synapse_models.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      441 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/simulator/pointnet/default_setters/synaptic_weights.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2409 2022-07-14 00:17:59.000000 bmtk-1.0.8/bmtk/simulator/pointnet/gids.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    26368 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/simulator/pointnet/glif_utils.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2820 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/pointnet/io_tools.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.461473 bmtk-1.0.8/bmtk/simulator/pointnet/modules/
--rw-rw-r--   0 kael      (1000) kael      (1000)      165 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/pointnet/modules/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4376 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/pointnet/modules/ecephys_module.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     2210 2023-03-23 01:37:03.000000 bmtk-1.0.8/bmtk/simulator/pointnet/modules/iclamp.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     7014 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/pointnet/modules/multimeter_reporter.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6456 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/pointnet/modules/record_spikes.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1751 2022-05-24 19:01:38.000000 bmtk-1.0.8/bmtk/simulator/pointnet/nest_utils.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    10782 2023-01-04 15:58:48.000000 bmtk-1.0.8/bmtk/simulator/pointnet/pointnetwork.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    11371 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/pointnet/pointsimulator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     7611 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/pointnet/property_map.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1616 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/simulator/pointnet/pyfunction_cache.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    14299 2023-01-04 15:58:48.000000 bmtk-1.0.8/bmtk/simulator/pointnet/sonata_adaptors.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6528 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/pointnet/utils.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.461473 bmtk-1.0.8/bmtk/simulator/popnet/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1622 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/popnet/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1818 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/popnet/config.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3583 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/popnet/popedge.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    17362 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/popnet/popnetwork.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     5797 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/popnet/popnode.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    13400 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/popnet/popsimulator.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      338 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/popnet/sonata_adaptors.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    10509 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/popnet/utils.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.461473 bmtk-1.0.8/bmtk/simulator/utils/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1521 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/simulator/utils/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4728 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/simulator/utils/simulation_inputs.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    11838 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/simulator/utils/simulation_reports.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.461473 bmtk-1.0.8/bmtk/utils/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1576 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/__init__.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.461473 bmtk-1.0.8/bmtk/utils/compile_mechanisms/
--rw-rw-r--   0 kael      (1000) kael      (1000)       66 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/compile_mechanisms/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      884 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/compile_mechanisms/__main__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1030 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/compile_mechanisms/compile_mechanisms.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.461473 bmtk-1.0.8/bmtk/utils/create_environment/
--rw-rw-r--   0 kael      (1000) kael      (1000)       50 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/create_environment/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6984 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/create_environment/__main__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4009 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/create_environment/create_environment.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    33910 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/utils/create_environment/env_builder.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      417 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/hdf5_helper.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/io/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1596 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/io/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    16015 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/io/cell_vars.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      951 2022-07-13 17:53:48.000000 bmtk-1.0.8/bmtk/utils/io/firing_rates.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      917 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/io/ioutils.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    15109 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/io/spike_trains.py
--rw-rw-r--   0 kael      (1000) kael      (1000)      260 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/lazy_property.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/reports/
--rw-rw-r--   0 kael      (1000) kael      (1000)       80 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/reports/__init__.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/reports/compartment/
--rw-rw-r--   0 kael      (1000) kael      (1000)       49 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/reports/compartment/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    10717 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/utils/reports/compartment/compartment_reader.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     1062 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/reports/compartment/compartment_report.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    21509 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/utils/reports/compartment/compartment_writer.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3841 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/reports/compartment/core.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    13144 2022-10-28 02:04:43.000000 bmtk-1.0.8/bmtk/utils/reports/compartment/plotting.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6450 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/reports/current_writer.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/reports/spike_trains/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1735 2022-06-14 03:21:34.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3054 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/core.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    16732 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/plotting.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    35586 2023-07-02 17:43:51.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_train_buffer.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    26892 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_train_readers.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    14343 2023-01-04 16:03:28.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_trains.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    14030 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_trains_api.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     6763 2023-06-21 19:55:18.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/spikes_file_writers.py
--rw-rw-r--   0 kael      (1000) kael      (1000)       46 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/reports/spike_trains/stats.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/scripts/
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/scripts/bionet/
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.465473 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)     5738 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/318331342_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     3563 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/472363762_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     3383 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/472912177_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     3348 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/473862421_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     3566 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863035_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     3558 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863510_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)     2695 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/485184849_fit.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      993 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/default_config.json
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.469473 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      661 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF2.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF2.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      667 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tOFF_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tOFF_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tOFF_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      681 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF8_demo.json
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.433472 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.473473 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/
--rw-rw-r--   0 kael      (1000) kael      (1000)      704 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/CaDynamics.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1211 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_HVA.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1069 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_LVA.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1005 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ih.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)      859 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)      761 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im_v2.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1161 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_P.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1031 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_T.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)      705 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kd.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1394 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv2like.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)      631 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv3_1.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1413 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTa.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1267 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTs.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     4061 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaV.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)     1170 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Nap.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)      942 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/SK.mod
--rw-rw-r--   0 kael      (1000) kael      (1000)      896 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/vecevent.mod
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.473473 bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/
--rw-rw-r--   0 kael      (1000) kael      (1000)    65973 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Nr5a1_471087815_m.swc
--rw-rw-r--   0 kael      (1000) kael      (1000)    53043 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Pvalb_469628681_m.swc
--rw-rw-r--   0 kael      (1000) kael      (1000)    83820 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Pvalb_470522102_m.swc
--rw-rw-r--   0 kael      (1000) kael      (1000)    95135 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Rorb_325404214_m.swc
--rw-rw-r--   0 kael      (1000) kael      (1000)   165301 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Scnn1a_473845048_m.swc
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.473473 bmtk-1.0.8/bmtk/utils/scripts/bionet/point_neuron_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)       68 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/point_neuron_models/IntFire1_exc_1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)       68 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/point_neuron_models/IntFire1_inh_1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      462 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/run_bionet.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.473473 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)       80 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/AMPA_ExcToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)       80 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/AMPA_ExcToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)       84 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/GABA_InhToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)       83 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/GABA_InhToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)       55 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/instantaneousExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)       56 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/synaptic_models/instantaneousInh.json
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.473473 bmtk-1.0.8/bmtk/utils/scripts/bionet/templates/
--rw-rw-r--   0 kael      (1000) kael      (1000)      437 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/templates/BioAllen_old.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)     1035 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/templates/BioAxonStub.hoc
--rw-rw-r--   0 kael      (1000) kael      (1000)      626 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/bionet/templates/Biophys1.hoc
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.473473 bmtk-1.0.8/bmtk/utils/scripts/filternet/
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.477473 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      661 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF2.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF2.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      667 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tOFF_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tOFF_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tOFF_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      681 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF8_demo.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      547 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/filternet/run_filternet.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.477473 bmtk-1.0.8/bmtk/utils/scripts/pointnet/
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.477473 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      661 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF2.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      676 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF1.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      671 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF2.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      667 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      692 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF15.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      675 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF4.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      677 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF8.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      681 2022-10-25 18:55:38.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF8_demo.json
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.481474 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)      119 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/472363762_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      119 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/472912177_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      118 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/473862421_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      119 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/473863035_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      118 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/473863510_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      119 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/IntFire1_exc_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      117 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/IntFire1_inh_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        4 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/point_neuron_models/filter_point.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      332 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/run_pointnet.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.481474 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)        4 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/ExcToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        4 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/ExcToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/InhToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/InhToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/instantaneousExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/pointnet/synaptic_models/instantaneousInh.json
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.481474 bmtk-1.0.8/bmtk/utils/scripts/popnet/
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.481474 bmtk-1.0.8/bmtk/utils/scripts/popnet/population_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)      143 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/population_models/exc_model.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      143 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/population_models/inh_model.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      415 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/run_popnet.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.481474 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/
--rw-rw-r--   0 kael      (1000) kael      (1000)        4 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/ExcToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        4 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/ExcToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/InhToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/InhToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        3 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/input_ExcToExc.json
--rw-rw-r--   0 kael      (1000) kael      (1000)        3 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/popnet/synaptic_models/input_ExcToInh.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      545 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/scripts/sonata.circuit_config.json
--rw-rw-r--   0 kael      (1000) kael      (1000)      450 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/scripts/sonata.simulation_config.json
--rw-rw-r--   0 kael      (1000) kael      (1000)    37691 2022-07-23 20:09:44.000000 bmtk-1.0.8/bmtk/utils/sim_setup.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.485474 bmtk-1.0.8/bmtk/utils/sonata/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1608 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/sonata/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3971 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/sonata/column_property.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.485474 bmtk-1.0.8/bmtk/utils/sonata/config/
--rw-rw-r--   0 kael      (1000) kael      (1000)     1606 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/config/__init__.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4215 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/config/config_schema.json
--rw-rw-r--   0 kael      (1000) kael      (1000)    19237 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/config/sonata_config.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     3453 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/sonata/edge.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     5537 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/sonata/file.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    13856 2019-10-23 23:40:04.000000 bmtk-1.0.8/bmtk/utils/sonata/file_root.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    19742 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/group.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4417 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/node.py
--rw-rw-r--   0 kael      (1000) kael      (1000)    25155 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/population.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     9090 2022-04-28 20:49:20.000000 bmtk-1.0.8/bmtk/utils/sonata/types_table.py
--rw-rw-r--   0 kael      (1000) kael      (1000)     4257 2022-07-18 16:28:21.000000 bmtk-1.0.8/bmtk/utils/sonata/utils.py
-drwxrwxr-x   0 kael      (1000) kael      (1000)        0 2023-07-02 17:52:21.433472 bmtk-1.0.8/bmtk.egg-info/
--rw-rw-r--   0 kael      (1000) kael      (1000)     3215 2023-07-02 17:52:19.000000 bmtk-1.0.8/bmtk.egg-info/PKG-INFO
--rw-rw-r--   0 kael      (1000) kael      (1000)    16761 2023-07-02 17:52:21.000000 bmtk-1.0.8/bmtk.egg-info/SOURCES.txt
--rw-rw-r--   0 kael      (1000) kael      (1000)        1 2023-07-02 17:52:19.000000 bmtk-1.0.8/bmtk.egg-info/dependency_links.txt
--rw-rw-r--   0 kael      (1000) kael      (1000)      181 2023-07-02 17:52:19.000000 bmtk-1.0.8/bmtk.egg-info/requires.txt
--rw-rw-r--   0 kael      (1000) kael      (1000)        5 2023-07-02 17:52:19.000000 bmtk-1.0.8/bmtk.egg-info/top_level.txt
--rw-rw-r--   0 kael      (1000) kael      (1000)      315 2023-07-02 17:52:21.485474 bmtk-1.0.8/setup.cfg
--rw-rw-r--   0 kael      (1000) kael      (1000)     2212 2023-01-04 16:03:28.000000 bmtk-1.0.8/setup.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.059797 bmtk-1.1.0/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1482 2024-04-01 22:41:49.000000 bmtk-1.1.0/LICENSE.txt
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      120 2024-04-01 22:41:49.000000 bmtk-1.1.0/MANIFEST.in
+-rw-r--r--   0 kaeld     (1229) kaeld     (1229)     3635 2024-04-01 22:47:51.059797 bmtk-1.1.0/PKG-INFO
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2223 2024-04-01 22:41:49.000000 bmtk-1.1.0/README.md
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.966797 bmtk-1.1.0/bmtk/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1543 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/__init__.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.971797 bmtk-1.1.0/bmtk/analyzer/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     7931 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/analyzer/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4336 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/analyzer/cell_vars.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     9180 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/analyzer/compartment.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3594 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/analyzer/ecp.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      274 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/analyzer/edges.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3751 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/analyzer/firing_rates.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      391 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/analyzer/io_tools.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    17928 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/analyzer/spike_trains.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4787 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/analyzer/spikes_analyzer.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3890 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/analyzer/spikes_loader.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      211 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/analyzer/utils.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.975797 bmtk-1.1.0/bmtk/builder/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1580 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/__init__.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.976797 bmtk-1.1.0/bmtk/builder/auxi/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1520 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/auxi/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2515 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/auxi/edge_connectors.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    40569 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/auxi/node_params.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.977797 bmtk-1.1.0/bmtk/builder/bionet/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      750 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/bionet/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    19079 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/bionet/swc_reader.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4784 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/builder_utils.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     9773 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/connection_map.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1796 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/connector.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3033 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/edge.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.978797 bmtk-1.1.0/bmtk/builder/edges_sorter/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      962 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/edges_sorter/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4007 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/edges_sorter/memory_sorter.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    27610 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/edges_sorter/merge_sorter.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2504 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/functor_cache.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3089 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/id_generator.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    17456 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/index_builders.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     5336 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/iterator.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.980797 bmtk-1.1.0/bmtk/builder/network_adaptors/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1632 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/network_adaptors/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    19836 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/network_adaptors/dm_network.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    23846 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/network_adaptors/dm_network_orig.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    11489 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/network_adaptors/edge_props_table.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    21380 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/network_adaptors/edges_collator.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    32877 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/network_adaptors/network.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3057 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/network_adaptors/nxnetwork.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    30657 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/network_builder.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      179 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/networks.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3055 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/node.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4202 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/node_pool.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3077 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/builder/node_set.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.980797 bmtk-1.1.0/bmtk/simulator/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1521 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/__init__.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.986797 bmtk-1.1.0/bmtk/simulator/bionet/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      153 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/README.md
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1862 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    20932 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/biocell.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    17281 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/bionetwork.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    17779 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/biosimulator.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3883 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/cell.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2367 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/config.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.987797 bmtk-1.1.0/bmtk/simulator/bionet/default_setters/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1606 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/default_setters/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    17512 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/default_setters/cell_models.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6112 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/default_setters/synapse_models.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2449 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/default_setters/synaptic_weights.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.988797 bmtk-1.1.0/bmtk/simulator/bionet/default_templates/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1036 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/default_templates/BioAxonStub.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      608 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/default_templates/Biophys1.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      239 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/default_templates/advance.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1110 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/gids.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3125 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/iclamp.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.990797 bmtk-1.1.0/bmtk/simulator/bionet/import3d/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    28325 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/import3d/import3d_gui.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    10086 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/import3d/import3d_sec.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2038 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/import3d/read_morphml.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    16444 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/import3d/read_nlcda.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    27594 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/import3d/read_nlcda3.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     7697 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/import3d/read_nts.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    12318 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/import3d/read_swc.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      335 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/import3d.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1905 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/io_tools.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.993797 bmtk-1.1.0/bmtk/simulator/bionet/modules/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1895 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    11526 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/comsol.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1434 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/ecephys_module.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    12928 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/ecp.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     5867 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/iclamp.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    13828 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/record_cellvars.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4732 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/record_clamp.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     9514 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/record_netcons.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4898 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/record_spikes.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    17767 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/save_synapses.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3356 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/sim_module.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6994 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/xstim.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4023 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/modules/xstim_waveforms.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    23657 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/morphology.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     5482 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/nml_reader.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3537 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/nrn.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6924 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/pointprocesscell.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      371 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/pointsomacell.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1679 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/pyfunction_cache.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.995797 bmtk-1.1.0/bmtk/simulator/bionet/schemas/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3335 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/schemas/config_schema.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      536 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/schemas/csv_edge_types.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      170 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/schemas/csv_node_types_external.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      347 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/schemas/csv_node_types_internal.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      162 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/schemas/csv_nodes_external.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      456 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/schemas/csv_nodes_internal.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2257 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/seclamp.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     8019 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/sonata_adaptors.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4278 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/utils.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3596 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/bionet/virtualcell.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.998797 bmtk-1.1.0/bmtk/simulator/core/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      426 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/edge_population.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    15605 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/graph.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4666 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/io_tools.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.000797 bmtk-1.1.0/bmtk/simulator/core/modules/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/modules/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    17106 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/modules/ecephys_module.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6954 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/modules/iclamp.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3186 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/modules/ndx-aibs-ecephys.extension.yaml
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      250 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/modules/ndx-aibs-ecephys.namespace.yaml
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3543 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/modules/simulator_module.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1772 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/network_reader.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      886 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/node_population.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1928 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/node_sets.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    14660 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/pyfunction_cache.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4610 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/simulation_config.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6008 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/simulation_config_validator.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      203 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/simulator.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    10605 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/simulator_network.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.001797 bmtk-1.1.0/bmtk/simulator/core/sonata_reader/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      159 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/sonata_reader/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     7777 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/sonata_reader/edge_adaptor.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    10541 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/sonata_reader/network_reader.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     7783 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/sonata_reader/node_adaptor.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.001797 bmtk-1.1.0/bmtk/simulator/core/sonata_schemas/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4394 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/core/sonata_schemas/config_schema.json
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.004797 bmtk-1.1.0/bmtk/simulator/filternet/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      234 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2920 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/auditory_processing.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1782 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/cell.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       57 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/cell_models.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      691 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/config.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.005797 bmtk-1.1.0/bmtk/simulator/filternet/default_setters/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       28 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/default_setters/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    13798 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/default_setters/cell_loaders.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2046 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/filternetwork.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      307 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/filters.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    11142 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/filtersimulator.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      756 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/io_tools.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.010797 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      195 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/__init__.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.012797 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/
+-rwxrwxr-x   0 kaeld     (1229) kaeld     (1229)    15615 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/sOFF_cell_data.csv
+-rwxrwxr-x   0 kaeld     (1229) kaeld     (1229)    12437 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/sON_cell_data.csv
+-rwxrwxr-x   0 kaeld     (1229) kaeld     (1229)     4186 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/sus_sus_cells_v3.csv
+-rwxrwxr-x   0 kaeld     (1229) kaeld     (1229)     9904 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/tOFF_cell_data.csv
+-rwxrwxr-x   0 kaeld     (1229) kaeld     (1229)     1003 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/tON_cell_data.csv
+-rwxrwxr-x   0 kaeld     (1229) kaeld     (1229)     2783 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/trans_sus_cells_v3.csv
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6361 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cellmetrics.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6596 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cellmodel.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    13122 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cursor.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3567 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/fitfuns.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3611 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/gaborfilter.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    17639 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/kernel.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     9140 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/lattice_unit_constructor.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2111 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/lgnmodel1.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4327 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/linearfilter.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4129 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/lnunit.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6022 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/make_cell_list.py
+-rwxrwxr-x   0 kaeld     (1229) kaeld     (1229)    15153 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/movie.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2528 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/poissongeneration.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      263 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/singleunitcell.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4644 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/spatialfilter.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3730 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/temporalfilter.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2268 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/transferfunction.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     7390 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/util_fns.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3188 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/utilities.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4829 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/waveletfilter.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.013797 bmtk-1.1.0/bmtk/simulator/filternet/modules/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       81 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/modules/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      161 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/modules/base.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4678 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/modules/create_spikes.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6390 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/modules/record_rates.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4158 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/pyfunction_cache.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    12319 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/sonata_adaptors.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       64 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/transfer_functions.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      150 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/filternet/utils.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.016797 bmtk-1.1.0/bmtk/simulator/pointnet/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1733 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2208 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/config.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.016797 bmtk-1.1.0/bmtk/simulator/pointnet/default_setters/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       59 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/default_setters/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      471 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/default_setters/synapse_models.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      441 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/default_setters/synaptic_weights.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3373 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/gids.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    26368 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/glif_utils.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2820 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/io_tools.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.018797 bmtk-1.1.0/bmtk/simulator/pointnet/modules/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      253 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/modules/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4376 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/modules/ecephys_module.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2210 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/modules/iclamp.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     7088 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/modules/multimeter_reporter.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6530 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/modules/record_spikes.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3544 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/modules/sim_module.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2412 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/modules/spikes_inputs.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2825 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/modules/weight_recorder.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1751 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/nest_utils.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    10782 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/pointnetwork.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    11258 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/pointsimulator.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     7611 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/property_map.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1616 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/pyfunction_cache.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    14299 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/sonata_adaptors.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6528 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/pointnet/utils.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.020797 bmtk-1.1.0/bmtk/simulator/popnet/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1622 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/popnet/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1818 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/popnet/config.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3583 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/popnet/popedge.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    17362 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/popnet/popnetwork.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     5797 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/popnet/popnode.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    13400 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/popnet/popsimulator.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      338 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/popnet/sonata_adaptors.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    10509 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/popnet/utils.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.021797 bmtk-1.1.0/bmtk/simulator/utils/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1521 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/utils/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4728 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/utils/simulation_inputs.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    12503 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/simulator/utils/simulation_reports.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.022797 bmtk-1.1.0/bmtk/utils/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1576 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/__init__.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.022797 bmtk-1.1.0/bmtk/utils/compile_mechanisms/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       66 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/compile_mechanisms/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      884 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/compile_mechanisms/__main__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1030 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/compile_mechanisms/compile_mechanisms.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.023797 bmtk-1.1.0/bmtk/utils/create_environment/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       50 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/create_environment/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6984 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/create_environment/__main__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4009 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/create_environment/create_environment.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    33910 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/create_environment/env_builder.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      417 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/hdf5_helper.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.025797 bmtk-1.1.0/bmtk/utils/io/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1596 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/io/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    16015 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/io/cell_vars.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      951 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/io/firing_rates.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      917 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/io/ioutils.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    15109 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/io/spike_trains.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      260 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/lazy_property.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.025797 bmtk-1.1.0/bmtk/utils/reports/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       80 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/__init__.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.026797 bmtk-1.1.0/bmtk/utils/reports/compartment/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       49 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/compartment/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    10717 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/compartment/compartment_reader.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1062 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/compartment/compartment_report.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    21509 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/compartment/compartment_writer.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3841 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/compartment/core.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    13144 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/compartment/plotting.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     6450 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/current_writer.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.029797 bmtk-1.1.0/bmtk/utils/reports/spike_trains/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1735 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/spike_trains/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3054 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/spike_trains/core.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    16732 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/spike_trains/plotting.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    35586 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/spike_trains/spike_train_buffer.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    26892 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/spike_trains/spike_train_readers.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    14343 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/spike_trains/spike_trains.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    14084 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/spike_trains/spike_trains_api.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     8916 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/spike_trains/spikes_file_writers.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       46 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/reports/spike_trains/stats.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.029797 bmtk-1.1.0/bmtk/utils/scripts/
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.030797 bmtk-1.1.0/bmtk/utils/scripts/bionet/
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.031797 bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     5738 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/318331342_fit.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3563 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/472363762_fit.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3383 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/472912177_fit.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3348 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/473862421_fit.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3566 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863035_fit.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3558 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863510_fit.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2695 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/485184849_fit.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      993 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/default_config.json
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.035797 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      675 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sOFF_TF1.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      661 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sOFF_TF15.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      676 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sOFF_TF2.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      675 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sOFF_TF4.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      671 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sOFF_TF8.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      676 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sON_TF1.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      671 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sON_TF2.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      667 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sON_TF4.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      677 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sON_TF8.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      692 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tOFF_TF15.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      675 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tOFF_TF4.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      677 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tOFF_TF8.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      692 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tON_TF15.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      675 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tON_TF4.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      677 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tON_TF8.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      681 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tON_TF8_demo.json
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.957797 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.039797 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      704 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/CaDynamics.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1211 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_HVA.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1069 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_LVA.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1005 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ih.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      859 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      761 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im_v2.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1161 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_P.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1031 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_T.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      705 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kd.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1394 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv2like.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      631 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv3_1.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1413 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTa.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1267 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTs.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4061 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaV.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1170 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Nap.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      942 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/SK.mod
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      896 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/vecevent.mod
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.040797 bmtk-1.1.0/bmtk/utils/scripts/bionet/morphologies/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    65973 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/morphologies/Nr5a1_471087815_m.swc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    53043 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/morphologies/Pvalb_469628681_m.swc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    83820 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/morphologies/Pvalb_470522102_m.swc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    95135 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/morphologies/Rorb_325404214_m.swc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)   165301 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/morphologies/Scnn1a_473845048_m.swc
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.041797 bmtk-1.1.0/bmtk/utils/scripts/bionet/point_neuron_models/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       68 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/point_neuron_models/IntFire1_exc_1.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       68 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/point_neuron_models/IntFire1_inh_1.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      462 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/run_bionet.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.042797 bmtk-1.1.0/bmtk/utils/scripts/bionet/synaptic_models/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       80 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/synaptic_models/AMPA_ExcToExc.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       80 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/synaptic_models/AMPA_ExcToInh.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       84 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/synaptic_models/GABA_InhToExc.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       83 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/synaptic_models/GABA_InhToInh.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       55 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/synaptic_models/instantaneousExc.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)       56 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/synaptic_models/instantaneousInh.json
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.043797 bmtk-1.1.0/bmtk/utils/scripts/bionet/templates/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      437 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/templates/BioAllen_old.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1035 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/templates/BioAxonStub.hoc
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      626 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/bionet/templates/Biophys1.hoc
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.043797 bmtk-1.1.0/bmtk/utils/scripts/filternet/
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.046797 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      675 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sOFF_TF1.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      661 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sOFF_TF15.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      676 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sOFF_TF2.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      675 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sOFF_TF4.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      671 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sOFF_TF8.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      676 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sON_TF1.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      671 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sON_TF2.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      667 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sON_TF4.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      677 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sON_TF8.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      692 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tOFF_TF15.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      675 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tOFF_TF4.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      677 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tOFF_TF8.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      692 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tON_TF15.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      675 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tON_TF4.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      677 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tON_TF8.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      681 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tON_TF8_demo.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      547 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/filternet/run_filternet.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.047797 bmtk-1.1.0/bmtk/utils/scripts/pointnet/
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.050797 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      675 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF1.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      661 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF15.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      676 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF2.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      675 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF4.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      671 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF8.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      676 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sON_TF1.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      671 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sON_TF2.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      667 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sON_TF4.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      677 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sON_TF8.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      692 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF15.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      675 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF4.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      677 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF8.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      692 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tON_TF15.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      675 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tON_TF4.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      677 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tON_TF8.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      681 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tON_TF8_demo.json
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.052797 bmtk-1.1.0/bmtk/utils/scripts/pointnet/point_neuron_models/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      119 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/point_neuron_models/472363762_point.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      119 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/point_neuron_models/472912177_point.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      118 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/point_neuron_models/473862421_point.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      119 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/point_neuron_models/473863035_point.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      118 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/point_neuron_models/473863510_point.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      119 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/point_neuron_models/IntFire1_exc_point.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      117 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/point_neuron_models/IntFire1_inh_point.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        4 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/point_neuron_models/filter_point.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      332 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/run_pointnet.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.053797 bmtk-1.1.0/bmtk/utils/scripts/pointnet/synaptic_models/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        4 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/synaptic_models/ExcToExc.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        4 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/synaptic_models/ExcToInh.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        5 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/synaptic_models/InhToExc.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        5 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/synaptic_models/InhToInh.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        5 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/synaptic_models/instantaneousExc.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        5 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/pointnet/synaptic_models/instantaneousInh.json
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.053797 bmtk-1.1.0/bmtk/utils/scripts/popnet/
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.054797 bmtk-1.1.0/bmtk/utils/scripts/popnet/population_models/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      143 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/popnet/population_models/exc_model.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      143 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/popnet/population_models/inh_model.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      415 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/popnet/run_popnet.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.055797 bmtk-1.1.0/bmtk/utils/scripts/popnet/synaptic_models/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        4 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/popnet/synaptic_models/ExcToExc.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        4 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/popnet/synaptic_models/ExcToInh.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        5 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/popnet/synaptic_models/InhToExc.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        5 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/popnet/synaptic_models/InhToInh.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        3 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/popnet/synaptic_models/input_ExcToExc.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        3 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/popnet/synaptic_models/input_ExcToInh.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      545 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/sonata.circuit_config.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      450 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/scripts/sonata.simulation_config.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    37691 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sim_setup.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.057797 bmtk-1.1.0/bmtk/utils/sonata/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1608 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3971 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/column_property.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:51.058797 bmtk-1.1.0/bmtk/utils/sonata/config/
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     1606 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/config/__init__.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4215 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/config/config_schema.json
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    19237 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/config/sonata_config.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     3453 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/edge.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    25123 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/edge_stats.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     5537 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/file.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    13856 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/file_root.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    19742 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/group.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4417 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/node.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    25155 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/population.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     9090 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/types_table.py
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     4257 2024-04-01 22:41:49.000000 bmtk-1.1.0/bmtk/utils/sonata/utils.py
+drwxrwxr-x   0 kaeld     (1229) kaeld     (1229)        0 2024-04-01 22:47:50.968797 bmtk-1.1.0/bmtk.egg-info/
+-rw-r--r--   0 kaeld     (1229) kaeld     (1229)     3635 2024-04-01 22:47:49.000000 bmtk-1.1.0/bmtk.egg-info/PKG-INFO
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)    17061 2024-04-01 22:47:49.000000 bmtk-1.1.0/bmtk.egg-info/SOURCES.txt
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        1 2024-04-01 22:47:49.000000 bmtk-1.1.0/bmtk.egg-info/dependency_links.txt
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      181 2024-04-01 22:47:49.000000 bmtk-1.1.0/bmtk.egg-info/requires.txt
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)        5 2024-04-01 22:47:49.000000 bmtk-1.1.0/bmtk.egg-info/top_level.txt
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)      315 2024-04-01 22:47:51.060797 bmtk-1.1.0/setup.cfg
+-rw-rw-r--   0 kaeld     (1229) kaeld     (1229)     2248 2024-04-01 22:41:50.000000 bmtk-1.1.0/setup.py
```

### Comparing `bmtk-1.0.8/LICENSE.txt` & `bmtk-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/README.md` & `bmtk-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/__init__.py` & `bmtk-1.1.0/bmtk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
-__version__ = '1.0.8'
+__version__ = '1.1.0'
```

### Comparing `bmtk-1.0.8/bmtk/analyzer/__init__.py` & `bmtk-1.1.0/bmtk/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/analyzer/cell_vars.py` & `bmtk-1.1.0/bmtk/analyzer/cell_vars.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/analyzer/compartment.py` & `bmtk-1.1.0/bmtk/analyzer/compartment.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/analyzer/ecp.py` & `bmtk-1.1.0/bmtk/analyzer/ecp.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/analyzer/firing_rates.py` & `bmtk-1.1.0/bmtk/analyzer/firing_rates.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/analyzer/spike_trains.py` & `bmtk-1.1.0/bmtk/analyzer/spike_trains.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/analyzer/spikes_analyzer.py` & `bmtk-1.1.0/bmtk/analyzer/spikes_analyzer.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/analyzer/spikes_loader.py` & `bmtk-1.1.0/bmtk/analyzer/spikes_loader.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/__init__.py` & `bmtk-1.1.0/bmtk/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/auxi/__init__.py` & `bmtk-1.1.0/bmtk/builder/auxi/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/auxi/edge_connectors.py` & `bmtk-1.1.0/bmtk/builder/auxi/edge_connectors.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/auxi/node_params.py` & `bmtk-1.1.0/bmtk/builder/auxi/node_params.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/bionet/__init__.py` & `bmtk-1.1.0/bmtk/builder/bionet/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/bionet/swc_reader.py` & `bmtk-1.1.0/bmtk/builder/bionet/swc_reader.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/builder_utils.py` & `bmtk-1.1.0/bmtk/builder/builder_utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/connection_map.py` & `bmtk-1.1.0/bmtk/builder/connection_map.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/connector.py` & `bmtk-1.1.0/bmtk/builder/connector.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/edge.py` & `bmtk-1.1.0/bmtk/builder/edge.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/edges_sorter/__init__.py` & `bmtk-1.1.0/bmtk/builder/edges_sorter/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/edges_sorter/memory_sorter.py` & `bmtk-1.1.0/bmtk/builder/edges_sorter/memory_sorter.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/edges_sorter/merge_sorter.py` & `bmtk-1.1.0/bmtk/builder/edges_sorter/merge_sorter.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/functor_cache.py` & `bmtk-1.1.0/bmtk/builder/functor_cache.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/id_generator.py` & `bmtk-1.1.0/bmtk/builder/id_generator.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/index_builders.py` & `bmtk-1.1.0/bmtk/builder/index_builders.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/iterator.py` & `bmtk-1.1.0/bmtk/builder/iterator.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/network_adaptors/__init__.py` & `bmtk-1.1.0/bmtk/builder/network_adaptors/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/network_adaptors/dm_network.py` & `bmtk-1.1.0/bmtk/builder/network_adaptors/dm_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,29 +226,27 @@
         trg_gap_ids = []
 
         if compression == 'none':
             compression = None  # legit option for h5py for no compression
 
         for et in self.__edges_tables:
             try:
-                is_gap = et['edge_types']['is_gap_junction']
+                is_gap = et.edge_type_properties['is_gap_junction']
             except:
                 continue
             if is_gap:
-                if et['source_network'] != et['target_network']:
+                if et.source_network != et.target_network:
                     raise Exception("All gap junctions must be two cells in the same network builder.")
-
-                table = et['syn_table']
-                junc_table = table.nsyn_table
-                locs = np.where(junc_table > 0)
-                for i in range(len(locs[0])):
-                    source_ids.append(table.source_ids[locs[0][i]])
-                    target_ids.append(table.target_ids[locs[1][i]])
-                    src_gap_ids.append(self._gj_id_gen.next())
-                    trg_gap_ids.append(self._gj_id_gen.next())
+                table = et.to_dataframe()
+                for index, row in table.iterrows():
+                    for _ in range(row["nsyns"]):
+                        source_ids.append(row["source_node_id"])
+                        target_ids.append(row["target_node_id"])
+                        src_gap_ids.append(self._gj_id_gen.next())
+                        trg_gap_ids.append(self._gj_id_gen.next())
             else:
                 continue
 
         if len(source_ids) > 0:
             with h5py.File(gj_file_name, 'w') as f:
                 add_hdf5_attrs(f)
                 f.create_dataset('source_ids', data=np.array(source_ids), compression=compression)
```

### Comparing `bmtk-1.0.8/bmtk/builder/network_adaptors/dm_network_orig.py` & `bmtk-1.1.0/bmtk/builder/network_adaptors/dm_network_orig.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/network_adaptors/edge_props_table.py` & `bmtk-1.1.0/bmtk/builder/network_adaptors/edge_props_table.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/network_adaptors/edges_collator.py` & `bmtk-1.1.0/bmtk/builder/network_adaptors/edges_collator.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/network_adaptors/network.py` & `bmtk-1.1.0/bmtk/builder/network_adaptors/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,26 +353,32 @@
             connection_rule = edge_type_properties['nsyns']
             del edge_type_properties['nsyns']
 
         connection = ConnectionMap(source, target, connection_rule, connection_params, iterator, edge_type_properties)
         self._connection_maps.append(connection)
         return connection
 
-    def add_gap_junctions(self, source=None, target=None, iterator='one_to_one', resistance=1,
-                          target_sections=['somatic'], connection_rule=1, connection_params=None):
-        """A special function for marking a edge group as gap junctions. Just a wrapper for add_edges"""
+    def add_gap_junctions(self, source=None, target=None, resistance=1., conductance=None,
+                          distance_range=[0.0, 300.0], target_sections=['somatic'],
+                          connection_rule=1, iterator='one_to_one', **edge_type_properties):
+        """A special function for marking a edge group as gap junctions. Just a wrapper for add_edges.
+
+        :param resistance: gap junction resistance (megaohm)
+        :param conductance: gap junction conductance (microsiemens). If specified, resistance is ignored.
+        """
         if target_sections is not None:
             logger.warning(
                 'For gap junctions, the target sections variable is used for both the source and target sections.'
             )
 
+        syn_weight = 1 / resistance if conductance is None else conductance
         return self.add_edges(
-            source=source, target=target, iterator=iterator, distance_range=[0.0, 300.0], syn_weight=resistance,
-            is_gap_junction=True, target_sections=target_sections, connection_rule=connection_rule,
-            connection_params=connection_params
+            source=source, target=target, syn_weight=syn_weight, is_gap_junction=True,
+            distance_range=distance_range, target_sections=target_sections,
+            connection_rule=connection_rule, iterator=iterator, **edge_type_properties
         )
 
     def nodes(self, **properties):
         """Returns an iterator of Node (glorified dictionary) objects, filtered by parameters.
 
         To get all nodes on a network::
```

### Comparing `bmtk-1.0.8/bmtk/builder/network_adaptors/nxnetwork.py` & `bmtk-1.1.0/bmtk/builder/network_adaptors/nxnetwork.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/network_builder.py` & `bmtk-1.1.0/bmtk/builder/network_builder.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/node.py` & `bmtk-1.1.0/bmtk/builder/node.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/node_pool.py` & `bmtk-1.1.0/bmtk/builder/node_pool.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/builder/node_set.py` & `bmtk-1.1.0/bmtk/builder/node_set.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/__init__.py` & `bmtk-1.1.0/bmtk/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/__init__.py` & `bmtk-1.1.0/bmtk/simulator/bionet/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,12 +16,12 @@
 # INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
 # DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
 # SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
-from bmtk.simulator.bionet.pyfunction_cache import synapse_model, synaptic_weight, cell_model, add_weight_function
+from bmtk.simulator.bionet.pyfunction_cache import synapse_model, synaptic_weight, cell_model, add_weight_function, model_processing
 from bmtk.simulator.bionet.config import Config
 from bmtk.simulator.bionet.bionetwork import BioNetwork
 from bmtk.simulator.bionet.biosimulator import BioSimulator
 from bmtk.simulator.bionet.nrn import reset
```

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/biocell.py` & `bmtk-1.1.0/bmtk/simulator/bionet/biocell.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/bionetwork.py` & `bmtk-1.1.0/bmtk/simulator/bionet/bionetwork.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/biosimulator.py` & `bmtk-1.1.0/bmtk/simulator/bionet/biosimulator.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/cell.py` & `bmtk-1.1.0/bmtk/simulator/bionet/cell.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/config.py` & `bmtk-1.1.0/bmtk/simulator/bionet/config.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/default_setters/__init__.py` & `bmtk-1.1.0/bmtk/simulator/bionet/default_setters/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/default_setters/cell_models.py` & `bmtk-1.1.0/bmtk/simulator/bionet/default_setters/cell_models.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/default_setters/synapse_models.py` & `bmtk-1.1.0/bmtk/simulator/bionet/default_setters/synapse_models.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/default_setters/synaptic_weights.py` & `bmtk-1.1.0/bmtk/simulator/bionet/default_setters/synaptic_weights.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/default_templates/BioAxonStub.hoc` & `bmtk-1.1.0/bmtk/simulator/bionet/default_templates/BioAxonStub.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/default_templates/Biophys1.hoc` & `bmtk-1.1.0/bmtk/simulator/bionet/default_templates/Biophys1.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/gids.py` & `bmtk-1.1.0/bmtk/simulator/bionet/gids.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/iclamp.py` & `bmtk-1.1.0/bmtk/simulator/bionet/iclamp.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/import3d/import3d_gui.hoc` & `bmtk-1.1.0/bmtk/simulator/bionet/import3d/import3d_gui.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/import3d/import3d_sec.hoc` & `bmtk-1.1.0/bmtk/simulator/bionet/import3d/import3d_sec.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_morphml.hoc` & `bmtk-1.1.0/bmtk/simulator/bionet/import3d/read_morphml.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_nlcda.hoc` & `bmtk-1.1.0/bmtk/simulator/bionet/import3d/read_nlcda.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_nlcda3.hoc` & `bmtk-1.1.0/bmtk/simulator/bionet/import3d/read_nlcda3.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_nts.hoc` & `bmtk-1.1.0/bmtk/simulator/bionet/import3d/read_nts.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/import3d/read_swc.hoc` & `bmtk-1.1.0/bmtk/simulator/bionet/import3d/read_swc.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/io_tools.py` & `bmtk-1.1.0/bmtk/simulator/bionet/io_tools.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/modules/__init__.py` & `bmtk-1.1.0/bmtk/simulator/bionet/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/modules/ecephys_module.py` & `bmtk-1.1.0/bmtk/simulator/bionet/modules/ecephys_module.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/modules/ecp.py` & `bmtk-1.1.0/bmtk/simulator/bionet/modules/ecp.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/modules/iclamp.py` & `bmtk-1.1.0/bmtk/simulator/bionet/modules/iclamp.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/modules/record_cellvars.py` & `bmtk-1.1.0/bmtk/simulator/bionet/modules/record_cellvars.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/modules/record_clamp.py` & `bmtk-1.1.0/bmtk/simulator/bionet/modules/record_clamp.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/modules/record_netcons.py` & `bmtk-1.1.0/bmtk/simulator/bionet/modules/record_netcons.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/modules/record_spikes.py` & `bmtk-1.1.0/bmtk/simulator/bionet/modules/record_spikes.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/modules/save_synapses.py` & `bmtk-1.1.0/bmtk/simulator/bionet/modules/save_synapses.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/modules/sim_module.py` & `bmtk-1.1.0/bmtk/simulator/bionet/modules/sim_module.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/modules/xstim.py` & `bmtk-1.1.0/bmtk/simulator/bionet/modules/xstim.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/modules/xstim_waveforms.py` & `bmtk-1.1.0/bmtk/simulator/bionet/modules/xstim_waveforms.py`

 * *Files 7% similar despite different names*

```diff
@@ -88,18 +88,18 @@
     Supports json config in conf as well as string pointer to a file.
     :rtype: BaseWaveformType
     """
     if isinstance(waveform, string_types):
         # if waveform_conf is str or unicode assume to be name of file in stim_dir
         # waveform_conf = str(waveform_conf)   # make consistent
         file_ext = os.path.splitext(waveform)
-        if file_ext == 'csv':
+        if file_ext[-1] == '.csv':
             return WaveformCustom(waveform)
 
-        elif file_ext == 'json':
+        elif file_ext[-1] == '.json':
             with open(waveform, 'r') as f:
                 waveform = json.load(f)
         else:
             io.log_warning('Unknown filetype for waveform')
 
     shape_key = waveform["shape"].lower()
 
@@ -120,8 +120,8 @@
 
     shape_key = iclamp_waveform_conf["shape"].lower()
 
     if shape_key not in shape_classes:
         io.log_warning('iclamp waveform shape not known')  # throw error?
 
     Constructor = shape_classes[shape_key]
-    return Constructor(iclamp_waveform_conf)
+    return Constructor(iclamp_waveform_conf)
```

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/morphology.py` & `bmtk-1.1.0/bmtk/simulator/bionet/morphology.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/nml_reader.py` & `bmtk-1.1.0/bmtk/simulator/bionet/nml_reader.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/nrn.py` & `bmtk-1.1.0/bmtk/simulator/bionet/nrn.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/pointprocesscell.py` & `bmtk-1.1.0/bmtk/simulator/bionet/pointprocesscell.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/pyfunction_cache.py` & `bmtk-1.1.0/bmtk/simulator/bionet/pyfunction_cache.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/schemas/config_schema.json` & `bmtk-1.1.0/bmtk/simulator/bionet/schemas/config_schema.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/schemas/csv_edge_types.json` & `bmtk-1.1.0/bmtk/simulator/bionet/schemas/csv_edge_types.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/seclamp.py` & `bmtk-1.1.0/bmtk/simulator/bionet/seclamp.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/sonata_adaptors.py` & `bmtk-1.1.0/bmtk/simulator/bionet/sonata_adaptors.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/utils.py` & `bmtk-1.1.0/bmtk/simulator/bionet/utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/bionet/virtualcell.py` & `bmtk-1.1.0/bmtk/simulator/bionet/virtualcell.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/graph.py` & `bmtk-1.1.0/bmtk/simulator/core/graph.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/io_tools.py` & `bmtk-1.1.0/bmtk/simulator/core/io_tools.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/modules/ecephys_module.py` & `bmtk-1.1.0/bmtk/simulator/core/modules/ecephys_module.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/modules/iclamp.py` & `bmtk-1.1.0/bmtk/simulator/core/modules/iclamp.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/modules/ndx-aibs-ecephys.extension.yaml` & `bmtk-1.1.0/bmtk/simulator/core/modules/ndx-aibs-ecephys.extension.yaml`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/modules/simulator_module.py` & `bmtk-1.1.0/bmtk/simulator/core/modules/simulator_module.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,21 @@
       sim = Simulation(...)
       mymod = MyModule(...)
       sim.add_mod(mymod)
       sim.run()
 
     """
 
+    def preload(self, sim):
+        """Will be called once at the beginning of the simulation run before network is loaded
+
+        :param sim: Simulation object
+        """
+        pass
+
     def initialize(self, sim):
         """Will be called once at the beginning of the simulation run, after the network and simulation parameters have
         all been finalized.
 
         :param sim: Simulation object
         """
         pass
```

### Comparing `bmtk-1.0.8/bmtk/simulator/core/network_reader.py` & `bmtk-1.1.0/bmtk/simulator/core/network_reader.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/node_population.py` & `bmtk-1.1.0/bmtk/simulator/core/node_population.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/node_sets.py` & `bmtk-1.1.0/bmtk/simulator/core/node_sets.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/pyfunction_cache.py` & `bmtk-1.1.0/bmtk/simulator/core/pyfunction_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -270,14 +270,39 @@
             py_modules.add_synapse_model(wkwargs['name'], func)
 
             @wraps(func)
             def func_wrapper(*args, **kwargs):
                 return func(*args, **kwargs)
             return func_wrapper
         return decorator
+    
+
+def model_processing(*wargs, **wkwargs):
+    if len(wargs) == 1 and callable(wargs[0]):
+        # for the case without decorator arguments, grab the function object in wargs and create a decorator
+        func = wargs[0]
+        py_modules.add_cell_processor(func.__name__, func)  # add function assigned to its original name
+
+        @wraps(func)
+        def func_wrapper(*args, **kwargs):
+            return func(*args, **kwargs)
+        return func_wrapper
+    else:
+        # for the case with decorator arguments
+        assert(all(k in ['name'] for k in wkwargs.keys()))
+
+        def decorator(func):
+            # store the function in py_modules but under the name given in the decorator arguments
+            py_modules.add_cell_processor(wkwargs['name'], func)
+
+            @wraps(func)
+            def func_wrapper(*args, **kwargs):
+                return func(*args, **kwargs)
+            return func_wrapper
+        return decorator
 
 
 def add_weight_function(func, name=None, overwrite=True):
     assert(callable(func))
     func_name = name if name is not None else func.__name__
     py_modules.add_synaptic_weight(func_name, func, overwrite)
```

### Comparing `bmtk-1.0.8/bmtk/simulator/core/simulation_config.py` & `bmtk-1.1.0/bmtk/simulator/core/simulation_config.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/simulation_config_validator.py` & `bmtk-1.1.0/bmtk/simulator/core/simulation_config_validator.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/simulator_network.py` & `bmtk-1.1.0/bmtk/simulator/core/simulator_network.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/sonata_reader/edge_adaptor.py` & `bmtk-1.1.0/bmtk/simulator/core/sonata_reader/edge_adaptor.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/sonata_reader/network_reader.py` & `bmtk-1.1.0/bmtk/simulator/core/sonata_reader/network_reader.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/sonata_reader/node_adaptor.py` & `bmtk-1.1.0/bmtk/simulator/core/sonata_reader/node_adaptor.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/core/sonata_schemas/config_schema.json` & `bmtk-1.1.0/bmtk/simulator/core/sonata_schemas/config_schema.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/cell.py` & `bmtk-1.1.0/bmtk/simulator/filternet/cell.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/config.py` & `bmtk-1.1.0/bmtk/simulator/filternet/config.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/filternetwork.py` & `bmtk-1.1.0/bmtk/simulator/filternet/filternetwork.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/io_tools.py` & `bmtk-1.1.0/bmtk/simulator/filternet/io_tools.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/sOFF_cell_data.csv` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/sOFF_cell_data.csv`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/sON_cell_data.csv` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/sON_cell_data.csv`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/sus_sus_cells_v3.csv` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/sus_sus_cells_v3.csv`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/tOFF_cell_data.csv` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/tOFF_cell_data.csv`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/tON_cell_data.csv` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/tON_cell_data.csv`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cell_metrics/trans_sus_cells_v3.csv` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cell_metrics/trans_sus_cells_v3.csv`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cellmetrics.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cellmetrics.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cellmodel.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cellmodel.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/cursor.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/cursor.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,48 @@
 import numpy as np
 import scipy.signal as spsig
 
-from .utilities import convert_tmin_tmax_framerate_to_trange
+try:
+    from mpi4py import MPI
+    mpi_size = MPI.COMM_WORLD.Get_size()
+    numba_parallel = mpi_size == 1  # if there is only 1 thread, turn on numba parallel
+except ImportError:
+    numba_parallel = True  # If there is no MPI, turn on numba parallel
+
+
+try:
+    from numba import njit, prange
+
+    # a faster version of the commented out part of the above class method. Results agree up to a round off error.
+    @njit(parallel=numba_parallel)
+    def kernel_dot_product(movie_data, ti_offset, kernel_t_inds, kernel_row_inds, kernel_col_inds, kernel_kernel):
+        t_inds = kernel_t_inds + ti_offset + 1
+        result = 0.0
+        for i in prange(len(t_inds)):
+            if t_inds[i] >= 0 and t_inds[i] < movie_data.shape[0]:
+                result = result + movie_data[t_inds[i], kernel_row_inds[i], kernel_col_inds[i]] * kernel_kernel[i]
+        return result
+except ImportError as ie:
+    
+    # Normal way to calculate dot-product not using numba library. Also had to create because for some reason numba
+    # is interfering with NEST (at-least ver 3.3) binary causing a segmentation fault.
+    def kernel_dot_product(movie_data, ti_offset, kernel_t_inds, kernel_row_inds, kernel_col_inds, kernel_kernel):
+        t_inds = kernel_t_inds + ti_offset + 1  # Offset by one nhc 14 Apr '17
+        min_ind, max_ind = 0, movie_data.shape[0]
+        allowed_inds = np.where(np.logical_and(min_ind <= t_inds, t_inds < max_ind))
+        t_inds = t_inds[allowed_inds]
+        row_inds = kernel_row_inds[allowed_inds]
+        col_inds = kernel_col_inds[allowed_inds]
+        kernel_vector = kernel_kernel[allowed_inds] 
+        return np.dot(movie_data[t_inds, row_inds, col_inds], kernel_vector)
 
 
+from .utilities import convert_tmin_tmax_framerate_to_trange
+from .linearfilter import SpatioTemporalFilter, SpectroTemporalFilter
+
 class KernelCursor(object):
     """A class that takes care of the convolution of the (non-separable) spatial-temporal linear filter with the move.
     """
     def __init__(self, kernel, movie):
         self.movie = movie
         self.kernel = kernel
         self.cache = {}
@@ -67,29 +102,28 @@
 
         if np.isnan(curr_rate):
             assert RuntimeError
         
         return curr_rate
 
     def apply_dot_product(self, ti_offset):
-        try:
-            # TODO: This needs to be altered asap
-            return self.cache[ti_offset]
-        
-        except KeyError:
-            t_inds = self.kernel.t_inds + ti_offset + 1  # Offset by one nhc 14 Apr '17
-            min_ind, max_ind = 0, self.movie.data.shape[0]
-            allowed_inds = np.where(np.logical_and(min_ind <= t_inds, t_inds < max_ind))
-            t_inds = t_inds[allowed_inds]
-            row_inds = self.kernel.row_inds[allowed_inds]
-            col_inds = self.kernel.col_inds[allowed_inds]
-            kernel_vector = self.kernel.kernel[allowed_inds] 
-            result = np.dot(self.movie[t_inds, row_inds, col_inds], kernel_vector)
+        if ti_offset in self.cache:
+            result = self.cache[ti_offset]
+        else:
+            result = kernel_dot_product(
+                movie_data=self.movie.data,
+                ti_offset=ti_offset,
+                kernel_t_inds=self.kernel.t_inds,
+                kernel_row_inds=self.kernel.row_inds,
+                kernel_col_inds=self.kernel.col_inds,
+                kernel_kernel=self.kernel.kernel,
+            )
             self.cache[ti_offset] = result
-            return result
+
+        return result
 
 
 class FilterCursor(KernelCursor):
     def __init__(self, spatiotemporal_filter, movie, threshold=0):
         # TODO: not sure why this needs to have it's own class and shouldn't be merged into parent?
         self.spatiotemporal_filter = spatiotemporal_filter
         kernel = self.spatiotemporal_filter.get_spatiotemporal_kernel(movie.row_range, movie.col_range,
@@ -102,16 +136,50 @@
 class LNUnitCursor(KernelCursor):
     """A class that takes care of applying a linear-nonlinear filter to a movie. Parent class is used to apply the
     spatial-termporal filter convolution to the movie, when then the lnunit non-linear transfer function is applied.
 
     """
     def __init__(self, lnunit, movie, threshold=0):
         self.lnunit = lnunit
-        kernel = lnunit.get_spatiotemporal_kernel(movie.row_range, movie.col_range, movie.t_range, reverse=True,
+        if hasattr(movie, "t_range_orig"):    # Reset padded to original
+            movie.t_range = movie.t_range_orig
+            movie.data = movie.data_orig
+            movie.row_range = movie.row_range_orig
+        if isinstance(self.lnunit.linear_filter, SpatioTemporalFilter):
+            kernel = lnunit.get_spatiotemporal_kernel(movie.row_range, movie.col_range, movie.t_range, reverse=True,
                                                   threshold=threshold)
+        elif isinstance(self.lnunit.linear_filter, SpectroTemporalFilter):
+            kernel = lnunit.get_spectrotemporal_kernel(movie.row_range, movie.t_range, reverse=True, threshold=0.05)
+            if movie.padding:
+                if movie.padding == 'edge':
+                    pre_pad = np.full((len(np.unique(kernel.t_inds))-1, movie.data.shape[1]),
+                                  movie.data[0, :, 0])
+                    pre_pad = pre_pad[:, :, np.newaxis]
+                    movie.data_orig = movie.data
+                    movie.data = np.concatenate((pre_pad, movie.data))
+                    lower_pad = np.full((movie.data.shape[0], len(np.unique(kernel.row_inds)) - 1, 1),
+                                        np.reshape(movie.data[:, 0, 0], (-1, 1, 1)))
+                    upper_pad = np.full((movie.data.shape[0], len(np.unique(kernel.row_inds)) - 1, 1),
+                                        np.reshape(movie.data[:, -1, 0], (-1, 1, 1)))
+                    movie.data = np.hstack((lower_pad, movie.data, upper_pad))
+                    kernel.t_range = np.linspace(kernel.t_range[0] - pre_pad.shape[0] * 1/movie.frame_rate,
+                                                 0, movie.data.shape[0])
+                    movie.t_range_orig = movie.t_range
+                    movie.t_range = kernel.t_range - kernel.t_range[0]
+                    # Treating it like an image, although technically strange to pad to negative frequencies
+                    kernel.row_range = np.linspace(kernel.row_range[0] -
+                                                   lower_pad.shape[1] * (kernel.row_range[1]-kernel.row_range[0]),
+                                                   kernel.row_range[-1] +
+                                                   upper_pad.shape[1] * (kernel.row_range[-1]-kernel.row_range[-2]),
+                                                   movie.data.shape[1])
+                    movie.row_range_orig = movie.row_range
+                    movie.row_range = kernel.row_range
+                    kernel.row_inds = kernel.row_inds + lower_pad.shape[1]
+        else:
+            pass
         kernel.apply_threshold(threshold)
              
         super(LNUnitCursor, self).__init__(kernel, movie)
     
     def __call__(self, t):
         # TODO: Don't use call operator, change to evaluate
         return self.lnunit.transfer_function(super(LNUnitCursor, self).__call__(t))
@@ -155,15 +223,18 @@
     def evaluate(self, threshold=0):
         full_spatial_kernel = np.array([self.spatial_kernel.full()])
         full_temporal_kernel = self.temporal_kernel.full()
 
         # Convolve every frame in the movie with the spatial filter. First find the range of rows (range min and max)
         #  and columns in the filter that are above threshold, that way only portion of movie/filter are multiplied
         # together
-        nonzero_inds = np.where(np.abs(full_spatial_kernel[0, :, :]) >= threshold)
+        
+        # Using > instead of >= makes the code faster if there are many zeros in the
+        # spatial kernel. This will not affect the results.
+        nonzero_inds = np.where(np.abs(full_spatial_kernel[0, :, :]) > threshold)
         rm, rM = nonzero_inds[0].min(), nonzero_inds[0].max()
         cm, cM = nonzero_inds[1].min(), nonzero_inds[1].max()
         convolution_answer_sep_spatial = (self.movie.data[:, rm:rM+1, cm:cM+1] *
                                           full_spatial_kernel[:, rm:rM+1, cm:cM+1]).sum(axis=1).sum(axis=1)
 
         # Convolve results of spatial convolution with the temporal filter
         sig_tmp = np.zeros(len(full_temporal_kernel) + len(convolution_answer_sep_spatial) - 1)
```

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/fitfuns.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/fitfuns.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/gaborfilter.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/spatialfilter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import numpy as np
 import itertools
 from six import string_types
 from scipy import ndimage
 
-#from . import utilities as util
+from . import utilities as util
 from .kernel import Kernel2D
 
 
 class ArrayFilter(object):
     def __init__(self, mask):
         self.mask = mask
         
@@ -20,41 +20,38 @@
 
         kernel_vals = self.mask[row_vals, col_vals]
         kernel_vals = amplitude*kernel_vals/kernel_vals.sum()
         
         return Kernel2D(row_range, col_range, row_vals, col_vals, kernel_vals)
     
 
-class GaborFilter(object):
-    def __init__(self, translate=4.0, sigma=1.0, theta=0.0, Lambda=1.0, psi=0.0, gamma=1.0):
+class GaussianSpatialFilter(object):
+    def __init__(self, translate=(0.0, 0.0), sigma=(1.0, 1.0), rotation=0, origin='center'):
         """A 2D gaussian used for filtering a part of the receptive field.
 
-        :param translate: float, the center frequency of the gabor
-        :param sigma: (float, float), the gaussian std
-        :param theta: float, rotation of the Gabor filter in radians
-        :param Lambda: float, wavelength of sinusoidal
-        :param psi: float, phase of sinusoidal factor relative to Gaussian in radians
-        :param gamma: aspect ratio of 2D Gaussian
+        :param translate: (float, float), the location of the gaussian on the screen relative to the origin in pixels.
+        :param sigma: (float, float), the x and y gaussian std
+        :param rotation: rotation of the gaussian in degrees
+        :param origin: origin of the receptive field (defaults center of image)
         """
 
+        # When w=1 and rotation=0, half-height will be at y=1
         self.translate = translate
+        self.rotation = rotation
 
         if isinstance(sigma, string_types):
             # TODO: Move this to calling method
             try:
                 sigma = ast.literal_eval(sigma)
             except Exception as exc:
                 pass
 
         self.sigma = sigma
-        self.theta = theta
-        self.Lambda = Lambda
-        self.psi = psi
-        self.gamma = gamma
-
+        self.origin = origin
+        
     def imshow(self, row_range, col_range, threshold=0, **kwargs):
         return self.get_kernel(row_range, col_range, threshold).imshow(**kwargs)
         
     def to_dict(self):
         return {
             'class': (__name__, self.__class__.__name__),
             'translate': self.translate,
@@ -106,8 +103,10 @@
         kernel_data = util.apply_transformation_matrix(on_filter_spatial, translation_matrix + rotation_matrix)
         
         kernel = Kernel2D.from_dense(row_range, col_range, kernel_data, threshold=0)
         kernel.apply_threshold(threshold)
         kernel.normalize()
         kernel.kernel *= amplitude
 
+        #kernel.imshow()
+
         return kernel
```

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/kernel.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/kernel.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,27 +126,45 @@
 
     def rescale(self):
         if np.abs(self.kernel.sum()) != 0:
             self.kernel /= np.abs(self.kernel.sum())
     
     def normalize(self):
         self.kernel /= np.abs(self.kernel.sum())
-            
+
+    def normalize2(self, remove_offset=True):
+        # Better for kernels that are not all positive
+        if remove_offset:
+            self.kernel -= self.kernel.mean()      # Set amplitude offset to 0
+        size = np.sum(np.abs(self.kernel))
+        self.kernel /= size        # Normalize overall size and maximum output
+
     @classmethod
     def from_dense(cls, row_range, col_range, kernel_array, threshold=0.):
         col_range = np.array(col_range).copy()
         row_range = np.array(row_range).copy()
         kernel_array = np.array(kernel_array).copy()
-        inds_to_keep = np.where(np.abs(kernel_array) > threshold)
-        kernel = kernel_array[inds_to_keep]
-        if len(inds_to_keep) == 1:
+        #inds_to_keep = np.where(np.abs(kernel_array) > threshold)
+        # Find cropped contiguous rectangle containing above threshold kernel values
+        above_thresh = np.abs(kernel_array) > threshold
+        start_ind0 = np.argmax(np.max(above_thresh, axis=1))
+        b = above_thresh[::-1,:]
+        end_ind0 = b.shape[0] - np.argmax(np.max(b,axis=1))
+        start_ind1 = np.argmax(np.max(above_thresh, axis=0))
+        b = above_thresh[:,::-1]
+        end_ind1 = b.shape[1] - np.argmax(np.max(b, axis=0))
+        #kernel = kernel_array[inds_to_keep]
+
+        col_inds, row_inds = [v.flatten() for v in
+                              np.meshgrid(range(start_ind0, end_ind0), range(start_ind1, end_ind1), indexing='ij')]
+
+        kernel = kernel_array[col_inds, row_inds]
+        if len(np.where(above_thresh)) == 1:
             col_inds, row_inds = np.array([]), np.array([])
-        else:
-            col_inds, row_inds = inds_to_keep
-        
+
         return cls(row_range, col_range, row_inds, col_inds,  kernel)
     
     @classmethod
     def copy(cls, instance):
         return cls(instance.row_range.copy(), 
                    instance.col_range.copy(), 
                    instance.row_inds.copy(),
@@ -182,44 +200,55 @@
         row_inds = np.array(row_inds_list)
         col_inds = np.array(col_inds_list)
         kernel = np.array(kernel_list)
         
         return Kernel2D(row_range, col_range, row_inds, col_inds, kernel)
     
     def apply_threshold(self, threshold):
-        
+
         inds_to_keep = np.where(np.abs(self.kernel) > threshold)
         self.row_inds = self.row_inds[inds_to_keep]
         self.col_inds = self.col_inds[inds_to_keep]
         self.kernel = self.kernel[inds_to_keep]
-        
-    def full(self):
+
+    def full(self, truncate_col=False):
         data = np.zeros((len(self.row_range), len(self.col_range)))
         data[self.row_inds, self.col_inds] = self.kernel
-        return data
+        if truncate_col:    # For spectrotemporal receptive fields where col is time dimension
+            ind_max = np.max(self.col_inds)
+            return data[:, :ind_max]
+        else:
+            return data
         
-    def imshow(self, ax=None, show=True, save_file_name=None, clim=None, colorbar=True):
+    def imshow(self, ax=None, show=True, save_file_name=None, clim=None, colorbar=True, truncate_col=False, xlabel=None,
+               ylabel=None):
         
         from mpl_toolkits.axes_grid1 import make_axes_locatable
         
         if ax is None:
             _, ax = plt.subplots(1, 1)
         
         if colorbar:
             divider = make_axes_locatable(ax)
             cax = divider.append_axes("right", size="5%", pad=0.05)
         
-        data = self.full()
-
+        data = self.full(truncate_col=truncate_col)
+        if truncate_col:
+            col_max = self.col_range[np.max(self.col_inds)]
+        else:
+            col_max = self.col_range[-1]
         if clim is not None:
-            im = ax.imshow(data, extent=(self.col_range[0], self.col_range[-1], self.row_range[0], self.row_range[-1]),
-                           origin='lower', clim=clim, interpolation='none')
+            im = ax.imshow(data, extent=(self.col_range[0], col_max, np.squeeze(self.row_range[0]),
+                                         np.squeeze(self.row_range[-1])), origin='lower', clim=clim, interpolation='none')
         else:
-            im = ax.imshow(data, extent=(self.col_range[0], self.col_range[-1], self.row_range[0], self.row_range[-1]),
-                           origin='lower', interpolation='none')
+            im = ax.imshow(data, extent=(self.col_range[0], col_max, np.squeeze(self.row_range[0]),
+                                         np.squeeze(self.row_range[-1])), origin='lower', interpolation='none',
+                                        aspect='auto')
+        ax.set_xlabel(xlabel)
+        ax.set_ylabel(ylabel)
         
         if colorbar:
             plt.colorbar(im, cax=cax)
 
         if save_file_name is not None:
             plt.savefig(save_file_name, transparent=True)
```

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/lattice_unit_constructor.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/lattice_unit_constructor.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/lgnmodel1.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/lgnmodel1.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/lnunit.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/lnunit.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,18 @@
         self.amplitude = amplitude
 
     def evaluate(self, movie, **kwargs):
         return self.get_cursor(movie, separable=kwargs.pop('separable', False)).evaluate(**kwargs)
  
     def get_spatiotemporal_kernel(self, *args, **kwargs):
         return self.linear_filter.get_spatiotemporal_kernel(*args, **kwargs)
-    
+
+    def get_spectrotemporal_kernel(self, *args, **kwargs):
+        return self.linear_filter.get_spectrotemporal_kernel(*args, **kwargs)
+
     def get_cursor(self, movie, threshold=0, separable=False):
         if separable:
             return SeparableLNUnitCursor(self, movie)
         else:
             return LNUnitCursor(self, movie, threshold=threshold)
     
     def show_temporal_filter(self, *args, **kwargs):
```

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/make_cell_list.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/make_cell_list.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/movie.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/movie.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 
 from .utilities import convert_tmin_tmax_framerate_to_trange
 from bmtk.simulator.filternet.io_tools import io
 
 
 class Movie(object):
     def __init__(self, data, row_range=None, col_range=None, labels=('time', 'y', 'x'),
-                 units=('second', 'pixel', 'pixel'), frame_rate=None, t_range=None):
+                 units=('second', 'pixel', 'pixel'), frame_rate=None, t_range=None, padding=False):
         self.data = data
         self.labels = labels
         self.units = units
+        self.padding=padding
         assert(units[0] == 'second')
 
         if t_range is None:
             self.frame_rate = float(frame_rate)
             self.t_range = np.arange(data.shape[0])*(1./self.frame_rate)
         else:
             self.t_range = np.array(t_range)
@@ -249,35 +250,37 @@
 class GratingMovie(Movie):
     def __init__(self, row_size, col_size, frame_rate=1000.0):
         self.row_size = row_size  # in degrees
         self.col_size = col_size  # in degrees
         self.frame_rate = float(frame_rate)  # in Hz
 
     def create_movie(self, t_min=0, t_max=1, gray_screen_dur=0, cpd=0.05, temporal_f=4, theta=45,
-                     phase=0., contrast=1.0, row_size_new=None, col_size_new=None):
+                     phase=0., contrast=1.0, degrees_per_pixel=None, row_size_new=None, col_size_new=None):
         """Create the grating movie with the desired parameters
 
         :param t_min: start time in seconds
         :param t_max: end time in seconds
         :param gray_screen_dur: Duration of gray screen before grating stimulus starts
         :param cpd: cycles per degree
         :param temporal_f: in Hz
         :param theta: orientation angle, in degrees
         :param phase: temporal phase, in degrees
         :param contrast: the maximum constrast, must be between 0 and 1.0
+        :param degrees_per_pixel: pixel pitch of the movie in degrees (default (if None) is 1.0/(cpd*10))
         :param row_size_new: Use to truncate screen, by default leaves original row dimension
         :param col_size_new: Use to truncate screen, by default leaves original col dimension
         :return: Movie object of grating with desired parameters
         """
         assert contrast <= 1, "Contrast must be <= 1"
         assert contrast > 0, "Contrast must be > 0"
 
-        physical_spacing = 1.0 / (float(cpd) * 10)  # To make sure no aliasing occurs
-        self.row_range = np.linspace(0, self.row_size, int(self.row_size/physical_spacing), endpoint=True)
-        self.col_range = np.linspace(0, self.col_size, int(self.col_size/physical_spacing), endpoint=True)
+        if degrees_per_pixel is None:  # default behavior when not specified
+            degrees_per_pixel = 1.0 / (float(cpd) * 10)  # To make sure no aliasing occurs
+        self.row_range = np.linspace(0, self.row_size, int(self.row_size/degrees_per_pixel), endpoint=True)
+        self.col_range = np.linspace(0, self.col_size, int(self.col_size/degrees_per_pixel), endpoint=True)
         numberFramesNeeded = int(round(self.frame_rate * (t_max - gray_screen_dur))) + 1
         time_range = np.linspace(0, t_max - gray_screen_dur, numberFramesNeeded, endpoint=True)
 
         # Creates a drifting grating panel
         tt, yy, xx = np.meshgrid(time_range, self.row_range, self.col_range, indexing='ij')
         theta_rad = np.pi*(180 - theta) / 180.
         phase_rad = np.pi*(180 - phase) / 180.
@@ -312,17 +315,17 @@
 
     def create_movie(self, t_looming=1, gray_screen_dur=0.5):
         """Create the looming movie with the desired parameters
 
         :param t_looming: duration of time looming
         :param gray_screen_dur:
         """
-        physical_spacing = 1.0  # To make sure no aliasing occurs
-        self.row_range = np.linspace(0, self.row_size, int(self.row_size/physical_spacing), endpoint=True)
-        self.col_range = np.linspace(0, self.col_size, int(self.col_size/physical_spacing), endpoint=True)
+        degrees_per_pixel = 1.0  # To make sure no aliasing occurs
+        self.row_range = np.linspace(0, self.row_size, int(self.row_size/degrees_per_pixel), endpoint=True)
+        self.col_range = np.linspace(0, self.col_size, int(self.col_size/degrees_per_pixel), endpoint=True)
         loomingFramesNeeded = int(round(self.frame_rate * t_looming))
         grayScreenFrames = int(round(self.frame_rate * gray_screen_dur))
         time_range = np.linspace(0, t_looming, loomingFramesNeeded, endpoint=True)
 
         data = np.zeros((grayScreenFrames + loomingFramesNeeded, self.row_size, self.col_size))
         # mgrid is a mesh creation helper
         xx, yy = np.mgrid[:self.row_size, :self.col_size]
```

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/poissongeneration.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/poissongeneration.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/temporalfilter.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/temporalfilter.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/transferfunction.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/transferfunction.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/util_fns.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/util_fns.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/lgnmodel/utilities.py` & `bmtk-1.1.0/bmtk/simulator/filternet/lgnmodel/utilities.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/modules/create_spikes.py` & `bmtk-1.1.0/bmtk/simulator/filternet/modules/create_spikes.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/modules/record_rates.py` & `bmtk-1.1.0/bmtk/simulator/filternet/modules/record_rates.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/pyfunction_cache.py` & `bmtk-1.1.0/bmtk/simulator/filternet/pyfunction_cache.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/filternet/sonata_adaptors.py` & `bmtk-1.1.0/bmtk/simulator/filternet/sonata_adaptors.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 import json
 import types
 import numpy as np
+from six import string_types
 
 from bmtk.simulator.core.sonata_reader import NodeAdaptor, SonataBaseNode, EdgeAdaptor, SonataBaseEdge
 
 
 class FilterNode(SonataBaseNode):
     def __init__(self, node, prop_adaptor):
         super(FilterNode, self).__init__(node, prop_adaptor)
@@ -58,15 +59,48 @@
     def kpeaks_non_dom(self):
         return self._prop_adaptor.kpeaks_non_dom(self._node)
 
     @property
     def delays_non_dom(self):
         return self._prop_adaptor.delays_non_dom(self._node)
 
+    @property
+    def sigma_f(self):
+        return self._prop_adaptor.sigma_f(self._node)
+
+    @property
+    def b_t(self):
+        return self._prop_adaptor.b_t(self._node)
+
+    @property
+    def order_t(self):
+        return self._prop_adaptor.order_t(self._node)
+
+    @property
+    def t_mod_freq(self):
+        return self._prop_adaptor.t_mod_freq(self._node)
+
+    @property
+    def sp_mod_freq(self):
+        return self._prop_adaptor.sp_mod_freq(self._node)
 
+    @property
+    def psi(self):
+        return self._prop_adaptor.psi(self._node)
+
+    @property
+    def delay(self):
+        return self._prop_adaptor.delay(self._node)
+
+    @property
+    def amplitude(self):
+        return self._prop_adaptor.amplitude(self._node)
+    @property
+    def direction(self):
+        return self._prop_adaptor.direction(self._node)
 class FilterNodeAdaptor(NodeAdaptor):
     def get_node(self, sonata_node):
         return FilterNode(sonata_node, self)
 
     @staticmethod
     def preprocess_node_types(network, node_population):
         NodeAdaptor.preprocess_node_types(network, node_population)
@@ -119,14 +153,16 @@
         find_kpeaks_params(node_group, node_adaptor)
         find_delays_params(node_group, node_adaptor)
 
         find_nondom_weight_params(node_group, node_adaptor)
         find_nondom_kpeaks_params(node_group, node_adaptor)
         find_nondom_delays_params(node_group, node_adaptor)
 
+        find_spectrotemporal_params(node_group, node_adaptor)
+
         return node_adaptor
 
 def non_dom_params(self, node):
     return node['non_dom_params']
 
 
 def return_none(self, node):
@@ -230,7 +266,56 @@
 
     elif 'delay_non_dom_0' in node_group.all_columns and 'delay_non_dom_1' in node_group.all_columns:
         node_adaptor.delays_non_dom = types.MethodType(
             lambda self, node: [node['delay_non_dom_0'], node['delay_non_dom_1']], node_adaptor
         )
     else:
         node_adaptor.delays_non_dom = types.MethodType(return_none, node_adaptor)
+
+
+def find_spectrotemporal_params(node_group, node_adaptor):
+    if 'sigma_f' in node_group.all_columns:
+        node_adaptor.sigma_f = types.MethodType(lambda self, node: node['sigma_f'], node_adaptor)
+    else:
+        node_adaptor.sigma_f = types.MethodType(return_none, node_adaptor)
+
+    if 'b_t' in node_group.all_columns:
+        node_adaptor.b_t = types.MethodType(lambda self, node: node['b_t'], node_adaptor)
+    else:
+        node_adaptor.b_t = types.MethodType(return_none, node_adaptor)
+
+    if 'order_t' in node_group.all_columns:
+        node_adaptor.order_t = types.MethodType(lambda self, node: node['order_t'], node_adaptor)
+    else:
+        node_adaptor.order_t = types.MethodType(return_none, node_adaptor)
+
+    if 't_mod_freq' in node_group.all_columns:
+        node_adaptor.t_mod_freq = types.MethodType(lambda self, node: node['t_mod_freq'], node_adaptor)
+    else:
+        node_adaptor.t_mod_freq = types.MethodType(return_none, node_adaptor)
+
+    if 'sp_mod_freq' in node_group.all_columns:
+        node_adaptor.sp_mod_freq = types.MethodType(lambda self, node: node['sp_mod_freq'], node_adaptor)
+    else:
+        node_adaptor.sp_mod_freq = types.MethodType(return_none, node_adaptor)
+
+    if 'psi' in node_group.all_columns:
+        node_adaptor.psi = types.MethodType(lambda self, node: node['psi'], node_adaptor)
+        if isinstance(node_adaptor.psi, string_types):
+            node_adaptor.psi = eval(node_adaptor.psi.replace('pi', 'np.pi'))
+    else:
+        node_adaptor.psi = types.MethodType(return_none, node_adaptor)
+
+    if 'delay' in node_group.all_columns:
+        node_adaptor.delay = types.MethodType(lambda self, node: node['delay'], node_adaptor)
+    else:
+        node_adaptor.delay = types.MethodType(return_none, node_adaptor)
+
+    if 'amplitude' in node_group.all_columns:
+        node_adaptor.amplitude = types.MethodType(lambda self, node: node['amplitude'], node_adaptor)
+    else:
+        node_adaptor.amplitude = types.MethodType(return_none, node_adaptor)
+
+    if 'direction' in node_group.all_columns:
+        node_adaptor.direction = types.MethodType(lambda self, node: node['direction'], node_adaptor)
+    else:
+        node_adaptor.direction = types.MethodType(return_none, node_adaptor)
```

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/__init__.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/config.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/config.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/gids.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/gids.py`

 * *Files 13% similar despite different names*

```diff
@@ -23,21 +23,36 @@
 
 class GidPool(object):
     def __init__(self):
         # self._popid2gid = {}  # (pop_name, node_id) --> nest_id
         self._gid2pop_id = {}  # nest_id --> (pop_name, node_id)
         self._nestid_lu = {}
 
+        self._nest_ids = []
+        self._node_ids = []
+        self._populations = []
+        self._nestid2nodeid_df = None
+
     @property
     def gids(self):
         return list(self._gid2pop_id.keys())
 
     @property
     def populations(self):
         return list(self._nestid_lu.keys())
+    
+    @property
+    def nestid2nodeid_df(self):
+        if self._nestid2nodeid_df is None:
+            self._nestid2nodeid_df = pd.DataFrame({
+                'nest_ids': self._nest_ids,
+                'node_ids': self._node_ids,
+                'populations': self._populations
+            }).set_index('nest_ids')
+        return self._nestid2nodeid_df
 
     def add(self, name, node_id, gid):
         raise NotImplementedError()
 
     def get_gid(self, name, node_id):
         return self.get_nestids(name=name, node_ids=[node_id])[0]
 
@@ -62,19 +77,31 @@
             # lu_table = lu_table.reindex(lu_table.index.values)
 
         self._nestid_lu[name] = lu_table
 
         for node_id, nest_id in zip(node_ids, nest_ids):
             self._gid2pop_id[nest_id] = PopulationID(population=name, node_id=node_id)
 
+        self._nestid2nodeid_df = None
+        self._nest_ids.extend(nest_ids)
+        self._node_ids.extend(node_ids)
+        self._populations.extend([name]*len(nest_ids))
+
     def add_gids(self, name, node_ids, gids):
         self.add_nestids(name=name, node_ids=node_ids, nest_ids=gids)
 
     def get_nestids(self, name, node_ids):
         nestids_table = self._nestid_lu[name]
         return nestids_table.loc[node_ids]['nest_ids'].values
 
     def get_gids(self, name, node_ids):
         return self.get_nestids(name=name, node_ids=node_ids)
 
+    def get_node_ids(self, nest_ids, with_populations=True):
+        sonata_ids_df = self.nestid2nodeid_df.loc[nest_ids]
+        if with_populations:
+            return sonata_ids_df['node_ids'].values, sonata_ids_df['populations'].values
+        else:
+            return sonata_ids_df['node_ids'].values
+
     def __len__(self):
         return len(self.gids)
```

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/glif_utils.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/glif_utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/io_tools.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/io_tools.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/modules/ecephys_module.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/modules/ecephys_module.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/modules/iclamp.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/modules/iclamp.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/modules/multimeter_reporter.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/modules/multimeter_reporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import glob
 import pandas as pd
 from bmtk.utils.reports import CompartmentReport
 from bmtk.simulator.pointnet.io_tools import io
 from bmtk.simulator.pointnet.nest_utils import nest_version
+from bmtk.simulator.pointnet.modules.sim_module import SimulatorMod
 
 import nest
 
 
 try:
     MPI_RANK = nest.Rank()
     N_HOSTS = nest.NumProcesses()
@@ -60,15 +61,15 @@
     create_multimeter = create_multimeter_nest3
     read_dat = read_dat_nest3
 else:
     create_multimeter = create_multimeter_nest2
     read_dat = read_dat_nest2
 
 
-class MultimeterMod(object):
+class MultimeterMod(SimulatorMod):
     def __init__(self, tmp_dir, file_name, variable_name, cells, tstart=None, tstop=None, interval=None, to_h5=True,
                  delete_dat=True, **opt_params):
         """For recording neuron properties using a NEST multimeter object
 
         :param tmp_dir: ouput directory
         :param file_name: Name of (SONATA hdf5) file that will be saved to
         :param variable_name: A list of the variable(s) being recorded. Must be valid according to the cells
```

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/modules/record_spikes.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/modules/record_spikes.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 import glob
 import csv
 import pandas as pd
 
 from bmtk.utils.reports.spike_trains import SpikeTrains, sort_order, sort_order_lu
 from bmtk.simulator.pointnet.io_tools import io
 from bmtk.simulator.pointnet.nest_utils import nest_version
+from bmtk.simulator.pointnet.modules.sim_module import SimulatorMod
 
 import nest
 
 
 try:
     MPI_RANK = nest.Rank()
     N_HOSTS = nest.NumProcesses()
@@ -87,15 +88,15 @@
     NEST_spikes_file_format = 'dat'
 else:
     create_spike_detector = create_spike_detector_nest2
     read_spikes_file = read_spikes_file_nest2
     NEST_spikes_file_format = 'gdf'
 
 
-class SpikesMod(object):
+class SpikesMod(SimulatorMod):
     """Module use for saving spikes
 
     """
 
     def __init__(self, tmp_dir, spikes_file_csv=None, spikes_file=None, spikes_file_nwb=None, spikes_sort_order=None,
                  cache_to_disk=True, compression='gzip'):
         def _get_path(file_name):
```

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/nest_utils.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/nest_utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/pointnetwork.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/pointnetwork.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/pointsimulator.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/pointsimulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -232,49 +232,53 @@
         graph.io.log_info('Setting up output directory')
         if not os.path.exists(config['output']['output_dir']):
             os.mkdir(config['output']['output_dir'])
         elif overwrite:
             for gfile in glob.glob(os.path.join(config['output']['output_dir'], '*.gdf')):
                 os.remove(gfile)
 
-        graph.io.log_info('Building cells.')
-        graph.build_nodes()
-
-        graph.io.log_info('Building recurrent connections')
-        graph.build_recurrent_edges()
-
         for sim_input in inputs.from_config(config):
-            node_set = graph.get_node_set(sim_input.node_set)
-            if sim_input.input_type == 'spikes' and sim_input.module in ['nwb', 'csv', 'sonata']:
-                io.log_info('Build virtual cell stimulations for {}'.format(sim_input.name))
-                path = sim_input.params['input_file']
-                spikes = SpikeTrains.load(path=path, file_type=sim_input.module, **sim_input.params)
-                #spikes = spike_trains.SpikesInput.load(name=sim_input.name, module=sim_input.module,
-                #                                       input_type=sim_input.input_type, params=sim_input.params)
-                graph.add_spike_trains(spikes, node_set, network.get_spike_generator_params())
-            
+            if sim_input.input_type == 'spikes' and sim_input.module in ['nwb', 'csv', 'sonata', 'h5', 'hdf5']:
+                network.add_mod(mods.SpikesInputsMod(
+                    name=sim_input.name,
+                    input_type=sim_input.input_type,
+                    module=sim_input.module,
+                    # node_set=sim_input.node_set,
+                    **sim_input.params
+                ))
+
             elif sim_input.module == 'IClamp':
                 network.add_mod(mods.IClampMod(input_type=sim_input.input_type, **sim_input.params))
 
             elif sim_input.module == 'ecephys_probe':
                 network.add_mod(mods.PointECEphysUnitsModule(name=sim_input.name, **sim_input.params))
             
             else:
                 graph.io.log_warning('Unknown input type {}'.format(sim_input.input_type))
 
         sim_reports = reports.from_config(config)
-        for report in sim_reports:
+        for report in sim_reports:           
             if report.module == 'spikes_report':
                 mod = mods.SpikesMod(**report.params)
 
             elif isinstance(report, reports.MembraneReport):
                 # For convience and for compliance with SONATA format. "membrane_report" and "multimeter_report is the
                 # same in pointnet.
                 mod = mods.MultimeterMod(**report.params)
+            
+            elif isinstance(report, reports.WeightRecorder):
+                mod = mods.WeightRecorder(name=report.report_name, **report.params)
 
             else:
                 graph.io.log_exception('Unknown report type {}'.format(report.module))
 
+            mod.preload(sim=graph)
             network.add_mod(mod)
 
+        graph.io.log_info('Building cells.')
+        graph.build_nodes()
+
+        graph.io.log_info('Building recurrent connections')
+        graph.build_recurrent_edges()
+
         io.log_info('Network created.')
         return network
```

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/property_map.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/property_map.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/pyfunction_cache.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/pyfunction_cache.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/sonata_adaptors.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/sonata_adaptors.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/pointnet/utils.py` & `bmtk-1.1.0/bmtk/simulator/pointnet/utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/popnet/__init__.py` & `bmtk-1.1.0/bmtk/simulator/popnet/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/popnet/config.py` & `bmtk-1.1.0/bmtk/simulator/popnet/config.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/popnet/popedge.py` & `bmtk-1.1.0/bmtk/simulator/popnet/popedge.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/popnet/popnetwork.py` & `bmtk-1.1.0/bmtk/simulator/popnet/popnetwork.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/popnet/popnode.py` & `bmtk-1.1.0/bmtk/simulator/popnet/popnode.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/popnet/popsimulator.py` & `bmtk-1.1.0/bmtk/simulator/popnet/popsimulator.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/popnet/utils.py` & `bmtk-1.1.0/bmtk/simulator/popnet/utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/utils/__init__.py` & `bmtk-1.1.0/bmtk/simulator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/utils/simulation_inputs.py` & `bmtk-1.1.0/bmtk/simulator/utils/simulation_inputs.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/simulator/utils/simulation_reports.py` & `bmtk-1.1.0/bmtk/simulator/utils/simulation_reports.py`

 * *Files 14% similar despite different names*

```diff
@@ -276,27 +276,46 @@
     @staticmethod
     def avail_modules():
         return 'SaveSynapses'
 
 
 @SimReport.register_module
 class MultimeterReport(MembraneReport):
-
     @staticmethod
     def avail_modules():
         return ['multimeter', 'multimeter_report']
 
 
 @SimReport.register_module
 class NetconReport(MembraneReport):
     @staticmethod
     def avail_modules():
         return ['netcon_report']
 
 
+@SimReport.register_module
+class WeightRecorder(SimReport):
+    @staticmethod
+    def avail_modules():
+        return 'weight_recorder'
+   
+    def _get_defaults(self):
+        output_dir = self.params.get('output_dir', self.default_dir)
+
+        file_name = self.params.get('file_name', None)
+        if file_name is None:
+            file_name = os.path.join(output_dir, '{}.csv'.format(self.report_name))
+        elif os.path.isabs(file_name):
+            file_name = file_name           
+        else:
+            file_name = os.path.join(output_dir, file_name)
+
+        return [('file_name', file_name), ('output_dir', output_dir), ('clean_temp_file', True)]
+
+
 def from_config(cfg):
     SimReport.default_dir = cfg.output_dir
 
     reports_list = []
     membrane_reports = []
     has_spikes_report = False
     for report_name, report_params in cfg.reports.items():
```

### Comparing `bmtk-1.0.8/bmtk/utils/__init__.py` & `bmtk-1.1.0/bmtk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/compile_mechanisms/__main__.py` & `bmtk-1.1.0/bmtk/utils/compile_mechanisms/__main__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/compile_mechanisms/compile_mechanisms.py` & `bmtk-1.1.0/bmtk/utils/compile_mechanisms/compile_mechanisms.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/create_environment/__main__.py` & `bmtk-1.1.0/bmtk/utils/create_environment/__main__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/create_environment/create_environment.py` & `bmtk-1.1.0/bmtk/utils/create_environment/create_environment.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/create_environment/env_builder.py` & `bmtk-1.1.0/bmtk/utils/create_environment/env_builder.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/io/__init__.py` & `bmtk-1.1.0/bmtk/utils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/io/cell_vars.py` & `bmtk-1.1.0/bmtk/utils/io/cell_vars.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/io/firing_rates.py` & `bmtk-1.1.0/bmtk/utils/io/firing_rates.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/io/ioutils.py` & `bmtk-1.1.0/bmtk/utils/io/ioutils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/io/spike_trains.py` & `bmtk-1.1.0/bmtk/utils/io/spike_trains.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/compartment/compartment_reader.py` & `bmtk-1.1.0/bmtk/utils/reports/compartment/compartment_reader.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/compartment/compartment_report.py` & `bmtk-1.1.0/bmtk/utils/reports/compartment/compartment_report.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/compartment/compartment_writer.py` & `bmtk-1.1.0/bmtk/utils/reports/compartment/compartment_writer.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/compartment/core.py` & `bmtk-1.1.0/bmtk/utils/reports/compartment/core.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/compartment/plotting.py` & `bmtk-1.1.0/bmtk/utils/reports/compartment/plotting.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/current_writer.py` & `bmtk-1.1.0/bmtk/utils/reports/current_writer.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/spike_trains/__init__.py` & `bmtk-1.1.0/bmtk/utils/reports/spike_trains/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/spike_trains/core.py` & `bmtk-1.1.0/bmtk/utils/reports/spike_trains/core.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/spike_trains/plotting.py` & `bmtk-1.1.0/bmtk/utils/reports/spike_trains/plotting.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_train_buffer.py` & `bmtk-1.1.0/bmtk/utils/reports/spike_trains/spike_train_buffer.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_train_readers.py` & `bmtk-1.1.0/bmtk/utils/reports/spike_trains/spike_train_readers.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_trains.py` & `bmtk-1.1.0/bmtk/utils/reports/spike_trains/spike_trains.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/reports/spike_trains/spike_trains_api.py` & `bmtk-1.1.0/bmtk/utils/reports/spike_trains/spike_trains_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 import numpy as np
 import warnings
 
 from .core import SortOrder
-from .spikes_file_writers import write_csv, write_sonata
+from .spikes_file_writers import write_csv, write_sonata, write_nwb
 
 
 class SpikeTrainsAPI(object):
     def add_spike(self, node_id, timestamp, population=None, **kwargs):
         """Add a single spike
 
         :param node_id: integer, id of node/cell that spike belongs too.
@@ -165,15 +165,15 @@
         :param sort_order:
         :param kwargs:
         :return:
         """
         write_csv(path=path, spiketrain_reader=self, mode=mode, sort_orders=sort_order, **kwargs)
 
     def to_nwb(self, path, mode='w', **kwargs):
-        raise NotImplemented()
+        write_nwb(path=path, spiketrain_reader=self, mode=mode, **kwargs)
 
     def merge(self, other):
         """Import Another SpikesTrain object into current file, always in-place.
 
         :param other: Another SpikeTrainsAPI object
         """
         raise NotImplementedError()
```

### Comparing `bmtk-1.0.8/bmtk/utils/reports/spike_trains/spikes_file_writers.py` & `bmtk-1.1.0/bmtk/utils/reports/spike_trains/spikes_file_writers.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,15 +20,17 @@
 # WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 import os
 import csv
 import h5py
 import numpy as np
+from datetime import datetime
 
+import bmtk
 from .core import SortOrder, csv_headers, col_population, find_conversion
 from .core import MPI_rank, comm_barrier
 from bmtk.utils.sonata.utils import add_hdf5_magic, add_hdf5_version
 
 
 def write_sonata(path, spiketrain_reader, mode='w', sort_order=SortOrder.none, units='ms',
                  population_renames=None, compression='gzip', **kwargs):
@@ -141,7 +143,51 @@
     for spk in spiketrain_reader.spikes(sort_order=sort_order):
         if MPI_rank == 0:
             ts = spk[0]*conv_factor
             c_data = [ts, spk[1], spk[2]] if include_population else [ts, spk[2]]
             csv_writer.writerow(c_data)
 
     comm_barrier()
+
+
+def write_nwb(path, spiketrain_reader, mode='w', include_population=True, units='ms', **kwargs):
+    import pynwb
+    
+    path_dir = os.path.dirname(path)
+    if MPI_rank == 0 and path_dir and not os.path.exists(path_dir):
+        os.makedirs(path_dir)
+
+    if MPI_rank == 0:
+        # Last checked pynwb doesn't support writing on multiple cores, must let first core do all the
+        # writing to NWB.
+        nwbfile = pynwb.NWBFile(
+            session_description='BMTK {} generated NWB spikes file'.format(bmtk.__version__),
+            identifier='Generated in-silico, no session id',  # TODO: No idea what to put here?
+            session_start_time=datetime.now().astimezone(),
+            # experiment_description=str(session.experiment_metadata['experiment_id'])
+        )
+
+        if include_population:
+            nwbfile.add_unit_column(name="population", description="node population identifier")
+            add_unit = lambda nid, pop, st: nwbfile.add_unit(id=nid, spike_times=st, population=pop, node_id=nid)
+        else:
+            add_unit = lambda nid, pop, st: nwbfile.add_unit(id=nid, spike_times=st, node_id=nid)
+
+        nwbfile.add_unit_column(name="node_id", description="id of each node within a population")
+
+        for population in spiketrain_reader.populations:
+            for node_id in spiketrain_reader.node_ids(population=population):
+                spikes_times = spiketrain_reader.get_times(node_id=node_id, population=population)
+                if spikes_times is None or len(spikes_times) == 0:
+                    # No spikes for given node, don't try to write to nwb 
+                    continue
+
+                # sometimes bmtk/sonata may default to use different 32 or unsigned data-types which will cause
+                # nwb to throw a fit. Need to explicity convert data-types just in case.
+                spikes_times = spikes_times.astype('float64')
+                node_id = int(node_id)
+                add_unit(node_id, population, spikes_times)
+
+        with pynwb.NWBHDF5IO(path, mode) as io:
+            io.write(nwbfile)
+
+    comm_barrier()
```

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/318331342_fit.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/318331342_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/472363762_fit.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/472363762_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/472912177_fit.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/472912177_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/473862421_fit.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/473862421_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863035_fit.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863035_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863510_fit.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/473863510_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/biophysical_neuron_models/485184849_fit.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/biophysical_neuron_models/485184849_fit.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/default_config.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/default_config.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF1.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sOFF_TF1.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF15.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sOFF_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF2.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sOFF_TF2.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF4.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sOFF_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sOFF_TF8.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sOFF_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF1.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sON_TF1.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF2.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sON_TF2.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF4.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sON_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/sON_TF8.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/sON_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tOFF_TF15.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tOFF_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tOFF_TF4.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tOFF_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tOFF_TF8.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tOFF_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF15.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tON_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF4.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tON_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF8.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tON_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/filter_models/tON_TF8_demo.json` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/filter_models/tON_TF8_demo.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/CaDynamics.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/CaDynamics.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_HVA.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_HVA.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_LVA.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ca_LVA.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ih.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Ih.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im_v2.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Im_v2.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_P.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_P.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_T.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/K_T.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kd.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kd.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv2like.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv2like.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv3_1.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Kv3_1.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTa.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTa.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTs.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaTs.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaV.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/NaV.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/Nap.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/Nap.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/SK.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/SK.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/mechanisms/modfiles/vecevent.mod` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/mechanisms/modfiles/vecevent.mod`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Nr5a1_471087815_m.swc` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/morphologies/Nr5a1_471087815_m.swc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Pvalb_469628681_m.swc` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/morphologies/Pvalb_469628681_m.swc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Pvalb_470522102_m.swc` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/morphologies/Pvalb_470522102_m.swc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Rorb_325404214_m.swc` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/morphologies/Rorb_325404214_m.swc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/morphologies/Scnn1a_473845048_m.swc` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/morphologies/Scnn1a_473845048_m.swc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/templates/BioAxonStub.hoc` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/templates/BioAxonStub.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/bionet/templates/Biophys1.hoc` & `bmtk-1.1.0/bmtk/utils/scripts/bionet/templates/Biophys1.hoc`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF1.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sOFF_TF1.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF15.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sOFF_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF2.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sOFF_TF2.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF4.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sOFF_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sOFF_TF8.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sOFF_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF1.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sON_TF1.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF2.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sON_TF2.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF4.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sON_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/sON_TF8.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/sON_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tOFF_TF15.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tOFF_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tOFF_TF4.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tOFF_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tOFF_TF8.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tOFF_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF15.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tON_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF4.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tON_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF8.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tON_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/filter_models/tON_TF8_demo.json` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/filter_models/tON_TF8_demo.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/filternet/run_filternet.py` & `bmtk-1.1.0/bmtk/utils/scripts/filternet/run_filternet.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF1.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF1.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF15.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF2.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF2.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF4.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF8.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sOFF_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF1.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sON_TF1.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF2.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sON_TF2.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF4.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sON_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/sON_TF8.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/sON_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF15.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF4.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF8.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tOFF_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF15.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tON_TF15.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF4.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tON_TF4.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF8.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tON_TF8.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/pointnet/filter_models/tON_TF8_demo.json` & `bmtk-1.1.0/bmtk/utils/scripts/pointnet/filter_models/tON_TF8_demo.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/scripts/sonata.circuit_config.json` & `bmtk-1.1.0/bmtk/utils/scripts/sonata.circuit_config.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sim_setup.py` & `bmtk-1.1.0/bmtk/utils/sim_setup.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/__init__.py` & `bmtk-1.1.0/bmtk/utils/sonata/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/column_property.py` & `bmtk-1.1.0/bmtk/utils/sonata/column_property.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/config/__init__.py` & `bmtk-1.1.0/bmtk/utils/sonata/config/__init__.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/config/config_schema.json` & `bmtk-1.1.0/bmtk/utils/sonata/config/config_schema.json`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/config/sonata_config.py` & `bmtk-1.1.0/bmtk/utils/sonata/config/sonata_config.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/edge.py` & `bmtk-1.1.0/bmtk/utils/sonata/edge.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/file.py` & `bmtk-1.1.0/bmtk/utils/sonata/file.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/file_root.py` & `bmtk-1.1.0/bmtk/utils/sonata/file_root.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/group.py` & `bmtk-1.1.0/bmtk/utils/sonata/group.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/node.py` & `bmtk-1.1.0/bmtk/utils/sonata/node.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/population.py` & `bmtk-1.1.0/bmtk/utils/sonata/population.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/types_table.py` & `bmtk-1.1.0/bmtk/utils/sonata/types_table.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk/utils/sonata/utils.py` & `bmtk-1.1.0/bmtk/utils/sonata/utils.py`

 * *Files identical despite different names*

### Comparing `bmtk-1.0.8/bmtk.egg-info/SOURCES.txt` & `bmtk-1.1.0/bmtk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 bmtk.egg-info/dependency_links.txt
 bmtk.egg-info/requires.txt
 bmtk.egg-info/top_level.txt
 bmtk/analyzer/__init__.py
 bmtk/analyzer/cell_vars.py
 bmtk/analyzer/compartment.py
 bmtk/analyzer/ecp.py
+bmtk/analyzer/edges.py
 bmtk/analyzer/firing_rates.py
 bmtk/analyzer/io_tools.py
 bmtk/analyzer/spike_trains.py
 bmtk/analyzer/spikes_analyzer.py
 bmtk/analyzer/spikes_loader.py
 bmtk/analyzer/utils.py
 bmtk/builder/__init__.py
@@ -123,14 +124,15 @@
 bmtk/simulator/core/modules/simulator_module.py
 bmtk/simulator/core/sonata_reader/__init__.py
 bmtk/simulator/core/sonata_reader/edge_adaptor.py
 bmtk/simulator/core/sonata_reader/network_reader.py
 bmtk/simulator/core/sonata_reader/node_adaptor.py
 bmtk/simulator/core/sonata_schemas/config_schema.json
 bmtk/simulator/filternet/__init__.py
+bmtk/simulator/filternet/auditory_processing.py
 bmtk/simulator/filternet/cell.py
 bmtk/simulator/filternet/cell_models.py
 bmtk/simulator/filternet/config.py
 bmtk/simulator/filternet/filternetwork.py
 bmtk/simulator/filternet/filters.py
 bmtk/simulator/filternet/filtersimulator.py
 bmtk/simulator/filternet/io_tools.py
@@ -156,14 +158,15 @@
 bmtk/simulator/filternet/lgnmodel/poissongeneration.py
 bmtk/simulator/filternet/lgnmodel/singleunitcell.py
 bmtk/simulator/filternet/lgnmodel/spatialfilter.py
 bmtk/simulator/filternet/lgnmodel/temporalfilter.py
 bmtk/simulator/filternet/lgnmodel/transferfunction.py
 bmtk/simulator/filternet/lgnmodel/util_fns.py
 bmtk/simulator/filternet/lgnmodel/utilities.py
+bmtk/simulator/filternet/lgnmodel/waveletfilter.py
 bmtk/simulator/filternet/lgnmodel/cell_metrics/sOFF_cell_data.csv
 bmtk/simulator/filternet/lgnmodel/cell_metrics/sON_cell_data.csv
 bmtk/simulator/filternet/lgnmodel/cell_metrics/sus_sus_cells_v3.csv
 bmtk/simulator/filternet/lgnmodel/cell_metrics/tOFF_cell_data.csv
 bmtk/simulator/filternet/lgnmodel/cell_metrics/tON_cell_data.csv
 bmtk/simulator/filternet/lgnmodel/cell_metrics/trans_sus_cells_v3.csv
 bmtk/simulator/filternet/modules/__init__.py
@@ -186,14 +189,17 @@
 bmtk/simulator/pointnet/default_setters/synapse_models.py
 bmtk/simulator/pointnet/default_setters/synaptic_weights.py
 bmtk/simulator/pointnet/modules/__init__.py
 bmtk/simulator/pointnet/modules/ecephys_module.py
 bmtk/simulator/pointnet/modules/iclamp.py
 bmtk/simulator/pointnet/modules/multimeter_reporter.py
 bmtk/simulator/pointnet/modules/record_spikes.py
+bmtk/simulator/pointnet/modules/sim_module.py
+bmtk/simulator/pointnet/modules/spikes_inputs.py
+bmtk/simulator/pointnet/modules/weight_recorder.py
 bmtk/simulator/popnet/__init__.py
 bmtk/simulator/popnet/config.py
 bmtk/simulator/popnet/popedge.py
 bmtk/simulator/popnet/popnetwork.py
 bmtk/simulator/popnet/popnode.py
 bmtk/simulator/popnet/popsimulator.py
 bmtk/simulator/popnet/sonata_adaptors.py
@@ -350,14 +356,15 @@
 bmtk/utils/scripts/popnet/synaptic_models/InhToExc.json
 bmtk/utils/scripts/popnet/synaptic_models/InhToInh.json
 bmtk/utils/scripts/popnet/synaptic_models/input_ExcToExc.json
 bmtk/utils/scripts/popnet/synaptic_models/input_ExcToInh.json
 bmtk/utils/sonata/__init__.py
 bmtk/utils/sonata/column_property.py
 bmtk/utils/sonata/edge.py
+bmtk/utils/sonata/edge_stats.py
 bmtk/utils/sonata/file.py
 bmtk/utils/sonata/file_root.py
 bmtk/utils/sonata/group.py
 bmtk/utils/sonata/node.py
 bmtk/utils/sonata/population.py
 bmtk/utils/sonata/types_table.py
 bmtk/utils/sonata/utils.py
```

### Comparing `bmtk-1.0.8/setup.py` & `bmtk-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         'six',
         'h5py',
         'matplotlib',
         'enum; python_version <= "2.7"',
         'scipy',
         'scikit-image',  # Only required for filternet, consider making optional
         'sympy',  # For FilterNet
+        # 'numba',  # For FilterNet
         'pynrrd'   # For nrrd reader
     ],
     extras_require={
         'bionet': ['NEURON'],
         'mintnet': ['tensorflow'],
         'pointnet': ['NEST'],
         'popnet': ['DiPDE']
```

