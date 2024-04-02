# Comparing `tmp/scCellFie-0.1.5.tar.gz` & `tmp/scCellFie-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scCellFie-0.1.5.tar", last modified: Thu Mar  7 14:10:17 2024, max compression
+gzip compressed data, was "scCellFie-0.1.6.tar", last modified: Tue Apr  2 13:52:05 2024, max compression
```

## Comparing `scCellFie-0.1.5.tar` & `scCellFie-0.1.6.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.063743 scCellFie-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-03-07 14:10:09.000000 scCellFie-0.1.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-07 14:10:17.059743 scCellFie-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-03-07 14:10:09.000000 scCellFie-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.059743 scCellFie-0.1.5/scCellFie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-03-07 14:10:17.000000 scCellFie-0.1.5/scCellFie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-07 14:10:17.000000 scCellFie-0.1.5/scCellFie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 14:10:17.000000 scCellFie-0.1.5/scCellFie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-07 14:10:17.000000 scCellFie-0.1.5/scCellFie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-07 14:10:17.000000 scCellFie-0.1.5/scCellFie.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.051743 scCellFie-0.1.5/sccellfie/
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.055743 scCellFie-0.1.5/sccellfie/expression/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/expression/aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.055743 scCellFie-0.1.5/sccellfie/expression/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/expression/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/expression/tests/test_aggregation.py
--rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/expression/tests/test_threshold.py
--rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/expression/thresholds.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.055743 scCellFie-0.1.5/sccellfie/external/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.055743 scCellFie-0.1.5/sccellfie/external/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/external/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/external/tests/test_tf_idf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/external/tf_idf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/gene_score.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.055743 scCellFie-0.1.5/sccellfie/io/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/io/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/io/save_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.055743 scCellFie-0.1.5/sccellfie/io/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/io/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/io/tests/test_load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/io/tests/test_save_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/metabolic_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.055743 scCellFie-0.1.5/sccellfie/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/preprocessing/prepare_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.059743 scCellFie-0.1.5/sccellfie/preprocessing/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/preprocessing/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/preprocessing/tests/test_prepare_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6938 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/reaction_activity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.059743 scCellFie-0.1.5/sccellfie/spatial/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/spatial/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/spatial/assortativity.py
--rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/spatial/hotspots.py
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/spatial/knn_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.059743 scCellFie-0.1.5/sccellfie/spatial/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/spatial/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/spatial/tests/test_assortativity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/spatial/tests/test_hotspots.py
--rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/spatial/tests/test_knn_network.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.059743 scCellFie-0.1.5/sccellfie/stats/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/stats/markers_from_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.059743 scCellFie-0.1.5/sccellfie/stats/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/stats/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/stats/tests/test_markers_from_task.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:17.059743 scCellFie-0.1.5/sccellfie/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/tests/test_gene_score.py
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/tests/test_metabolic_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4572 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/tests/test_reaction_activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-03-07 14:10:09.000000 scCellFie-0.1.5/sccellfie/tests/toy_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 14:10:17.063743 scCellFie-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-03-07 14:10:09.000000 scCellFie-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.964008 scCellFie-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-04-02 13:52:01.000000 scCellFie-0.1.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-02 13:52:05.960008 scCellFie-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2490 2024-04-02 13:52:01.000000 scCellFie-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/scCellFie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-04-02 13:52:05.000000 scCellFie-0.1.6/scCellFie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-02 13:52:05.000000 scCellFie-0.1.6/scCellFie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 13:52:05.000000 scCellFie-0.1.6/scCellFie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 13:52:05.000000 scCellFie-0.1.6/scCellFie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-02 13:52:05.000000 scCellFie-0.1.6/scCellFie.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/expression/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/expression/aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/expression/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/expression/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/expression/tests/test_aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13213 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/expression/tests/test_threshold.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9981 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/expression/thresholds.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/external/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/external/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/external/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/external/tests/test_tf_idf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5360 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/external/tf_idf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/gene_score.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4051 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/io/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/io/save_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/io/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/io/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/io/tests/test_load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/io/tests/test_save_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/metabolic_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.956008 scCellFie-0.1.6/sccellfie/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3762 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/preprocessing/prepare_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/sccellfie/preprocessing/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/preprocessing/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/preprocessing/tests/test_prepare_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/reaction_activity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/sccellfie/spatial/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/assortativity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/hotspots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/knn_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/sccellfie/spatial/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/tests/test_assortativity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/tests/test_hotspots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3222 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/spatial/tests/test_knn_network.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/sccellfie/stats/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/stats/markers_from_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/sccellfie/stats/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/stats/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4211 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/stats/tests/test_markers_from_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 13:52:05.960008 scCellFie-0.1.6/sccellfie/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/tests/test_gene_score.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/tests/test_metabolic_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/tests/test_reaction_activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-04-02 13:52:01.000000 scCellFie-0.1.6/sccellfie/tests/toy_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 13:52:05.964008 scCellFie-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-02 13:52:01.000000 scCellFie-0.1.6/setup.py
```

### Comparing `scCellFie-0.1.5/LICENSE.txt` & `scCellFie-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/PKG-INFO` & `scCellFie-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scCellFie
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool for studying metabolic tasks from single-cell and spatial transcriptomics
 Home-page: https://github.com/earmingol/scCellFie
 Author: Erick Armingol
 Author-email: erickarmingol@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scCellFie-0.1.5/README.md` & `scCellFie-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/scCellFie.egg-info/PKG-INFO` & `scCellFie-0.1.6/scCellFie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scCellFie
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool for studying metabolic tasks from single-cell and spatial transcriptomics
 Home-page: https://github.com/earmingol/scCellFie
 Author: Erick Armingol
 Author-email: erickarmingol@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `scCellFie-0.1.5/scCellFie.egg-info/SOURCES.txt` & `scCellFie-0.1.6/scCellFie.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/expression/aggregation.py` & `scCellFie-0.1.6/sccellfie/expression/aggregation.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/expression/tests/test_aggregation.py` & `scCellFie-0.1.6/sccellfie/expression/tests/test_aggregation.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/expression/tests/test_threshold.py` & `scCellFie-0.1.6/sccellfie/expression/tests/test_threshold.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/expression/thresholds.py` & `scCellFie-0.1.6/sccellfie/expression/thresholds.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/external/tests/test_tf_idf.py` & `scCellFie-0.1.6/sccellfie/external/tests/test_tf_idf.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/external/tf_idf.py` & `scCellFie-0.1.6/sccellfie/external/tf_idf.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/gene_score.py` & `scCellFie-0.1.6/sccellfie/gene_score.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import ast
 import cobra
 import numpy as np
 
 from scipy.sparse import issparse
+from sccellfie.tests import PCOUNT
 
 
 def gene_score(gene_expression, gene_threshold):
     '''
     Computes the gene score for a given gene expression and threshold.
 
     Parameters
@@ -22,15 +23,15 @@
     gene_scores: float numpy.ndarray
         A float or a numpy array containing the gene scores.
 
     Notes
     -----
     This score is computed as previously indicated in the CellFie paper (https://doi.org/10.1016/j.cels.2019.05.012).
     '''
-    return 5*np.log(1 + gene_expression/(gene_threshold+0.01)) # Added small value to threshold to avoid division by zero
+    return 5*np.log(1 + gene_expression/(gene_threshold + PCOUNT)) # Added small value to threshold to avoid division by zero
 
 
 def compute_gene_scores(adata, thresholds, use_raw=False, layer='gene_scores'):
     '''
     Computes the gene scores from CellFie for each gene in an AnnData object given
     specific threshold values.
```

### Comparing `scCellFie-0.1.5/sccellfie/io/load_data.py` & `scCellFie-0.1.6/sccellfie/io/load_data.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/io/save_data.py` & `scCellFie-0.1.6/sccellfie/io/save_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
         The AnnData object is saved to folder/filename.h5ad.
         The scCellFie attributes are saved to:
             - reactions: folder/filename_reactions.h5ad.
             - metabolic_tasks: folder/filename_metabolic_tasks.h5ad.
     '''
     # Check folder path
     Path(folder).mkdir(parents=True, exist_ok=True)
-
     if spatial_network_key in adata.uns.keys():
         if isinstance(adata.uns[spatial_network_key]['graph'], nx.Graph):
             adata.uns[spatial_network_key]['graph'] = nx.to_pandas_adjacency(adata.uns[spatial_network_key]['graph'])
             warn = f"adata.uns['{spatial_network_key}']['graph'] was converted from a networkx.Graph object to a pandas adjacency matrix to be saved with the AnnData object."
             warnings.warn(warn)
 
     adata_filename = f'{folder}/{filename}.h5ad'
```

### Comparing `scCellFie-0.1.5/sccellfie/io/tests/test_load_data.py` & `scCellFie-0.1.6/sccellfie/io/tests/test_load_data.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/io/tests/test_save_data.py` & `scCellFie-0.1.6/sccellfie/io/tests/test_save_data.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/metabolic_task.py` & `scCellFie-0.1.6/sccellfie/metabolic_task.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import numpy as np
 import scanpy as sc
 
-def compute_mt_score(adata, task_by_rxn):
+def compute_mt_score(adata, task_by_rxn, verbose=True):
     '''
     Computes the metabolic task score for each cell in an AnnData object given
     specific reaction activity levels.
 
     Parameters
     ----------
     adata: AnnData object
         Annotated data matrix.
 
     task_by_rxn: pandas.DataFrame
         A pandas.DataFrame object where rows are metabolic tasks and columns are
         reactions. Each cell contains ones or zeros, indicating whether a reaction
         is involved in a metabolic task.
 
+    verbose: bool, optional (default: True)
+        Whether to print information about the analysis.
+
     Returns
     -------
     None
         An AnnData object is added to the adata object in adata.metabolic_tasks. This object
         contains the metabolic task scores for each cell in adata.obs_names. Here,
         each metabolic task is an element of var_name in adata.metabolic_tasks. The metabolic task scores
         are stored in adata.metabolic_tasks.X.
@@ -55,15 +58,16 @@
     mts = mts.divide(rxns_per_task).fillna(0.0)
 
     # Remove tasks with zeros across cells
     old_cols = set(mts.columns)
     mts = mts.loc[:, (mts != 0).any(axis=0)]
     new_cols = set(mts.columns)
     removed_cols = old_cols.difference(new_cols)
-    print(f"Removed {len(removed_cols)} metabolic tasks with zeros across all cells.")
+    if verbose:
+        print(f"Removed {len(removed_cols)} metabolic tasks with zeros across all cells.")
 
     # Prepare output
     drop_cols = [col for col in mts.columns if col in adata.obs.columns]
     adata.metabolic_tasks = sc.AnnData(mts,
                                        obs=adata.obs.drop(columns=drop_cols).copy(),
                                        obsm=adata.obsm.copy(),
                                        obsp=adata.obsp.copy(),
```

### Comparing `scCellFie-0.1.5/sccellfie/preprocessing/prepare_inputs.py` & `scCellFie-0.1.6/sccellfie/preprocessing/prepare_inputs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-
+import cobra
 
 
 def preprocess_inputs(adata, gpr_info, task_by_gene, rxn_by_gene, task_by_rxn, verbose=True):
     '''
     Preprocess inputs for sccellfie.
 
     Parameters
@@ -34,14 +34,16 @@
     Returns
     -------
     adata2: AnnData object
         Annotated data matrix with only genes present in task_by_gene, rxn_by_gene, and adata.var_names.
 
     gpr_rules: dict
         A dictionary with reaction IDs as keys and Gene-Protein Rules (GPRs) as values.
+        GPRs are in the format of the ast library after initialization with cobra from strings
+        to tree format for AND and OR rules.
 
     task_by_gene: pandas.DataFrame
         A pandas.DataFrame object where rows are metabolic tasks and columns are
         genes. Each cell contains ones or zeros, indicating whether a gene
         is involved in a metabolic task.
 
     rxn_by_gene: pandas.DataFrame
@@ -60,15 +62,18 @@
 
     task_by_gene = task_by_gene.loc[:, genes]
     task_by_gene = task_by_gene.loc[(task_by_gene != 0).any(axis=1)]
 
     rxn_by_gene = rxn_by_gene.loc[:, genes]
     rxn_by_gene = rxn_by_gene.loc[(rxn_by_gene != 0).any(axis=1)]
 
-    gpr_rules = {k: v for k, v in gpr_rules.items() if k in rxn_by_gene.index.tolist()}
+    gpr_rules = {k: v.replace(' AND ', ' and ').replace(' OR ', ' or ') for k, v in gpr_rules.items() if k in rxn_by_gene.index.tolist()}
+
+    # Initialize GPRs
+    gpr_rules = {k: cobra.core.gene.GPR().from_string(gpr) for k, gpr in gpr_rules.items()}
 
     tasks = task_by_gene.index.tolist()
     rxns = list(gpr_rules.keys())
 
     task_by_rxn = task_by_rxn.loc[tasks, rxns]
     task_by_rxn = task_by_rxn.loc[(task_by_rxn != 0).any(axis=1)]
```

### Comparing `scCellFie-0.1.5/sccellfie/preprocessing/tests/test_prepare_inputs.py` & `scCellFie-0.1.6/sccellfie/preprocessing/tests/test_prepare_inputs.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from sccellfie.tests.toy_inputs import create_random_adata, create_controlled_adata, create_controlled_gpr_dict, create_controlled_task_by_rxn, create_controlled_task_by_gene, create_controlled_rxn_by_gene
 
 
 def test_preprocess_inputs():
     # Create controlled inputs
     adata = create_controlled_adata()
     gpr_dict_expected = create_controlled_gpr_dict()
-    gpr_info = pd.DataFrame.from_dict(gpr_dict_expected, orient='index').reset_index()
+    str_gpr_dict_expected = {k : v._ast2str(v) for k, v in gpr_dict_expected.items()}
+    gpr_info = pd.DataFrame.from_dict(str_gpr_dict_expected, orient='index').reset_index()
     gpr_info.columns = ['Reaction', 'GPR-symbol']
     task_by_gene = create_controlled_task_by_gene()
     rxn_by_gene = create_controlled_rxn_by_gene()
     task_by_rxn = create_controlled_task_by_rxn()
 
     # Preprocess inputs
     adata2, gpr_rules, task_by_gene2, rxn_by_gene2, task_by_rxn2 = preprocess_inputs(adata, gpr_info, task_by_gene, rxn_by_gene, task_by_rxn)
@@ -25,15 +26,16 @@
 
 
 def test_shapes():
     # Create controlled inputs
     adata_controlled = create_controlled_adata()
     adata_random = create_random_adata(n_obs=10, n_vars=3)
     gpr_dict_expected = create_controlled_gpr_dict()
-    gpr_info = pd.DataFrame.from_dict(gpr_dict_expected, orient='index').reset_index()
+    str_gpr_dict_expected = {k: v._ast2str(v) for k, v in gpr_dict_expected.items()}
+    gpr_info = pd.DataFrame.from_dict(str_gpr_dict_expected, orient='index').reset_index()
     gpr_info.columns = ['Reaction', 'GPR-symbol']
     task_by_gene = create_controlled_task_by_gene()
     rxn_by_gene = create_controlled_rxn_by_gene()
     task_by_rxn = create_controlled_task_by_rxn()
 
     # Remove one gene from adata_random that is in the controlled inputs
     adata = adata_random[:, adata_random.var_names[1:]]
```

### Comparing `scCellFie-0.1.5/sccellfie/reaction_activity.py` & `scCellFie-0.1.6/sccellfie/reaction_activity.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     Parameters
     ----------
     adata: AnnData object
         Annotated data matrix.
 
     gpr_dict: dict
         A dictionary with reaction IDs as keys and Gene-Protein Rules (GPRs) as values.
+        GPRs are in the format of the ast library after initialization with cobra from strings
+        to tree format for AND and OR rules.
 
     use_specificity: bool, optional (default: True)
         Whether to use the specificity of the determinant gene to compute reaction
         activity levels. The specificity is the inverse of the number of reactions
         that the determinant gene is involved in.
 
     layer: str, optional (default: 'gene_scores')
@@ -52,31 +54,28 @@
     This score is computed as previously indicated in the CellFie paper (https://doi.org/10.1016/j.crmeth.2021.100040).
     '''
     genes = adata.var_names
     gene_scores = adata.layers[layer]
     rxns = gpr_dict.keys()
     ral = np.zeros((gene_scores.shape[0], len(rxns)))
 
-    # Initialize GPRs
-    gpr_cobra_dict = {k : cobra.core.gene.GPR().from_string(gpr) for k, gpr in gpr_dict.items()}
-
     # This could be optimized by paralellization, returning multiple vectors (one per cell)
     # And concatenating them later.
     rxn_max_genes = []
-    for i in tqdm(range(gene_scores.shape[0]), disable=disable_pbar): # Iterate through single cells
+    for i in tqdm(range(gene_scores.shape[0]), disable=disable_pbar, desc='Cell Rxn Activities', leave=False): # Iterate through single cells
         max_gene_vector = []
         scores = defaultdict(float)
         scores.update({name: value for name, value in zip(genes, gene_scores[i, :])})
 
         # For accounting for specificity
         selected_gene = defaultdict(float)
         rxn_ids_gene = defaultdict(list)
 
         for j, k in enumerate(rxns):
-            gpr = gpr_cobra_dict[k]
+            gpr = gpr_dict[k]
             score, gene = compute_gpr_gene_score(gpr, scores)
             ral[i, j] = score
             selected_gene[gene] += 1
             rxn_ids_gene[gene].append(j)
             max_gene_vector.append(gene)
 
         rxn_max_genes.append(max_gene_vector)
```

### Comparing `scCellFie-0.1.5/sccellfie/spatial/assortativity.py` & `scCellFie-0.1.6/sccellfie/spatial/assortativity.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
     assortativity: float
         The assortativity of the variable in the spatial network.
     '''
     if spatial_network_key not in adata.uns.keys():
         raise ValueError(f'{spatial_network_key} not found in adata.uns. Run sccellfie.spatial.knn_network.create_knn_network() first.')
     H = adata.uns[spatial_network_key]['graph'].copy()
 
+    if isinstance(H, pd.DataFrame):
+        H = nx.from_pandas_adjacency(H)
+
     if use_raw:
         X = adata.raw.X
     else:
         X = adata.X
 
     if issparse(X):
         X = X.toarray()
```

### Comparing `scCellFie-0.1.5/sccellfie/spatial/hotspots.py` & `scCellFie-0.1.6/sccellfie/spatial/hotspots.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/spatial/knn_network.py` & `scCellFie-0.1.6/sccellfie/spatial/knn_network.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/spatial/tests/test_assortativity.py` & `scCellFie-0.1.6/sccellfie/spatial/tests/test_assortativity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+import networkx as nx
 import pandas as pd
 
 from sccellfie.spatial.assortativity import compute_var_assortativity, compute_assortativity
 from sccellfie.spatial.knn_network import create_knn_network
 from sccellfie.tests.toy_inputs import create_random_adata_with_spatial
 
 
@@ -10,14 +11,22 @@
 def test_compute_var_assortativity(use_raw):
     adata = create_random_adata_with_spatial(spatial_key='X_spatial')
     create_knn_network(adata, n_neighbors=2, spatial_key='X_spatial')
     assortativity = compute_var_assortativity(adata, var_name='gene1', use_raw=use_raw)
     assert isinstance(assortativity, float), "Output is not a float"
 
 
+def test_compute_var_assortativity_pandas_graph():
+    adata = create_random_adata_with_spatial(spatial_key='X_spatial')
+    create_knn_network(adata, n_neighbors=2, spatial_key='X_spatial')
+    adata.uns['spatial_network']['graph'] = nx.to_pandas_adjacency(adata.uns['spatial_network']['graph'])
+    assortativity = compute_var_assortativity(adata, var_name='gene1')
+    assert isinstance(assortativity, float), "Output is not a float"
+
+
 def test_compute_var_assortativity_fail():
     adata = create_random_adata_with_spatial(spatial_key='X_spatial')
     with pytest.raises(ValueError):
         compute_var_assortativity(adata, var_name='gene1', use_raw=False)
 
 
 def test_compute_assortativity():
```

### Comparing `scCellFie-0.1.5/sccellfie/spatial/tests/test_hotspots.py` & `scCellFie-0.1.6/sccellfie/spatial/tests/test_hotspots.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/spatial/tests/test_knn_network.py` & `scCellFie-0.1.6/sccellfie/spatial/tests/test_knn_network.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/stats/markers_from_task.py` & `scCellFie-0.1.6/sccellfie/stats/markers_from_task.py`

 * *Files identical despite different names*

### Comparing `scCellFie-0.1.5/sccellfie/stats/tests/test_markers_from_task.py` & `scCellFie-0.1.6/sccellfie/stats/tests/test_markers_from_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,20 +51,20 @@
                                            min_activity=min_activity)
 
     # Expected determinant genes
     if groupby is None:
         expected_df = pd.DataFrame(data={'Group': ['All-Groups', 'All-Groups', 'All-Groups'],
                                          'Rxn': ['rxn3', 'rxn3', 'rxn1'],
                                          'Det-Gene': ['gene2', 'gene3', 'gene1'],
-                                         'RAL': [2.740987, 2.676485, 2.585926]})
+                                         'RAL': [2.746531, 2.682397, 2.591538]})
     else:
         expected_df = pd.DataFrame(data={'Group': ['B', 'B', 'B', 'A', 'A'],
                                         'Rxn': ['rxn3', 'rxn1', 'rxn3', 'rxn3', 'rxn1'],
                                         'Det-Gene': ['gene3', 'gene1', 'gene2', 'gene3', 'gene1'],
-                                        'RAL': [5.481975, 3.948932, 2.740987, 1.273740, 1.22920]})
+                                        'RAL': [5.493061, 3.957039, 2.746531, 1.277064, 1.226037]})
         if group is not None:
             if isinstance(group, list):
                 groups = group
             else:
                 groups = [group]
             expected_df = expected_df[expected_df['Group'].isin(groups)].reset_index(drop=True)
     expected_df = expected_df[expected_df['RAL'] >= min_activity].reset_index(drop=True)
```

### Comparing `scCellFie-0.1.5/sccellfie/tests/test_gene_score.py` & `scCellFie-0.1.6/sccellfie/tests/test_gene_score.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 import numpy as np
 import pandas as pd
 
 from cobra.core.gene import GPR
 from scipy.sparse import issparse
 
 from sccellfie.gene_score import gene_score, compute_gene_scores, compute_gpr_gene_score
+from sccellfie.tests import PCOUNT
 from sccellfie.tests.toy_inputs import create_controlled_adata
 
 
 def test_gene_score():
     # Test data
     gene_expression = np.array([1, 2, 3])
     gene_threshold = np.array([0.1, 0.2, 0.3])
 
     # Expected results
-    expected_scores = 5 * np.log(1 + gene_expression / (gene_threshold + 0.01))
+    expected_scores = 5 * np.log(1 + gene_expression / (gene_threshold + PCOUNT))
 
     # Actual results
     actual_scores = gene_score(gene_expression, gene_threshold)
 
     # Assert equality
     np.testing.assert_allclose(actual_scores, expected_scores, rtol=1e-5)
 
@@ -37,15 +38,15 @@
     if issparse(X):
         X = X.toarray()
 
     # Define known thresholds
     thresholds = pd.DataFrame({'gene_threshold': [0.5, 3, 5]}, index=['gene1', 'gene2', 'gene3'])
 
     # Expected gene scores based on the defined formula
-    expected_scores = 5 * np.log(1 + X / (thresholds.values.T + 0.01))
+    expected_scores = 5 * np.log(1 + X / (thresholds.values.T + PCOUNT))
 
     # Compute gene scores using the function
     compute_gene_scores(adata, thresholds, use_raw=use_raw)
 
     # Retrieve the computed gene scores from adata
     computed_scores = adata.layers['gene_scores']
```

### Comparing `scCellFie-0.1.5/sccellfie/tests/test_metabolic_task.py` & `scCellFie-0.1.6/sccellfie/tests/test_metabolic_task.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 import numpy as np
 
 from sccellfie.gene_score import compute_gene_scores
 from sccellfie.reaction_activity import compute_reaction_activity
 from sccellfie.metabolic_task import compute_mt_score
+from sccellfie.tests import PCOUNT
 from sccellfie.tests.toy_inputs import create_controlled_adata, create_controlled_gpr_dict, create_global_threshold, create_controlled_task_by_rxn
 
 
 @pytest.mark.parametrize("use_specificity", [True, False])
 def test_compute_mt_score(use_specificity):
     # Create a small, controlled AnnData object, GPR dictionary, and a task_by_rxn DataFrame
     adata = create_controlled_adata()
@@ -30,34 +31,33 @@
     compute_mt_score(adata, task_by_rxn)
 
     # Compute the expected MTS
     if use_specificity:
         denom = 2
     else:
         denom = 1
-    pcount = 0.01  # Pseudocount used in function sccellfie.gene_score.gene_score()
-    expected_ral = np.array([[5 * np.log(1 + 1 / (threshold_val + pcount)) / denom,  # Cell1, Rxn1
-                              5 * np.log(1 + 2 / (threshold_val + pcount)),  # Cell1, Rxn2
-                              5 * np.log(1 + 0 / (threshold_val + pcount)),  # Cell1, Rxn3
-                              5 * np.log(1 + 1 / (threshold_val + pcount)) / denom,  # Cell1, Rxn4
+    expected_ral = np.array([[5 * np.log(1 + 1 / (threshold_val + PCOUNT)) / denom,  # Cell1, Rxn1
+                              5 * np.log(1 + 2 / (threshold_val + PCOUNT)),  # Cell1, Rxn2
+                              5 * np.log(1 + 0 / (threshold_val + PCOUNT)),  # Cell1, Rxn3
+                              5 * np.log(1 + 1 / (threshold_val + PCOUNT)) / denom,  # Cell1, Rxn4
                               ],
-                             [5 * np.log(1 + 3 / (threshold_val + pcount)) / denom,  # Cell2, Rxn1
-                              5 * np.log(1 + 4 / (threshold_val + pcount)),  # Cell2, Rxn2
-                              5 * np.log(1 + 2 / (threshold_val + pcount)),  # Cell2, Rxn3
-                              5 * np.log(1 + 3 / (threshold_val + pcount)) / denom,  # Cell2, Rxn4
+                             [5 * np.log(1 + 3 / (threshold_val + PCOUNT)) / denom,  # Cell2, Rxn1
+                              5 * np.log(1 + 4 / (threshold_val + PCOUNT)),  # Cell2, Rxn2
+                              5 * np.log(1 + 2 / (threshold_val + PCOUNT)),  # Cell2, Rxn3
+                              5 * np.log(1 + 3 / (threshold_val + PCOUNT)) / denom,  # Cell2, Rxn4
                               ],
-                             [5 * np.log(1 + 5 / (threshold_val + pcount)),  # Cell3, Rxn1
-                              5 * np.log(1 + 6 / (threshold_val + pcount)) / denom,  # Cell3, Rxn2
-                              5 * np.log(1 + 6 / (threshold_val + pcount)) / denom,  # Cell3, Rxn3
-                              5 * np.log(1 + 10 / (threshold_val + pcount)),  # Cell3, Rxn4
+                             [5 * np.log(1 + 5 / (threshold_val + PCOUNT)),  # Cell3, Rxn1
+                              5 * np.log(1 + 6 / (threshold_val + PCOUNT)) / denom,  # Cell3, Rxn2
+                              5 * np.log(1 + 6 / (threshold_val + PCOUNT)) / denom,  # Cell3, Rxn3
+                              5 * np.log(1 + 10 / (threshold_val + PCOUNT)),  # Cell3, Rxn4
                               ],
-                             [5 * np.log(1 + 7 / (threshold_val + pcount)) / denom,  # Cell4, Rxn1
-                              5 * np.log(1 + 8 / (threshold_val + pcount)),  # Cell4, Rxn2
-                              5 * np.log(1 + 6 / (threshold_val + pcount)),  # Cell4, Rxn3
-                              5 * np.log(1 + 7 / (threshold_val + pcount)) / denom,  # Cell4, Rxn4
+                             [5 * np.log(1 + 7 / (threshold_val + PCOUNT)) / denom,  # Cell4, Rxn1
+                              5 * np.log(1 + 8 / (threshold_val + PCOUNT)),  # Cell4, Rxn2
+                              5 * np.log(1 + 6 / (threshold_val + PCOUNT)),  # Cell4, Rxn3
+                              5 * np.log(1 + 7 / (threshold_val + PCOUNT)) / denom,  # Cell4, Rxn4
                               ],
                              ])
     expected_mts = np.matmul(expected_ral, task_by_rxn.T) / task_by_rxn.sum(axis=1)
 
     # Verify the values of metabolic task scores
     assert hasattr(adata, 'metabolic_tasks')
     np.testing.assert_almost_equal(adata.metabolic_tasks.X, expected_mts, decimal=5)
```

### Comparing `scCellFie-0.1.5/sccellfie/tests/test_reaction_activity.py` & `scCellFie-0.1.6/sccellfie/tests/test_reaction_activity.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
 import numpy as np
 import pandas as pd
 
 from sccellfie.gene_score import compute_gene_scores
 from sccellfie.reaction_activity import compute_reaction_activity
+from sccellfie.tests import PCOUNT
 from sccellfie.tests.toy_inputs import create_controlled_adata, create_controlled_gpr_dict, create_global_threshold
 
 
 @pytest.mark.parametrize("use_specificity", [True, False])
 def test_compute_reaction_activity(use_specificity):
     # Create a small, controlled AnnData object
     adata = create_controlled_adata()
@@ -28,34 +29,33 @@
                               disable_pbar=True)
 
     # Expected reaction activity
     if use_specificity:
         denom = 2
     else:
         denom = 1
-    pcount = 0.01 # Pseudocount used in function sccellfie.gene_score.gene_score()
-    expected_ral = np.array([[5 * np.log(1 + 1 / (threshold_val + pcount)) / denom, # Cell1, Rxn1
-                              5 * np.log(1 + 2 / (threshold_val + pcount)), # Cell1, Rxn2
-                              5 * np.log(1 + 0 / (threshold_val + pcount)), # Cell1, Rxn3
-                              5 * np.log(1 + 1 / (threshold_val + pcount)) / denom, # Cell1, Rxn4
+    expected_ral = np.array([[5 * np.log(1 + 1 / (threshold_val + PCOUNT)) / denom, # Cell1, Rxn1
+                              5 * np.log(1 + 2 / (threshold_val + PCOUNT)), # Cell1, Rxn2
+                              5 * np.log(1 + 0 / (threshold_val + PCOUNT)), # Cell1, Rxn3
+                              5 * np.log(1 + 1 / (threshold_val + PCOUNT)) / denom, # Cell1, Rxn4
                               ],
-                             [5 * np.log(1 + 3 / (threshold_val + pcount)) / denom, # Cell2, Rxn1
-                              5 * np.log(1 + 4 / (threshold_val + pcount)), # Cell2, Rxn2
-                              5 * np.log(1 + 2 / (threshold_val + pcount)), # Cell2, Rxn3
-                              5 * np.log(1 + 3 / (threshold_val + pcount)) / denom, # Cell2, Rxn4
+                             [5 * np.log(1 + 3 / (threshold_val + PCOUNT)) / denom, # Cell2, Rxn1
+                              5 * np.log(1 + 4 / (threshold_val + PCOUNT)), # Cell2, Rxn2
+                              5 * np.log(1 + 2 / (threshold_val + PCOUNT)), # Cell2, Rxn3
+                              5 * np.log(1 + 3 / (threshold_val + PCOUNT)) / denom, # Cell2, Rxn4
                               ],
-                             [5 * np.log(1 + 5 / (threshold_val + pcount)), # Cell3, Rxn1
-                              5 * np.log(1 + 6 / (threshold_val + pcount)) / denom, # Cell3, Rxn2
-                              5 * np.log(1 + 6 / (threshold_val + pcount)) / denom, # Cell3, Rxn3
-                              5 * np.log(1 + 10 / (threshold_val + pcount)), # Cell3, Rxn4
+                             [5 * np.log(1 + 5 / (threshold_val + PCOUNT)), # Cell3, Rxn1
+                              5 * np.log(1 + 6 / (threshold_val + PCOUNT)) / denom, # Cell3, Rxn2
+                              5 * np.log(1 + 6 / (threshold_val + PCOUNT)) / denom, # Cell3, Rxn3
+                              5 * np.log(1 + 10 / (threshold_val + PCOUNT)), # Cell3, Rxn4
                               ],
-                             [5 * np.log(1 + 7 / (threshold_val + pcount)) / denom, # Cell4, Rxn1
-                              5 * np.log(1 + 8 / (threshold_val + pcount)), # Cell4, Rxn2
-                              5 * np.log(1 + 6 / (threshold_val + pcount)), # Cell4, Rxn3
-                              5 * np.log(1 + 7 / (threshold_val + pcount)) / denom, # Cell4, Rxn4
+                             [5 * np.log(1 + 7 / (threshold_val + PCOUNT)) / denom, # Cell4, Rxn1
+                              5 * np.log(1 + 8 / (threshold_val + PCOUNT)), # Cell4, Rxn2
+                              5 * np.log(1 + 6 / (threshold_val + PCOUNT)), # Cell4, Rxn3
+                              5 * np.log(1 + 7 / (threshold_val + PCOUNT)) / denom, # Cell4, Rxn4
                               ],
                              ])
 
     # Verify the structure and values of reaction activity data
     assert hasattr(adata, 'reactions')
     np.testing.assert_almost_equal(adata.reactions.X, expected_ral, decimal=5)
```

### Comparing `scCellFie-0.1.5/sccellfie/tests/toy_inputs.py` & `scCellFie-0.1.6/sccellfie/tests/toy_inputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import cobra
 import numpy as np
 import pandas as pd
 
 import scanpy as sc
 from scipy import sparse
 
 
@@ -80,14 +81,17 @@
 
 def create_controlled_gpr_dict():
     gpr_dict = {'rxn1': 'gene1',
                 'rxn2': 'gene2',
                 'rxn3': 'gene2 and gene3',
                 'rxn4': 'gene1 or gene3'
                 }
+
+    # Initialize GPRs
+    gpr_dict = {k: cobra.core.gene.GPR().from_string(gpr) for k, gpr in gpr_dict.items()}
     return gpr_dict
 
 
 def create_controlled_task_by_rxn():
     task_by_rxn = pd.DataFrame(data=[[1, 0, 1, 0],
                                      [0, 1, 0, 1],
                                      [1, 0, 0, 0],
```

### Comparing `scCellFie-0.1.5/setup.py` & `scCellFie-0.1.6/setup.py`

 * *Files identical despite different names*

