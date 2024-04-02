# Comparing `tmp/RL_OM-0.7.80.tar.gz` & `tmp/RL_OM-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.7.80.tar", last modified: Mon Apr  1 10:16:34 2024, max compression
+gzip compressed data, was "RL_OM-0.7.9.tar", last modified: Wed Mar  6 06:13:50 2024, max compression
```

## Comparing `RL_OM-0.7.80.tar` & `RL_OM-0.7.9.tar`

### file list

```diff
@@ -1,85 +1,79 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.580789 RL_OM-0.7.80/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.7.80/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.7.80/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-04-01 10:16:34.580619 RL_OM-0.7.80/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.7.80/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.570540 RL_OM-0.7.80/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)     1284 2024-03-23 05:21:04.000000 RL_OM-0.7.80/RL_OM/MLtools.py
--rw-r--r--   0 magnus     (501) staff       (20)       23 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)   231218 2024-03-21 02:54:55.000000 RL_OM-0.7.80/RL_OM/_modidx 2.py
--rw-r--r--   0 magnus     (501) staff       (20)   240779 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.571935 RL_OM-0.7.80/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.573854 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     1707 2023-12-01 14:08:43.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/PPO_SB3.py
--rw-r--r--   0 magnus     (501) staff       (20)      468 2023-12-01 14:08:43.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/PPO_TEMP.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6605 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/cbs.py
--rw-r--r--   0 magnus     (501) staff       (20)     6389 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/eoq.py
--rw-r--r--   0 magnus     (501) staff       (20)     8752 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/mp_agents_ERM.py
--rw-r--r--   0 magnus     (501) staff       (20)     2355 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/nv_agents.py
--rw-r--r--   0 magnus     (501) staff       (20)    62375 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/nv_agents_ERM.py
--rw-r--r--   0 magnus     (501) staff       (20)     9918 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/nv_agents_SAA.py
--rw-r--r--   0 magnus     (501) staff       (20)     9350 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py
--rw-r--r--   0 magnus     (501) staff       (20)    23263 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/qr.py
--rw-r--r--   0 magnus     (501) staff       (20)    14565 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/saa.py
--rw-r--r--   0 magnus     (501) staff       (20)    13815 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/benchmark_agents/ss.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.574412 RL_OM-0.7.80/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6890 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1369 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     9657 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.574807 RL_OM-0.7.80/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1162 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/processors/eoq_preprocessors.py
--rw-r--r--   0 magnus     (501) staff       (20)     6401 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.575673 RL_OM-0.7.80/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.576579 RL_OM-0.7.80/RL_OM/agents/rl_agents/algorithms/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/algorithms/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14243 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13708 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19176 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19614 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19118 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.578330 RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     3234 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)    12009 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py
--rw-r--r--   0 magnus     (501) staff       (20)     4995 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)     5053 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)     5269 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    16656 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)     5082 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
--rw-r--r--   0 magnus     (501) staff       (20)     4875 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.7.80/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.579282 RL_OM-0.7.80/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    16571 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)     6137 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/environments/data_generators.py
--rw-r--r--   0 magnus     (501) staff       (20)     2575 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/environments/feature_converters.py
--rw-r--r--   0 magnus     (501) staff       (20)    42643 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.579849 RL_OM-0.7.80/RL_OM/experiment_functions/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/experiment_functions/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    32862 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/experiment_functions/run_experiment.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.580359 RL_OM-0.7.80/RL_OM/utils/
--rw-r--r--   0 magnus     (501) staff       (20)     1259 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/utils/MLtools.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/utils/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    10828 2024-04-01 10:16:24.000000 RL_OM-0.7.80/RL_OM/utils/utils.py
--rw-r--r--   0 magnus     (501) staff       (20)    10817 2024-03-23 04:58:03.000000 RL_OM-0.7.80/RL_OM/utils.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-04-01 10:16:34.571789 RL_OM-0.7.80/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1087 2024-04-01 10:16:34.000000 RL_OM-0.7.80/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     2613 2024-04-01 10:16:34.000000 RL_OM-0.7.80/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2024-04-01 10:16:34.000000 RL_OM-0.7.80/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2024-04-01 10:16:34.000000 RL_OM-0.7.80/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.7.80/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2024-04-01 10:16:34.000000 RL_OM-0.7.80/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2024-04-01 10:16:34.000000 RL_OM-0.7.80/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      990 2024-04-01 10:16:32.000000 RL_OM-0.7.80/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2024-04-01 10:16:34.580834 RL_OM-0.7.80/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.7.80/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.762518 RL_OM-0.7.9/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.7.9/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.7.9/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2024-03-06 06:13:50.762386 RL_OM-0.7.9/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.7.9/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.752945 RL_OM-0.7.9/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)       22 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)   210138 2024-02-28 03:50:17.000000 RL_OM-0.7.9/RL_OM/_modidx 2.py
+-rw-r--r--   0 magnus     (501) staff       (20)   226125 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.754226 RL_OM-0.7.9/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.755989 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     1707 2023-12-01 14:08:43.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/PPO_SB3.py
+-rw-r--r--   0 magnus     (501) staff       (20)      468 2023-12-01 14:08:43.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/PPO_TEMP.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6605 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/cbs.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6387 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/eoq.py
+-rw-r--r--   0 magnus     (501) staff       (20)     8752 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/mp_agents_ERM.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2355 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/nv_agents.py
+-rw-r--r--   0 magnus     (501) staff       (20)    51907 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/nv_agents_ERM.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9861 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/nv_agents_SAA.py
+-rw-r--r--   0 magnus     (501) staff       (20)    23262 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/qr.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14565 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/saa.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13804 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/benchmark_agents/ss.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.756617 RL_OM-0.7.9/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6544 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1369 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     9696 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.757022 RL_OM-0.7.9/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1141 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/processors/eoq_preprocessors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6362 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.758095 RL_OM-0.7.9/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.759225 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14243 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13708 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19176 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19614 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19118 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.760915 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     3134 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)    12069 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4895 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5053 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5269 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16656 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5082 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4775 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.761772 RL_OM-0.7.9/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13064 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6137 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/environments/data_generators.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2575 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/environments/feature_converters.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16762 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.762149 RL_OM-0.7.9/RL_OM/experiment_functions/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/experiment_functions/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    31373 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/experiment_functions/run_experiment.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10817 2024-03-06 06:13:27.000000 RL_OM-0.7.9/RL_OM/utils.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2024-03-06 06:13:50.754093 RL_OM-0.7.9/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2024-03-06 06:13:50.000000 RL_OM-0.7.9/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     2467 2024-03-06 06:13:50.000000 RL_OM-0.7.9/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2024-03-06 06:13:50.000000 RL_OM-0.7.9/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2024-03-06 06:13:50.000000 RL_OM-0.7.9/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.7.9/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2024-03-06 06:13:50.000000 RL_OM-0.7.9/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2024-03-06 06:13:50.000000 RL_OM-0.7.9/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      989 2024-03-06 06:13:38.000000 RL_OM-0.7.9/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2024-03-06 06:13:50.762561 RL_OM-0.7.9/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.7.9/setup.py
```

### Comparing `RL_OM-0.7.80/LICENSE` & `RL_OM-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/PKG-INFO` & `RL_OM-0.7.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.7.80
+Version: 0.7.9
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.7.80/RL_OM/_modidx 2.py` & `RL_OM-0.7.9/RL_OM/_modidx.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,22 +232,14 @@
                                                                                                                              'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorData.__getitem__': ( 'agents/benchmark_agents/erm_agents.html#newsvendordata.__getitem__',
                                                                                                                                          'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorData.__init__': ( 'agents/benchmark_agents/erm_agents.html#newsvendordata.__init__',
                                                                                                                                       'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorData.__len__': ( 'agents/benchmark_agents/erm_agents.html#newsvendordata.__len__',
                                                                                                                                      'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorDataMeta': ( 'agents/benchmark_agents/erm_agents.html#newsvendordatameta',
-                                                                                                                                 'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorDataMeta.__getitem__': ( 'agents/benchmark_agents/erm_agents.html#newsvendordatameta.__getitem__',
-                                                                                                                                             'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorDataMeta.__init__': ( 'agents/benchmark_agents/erm_agents.html#newsvendordatameta.__init__',
-                                                                                                                                          'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorDataMeta.__len__': ( 'agents/benchmark_agents/erm_agents.html#newsvendordatameta.__len__',
-                                                                                                                                         'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.RMSNorm': ( 'agents/benchmark_agents/erm_agents.html#rmsnorm',
                                                                                                                       'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.RMSNorm.__init__': ( 'agents/benchmark_agents/erm_agents.html#rmsnorm.__init__',
                                                                                                                                'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.RMSNorm.forward': ( 'agents/benchmark_agents/erm_agents.html#rmsnorm.forward',
                                                                                                                               'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNN': ( 'agents/benchmark_agents/erm_agents.html#rnn',
@@ -1149,16 +1141,14 @@
             'RL_OM.core': {'RL_OM.core.foo': ('core.html#foo', 'RL_OM/core.py')},
             'RL_OM.environments.calculation_functions': { 'RL_OM.environments.calculation_functions.eoq_qr_calculations_qr_action': ( 'environments/calculation_functions.html#eoq_qr_calculations_qr_action',
                                                                                                                                       'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.eoq_qr_calculations_single_action': ( 'environments/calculation_functions.html#eoq_qr_calculations_single_action',
                                                                                                                                           'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.get_fixed_ordering_cost': ( 'environments/calculation_functions.html#get_fixed_ordering_cost',
                                                                                                                                 'RL_OM/environments/calculation_functions.py'),
-                                                          'RL_OM.environments.calculation_functions.get_orders_arriving_stochastic': ( 'environments/calculation_functions.html#get_orders_arriving_stochastic',
-                                                                                                                                       'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.mpfc_calculations_ss_action': ( 'environments/calculation_functions.html#mpfc_calculations_ss_action',
                                                                                                                                     'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.normalize_reward_FC': ( 'environments/calculation_functions.html#normalize_reward_fc',
                                                                                                                             'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.normalize_reward_NV': ( 'environments/calculation_functions.html#normalize_reward_nv',
                                                                                                                             'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.nv_calculations': ( 'environments/calculation_functions.html#nv_calculations',
@@ -1188,31 +1178,15 @@
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.reset': ( 'environments/multi_period_inventory.html#multiperiodenv.reset',
                                                                                                                                'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.set_observation_space': ( 'environments/multi_period_inventory.html#multiperiodenv.set_observation_space',
                                                                                                                                                'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.set_observation_state': ( 'environments/multi_period_inventory.html#multiperiodenv.set_observation_state',
                                                                                                                                                'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.step': ( 'environments/multi_period_inventory.html#multiperiodenv.step',
-                                                                                                                              'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP': ( 'environments/multi_period_inventory.html#multiperiodenvmp',
-                                                                                                                           'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.__init__': ( 'environments/multi_period_inventory.html#multiperiodenvmp.__init__',
-                                                                                                                                    'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.convert_to_numpy_array': ( 'environments/multi_period_inventory.html#multiperiodenvmp.convert_to_numpy_array',
-                                                                                                                                                  'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.render': ( 'environments/multi_period_inventory.html#multiperiodenvmp.render',
-                                                                                                                                  'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.reset': ( 'environments/multi_period_inventory.html#multiperiodenvmp.reset',
-                                                                                                                                 'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.set_observation_space': ( 'environments/multi_period_inventory.html#multiperiodenvmp.set_observation_space',
-                                                                                                                                                 'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.set_observation_state': ( 'environments/multi_period_inventory.html#multiperiodenvmp.set_observation_state',
-                                                                                                                                                 'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.step': ( 'environments/multi_period_inventory.html#multiperiodenvmp.step',
-                                                                                                                                'RL_OM/environments/multi_period_inventory.py')},
+                                                                                                                              'RL_OM/environments/multi_period_inventory.py')},
             'RL_OM.experiment_functions.run_experiment': { 'RL_OM.experiment_functions.run_experiment.check_val_test': ( 'experiment_functions/run_experiment.html#check_val_test',
                                                                                                                          'RL_OM/experiment_functions/run_experiment.py'),
                                                            'RL_OM.experiment_functions.run_experiment.experiment_stepwise': ( 'experiment_functions/run_experiment.html#experiment_stepwise',
                                                                                                                               'RL_OM/experiment_functions/run_experiment.py'),
                                                            'RL_OM.experiment_functions.run_experiment.experiment_stepwise_no_log': ( 'experiment_functions/run_experiment.html#experiment_stepwise_no_log',
                                                                                                                                      'RL_OM/experiment_functions/run_experiment.py'),
                                                            'RL_OM.experiment_functions.run_experiment.experiment_wandb': ( 'experiment_functions/run_experiment.html#experiment_wandb',
```

### Comparing `RL_OM-0.7.80/RL_OM/_modidx.py` & `RL_OM-0.7.9/RL_OM/_modidx 2.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/RL_OM',
                 'doc_host': 'https://majoma7.github.io',
                 'git_url': 'https://github.com/majoma7/RL_OM',
                 'lib_path': 'RL_OM'},
-  'syms': { 'RL_OM.MLtools': { 'RL_OM.MLtools.LRSchedulerPerStep': ('utils/ml_tools.html#lrschedulerperstep', 'RL_OM/MLtools.py'),
-                               'RL_OM.MLtools.LRSchedulerPerStep.__init__': ( 'utils/ml_tools.html#lrschedulerperstep.__init__',
-                                                                              'RL_OM/MLtools.py'),
-                               'RL_OM.MLtools.LRSchedulerPerStep.step': ( 'utils/ml_tools.html#lrschedulerperstep.step',
-                                                                          'RL_OM/MLtools.py')},
-            'RL_OM.agents.benchmark_agents.PPO_SB3': { 'RL_OM.agents.benchmark_agents.PPO_SB3.PPOAgent': ( 'agents/benchmark_agents/temp_ppo_sb3.html#ppoagent',
+  'syms': { 'RL_OM.agents.benchmark_agents.PPO_SB3': { 'RL_OM.agents.benchmark_agents.PPO_SB3.PPOAgent': ( 'agents/benchmark_agents/temp_ppo_sb3.html#ppoagent',
                                                                                                            'RL_OM/agents/benchmark_agents/PPO_SB3.py'),
                                                        'RL_OM.agents.benchmark_agents.PPO_SB3.PPOAgent.__init__': ( 'agents/benchmark_agents/temp_ppo_sb3.html#ppoagent.__init__',
                                                                                                                     'RL_OM/agents/benchmark_agents/PPO_SB3.py'),
                                                        'RL_OM.agents.benchmark_agents.PPO_SB3.PPOAgent.fit': ( 'agents/benchmark_agents/temp_ppo_sb3.html#ppoagent.fit',
                                                                                                                'RL_OM/agents/benchmark_agents/PPO_SB3.py'),
                                                        'RL_OM.agents.benchmark_agents.PPO_SB3.PPOPolicy': ( 'agents/benchmark_agents/temp_ppo_sb3.html#ppopolicy',
                                                                                                             'RL_OM/agents/benchmark_agents/PPO_SB3.py'),
@@ -133,102 +128,44 @@
                                                                                                                   'RL_OM/agents/benchmark_agents/nv_agents.py'),
                                                          'RL_OM.agents.benchmark_agents.nv_agents.RandomAgent.__init__': ( 'agents/benchmark_agents/basic_nv_agents.html#randomagent.__init__',
                                                                                                                            'RL_OM/agents/benchmark_agents/nv_agents.py'),
                                                          'RL_OM.agents.benchmark_agents.nv_agents.RandomAgent.draw_action': ( 'agents/benchmark_agents/basic_nv_agents.html#randomagent.draw_action',
                                                                                                                               'RL_OM/agents/benchmark_agents/nv_agents.py'),
                                                          'RL_OM.agents.benchmark_agents.nv_agents.RandomAgent.fit': ( 'agents/benchmark_agents/basic_nv_agents.html#randomagent.fit',
                                                                                                                       'RL_OM/agents/benchmark_agents/nv_agents.py')},
-            'RL_OM.agents.benchmark_agents.nv_agents_ERM': { 'RL_OM.agents.benchmark_agents.nv_agents_ERM.Block': ( 'agents/benchmark_agents/erm_agents.html#block',
-                                                                                                                    'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.Block.__init__': ( 'agents/benchmark_agents/erm_agents.html#block.__init__',
-                                                                                                                             'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.Block.forward': ( 'agents/benchmark_agents/erm_agents.html#block.forward',
-                                                                                                                            'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.CausalSelfAttention': ( 'agents/benchmark_agents/erm_agents.html#causalselfattention',
-                                                                                                                                  'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.CausalSelfAttention.__init__': ( 'agents/benchmark_agents/erm_agents.html#causalselfattention.__init__',
-                                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.CausalSelfAttention._init_rope': ( 'agents/benchmark_agents/erm_agents.html#causalselfattention._init_rope',
-                                                                                                                                             'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.CausalSelfAttention.forward': ( 'agents/benchmark_agents/erm_agents.html#causalselfattention.forward',
-                                                                                                                                          'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.FakePolicy': ( 'agents/benchmark_agents/erm_agents.html#fakepolicy',
+            'RL_OM.agents.benchmark_agents.nv_agents_ERM': { 'RL_OM.agents.benchmark_agents.nv_agents_ERM.FakePolicy': ( 'agents/benchmark_agents/erm_agents.html#fakepolicy',
                                                                                                                          'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.FakePolicy.reset': ( 'agents/benchmark_agents/erm_agents.html#fakepolicy.reset',
                                                                                                                                'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.LERMsgdAgent': ( 'agents/benchmark_agents/erm_agents.html#lermsgdagent',
                                                                                                                            'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.LERMsgdAgent.__init__': ( 'agents/benchmark_agents/erm_agents.html#lermsgdagent.__init__',
                                                                                                                                     'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.LERMsgdAgent.draw_action': ( 'agents/benchmark_agents/erm_agents.html#lermsgdagent.draw_action',
                                                                                                                                        'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.LERMsgdAgent.fit_epoch': ( 'agents/benchmark_agents/erm_agents.html#lermsgdagent.fit_epoch',
                                                                                                                                      'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlama': ( 'agents/benchmark_agents/erm_agents.html#lagllama',
-                                                                                                                       'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlama.__init__': ( 'agents/benchmark_agents/erm_agents.html#lagllama.__init__',
-                                                                                                                                'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlama.forward': ( 'agents/benchmark_agents/erm_agents.html#lagllama.forward',
-                                                                                                                               'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlama.reset_cache': ( 'agents/benchmark_agents/erm_agents.html#lagllama.reset_cache',
-                                                                                                                                   'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlamasgdAgent': ( 'agents/benchmark_agents/erm_agents.html#lagllamasgdagent',
-                                                                                                                               'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlamasgdAgent.__init__': ( 'agents/benchmark_agents/erm_agents.html#lagllamasgdagent.__init__',
-                                                                                                                                        'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlamasgdAgent.draw_action': ( 'agents/benchmark_agents/erm_agents.html#lagllamasgdagent.draw_action',
-                                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlamasgdAgent.fit_epoch': ( 'agents/benchmark_agents/erm_agents.html#lagllamasgdagent.fit_epoch',
-                                                                                                                                         'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlamasgdMetaAgent': ( 'agents/benchmark_agents/erm_agents.html#lagllamasgdmetaagent',
-                                                                                                                                   'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlamasgdMetaAgent.__init__': ( 'agents/benchmark_agents/erm_agents.html#lagllamasgdmetaagent.__init__',
-                                                                                                                                            'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlamasgdMetaAgent.draw_action': ( 'agents/benchmark_agents/erm_agents.html#lagllamasgdmetaagent.draw_action',
-                                                                                                                                               'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlamasgdMetaAgent.fit': ( 'agents/benchmark_agents/erm_agents.html#lagllamasgdmetaagent.fit',
-                                                                                                                                       'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlamasgdMetaAgent.fit_epoch': ( 'agents/benchmark_agents/erm_agents.html#lagllamasgdmetaagent.fit_epoch',
-                                                                                                                                             'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlamasgdMetaAgent.pinball_loss': ( 'agents/benchmark_agents/erm_agents.html#lagllamasgdmetaagent.pinball_loss',
-                                                                                                                                                'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LagLlamasgdMetaAgent.predict': ( 'agents/benchmark_agents/erm_agents.html#lagllamasgdmetaagent.predict',
-                                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.LinearModel': ( 'agents/benchmark_agents/erm_agents.html#linearmodel',
                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.LinearModel.__init__': ( 'agents/benchmark_agents/erm_agents.html#linearmodel.__init__',
                                                                                                                                    'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.LinearModel.forward': ( 'agents/benchmark_agents/erm_agents.html#linearmodel.forward',
                                                                                                                                   'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LlamaRotaryEmbedding': ( 'agents/benchmark_agents/erm_agents.html#llamarotaryembedding',
-                                                                                                                                   'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LlamaRotaryEmbedding.__init__': ( 'agents/benchmark_agents/erm_agents.html#llamarotaryembedding.__init__',
-                                                                                                                                            'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LlamaRotaryEmbedding._set_cos_sin_cache': ( 'agents/benchmark_agents/erm_agents.html#llamarotaryembedding._set_cos_sin_cache',
-                                                                                                                                                      'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.LlamaRotaryEmbedding.forward': ( 'agents/benchmark_agents/erm_agents.html#llamarotaryembedding.forward',
-                                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLP': ( 'agents/benchmark_agents/erm_agents.html#mlp',
                                                                                                                   'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLP.__init__': ( 'agents/benchmark_agents/erm_agents.html#mlp.__init__',
                                                                                                                            'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLP.forward': ( 'agents/benchmark_agents/erm_agents.html#mlp.forward',
                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLP_BLOCK': ( 'agents/benchmark_agents/erm_agents.html#mlp_block',
                                                                                                                         'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLP_BLOCK.__init__': ( 'agents/benchmark_agents/erm_agents.html#mlp_block.__init__',
                                                                                                                                  'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLP_BLOCK.forward': ( 'agents/benchmark_agents/erm_agents.html#mlp_block.forward',
                                                                                                                                 'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLP_block': ( 'agents/benchmark_agents/erm_agents.html#mlp_block',
-                                                                                                                        'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLP_block.__init__': ( 'agents/benchmark_agents/erm_agents.html#mlp_block.__init__',
-                                                                                                                                 'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLP_block.forward': ( 'agents/benchmark_agents/erm_agents.html#mlp_block.forward',
-                                                                                                                                'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLPsgdAgent': ( 'agents/benchmark_agents/erm_agents.html#mlpsgdagent',
                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLPsgdAgent.__init__': ( 'agents/benchmark_agents/erm_agents.html#mlpsgdagent.__init__',
                                                                                                                                    'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLPsgdAgent.draw_action': ( 'agents/benchmark_agents/erm_agents.html#mlpsgdagent.draw_action',
                                                                                                                                       'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.MLPsgdAgent.fit_epoch': ( 'agents/benchmark_agents/erm_agents.html#mlpsgdagent.fit_epoch',
@@ -237,56 +174,28 @@
                                                                                                                              'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorData.__getitem__': ( 'agents/benchmark_agents/erm_agents.html#newsvendordata.__getitem__',
                                                                                                                                          'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorData.__init__': ( 'agents/benchmark_agents/erm_agents.html#newsvendordata.__init__',
                                                                                                                                       'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorData.__len__': ( 'agents/benchmark_agents/erm_agents.html#newsvendordata.__len__',
                                                                                                                                      'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorDataMeta': ( 'agents/benchmark_agents/erm_agents.html#newsvendordatameta',
-                                                                                                                                 'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorDataMeta.__getitem__': ( 'agents/benchmark_agents/erm_agents.html#newsvendordatameta.__getitem__',
-                                                                                                                                             'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorDataMeta.__init__': ( 'agents/benchmark_agents/erm_agents.html#newsvendordatameta.__init__',
-                                                                                                                                          'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.NewsvendorDataMeta.__len__': ( 'agents/benchmark_agents/erm_agents.html#newsvendordatameta.__len__',
-                                                                                                                                         'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.RMSNorm': ( 'agents/benchmark_agents/erm_agents.html#rmsnorm',
-                                                                                                                      'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.RMSNorm.__init__': ( 'agents/benchmark_agents/erm_agents.html#rmsnorm.__init__',
-                                                                                                                               'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.RMSNorm.forward': ( 'agents/benchmark_agents/erm_agents.html#rmsnorm.forward',
-                                                                                                                              'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNN': ( 'agents/benchmark_agents/erm_agents.html#rnn',
                                                                                                                   'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNN.__init__': ( 'agents/benchmark_agents/erm_agents.html#rnn.__init__',
                                                                                                                            'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNN.forward': ( 'agents/benchmark_agents/erm_agents.html#rnn.forward',
                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNNsgdAgent': ( 'agents/benchmark_agents/erm_agents.html#rnnsgdagent',
                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNNsgdAgent.__init__': ( 'agents/benchmark_agents/erm_agents.html#rnnsgdagent.__init__',
                                                                                                                                    'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNNsgdAgent.draw_action': ( 'agents/benchmark_agents/erm_agents.html#rnnsgdagent.draw_action',
                                                                                                                                       'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNNsgdAgent.fit_epoch': ( 'agents/benchmark_agents/erm_agents.html#rnnsgdagent.fit_epoch',
                                                                                                                                     'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNNsgdMetaAgent': ( 'agents/benchmark_agents/erm_agents.html#rnnsgdmetaagent',
-                                                                                                                              'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNNsgdMetaAgent.__init__': ( 'agents/benchmark_agents/erm_agents.html#rnnsgdmetaagent.__init__',
-                                                                                                                                       'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNNsgdMetaAgent.draw_action': ( 'agents/benchmark_agents/erm_agents.html#rnnsgdmetaagent.draw_action',
-                                                                                                                                          'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNNsgdMetaAgent.fit': ( 'agents/benchmark_agents/erm_agents.html#rnnsgdmetaagent.fit',
-                                                                                                                                  'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNNsgdMetaAgent.fit_epoch': ( 'agents/benchmark_agents/erm_agents.html#rnnsgdmetaagent.fit_epoch',
-                                                                                                                                        'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNNsgdMetaAgent.pinball_loss': ( 'agents/benchmark_agents/erm_agents.html#rnnsgdmetaagent.pinball_loss',
-                                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.RNNsgdMetaAgent.predict': ( 'agents/benchmark_agents/erm_agents.html#rnnsgdmetaagent.predict',
-                                                                                                                                      'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.SGDBase': ( 'agents/benchmark_agents/erm_agents.html#sgdbase',
                                                                                                                       'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.SGDBase.__init__': ( 'agents/benchmark_agents/erm_agents.html#sgdbase.__init__',
                                                                                                                                'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.SGDBase.eval': ( 'agents/benchmark_agents/erm_agents.html#sgdbase.eval',
                                                                                                                            'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.SGDBase.fit': ( 'agents/benchmark_agents/erm_agents.html#sgdbase.fit',
@@ -294,21 +203,15 @@
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.SGDBase.max_or_zero': ( 'agents/benchmark_agents/erm_agents.html#sgdbase.max_or_zero',
                                                                                                                                   'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.SGDBase.pinball_loss': ( 'agents/benchmark_agents/erm_agents.html#sgdbase.pinball_loss',
                                                                                                                                    'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.SGDBase.predict': ( 'agents/benchmark_agents/erm_agents.html#sgdbase.predict',
                                                                                                                               'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_ERM.SGDBase.train': ( 'agents/benchmark_agents/erm_agents.html#sgdbase.train',
-                                                                                                                            'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.apply_rotary_pos_emb': ( 'agents/benchmark_agents/erm_agents.html#apply_rotary_pos_emb',
-                                                                                                                                   'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.find_multiple': ( 'agents/benchmark_agents/erm_agents.html#find_multiple',
-                                                                                                                            'RL_OM/agents/benchmark_agents/nv_agents_ERM.py'),
-                                                             'RL_OM.agents.benchmark_agents.nv_agents_ERM.rotate_half': ( 'agents/benchmark_agents/erm_agents.html#rotate_half',
-                                                                                                                          'RL_OM/agents/benchmark_agents/nv_agents_ERM.py')},
+                                                                                                                            'RL_OM/agents/benchmark_agents/nv_agents_ERM.py')},
             'RL_OM.agents.benchmark_agents.nv_agents_SAA': { 'RL_OM.agents.benchmark_agents.nv_agents_SAA.FakePolicy': ( 'agents/benchmark_agents/saa_agents.html#fakepolicy',
                                                                                                                          'RL_OM/agents/benchmark_agents/nv_agents_SAA.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_SAA.FakePolicy.reset': ( 'agents/benchmark_agents/saa_agents.html#fakepolicy.reset',
                                                                                                                                'RL_OM/agents/benchmark_agents/nv_agents_SAA.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_SAA.SAAAgent': ( 'agents/benchmark_agents/saa_agents.html#saaagent',
                                                                                                                        'RL_OM/agents/benchmark_agents/nv_agents_SAA.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_SAA.SAAAgent.__init__': ( 'agents/benchmark_agents/saa_agents.html#saaagent.__init__',
@@ -333,38 +236,14 @@
                                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_SAA.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_SAA.WSAAAgent.draw_action': ( 'agents/benchmark_agents/saa_agents.html#wsaaagent.draw_action',
                                                                                                                                     'RL_OM/agents/benchmark_agents/nv_agents_SAA.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_SAA.WSAAAgent.fit': ( 'agents/benchmark_agents/saa_agents.html#wsaaagent.fit',
                                                                                                                             'RL_OM/agents/benchmark_agents/nv_agents_SAA.py'),
                                                              'RL_OM.agents.benchmark_agents.nv_agents_SAA.check_cu_co': ( 'agents/benchmark_agents/saa_agents.html#check_cu_co',
                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_SAA.py')},
-            'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting': { 'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting.FakePolicy': ( 'agents/benchmark_agents/gradient_boosting_nv_agents.html#fakepolicy',
-                                                                                                                                                     'RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py'),
-                                                                           'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting.FakePolicy.reset': ( 'agents/benchmark_agents/gradient_boosting_nv_agents.html#fakepolicy.reset',
-                                                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py'),
-                                                                           'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting.XGBAgent': ( 'agents/benchmark_agents/gradient_boosting_nv_agents.html#xgbagent',
-                                                                                                                                                   'RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py'),
-                                                                           'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting.XGBAgent.__init__': ( 'agents/benchmark_agents/gradient_boosting_nv_agents.html#xgbagent.__init__',
-                                                                                                                                                            'RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py'),
-                                                                           'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting.XGBAgent._get_fitted_model': ( 'agents/benchmark_agents/gradient_boosting_nv_agents.html#xgbagent._get_fitted_model',
-                                                                                                                                                                     'RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py'),
-                                                                           'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting.XGBAgent.draw_action': ( 'agents/benchmark_agents/gradient_boosting_nv_agents.html#xgbagent.draw_action',
-                                                                                                                                                               'RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py'),
-                                                                           'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting.XGBAgent.fit': ( 'agents/benchmark_agents/gradient_boosting_nv_agents.html#xgbagent.fit',
-                                                                                                                                                       'RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py'),
-                                                                           'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting.XGBMetaAgent': ( 'agents/benchmark_agents/gradient_boosting_nv_agents.html#xgbmetaagent',
-                                                                                                                                                       'RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py'),
-                                                                           'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting.XGBMetaAgent.__init__': ( 'agents/benchmark_agents/gradient_boosting_nv_agents.html#xgbmetaagent.__init__',
-                                                                                                                                                                'RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py'),
-                                                                           'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting.XGBMetaAgent._get_fitted_model': ( 'agents/benchmark_agents/gradient_boosting_nv_agents.html#xgbmetaagent._get_fitted_model',
-                                                                                                                                                                         'RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py'),
-                                                                           'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting.XGBMetaAgent.draw_action': ( 'agents/benchmark_agents/gradient_boosting_nv_agents.html#xgbmetaagent.draw_action',
-                                                                                                                                                                   'RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py'),
-                                                                           'RL_OM.agents.benchmark_agents.nv_agents_gradient_boosting.XGBMetaAgent.fit': ( 'agents/benchmark_agents/gradient_boosting_nv_agents.html#xgbmetaagent.fit',
-                                                                                                                                                           'RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py')},
             'RL_OM.agents.benchmark_agents.qr': { 'RL_OM.agents.benchmark_agents.qr.QRAgent': ( 'agents/benchmark_agents/qr.html#qragent',
                                                                                                 'RL_OM/agents/benchmark_agents/qr.py'),
                                                   'RL_OM.agents.benchmark_agents.qr.QRAgent.__init__': ( 'agents/benchmark_agents/qr.html#qragent.__init__',
                                                                                                          'RL_OM/agents/benchmark_agents/qr.py'),
                                                   'RL_OM.agents.benchmark_agents.qr.QRAgent.fit': ( 'agents/benchmark_agents/qr.html#qragent.fit',
                                                                                                     'RL_OM/agents/benchmark_agents/qr.py'),
                                                   'RL_OM.agents.benchmark_agents.qr.QRAgent_v2': ( 'agents/benchmark_agents/qr.html#qragent_v2',
@@ -1178,16 +1057,14 @@
             'RL_OM.core': {'RL_OM.core.foo': ('core.html#foo', 'RL_OM/core.py')},
             'RL_OM.environments.calculation_functions': { 'RL_OM.environments.calculation_functions.eoq_qr_calculations_qr_action': ( 'environments/calculation_functions.html#eoq_qr_calculations_qr_action',
                                                                                                                                       'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.eoq_qr_calculations_single_action': ( 'environments/calculation_functions.html#eoq_qr_calculations_single_action',
                                                                                                                                           'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.get_fixed_ordering_cost': ( 'environments/calculation_functions.html#get_fixed_ordering_cost',
                                                                                                                                 'RL_OM/environments/calculation_functions.py'),
-                                                          'RL_OM.environments.calculation_functions.get_orders_arriving_stochastic': ( 'environments/calculation_functions.html#get_orders_arriving_stochastic',
-                                                                                                                                       'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.mpfc_calculations_ss_action': ( 'environments/calculation_functions.html#mpfc_calculations_ss_action',
                                                                                                                                     'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.normalize_reward_FC': ( 'environments/calculation_functions.html#normalize_reward_fc',
                                                                                                                             'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.normalize_reward_NV': ( 'environments/calculation_functions.html#normalize_reward_nv',
                                                                                                                             'RL_OM/environments/calculation_functions.py'),
                                                           'RL_OM.environments.calculation_functions.nv_calculations': ( 'environments/calculation_functions.html#nv_calculations',
@@ -1217,31 +1094,15 @@
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.reset': ( 'environments/multi_period_inventory.html#multiperiodenv.reset',
                                                                                                                                'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.set_observation_space': ( 'environments/multi_period_inventory.html#multiperiodenv.set_observation_space',
                                                                                                                                                'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.set_observation_state': ( 'environments/multi_period_inventory.html#multiperiodenv.set_observation_state',
                                                                                                                                                'RL_OM/environments/multi_period_inventory.py'),
                                                            'RL_OM.environments.multi_period_inventory.MultiPeriodEnv.step': ( 'environments/multi_period_inventory.html#multiperiodenv.step',
-                                                                                                                              'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP': ( 'environments/multi_period_inventory.html#multiperiodenvmp',
-                                                                                                                           'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.__init__': ( 'environments/multi_period_inventory.html#multiperiodenvmp.__init__',
-                                                                                                                                    'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.convert_to_numpy_array': ( 'environments/multi_period_inventory.html#multiperiodenvmp.convert_to_numpy_array',
-                                                                                                                                                  'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.render': ( 'environments/multi_period_inventory.html#multiperiodenvmp.render',
-                                                                                                                                  'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.reset': ( 'environments/multi_period_inventory.html#multiperiodenvmp.reset',
-                                                                                                                                 'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.set_observation_space': ( 'environments/multi_period_inventory.html#multiperiodenvmp.set_observation_space',
-                                                                                                                                                 'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.set_observation_state': ( 'environments/multi_period_inventory.html#multiperiodenvmp.set_observation_state',
-                                                                                                                                                 'RL_OM/environments/multi_period_inventory.py'),
-                                                           'RL_OM.environments.multi_period_inventory.MultiPeriodEnvMP.step': ( 'environments/multi_period_inventory.html#multiperiodenvmp.step',
-                                                                                                                                'RL_OM/environments/multi_period_inventory.py')},
+                                                                                                                              'RL_OM/environments/multi_period_inventory.py')},
             'RL_OM.experiment_functions.run_experiment': { 'RL_OM.experiment_functions.run_experiment.check_val_test': ( 'experiment_functions/run_experiment.html#check_val_test',
                                                                                                                          'RL_OM/experiment_functions/run_experiment.py'),
                                                            'RL_OM.experiment_functions.run_experiment.experiment_stepwise': ( 'experiment_functions/run_experiment.html#experiment_stepwise',
                                                                                                                               'RL_OM/experiment_functions/run_experiment.py'),
                                                            'RL_OM.experiment_functions.run_experiment.experiment_stepwise_no_log': ( 'experiment_functions/run_experiment.html#experiment_stepwise_no_log',
                                                                                                                                      'RL_OM/experiment_functions/run_experiment.py'),
                                                            'RL_OM.experiment_functions.run_experiment.experiment_wandb': ( 'experiment_functions/run_experiment.html#experiment_wandb',
@@ -1265,37 +1126,8 @@
                              'RL_OM.utils.init_pipeline': ('utils/utils.html#init_pipeline', 'RL_OM/utils.py'),
                              'RL_OM.utils.load_agent_function': ('utils/utils.html#load_agent_function', 'RL_OM/utils.py'),
                              'RL_OM.utils.merge_with_namespace': ('utils/utils.html#merge_with_namespace', 'RL_OM/utils.py'),
                              'RL_OM.utils.prepare_calculation_function': ( 'utils/utils.html#prepare_calculation_function',
                                                                            'RL_OM/utils.py'),
                              'RL_OM.utils.prepare_hyperparameter_opt': ('utils/utils.html#prepare_hyperparameter_opt', 'RL_OM/utils.py'),
                              'RL_OM.utils.prepare_lag_window': ('utils/utils.html#prepare_lag_window', 'RL_OM/utils.py'),
-                             'RL_OM.utils.track_normalization': ('utils/utils.html#track_normalization', 'RL_OM/utils.py')},
-            'RL_OM.utils.MLtools': { 'RL_OM.utils.MLtools.LRSchedulerPerStep': ( 'utils/ml_tools.html#lrschedulerperstep',
-                                                                                 'RL_OM/utils/MLtools.py'),
-                                     'RL_OM.utils.MLtools.LRSchedulerPerStep.__init__': ( 'utils/ml_tools.html#lrschedulerperstep.__init__',
-                                                                                          'RL_OM/utils/MLtools.py'),
-                                     'RL_OM.utils.MLtools.LRSchedulerPerStep.step': ( 'utils/ml_tools.html#lrschedulerperstep.step',
-                                                                                      'RL_OM/utils/MLtools.py')},
-            'RL_OM.utils.utils': { 'RL_OM.utils.utils.combine_dict': ('utils/utils.html#combine_dict', 'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.convert_str_none_to_none': ( 'utils/utils.html#convert_str_none_to_none',
-                                                                                   'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.create_env_agent': ('utils/utils.html#create_env_agent', 'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.delete_lag_window_from_config': ( 'utils/utils.html#delete_lag_window_from_config',
-                                                                                        'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.get_actions_per_product': ( 'utils/utils.html#get_actions_per_product',
-                                                                                  'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.get_git_revision_hash': ( 'utils/utils.html#get_git_revision_hash',
-                                                                                'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.get_version': ('utils/utils.html#get_version', 'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.init_pipeline': ('utils/utils.html#init_pipeline', 'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.load_agent_function': ( 'utils/utils.html#load_agent_function',
-                                                                              'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.merge_with_namespace': ( 'utils/utils.html#merge_with_namespace',
-                                                                               'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.prepare_calculation_function': ( 'utils/utils.html#prepare_calculation_function',
-                                                                                       'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.prepare_hyperparameter_opt': ( 'utils/utils.html#prepare_hyperparameter_opt',
-                                                                                     'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.prepare_lag_window': ('utils/utils.html#prepare_lag_window', 'RL_OM/utils/utils.py'),
-                                   'RL_OM.utils.utils.track_normalization': ( 'utils/utils.html#track_normalization',
-                                                                              'RL_OM/utils/utils.py')}}}
+                             'RL_OM.utils.track_normalization': ('utils/utils.html#track_normalization', 'RL_OM/utils.py')}}}
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/benchmark_agents/PPO_SB3.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/PPO_SB3.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/benchmark_agents/cbs.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/cbs.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files 4% similar despite different names*

```diff
@@ -176,18 +176,18 @@
         for preprocessor in self.preprocessors:
             input = preprocessor(input)
 
         if self.l is None:
             action = np.where(input >= self.d, 0, self.q_star)
 
         else:
-            pipeline_vector = input[:-self.num_products]
+            pipeline_vector = input[self.num_products:]
             pipeline = np.reshape(pipeline_vector, (self.num_products, max(self.l)))
             pipeline_sum = np.sum(pipeline, axis=1)
-            inventory = input[-self.num_products:]
+            inventory = input[:self.num_products]
             # print("printing inventory, pipeline, lead time, average demand")
             # print(inventory)
             # print(pipeline_sum)
             inventory_position = inventory + pipeline_sum
             # print(self.l)
             # print(self.d)
             action = np.where((inventory_position-self.l*self.d >= 0), 0, self.q_star)
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/benchmark_agents/mp_agents_ERM.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/mp_agents_ERM.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/benchmark_agents/nv_agents.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/nv_agents.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/benchmark_agents/nv_agents_ERM.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/nv_agents_ERM.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../../nbs/agents/benchmark_agents/03_ERM_agents.ipynb.
 
 # %% auto 0
 __all__ = ['FakePolicy', 'NewsvendorData', 'LinearModel', 'MLP', 'MLP_BLOCK', 'RNN', 'SGDBase', 'LERMsgdAgent', 'MLPsgdAgent',
            'RNNsgdAgent', 'RNNsgdMetaAgent', 'LlamaRotaryEmbedding', 'rotate_half', 'apply_rotary_pos_emb',
            'CausalSelfAttention', 'find_multiple', 'MLP_block', 'RMSNorm', 'Block', 'LagLlama', 'LagLlamasgdAgent',
-           'NewsvendorDataMeta', 'LagLlamasgdMetaAgent']
+           'LagLlamasgdMetaAgent']
 
 # %% ../../../nbs/agents/benchmark_agents/03_ERM_agents.ipynb 4
 # General libraries:
 import numpy as np
 from scipy.stats import norm
 from tqdm import trange, tqdm
 from time import sleep
 
 # Torch
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from torch.utils.data import Dataset, DataLoader
-from torch.cuda.amp import GradScaler, autocast
-
-
 from ..processors.processors import GetTimeSeriesAndStaticFeatures
 
 
 # Mushroom libraries
 from mushroom_rl.core import Agent
 
-from timeit import default_timer as timer
-
-from ...utils.MLtools import LRSchedulerPerStep
-
-from torchinfo import summary
-
 # %% ../../../nbs/agents/benchmark_agents/03_ERM_agents.ipynb 6
 class FakePolicy():
     def reset(*args, **kwargs):
         pass
 
 class NewsvendorData(Dataset):
 
@@ -228,43 +219,25 @@
 
         # print(x.shape)
     
         return x    
 
 class SGDBase(Agent):
 
-    def __init__(self, config=None, input_size=None, hidden_size=64, output_size=1, learning_rate=0.01, num_hidden_layers=3, num_RNN_layers=None, drop_prob=0.0, l2_reg=0.0, learning_rate_scheduler=None,  scheduler_params=None, num_time_series_features=None, lag_window=None, relu_output=False):
+    def __init__(self, config=None, input_size=None, hidden_size=64, output_size=1, learning_rate=0.01, num_hidden_layers=3, num_RNN_layers=None, drop_prob=0.0, l2_reg=0.0, num_time_series_features=None, lag_window=None, relu_output=False):
         if self.model_type=="Linear":
             self.model=LinearModel(input_size, output_size, relu_output=relu_output)
         elif self.model_type=="MLP":
             self.model=MLP(input_size, hidden_size, output_size, num_hidden_layers=num_hidden_layers, drop_prob=drop_prob, relu_output=relu_output)
         elif self.model_type=="RNN":
             self.model=RNN(input_size, hidden_size, output_size, num_hidden_layers=num_hidden_layers, num_RNN_layers=num_RNN_layers, drop_prob=drop_prob, num_time_series_features=num_time_series_features, lag_window=lag_window, relu_output=relu_output)
         elif self.model_type=="LagLlama":
             # print("config: ", config)
             self.model=LagLlama(**config)
-
-            #print model and number of parameters
-
-        # check if input siize is integer
-        if isinstance(input_size, int):
-            input_size = [input_size]
-        summary(self.model, input_size=input_size)
-        
         self.optimizer = torch.optim.Adam(self.model.parameters(), lr=learning_rate, weight_decay=l2_reg)
-        
-        if learning_rate_scheduler == "LinearWarmupWithDecay":
-            self.scheduler = LRSchedulerPerStep(self.optimizer, base_learning_rate=learning_rate, **scheduler_params)
-            self.scheduler.step()
-        elif learning_rate_scheduler == None:
-            self.scheduler = None
-        else:
-            raise ValueError("Learning rate scheduler not recognized")
-
-
         self.criterion = nn.MSELoss()
 
 
     def fit(self, X_train, y_train, mask, cu, co, batch_size=64, learning_rate=0.01, device="cpu"):
         
         if y_train.ndim == 1:
             y_train = y.reshape(-1, 1)
@@ -285,15 +258,14 @@
                     masks=None
                 else:
                     feat, labels, masks = output
                     masks=masks.to(device)
                 
                 feat=feat.to(device)
                 labels=labels.to(device)
-
                 outputs=self.model(feat)
 
                 loss = torch.mean(SGDBase.pinball_loss(cu, co, labels, outputs, masks))
                 
                 total_loss += loss.item()
 
                 #backward
@@ -307,23 +279,19 @@
 
         return self.model
 
     def predict(self, X):
 
         # if len(X.shape)==1:
         #     X = np.expand_dims(X, axis=0)
-
-        self.model.to("cpu")
         
         self.model.eval()
-
         with torch.no_grad():
             X=torch.from_numpy(X)
             X=X.float()
-            
             output=self.model(X)
             output=output.numpy()
         
         if len(output.shape)==2:
             output=output.reshape(-1)
         
         return output
@@ -491,15 +459,15 @@
     
         if final_activation=="identity":
             self.final_activation = False
         elif final_activation=="relu":
             self.final_activation = True
 
         super().__init__(input_size=input_size, hidden_size=hidden_size, output_size=output_size, learning_rate=learning_rate, num_hidden_layers=num_hidden_layers, num_RNN_layers=num_RNN_layers, drop_prob=drop_prob, l2_reg=l2_reg, num_time_series_features=num_time_series_features, lag_window=lag_window, relu_output=self.final_activation, )
-        
+
     def fit_epoch(self, features_train, demand_train, mask=None):
         super().fit(features_train, demand_train, mask=mask, cu=self.cu, co=self.co, batch_size=self.batch_size, learning_rate=self.learning_rate, device=self.device)
 
     def draw_action(self, X):
         return super().predict(X)
 
 class RNNsgdMetaAgent(SGDBase):
@@ -571,15 +539,15 @@
         for i, (output) in tqdm(enumerate(train_loader)):
 
                 if len(output)==3:
                     feat, labels, product = output
                     masks=None
                 else:
                     feat, labels, masks, product = output
-                    masks=masks.to(device)
+                    masks=masks.to(device)   
 
                 feat=feat.to(device)
                 labels=labels.to(device)
                 outputs=self.model(feat)
 
                 cu_selected = cu[product]
                 co_selected = co[product]
@@ -601,44 +569,35 @@
         return self.model
 
     def draw_action(self, X):
         return self.predict(X)
     
     def predict(self, X):
         self.model.eval()
-        self.model.to(self.device)
-
-        if len(X.shape) == 1:
-            X = np.expand_dims(X, axis=0)
-
-        # Initialize a list to hold the X_i batches
-        X_batches = []
-
-        # Create batches
         for i in range(self.feature_map.shape[1]):
-            X_i = X[:, self.feature_map[:, i].astype(bool)]
-            X_batches.append(X_i)
-
-        X_batch = np.concatenate([x for x in X_batches], axis=0)
-        X_batch = torch.from_numpy(X_batch)
-        X_batch = X_batch.float().to(self.device)
-
-        with torch.no_grad():
-            output = self.model(X_batch)
-            output = output.cpu().numpy()
-
-        # reduce output dimension
+            if len(X.shape)==1:
+                X = np.expand_dims(X, axis=0)
+            X_i = X[:,self.feature_map[:,i].astype(bool)]
+            with torch.no_grad():
+                X_i=torch.from_numpy(X_i)
+                X_i=X_i.float()
+                # X_i=X_i.to(self.device)
+                output=self.model(X_i)
+                output=output.numpy()
+            
+            if i == 0:
+                outputs = output
+            else:
+                outputs = np.hstack((outputs, output))
 
-        output = output.squeeze(1)
-        
         # print(outputs)
 
         # check if outputs need to got to cpu or handled by mushroomrl
 
-        return output
+        return outputs
 
     @staticmethod
     def pinball_loss(cu, co, demand, order_quantity, mask):
 
         if len(demand.shape)==1:
             demand = demand.unsqueeze(1)
         
@@ -879,22 +838,14 @@
             y = F.scaled_dot_product_attention(
                 q, k, v, attn_mask=None, dropout_p=self.dropout, is_causal=False
             )
         else:
             y = F.scaled_dot_product_attention(
                 q, k, v, attn_mask=None, dropout_p=self.dropout, is_causal=True
             )
-        
-        # debug
-        if not torch.isfinite(y).all():
-            print("y is not finite")
-            print(y)
-            print(q)
-            print(k)
-            print(v)
 
         # re-assemble all head outputs side by side
         y = y.transpose(1, 2).contiguous().view(B, T, C)
 
         # output projection
         y = self.c_proj(y)
 
@@ -954,16 +905,15 @@
         # NOTE: the original RMSNorm paper implementation is not equivalent
         # norm_x = x.norm(2, dim=self.dim, keepdim=True)
         # rms_x = norm_x * d_x ** (-1. / 2)
         # x_normed = x / (rms_x + self.eps)
         # keep RMSNorm in float32
         norm_x = x.to(torch.float32).pow(2).mean(dim=self.dim, keepdim=True)
         x_normed = x * torch.rsqrt(norm_x + self.eps)
-        output = (self.scale * x_normed).type_as(x)
-        return output
+        return (self.scale * x_normed).type_as(x)
 
 class Block(nn.Module):
     def __init__(self, n_embd_per_head, n_head, block_size, dropout, min_multiple = 256, n_mlp_layers=2) -> None:
         super().__init__()
         self.rms_1 = RMSNorm(n_embd_per_head * n_head)
         self.attn = CausalSelfAttention(n_embd_per_head, n_head, block_size, dropout)
         self.rms_2 = RMSNorm(n_embd_per_head * n_head)
@@ -974,15 +924,14 @@
         y = x + self.mlp(self.rms_2(x))
         return y
 
 class LagLlama(nn.Module):
     def __init__(self,
                 input_size,
                 output_size,
-                convert_input,
 
                 context_length = 16,
                 max_context_length = 16, # check what context and max_context do
                 n_layer = 1, # default LagLlama paper: 32
                 n_head = 4, # default LagLlama paper: 32
                 n_embd_per_head = 32, # default LagLlama paper: 128
                 rope_scaling = None, # not yet implemetned (scaled version of rotary embeddings)
@@ -998,44 +947,51 @@
                 relu_output=False):
 
         super().__init__()
 
         block_size = max_context_length
         self.context_length = context_length
 
-        self.input_processor = GetTimeSeriesAndStaticFeatures(num_time_series_features,lag_window)
-        self.convert_input = convert_input
 
         # did not implement optional time_features as all inputs are day-level.
         # Any other time-features (e.g., weekday) can be included in preprocessing
         # and added as part of the feature vector
 
+
         # self.num_parallel_samples = num_parallel_samples
+        self.input_processor = GetTimeSeriesAndStaticFeatures(num_time_series_features,lag_window)
 
-        self.input_size = input_size # size of input vector (features + demand) on one timestep without positional embeddings
+        self.input_size = int(input_size/lag_window) # size of input vector (features + demand) on one timestep without positional embeddings
+        
         
-        # print("input size: ", self.input_size)
+        feature_size = self.input_size # Features for Transformer equal exactly the input size
+        
+        # No lags per timestep used
+        # feature_size = input_size * (len(self.lags_seq)) + 2 * input_size # TODO need to check this
+
+        print("feature size: ", feature_size)
         #! Note that no scaling is implemented in the model, needs to be addressed in pre-processing
 
         # self.distr_output = distr_output # TODO check later how to get rid of
 
         # changed from PropabilisticForecastingNetwork to sinlge output
-        self.param_proj = nn.Linear(n_embd_per_head * n_head, output_size)
+        self.param_proj = nn.Linear(n_embd_per_head * n_head, output_size
+        )
 
         self.transformer = nn.ModuleDict(
             dict(
                 wte=nn.Linear(
-                    self.input_size, n_embd_per_head * n_head
+                    feature_size, n_embd_per_head * n_head
                 ),
                 h=nn.ModuleList([Block(n_embd_per_head, n_head, block_size, drop_prob, min_multiple = min_multiple, n_mlp_layers=n_mlp_layers) for _ in range(n_layer)]),
                 ln_f=RMSNorm(n_embd_per_head * n_head),
             )
         )
         self.y_cache = False  # used at time of inference when kv cached is used
-        
+
         if relu_output:
             self.final_activation = nn.ReLU()  # output is non-negative
         else:
             self.final_activation = nn.Identity()
 
 
         def _init_weights(self, module: nn.Module) -> None:
@@ -1116,22 +1072,22 @@
         #     else:
         #         return torch.cat((lags, expanded_static_feat), dim=-1), loc, scale
 
     def forward(    self,
                     x: torch.Tensor,
                     use_kv_cache: bool = False,) -> torch.Tensor:
 
+        # if shape is 1 then expand
+        if len(x.shape)==1:
+            x=x.unsqueeze(0)
+        x = self.input_processor(x)[0] # no static data returned as no inventory
 
-        if self.convert_input:
-            # if shape is 1 then expand
-            if x.ndim == 1:
-                x = x.unsqueeze(0)
 
-            x = self.input_processor(x)[0] # no static data returned as no inventory
-            
+        # TODO: Confirm size of x is btc
+        
         (B, T, C) = x.size()
 
         # past_target = None
         # past_observed_values = None
         # past_time_feat = None
         # future_time_feat = None
         # future_target = None
@@ -1141,101 +1097,62 @@
         #     past_observed_values=None, # not scaling applied
         #     future_target=future_target,
         #     past_time_feat=past_time_feat,
         #     future_time_feat=future_time_feat,
         # )
 
         transformer_input = x
-        #transformer_input = transformer_input.to(torch.float16) # solution to problem of getting NaN during training
 
         if use_kv_cache and self.y_cache:
-            used_kv_cache = True
             # Only use the most recent one, rest is in cache
             transformer_input = transformer_input[:, -1:]
-        else:
-            used_kv_cache = False
         
-        # print("before embedding:", x.shape)
         x = self.transformer.wte(
             transformer_input
         )  # token embeddings of shape (b, t, n_embd_per_head*n_head) # (bsz, context_length+(pred_len-1), n_embd_per_head*n_head)
-        # print("after embedding", x.shape)
-
-        # sleep(2)
 
-        embeddings = x
-        if torch.isnan(x).any():
-            print("nan in embeddings")
-        if not torch.isfinite(x).all():
-            print("infinite in embeddings")
-            for i in x:
-                if not torch.isfinite(i).all():
-                    print("infinite in one row")
-                    print(i)
-        
         for block in self.transformer.h:
             x = block(x, use_kv_cache)
         x = self.transformer.ln_f(
             x
         )  # (bsz, context_length+(pred_len-1), n_embd_per_head*n_head)
         if use_kv_cache:
             self.y_cache = True
-
-        raw_output = x
-        
-        
         output = self.param_proj(
             x
         )  # (bsz, context_length+(pred_len-1)) ; (bsz, context_length+(pred_len-1))
 
-        output_after_projection = output
-        
         output = self.final_activation(output)
 
-        # check if na in output
-        if torch.isnan(output).any():
-            print("nan in output")
-            print("used_kv_cache: ", used_kv_cache)
-    
-            print(transformer_input)
-            if torch.isnan(transformer_input).any():
-                print("nan in transformer_input")
-            else:
-                print("no nan in input")
-            print(raw_output)
-            print(embeddings)
-            print(output_after_projection)
-            print(output)
-
-            print(x)
-            
         output = output[:, -1, :]
         # print(output.shape)
         return output
     
     def reset_cache(self) -> None:
         """
         Resets all cached key-values in attention.
         Has to be called after prediction loop in predictor
         """
         for block in self.transformer.h:
             block.y_cache = None
             block.attn.kv_cache = None
 
+
 class LagLlamasgdAgent(SGDBase):
 
     def __init__(self,
                     input_size,
                     output_size,
                     cu,
                     co,
                     num_time_series_features,
                     lag_window,
                     agent_name = "DLNV_LagLlama",
 
+
                     final_activation="identity",
 
                     # TRansformer block params
                     context_length = None, # if context length is not provided, it is set to the lag_window
                     max_context_length = None,  # if max_context_length is not provided, it is set to the context_length
                                                 # max context length used for RoPE - can be longer than lag_window during training
                     n_layer = 1, # default LagLlama paper: 32
@@ -1270,15 +1187,15 @@
         if context_length is None:
             context_length = lag_window
         if max_context_length is None:
             max_context_length = context_length
 
         config = {
 
-            "input_size": num_time_series_features, # all features are time series features
+            "input_size": input_size,
             "output_size": output_size,
             "num_time_series_features": num_time_series_features,
 
             "context_length": context_length,
             "max_context_length": max_context_length,
             "n_layer": n_layer,
             "n_head": n_head,
@@ -1286,17 +1203,15 @@
             "rope_scaling": rope_scaling,
             "min_multiple": min_multiple,
             "n_mlp_layers": n_mlp_layers,
 
             "drop_prob": drop_prob,
             "num_time_series_features": num_time_series_features,
             "lag_window": lag_window,
-            "relu_output": final_activation,
-
-            "convert_input": True, 
+            "relu_output": final_activation
         }
 
         
         self.batch_size=batch_size
         self.learning_rate=learning_rate
 
         self.policy=FakePolicy()
@@ -1310,139 +1225,31 @@
         elif final_activation=="relu":
             self.final_activation = True
 
         print("init parent")
         print("config: ", config)
         super().__init__(learning_rate = learning_rate, l2_reg=l2_reg, config=config)
 
+
     def fit_epoch(self, features_train, demand_train, mask=None):
         super().fit(features_train, demand_train, mask=mask, cu=self.cu, co=self.co, batch_size=self.batch_size, learning_rate=self.learning_rate, device=self.device)
 
     def draw_action(self, X):
         return super().predict(X)
 
-
-class NewsvendorDataMeta(Dataset):
-
-    def __init__(self, x_time_dependent, x_timeless, y, feature_map, lag_window, feature_size, lag_features):
-
-        # Function to handle mask not built in.
-
-        self.x_time_dependent = x_time_dependent
-        self.x_timeless = x_timeless
-        self.y = y
-        self.feature_map = feature_map
-
-        self.lag_window = lag_window
-        self.feature_size = feature_size
-        self.num_products = y.shape[1]
-
-        print("lag lookback: ", lag_window)
-
-        self.n_samples=(y.shape[0]-lag_window)*y.shape[1]
-        self.index_mapping = dict()
-
-        self.lag_features = lag_features
-        
-        index_used=0
-        for i in range(y.shape[0]-lag_window):
-            for j in range(y.shape[1]):
-                self.index_mapping[index_used] = (i,j)
-                index_used+=1
-
-    def __getitem__(self, index):
-        
-        coordinates = self.index_mapping[index]
-
-        time = coordinates[0]+self.lag_window
-        product = coordinates[1]
-
-        y = self.y[:, product]
-
-        x = np.zeros((self.lag_window, self.feature_size))
-
-        ####### ADD LAG DEMAND
-
-        relevant_demand = np.zeros((self.lag_window, len(self.lag_features)))
-        for i in range(len(self.lag_features)):
-            lag = self.lag_features[i]
-            start_index = time-self.lag_window-lag+1
-            end_index = time-lag+1
-
-            if start_index < 0:
-                if end_index >0:
-                    num_zeros = np.abs(start_index)
-                    relevant_demand[:num_zeros, i] = 0
-                    relevant_demand[num_zeros:, i] = y[:end_index].T
-                else:
-                    relevant_demand[:, i] = 0
-            else:
-                relevant_demand[:, i] = y[time-self.lag_window-lag+1:time-lag+1]
-        x[:,0:len(self.lag_features)] = relevant_demand
-
-        # relevant_demand = np.zeros((self.lag_window, len(self.lag_features)))
-        # for i in range(len(self.lag_features)):
-        #     lag = self.lag_features[i]
-        #     start_index = time - self.lag_window - lag + 1
-        #     end_index = time - lag + 1
-
-        #     if start_index < 0:
-        #         # If the start_index is negative, determine how many slots should be zero
-        #         num_zeros = abs(start_index)
-        #         # Adjust the start_index to 0 for valid slicing
-        #         start_index = 0
-        #         # First, fill the beginning part of the column with zeros (if needed)
-        #         relevant_demand[:num_zeros, i] = 0
-        #         # Then, fill the rest with data from 'y'
-        #         relevant_demand[num_zeros:, i] = y[start_index:end_index]
-        #     else:
-        #         # When all the data is within the available range
-        #         relevant_demand[:, i] = y[start_index:end_index]
-
-        # x[:, 0:len(self.lag_features)] = relevant_demand
-
-        ####### ADD TIMELESS FEATURES
-        features_timeless = np.expand_dims(self.x_timeless[product], axis=0)
-        features_timeless = np.repeat(features_timeless, self.lag_window, axis=0)     
-        x[:,len(self.lag_features):len(self.lag_features)+features_timeless.shape[1]] = features_timeless  
-
-        ####### ADD TIME DEPENDENT FEATURES
-        relevant_features = self.x_time_dependent[(time-self.lag_window+1):time+1] # +1 because features of current period are visible to the agent.
-
-        # get starting overarching features
-        relevant_features_specific = relevant_features[:,:-self.num_products*2] #! TDOD make the 2 variable
-        relevant_features_specific_mapped = relevant_features_specific[:, self.feature_map[product]]
-
-        # get features unique per product
-        relevant_features_product = relevant_features[:,-self.num_products*2:][:, [product, self.num_products+product]] #! TDOD make the 2 variable
-
-        x[:,len(self.lag_features)+features_timeless.shape[1]:len(self.lag_features)+features_timeless.shape[1]+relevant_features_specific_mapped.shape[1]] = relevant_features_specific_mapped
-        x[:,len(self.lag_features)+features_timeless.shape[1]+relevant_features_specific_mapped.shape[1]:len(self.lag_features)+features_timeless.shape[1]+relevant_features_specific_mapped.shape[1]+relevant_features_product.shape[1]] = relevant_features_product
-        
-        y_target = y[time]
-        x = torch.tensor(x, dtype=torch.float32)
-        y = torch.tensor(y, dtype=torch.float32)
-        product = torch.tensor(product, dtype=torch.long)
-
-        return x, y_target, product
-
-    def __len__(self):
-        return self.n_samples
-
 class LagLlamasgdMetaAgent(SGDBase):
 
     def __init__(self,
                     feature_map,
                     input_size,
                     output_size,
                     cu,
                     co,
                     num_time_series_features,
                     lag_window,
-                    lag_features = [1],
                     agent_name = "DLNV_LagLlama",
 
                     final_activation="identity",
 
                     # TRansformer block params
                     context_length = None, # if context length is not provided, it is set to the lag_window
                     max_context_length = None,  # if max_context_length is not provided, it is set to the context_length
@@ -1452,37 +1259,32 @@
                     n_embd_per_head = 32, # default LagLlama paper: 128
                     rope_scaling = None, # not yet implemented (scaled version of rotary embeddings)
                     min_multiple = 256,
                     n_mlp_layers = 2,
                     
                     # General params
                     drop_prob=0.0, 
-                    batch_size=128, # batch size for training
+                    batch_size=128,
                     learning_rate=0.01,
                     l2_reg=0.0,
-                    learning_rate_scheduler=None, # Other: "LinearWarmupWithDecay"
-                    scheduler_params=None, # For LinearWarmupWithDecay warmup_steps=..., learning_rate will be interpreted as base learning rate.
                     device="cpu",
 
-                    max_batch_size=2048, # relevant for inference only
-
-                    weight_products = False,
                     ):
 
         print("in init") 
-        
+
         self.feature_map = feature_map
         
         self.name=agent_name
         self.model_type="LagLlama"
         self.cu = cu
         self.co = co
         self.device = device
 
-        print("in lag lama agent:", input_size)
+        input_size = np.sum(self.feature_map[:,0])
         output_size = 1
 
         if final_activation=="identity":
             final_activation = False
         elif final_activation=="relu":
             final_activation = True
 
@@ -1505,220 +1307,120 @@
             "rope_scaling": rope_scaling,
             "min_multiple": min_multiple,
             "n_mlp_layers": n_mlp_layers,
 
             "drop_prob": drop_prob,
             "num_time_series_features": num_time_series_features,
             "lag_window": lag_window,
-            "relu_output": final_activation,
-
-            "convert_input": False,
+            "relu_output": final_activation
         }
 
         
         self.batch_size=batch_size
         self.learning_rate=learning_rate
 
         self.policy=FakePolicy()
         self._postprocessors = list()
         self._preprocessors = list()
         self.train_directly=True
         self.train_mode = "epochs"
-
-        self.lag_window = lag_window
-        self.input_size = input_size
-
-        self.max_batch_size = max_batch_size
     
         if final_activation=="identity":
             self.final_activation = False
         elif final_activation=="relu":
             self.final_activation = True
 
-        self.weight_products = weight_products
-
-        self.lag_features = lag_features
+        print("init parent")
+        print("config: ", config)
+        super().__init__(learning_rate = learning_rate, l2_reg=l2_reg, config=config)
 
-        super().__init__(learning_rate = learning_rate, l2_reg=l2_reg, learning_rate_scheduler=learning_rate_scheduler, scheduler_params=scheduler_params, config=config)
-    
     def fit_epoch(self, features_train, demand_train, mask=None):
         self.fit(features_train, demand_train, mask=mask, cu=self.cu, co=self.co, batch_size=self.batch_size, learning_rate=self.learning_rate, device=self.device)
 
     def fit(self, X_train, y_train, mask, cu, co, batch_size=64, learning_rate=0.01, device="cpu"):
         
-        # self.model.half()
-
-        torch.autograd.set_detect_anomaly(True)
-        scaler = GradScaler()
-
-        start_total_time = timer()
-        start_preparation = timer()
-
-        features_time_dependent = X_train[0]
-        features_timeless = X_train[1]
+        if y_train.ndim == 1:
+            y_train = y.reshape(-1, 1)
         
-        dataset_train=NewsvendorDataMeta(features_time_dependent, features_timeless, y_train, self.feature_map, self.lag_window, self.input_size, self.lag_features)
+        dataset_train=NewsvendorData(X_train, y_train, mask, self.feature_map)
 
         self.model.to(device)
         
-        train_loader=DataLoader(dataset=dataset_train, batch_size=batch_size, shuffle=True, num_workers=1,) # make shuffle true
+        train_loader=DataLoader(dataset=dataset_train, batch_size=batch_size, shuffle=False) # make shuffle true
 
         self.model.train()
 
         total_loss = 0
-
-        end_preparation = timer()
-
-        start_time_loop = timer()
-        time_to_train_model = 0
-
         for i, (output) in tqdm(enumerate(train_loader)):
 
-            feat, labels, product = output
-
-            start_time_training = timer()
+                if len(output)==3:
+                    feat, labels, product = output
+                    masks=None
+                else:
+                    feat, labels, masks, product = output
+                    masks=masks.to(device)   
 
-            feat=feat.to(device)
-            labels=labels.to(device)
-            with autocast():
-                outputs=self.model(feat.to(torch.float16))
+                feat=feat.to(device)
+                labels=labels.to(device)
+                outputs=self.model(feat)
 
                 cu_selected = cu[product]
                 co_selected = co[product]
-
-                loss_per_product = self.pinball_loss(cu_selected, co_selected, labels, outputs)
-            
-                if self.weight_products:
-                    # print(loss_per_product.shape)
-                    # print(torch.sum(loss_per_product))
-                    loss_per_product = loss_per_product * weights[product].unsqueeze(-1)
-                    # print(loss_per_product.shape)
-                    # print(torch.sum(loss_per_product))
                 
+                loss_per_product = self.pinball_loss(cu_selected, co_selected, labels, outputs, masks)
                 loss = torch.mean(loss_per_product)
-            
+                
                 total_loss += loss.item()
 
                 #backward
                 self.optimizer.zero_grad()
-                scaler.scale(loss).backward()
-                #loss.backward()
-                scaler.step(self.optimizer)
-                scaler.update()
-                #self.optimizer.step()
-            
-            if self.scheduler is not None:
-                self.scheduler.step()
-
-            # check if nan in loss tensor
-            if torch.isnan(loss):
-                raise ValueError("got nan")
-
-            end_time_training = timer()
-            time_to_train_model += end_time_training-start_time_training
-
-        end_time_loop = timer()
+                loss.backward()
+                self.optimizer.step()
 
         print("training loss: ", total_loss)   
         self.model.eval()
         self.model.to("cpu")
 
-        end_total_time = timer()
-
-        print("total time: ", end_total_time-start_total_time)
-        print("preparation time: ", end_preparation-start_preparation)
-        print("total time in loop: ", end_time_loop-start_time_loop)
-        print("thereof time to train model: ", time_to_train_model)
-
-        # self.model = self.model.float()
-
         return self.model
 
     def draw_action(self, X):
+        return self.predict(X)
     
-        # assert X does not contain nan values
-
-        for i in X:
-            if np.isnan(i).any():
-                print("nan values in input")
-                raise ValueError("NaN values in Input")
-            break
-        
-        action = self.predict(X)
-
-        if np.isnan(action).any():
-            print("nan values in action")
-            raise ValueError("NaN values in Output")
-
-        return action
-    
-    # def predict(self, X):
-    #     self.model.eval()
-    #     self.model.to(self.device)
-
-    #     if len(X.shape) == 1:
-    #         X = np.expand_dims(X, axis=0)
-
-    #     # Initialize a list to hold the X_i batches
-    #     X_batches = []
-
-    #     # Create batches
-    #     for i in range(self.feature_map.shape[1]):
-    #         X_i = X[:, self.feature_map[:, i].astype(bool)]
-    #         X_batches.append(X_i)
-
-    #     X_batch = np.concatenate([x for x in X_batches], axis=0)
-    #     X_batch = torch.from_numpy(X_batch)
-    #     X_batch = X_batch.float().to(self.device)
-
-    #     with torch.no_grad():
-    #         output = self.model(X_batch)
-    #         output = output.cpu().numpy()
-
-    #     # reduce output dimension
-
-    #     output = output.squeeze(1)
-        
-    #     # print(outputs)
-
-    #     # check if outputs need to got to cpu or handled by mushroomrl
-
-    #     return output
-
     def predict(self, X):
         self.model.eval()
         self.model.to(self.device)
 
-        X = torch.from_numpy(X).to(self.device)
-        X = X.float()
+        if len(X.shape) == 1:
+            X = np.expand_dims(X, axis=0)
 
-        if X.size(0) > self.max_batch_size:
-            batches = []
-            for i in range(0, X.size(0), self.max_batch_size):
-                batch = X[i:i+self.max_batch_size]
-                batches.append(batch)
-        else:
-            batches = [X]
-   
-        outputs = []
-        for X_batch in batches:
-            with torch.no_grad():
-                output_part = self.model(X_batch)
-                outputs.append(output_part.cpu().numpy())
+        # Initialize a list to hold the X_i batches
+        X_batches = []
+
+        # Create batches
+        for i in range(self.feature_map.shape[1]):
+            X_i = X[:, self.feature_map[:, i].astype(bool)]
+            X_batches.append(X_i)
+
+        X_batch = np.concatenate([x for x in X_batches], axis=0)
+        X_batch = torch.from_numpy(X_batch)
+        X_batch = X_batch.float().to(self.device)
+
+        with torch.no_grad():
+            output = self.model(X_batch)
+            output = output.cpu().numpy()
         
-        # Concatenate the results from the smaller batches
-        output = np.concatenate(outputs, axis=0)
+        # print(outputs)
 
-        # Reduce output dimension
-        output = output.squeeze()
+        # check if outputs need to got to cpu or handled by mushroomrl
 
         return output
 
     @staticmethod
-    def pinball_loss(cu, co, demand, order_quantity):
+    def pinball_loss(cu, co, demand, order_quantity, mask):
+
 
         if len(demand.shape)==1:
             demand = demand.unsqueeze(1)
         
         assert demand.shape == order_quantity.shape
 
         cu = torch.tensor(cu, dtype=torch.float32)
@@ -1737,8 +1439,10 @@
         assert co.shape == overage_quantity.shape
 
         underage=cu*underage_quantity
         overage=co*overage_quantity
 
         loss=underage+overage
  
+        if mask is not None:
+            loss = loss*mask
         return loss
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/benchmark_agents/nv_agents_SAA.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/nv_agents_SAA.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
                  co=None,
                  criterion="mse",
                  n_estimators=100,
                  max_depth=None,
                  min_samples_split=6, # starndard 2
                  min_samples_leaf=3, # standard 1
                  min_weight_fraction_leaf=0.,
-                 max_features="sqrt",
+                 max_features="auto",
                  max_leaf_nodes=None,
                  min_impurity_decrease=0.,
                  bootstrap=True,
                  oob_score=False,
                  n_jobs=None,
                  random_state=None,
                  verbose=0,
@@ -73,15 +73,14 @@
         self._postprocessors=list()
         self._preprocessors=list() 
 
         self.name = agent_name
         self.fitted=False
         
     def _get_fitted_model(self, X, y, mask=None):
-        print(self.max_features)
         model = RandomForestRegressor(
             criterion=self.criterion,
             n_estimators=self.n_estimators,
             max_depth=self.max_depth,
             min_samples_split=self.min_samples_split,
             min_samples_leaf=self.min_samples_leaf,
             min_weight_fraction_leaf=self.min_weight_fraction_leaf,
@@ -94,16 +93,14 @@
             random_state=self.random_state,
             verbose=self.verbose,
             warm_start=self.warm_start,
             ccp_alpha=self.ccp_alpha,
             max_samples=self.max_samples
         )
 
-        print(X.shape)
-
         self.model_ = model.fit(X, y)
         self.train_leaf_indices_ = model.apply(X)
         
 
     def _calc_weights(self, sample):
         sample_leaf_indices = self.model_.apply([sample])
         if self.weight_function == "w1":
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/benchmark_agents/qr.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/qr.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,15 @@
 
         # assert self.q is not None, "q is not set"
         # assert self.r is not None, "r is not set"
 
         for preprocessor in self.preprocessors:
             input = preprocessor(input)
 
-        pipeline_vector = input[:-self.num_products]
+        pipeline_vector = input[self.num_products:]
         pipeline = np.reshape(pipeline_vector, (self.num_products, max(self.l)))
         pipeline_sum = np.sum(pipeline, axis=1)
 
         if self.include_l:
             r = (self.r - pipeline_sum)[0]
         else:
             r = -1 if pipeline_sum != 0 else self.r
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/benchmark_agents/saa.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/saa.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/benchmark_agents/ss.py` & `RL_OM-0.7.9/RL_OM/agents/benchmark_agents/ss.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         
         self.train_directly=True
         self.train_mode = "direct"
 
         super().__init__(mdp_info, policy)
 
 
-    def fit(self, features = None, demand=None, mask=None):
+    def fit(self, features = None, demand=None):
 
         """ 
         Fit the QR policy to the given demand.
 
         # TODO adjust description
 
         This method allows the EOQ agent to adapt its policy to historic demand data, assuming a fixed demand rate without uncertainty.
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/networks/actors.py` & `RL_OM-0.7.9/RL_OM/agents/networks/actors.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 class ActorNetworkRNN(nn.Module):
     """
     Simple 3-Layer network for the actor function approximator.
     
     """
     # TODO make the network architecture more flexible
 
-    def __init__(self, input_shape, output_shape, input_shape_RNN, n_features, input_processor = None, device = None, **kwargs):
+    def __init__(self, input_shape, output_shape, input_shape_RNN, n_features, input_processor = None, use_cuda=False, **kwargs):
         super(ActorNetworkRNN, self).__init__()
 
         # print("setting up actor")
         self._n_input_RNN = input_shape_RNN # first dimension: number of features; second dimension: sequence length
         self._n_output = output_shape[0]
         self._n_features = n_features
 
@@ -82,20 +82,18 @@
 
         # print("setting up weights")
         nn.init.xavier_uniform_(self._h2.weight,
                                 gain=nn.init.calculate_gain('relu'))
         nn.init.xavier_uniform_(self._h3.weight,
                                 gain=nn.init.calculate_gain('linear'))
 
-        self.device = device
-
-        # if "cuda" in self.device:
-        #     self.use_cuda = True
-        # else:
-        #     self.use_cuda = False
+        if use_cuda:
+            self.device = torch.device("cuda")
+        else:
+            self.device = torch.device("cpu")   
         
         # print("device: ", self.device)
 
         # print("actor set up")
     
 
     def forward(self, state):
@@ -126,15 +124,15 @@
 class ActorNetworkRNN_MLP_hybrid(nn.Module):
     """
     Simple 3-Layer network for the actor function approximator.
     
     """
     # TODO make the network architecture more flexible
 
-    def __init__(self, input_shape, output_shape, input_shape_RNN, input_shape_MLP, n_features, input_processor = None, device=None, **kwargs):
+    def __init__(self, input_shape, output_shape, input_shape_RNN, input_shape_MLP, n_features, input_processor = None, use_cuda=False, **kwargs):
         super(ActorNetworkRNN_MLP_hybrid, self).__init__()
 
         self._n_input_RNN = input_shape_RNN # first dimension: number of features; second dimension: sequence length
         self._n_input_MLP = input_shape_MLP[0]
         self._n_output = output_shape[0]
         self._n_features = n_features
 
@@ -148,22 +146,21 @@
         self._h3 = nn.Linear(self._n_features, self._n_output)
 
         nn.init.xavier_uniform_(self._h1_mlp.weight,
                                 gain=nn.init.calculate_gain('relu'))
         nn.init.xavier_uniform_(self._h2.weight,
                                 gain=nn.init.calculate_gain('relu'))
         nn.init.xavier_uniform_(self._h3.weight,
-                                gain=nn.init.calculate_gain('linear')) 
-
-        self.device = device
+                                gain=nn.init.calculate_gain('linear'))
 
-        # if "cuda" in self.device:
-        #     self.use_cuda = True
-        # else:
-        #     self.use_cuda = False
+        if use_cuda:
+            self.device = torch.device("cuda")
+        else:
+            self.device = torch.device("cpu")   
+    
 
     def forward(self, state):
 
         # print("state before transform:",  state.device)
 
         state = self.input_processor(state)
 
@@ -172,22 +169,14 @@
         state_ts = state[0].to(self.device)
         state_static = state[1].to(self.device)
 
         self._h1_recurrent.flatten_parameters()
 
         h0 = torch.zeros(1 , state_ts.size(0), int(self._n_features/2)).requires_grad_().to(self.device)
         
-        # get devices
-        # print("state_ts.device: ", state_ts.device)
-        # print("h0.device: ", h0.device)
-        # print("state_static.device: ", state_static.device)
-
-        # # get device of _h1_recurrent
-        # print("self._h1_recurrent.weight.device: ", self._h1_recurrent.weight.device)
-
         features1_rnn, _ = self._h1_recurrent(state_ts.float(), h0.detach())
         features1_rnn = features1_rnn[:, -1, :]
         #features1_rnn = torch.zeros(state_ts.size(0), int(self._n_features/2))
         features1_mpl = F.relu(self._h1_mlp(state_static.float()))
         features1 = torch.cat((features1_rnn, features1_mpl), dim = 1)
 
         features2 = F.relu(self._h2(features1))
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/networks/base.py` & `RL_OM-0.7.9/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/networks/critics.py` & `RL_OM-0.7.9/RL_OM/agents/networks/critics.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 # %% ../../../nbs/agents/networks/01_critics.ipynb 8
 class CriticNetworkStateActionRNN(nn.Module):
     """
     #TODO update docstring
     Base class for simple 3-Layer network.
     """
 
-    def __init__(self, input_shape, output_shape, input_shape_RNN, input_shape_MLP, n_features, input_processor = None, squeeze_output = False, device = None, **kwargs):
+    def __init__(self, input_shape, output_shape, input_shape_RNN, input_shape_MLP, n_features, input_processor = None, squeeze_output = False, use_cuda=False, **kwargs):
      
         super(CriticNetworkStateActionRNN, self).__init__()
 
         # print("setting critic network")
         self._n_input_RNN = input_shape_RNN # first dimension: number of features; second dimension: sequence length
 
         self._n_input_MLP = input_shape_MLP[0]
@@ -118,21 +118,20 @@
                                 gain=nn.init.calculate_gain('relu'))
         nn.init.xavier_uniform_(self._h2.weight,
                                 gain=nn.init.calculate_gain('relu'))
         nn.init.xavier_uniform_(self._h3.weight,
                                 gain=nn.init.calculate_gain('linear'))
         
         self.squeeze = squeeze_output #! check what option is correct here
-         
-        self.device = device
-
-        # if "cuda" in self.device:
-        #     self.use_cuda = True
-        # else:
-        #     self.use_cuda = False
+        
+        if use_cuda:
+            self.device = torch.device("cuda")
+        else:
+            self.device = torch.device("cpu")   
+        print("device: ", self.device)
 
         # print("done setting critic network")
 
     def forward(self, state, action):
 
         state = self.input_processor(state)
 
@@ -164,15 +163,15 @@
 # %% ../../../nbs/agents/networks/01_critics.ipynb 9
 class CriticNetworkStateActionRNN_MLP_hybrid(nn.Module):
     """
     #TODO update docstring
     Base class for simple 3-Layer network.
     """
 
-    def __init__(self, input_shape, output_shape, input_shape_RNN, input_shape_MLP, n_features, input_processor = None, squeeze_output = False, device=None, **kwargs):
+    def __init__(self, input_shape, output_shape, input_shape_RNN, input_shape_MLP, n_features, input_processor = None, squeeze_output = False, use_cuda=False, **kwargs):
      
         super(CriticNetworkStateActionRNN, self).__init__()
 
         self._n_input_RNN = input_shape_RNN # first dimension: number of features; second dimension: sequence length
         self._n_input_MLP = input_shape_MLP[0]
         self._n_output = output_shape[0]
         self._n_features = n_features
@@ -194,20 +193,19 @@
         nn.init.xavier_uniform_(self._h2.weight,
                                 gain=nn.init.calculate_gain('relu'))
         nn.init.xavier_uniform_(self._h3.weight,
                                 gain=nn.init.calculate_gain('linear'))
         
         self.squeeze = squeeze_output #! check what option is correct here
 
-        self.device=device
-
-        # if "cuda" in self.device:
-        #     self.use_cuda = True
-        # else:
-        #     self.use_cuda = False
+        if use_cuda:
+            self.device = torch.device("cuda")
+        else:
+            self.device = torch.device("cpu")   
+        print("device: ", self.device)
 
     def forward(self, state, action):
 
         # print("in critic")
 
         state = self.input_processor(state)
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/processors/eoq_preprocessors.py` & `RL_OM-0.7.9/RL_OM/agents/processors/eoq_preprocessors.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,22 +13,22 @@
     This class implements a processor that get the inventory from the state.
 
     Args:
         num_features (int): Number of features in the state.
         num_products (int): Number of products in the state.
 
     """
+    
 
     def __init__(self, num_features, num_products, max_l = None):
         self.num_features = num_features
         self.num_products = num_products
         self.max_l = max_l
-        assert np.isscalar(max_l)
     
     def __call__(self, input):
         #assert len(input) == self.num_features + self.num_products
         assert len(input.shape) == 1
         
         if self.max_l is not None:
-            return input[self.num_features:self.num_features+self.num_products+self.max_l*self.num_products]
+            return input[self.num_features:self.num_features+self.num_products+np.max(self.max_l)*self.num_products]
         else:
             return input[self.num_features:self.num_features+self.num_products]
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/processors/processors.py` & `RL_OM-0.7.9/RL_OM/agents/processors/processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,12 +188,10 @@
         self.len_ts_features = len_ts_features
         
     def __call__(self, state):
 
         ts_data = state[:,:self.num_ts_features*self.len_ts_features]
         static_data = state[:,self.num_ts_features*self.len_ts_features:]
 
-        temp_data = ts_data.reshape(state.shape[0], self.num_ts_features, self.len_ts_features)
+        ts_data = ts_data.reshape(state.shape[0], self.num_ts_features, self.len_ts_features).transpose(1, 2)
 
-        ts_data = temp_data.transpose(2, 1)
-        
         return [ts_data, static_data]
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/algorithms/sac_discrete.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/PPO_classic.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,18 +49,14 @@
             squeeze_output = True,
             use_cuda = True,
             agent_name = None): 
 
         self.n_steps_per_fit=n_steps_per_fit
         
         use_cuda = use_cuda and torch.cuda.is_available()
-        if use_cuda:
-            self.device = "cuda"
-        else:
-            self.device = "cpu"
 
         input_shape = mdp_info.observation_space.shape
         print("input shape: ", input_shape)
         actor_output_shape = (mdp_info.action_space.shape[0],) 
 
         if learning_rate_critic is None:
             learning_rate_critic = learning_rate_actor
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_RNN.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 # Algorithms
 from mushroom_rl.algorithms.actor_critic.deep_actor_critic import SAC
 
 # Processors
 from ...processors.processors import HybridToContinuous
 
 
-from time import sleep
-
 # %% ../../../../nbs/agents/rl_agents/pre_specified_agents/12_SAC_RNN.ipynb 6
 class SACRNN():
 
     """
     # TODO Update docstring
     Soft Actor Critic (SAC) agent with hybrid action, both based on Gaussian. The binary action is 
     0 if the output of the network is less or equal than 0, and 1 otherwise.
@@ -71,21 +69,19 @@
             tau = 0.005,
             log_std_min = -20,
             log_std_max = 2,
             target_entropy = None,
             RNN_unit = "GRU", # TODO: Make RNN and LSTM possible
             optimizer = optim.Adam,
             squeeze_output = True,
-            device = None,
+            use_cuda = True,
             agent_name = None):
-
-        # TODO: remove this double definition
-        if self.device is not None:
-            self.device = device
         
+        use_cuda = use_cuda and torch.cuda.is_available()
+
         input_shape_data = mdp_info.observation_space.shape
         input_shape_RNN = (num_time_series_features, window_size)
         input_shape_MLP = (num_non_time_series_features,)
 
         actor_output_shape = (mdp_info.action_space.shape[0],)
 
         if learning_rate_critic is None:
@@ -94,24 +90,24 @@
         actor_mu_params = dict(network=ActorNetworkRNN,
                                 n_features=n_features,
                                 input_shape=input_shape_data,
                                 input_shape_RNN=input_shape_RNN,
                                 input_shape_MLP=input_shape_MLP,
                                 output_shape=actor_output_shape,
                                 input_processor=GetTimeSeriesAndStaticFeatures(num_time_series_features,window_size),
-                                device=device)
+                                use_cuda=use_cuda)
 
         actor_sigma_params = dict(network=ActorNetworkRNN,
                                     n_features=n_features,
                                     input_shape= input_shape_data,
                                     input_shape_RNN=input_shape_RNN,
                                     input_shape_MLP=input_shape_MLP,
                                     output_shape=actor_output_shape,
                                     input_processor=GetTimeSeriesAndStaticFeatures(num_time_series_features,window_size),
-                                    device=device)
+                                    use_cuda=use_cuda)
         
         actor_optimizer = {'class': optimizer,
                     'params': {'lr': learning_rate_actor}} 
         
         critic_input_shape = (input_shape_data[0] + actor_output_shape[0],)
         input_shape_RNN = (num_time_series_features, window_size)
         input_shape_MLP = (num_non_time_series_features + actor_output_shape[0],)
@@ -123,15 +119,15 @@
                         n_features=n_features,
                         input_shape=critic_input_shape,
                         input_shape_RNN = input_shape_RNN,
                         input_shape_MLP = input_shape_MLP,
                         output_shape=(1,),
                         input_processor=GetTimeSeriesAndStaticFeatures(num_time_series_features,window_size),
                         squeeze_output=squeeze_output,
-                        device=device)
+                        use_cuda=use_cuda)
         
         self.agent = SAC(mdp_info, actor_mu_params, actor_sigma_params,
                     actor_optimizer, critic_params, batch_size, initial_replay_size,
                     max_replay_size, warmup_transitions, tau, lr_alpha, log_std_min, log_std_max, target_entropy,
                     critic_fit_params=None)
         
         if agent_name is None:
@@ -186,73 +182,77 @@
             tau = 0.005,
             log_std_min = -20,
             log_std_max = 2,
             target_entropy = None,
             RNN_unit = "GRU", # TODO: Make RNN and LSTM possible
             optimizer = optim.Adam,
             squeeze_output = True,
-            device = "cpu",
+            use_cuda = True,
             agent_name = None):
-
-        self.device = device
-
-        if "cuda" in device:
-            use_cuda = True
-        else:
-            use_cuda = False
+        
+        use_cuda = use_cuda and torch.cuda.is_available()
 
         input_shape_data = mdp_info.observation_space.shape
         input_shape_RNN = (num_time_series_features, window_size)
         input_shape_MLP = (num_non_time_series_features,)
 
         actor_output_shape = (mdp_info.action_space.shape[0],)
 
         if learning_rate_critic is None:
             learning_rate_critic = learning_rate_actor
-        
+
+        print("shapes:")
+        print("data:", input_shape_data)
+        print("RNN:", input_shape_RNN)
+        print("MLP:", input_shape_MLP)
+        print("output:", actor_output_shape)
+
+
         actor_mu_params = dict(network=ActorNetworkRNN_MLP_hybrid,
                                 n_features=n_features,
                                 input_shape=input_shape_data,
                                 input_shape_RNN=input_shape_RNN,
                                 input_shape_MLP=input_shape_MLP,
                                 output_shape=actor_output_shape,
                                 input_processor=GetTimeSeriesAndStaticFeatures(num_time_series_features,window_size),
-                                use_cuda = use_cuda,
-                                device=device)
+                                use_cuda=use_cuda)
 
         actor_sigma_params = dict(network=ActorNetworkRNN_MLP_hybrid,
                                     n_features=n_features,
                                     input_shape= input_shape_data,
                                     input_shape_RNN=input_shape_RNN,
                                     input_shape_MLP=input_shape_MLP,
                                     output_shape=actor_output_shape,
                                     input_processor=GetTimeSeriesAndStaticFeatures(num_time_series_features,window_size),
-                                    use_cuda = use_cuda,
-                                    device=device)
+                                    use_cuda=use_cuda)
         
         actor_optimizer = {'class': optimizer,
                     'params': {'lr': learning_rate_actor}} 
         
         critic_input_shape = (input_shape_data[0] + actor_output_shape[0],)
         input_shape_RNN = (num_time_series_features, window_size)
+        print(num_non_time_series_features)
+        print(actor_output_shape[0])
+        print("XXXXX")
         input_shape_MLP = (num_non_time_series_features + actor_output_shape[0],)
 
+        print("input mlp:", input_shape_MLP)
+
         critic_params = dict(network=CriticNetworkStateActionRNN,
                         optimizer={'class': optim.Adam,
                                 'params': {'lr': learning_rate_critic}}, 
                         loss=F.mse_loss,
                         n_features=n_features,
                         input_shape=critic_input_shape,
                         input_shape_RNN = input_shape_RNN,
                         input_shape_MLP = input_shape_MLP,
                         output_shape=(1,),
                         input_processor=GetTimeSeriesAndStaticFeatures(num_time_series_features,window_size),
                         squeeze_output=squeeze_output,
-                        use_cuda = use_cuda,
-                        device=device)
+                        use_cuda=use_cuda)
         
         self.agent = SAC(mdp_info, actor_mu_params, actor_sigma_params,
                     actor_optimizer, critic_params, batch_size, initial_replay_size,
                     max_replay_size, warmup_transitions, tau, lr_alpha, log_std_min, log_std_max, target_entropy,
                     critic_fit_params=None)
         
         if agent_name is None:
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_classic.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,18 +67,14 @@
             target_entropy = None,
             optimizer = optim.Adam,
             squeeze_output = True,
             use_cuda = True,
             agent_name = None): 
         
         use_cuda = use_cuda and torch.cuda.is_available()
-        if use_cuda:
-            self.device = "cuda"
-        else:
-            self.device = "cpu"
 
         input_shape = mdp_info.observation_space.shape
         actor_output_shape = (mdp_info.action_space.shape[0],) 
 
         if learning_rate_critic is None:
             learning_rate_critic = learning_rate_actor
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/pre_specified_agents/TD3_classic.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,18 +73,14 @@
         
         # print("in init fubction")
         
         self.policy_class = OrnsteinUhlenbeckPolicy
         self.policy_params = dict(sigma=np.ones(1) * sigma_scale, theta=theta, dt=dt)
         
         use_cuda = use_cuda and torch.cuda.is_available()
-        if use_cuda:
-            self.device = "cuda"
-        else:
-            self.device = "cpu"
 
         input_shape = mdp_info.observation_space.shape
         actor_output_shape = (mdp_info.action_space.shape[0],) 
 
         if learning_rate_critic is None:
             learning_rate_critic = learning_rate_actor
```

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/sac_discrete.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.7.9/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/environments/calculation_functions.py` & `RL_OM-0.7.9/RL_OM/environments/calculation_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/environments/10_calculation_functions.ipynb.
 
 # %% auto 0
-__all__ = ['normalize_reward_FC', 'normalize_reward_NV', 'get_orders_arriving_stochastic', 'eoq_qr_calculations_single_action',
-           'eoq_qr_calculations_qr_action', 'mpfc_calculations_ss_action', 'nv_calculations', 'get_fixed_ordering_cost']
+__all__ = ['normalize_reward_FC', 'normalize_reward_NV', 'eoq_qr_calculations_single_action', 'eoq_qr_calculations_qr_action',
+           'mpfc_calculations_ss_action', 'nv_calculations', 'get_fixed_ordering_cost']
 
 # %% ../../nbs/environments/10_calculation_functions.ipynb 4
 # General libraries:
 import numpy as np
 import time
 
 # %% ../../nbs/environments/10_calculation_functions.ipynb 8
@@ -47,82 +47,14 @@
     else:
         # print("not normalizing")
         reward_norm = reward
 
     return reward_norm
 
 # %% ../../nbs/environments/10_calculation_functions.ipynb 10
-def get_orders_arriving_stochastic(self, action):
-
-
-    # print("xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx")
-    # print("initial state")
-
-    # print("lead times:", self.lead_time_realizations)
-    # print("full order pipeline:", self.full_order_pipeline)
-    # print("order pipeline:", self.order_pipeline)
-
-    # print("order placed:", action)
-    
-    all_orders_arriving = np.zeros(self.num_products) 
-            
-    for i in range(self.num_products):
-        arriving_mask = self.lead_time_realizations[i] == 0
-        orders_arriving = np.sum(self.full_order_pipeline[i][arriving_mask])
-        self.full_order_pipeline[i][arriving_mask] = 0
-        all_orders_arriving[i] = orders_arriving
-    
-    # print("arriving orders:", all_orders_arriving)
-    
-    self.full_order_pipeline[:,:-1] = self.full_order_pipeline[:,1:].copy()
-    self.full_order_pipeline[:,-1] = action
-
-    # print("full order pipeline after update1:", self.full_order_pipeline)
-
-    self.lead_time_realizations[:,:-1] = self.lead_time_realizations[:,1:].copy()
-
-    if self.lead_time_stochastic == "gamma":
-        lead_time_drawn_raw = np.random.gamma(self.lead_time-1, 1, self.num_products)+1
-    elif self.lead_time_stochastic == "normal":
-        lead_time_drawn_raw = np.random.normal(self.lead_time, self.lead_time_variance, self.num_products)
-        lead_time_drawn_raw = np.maximum(lead_time_drawn_raw, 1)
-    else:
-        raise ValueError("lead time distribution unknown")
-    
-    self.lead_time_realizations[:,-1] = int(np.round(np.minimum(lead_time_drawn_raw, self.max_lead_time), 0))
-    # print("lead time of order:", self.lead_time_realizations[:,-1])
-    self.lead_time_realizations = np.maximum(self.lead_time_realizations-1, 0)
-
-    # below also accounts for the c  ase that lag window is larger than max lead time
-
-    # print("full order pipeline after update2:", self.full_order_pipeline)
-
-    if self.max_lead_time > self.max_observation_lead_time:
-        self.order_pipeline = self.full_order_pipeline[:,-self.max_observation_lead_time:].copy()
-    else:
-        self.order_pipeline[:,-self.max_lead_time:] = self.full_order_pipeline.copy()
-
-
-    # print("full order pipeline after update3:", self.full_order_pipeline)
-
-    self.order_pipeline[:,0] = self.order_pipeline[:,0] + np.sum(self.full_order_pipeline[:,:-self.max_observation_lead_time], axis = 1) 
-
-
-    # print("final state")
-
-    # print("lead times:", self.lead_time_realizations)  
-    # print("full order pipeline:", self.full_order_pipeline)
-    # print("order pipeline:", self.order_pipeline)
-
-
-    # time.sleep(10)
-
-    return all_orders_arriving
-
-# %% ../../nbs/environments/10_calculation_functions.ipynb 11
 def eoq_qr_calculations_single_action(self, action):
 
     # TODO Think about naming of the function
 
     # print(f"action: {action}")
     # print(f"self.inventory: {self.inventory}")
     # # print pipeline
@@ -141,32 +73,21 @@
     # print("start inventory:", self.inventory)
     # print("start pipeline:", self.order_pipeline)
 
     # print("pipeline last element:" self.order_pipeline[:,-1])
 
     # print("action:", action)
 
-    order = action
-
     if self.use_order_pipeline:
-        if self.lead_time_stochastic:
-
-            orders_arriving = get_orders_arriving_stochastic(self, order)
-         
-        else:
-            orders_arriving = self.order_pipeline[:,-1].copy()
-            # print("orders_arriving: ", orders_arriving)
-            #Move elements one slot to the right in order_pipeline
-            self.order_pipeline[:, 1:] = self.order_pipeline[:, :-1]
-            product_indices = np.arange(self.num_products)
-            insert_indices = -self.lead_time
-            self.order_pipeline[product_indices, insert_indices] = order
-
+        orders_arriving = self.order_pipeline[:,-1].copy()
+            # Move elements one slot to the right in order_pipeline
+        self.order_pipeline[:, 1:] = self.order_pipeline[:, :-1]
+        self.order_pipeline[:, 0] = action
     else:
-        orders_arriving = order
+        orders_arriving = action
 
     # print("orders_arriving:", orders_arriving)
     # print("new pipeline:", self.order_pipeline)
 
     self.inventory += orders_arriving # first, the order will be added to inventory (meaning lead-time is 0)
 
     # print("inventory after order:", self.inventory)
@@ -216,15 +137,15 @@
             fixed_ordering = fixed_ordering_cost_step,
     )
 
     self.period += 1
 
     return reward_norm, info
 
-# %% ../../nbs/environments/10_calculation_functions.ipynb 12
+# %% ../../nbs/environments/10_calculation_functions.ipynb 11
 def eoq_qr_calculations_qr_action(self, action):
 
     # TODO Think about naming of the function
     
     # print("inventory: ", self.inventory)
     # print("pipeline: ", self.order_pipeline)
     # print("action: ", action.shape)
@@ -242,26 +163,21 @@
     fixed_ordering_cost_step = get_fixed_ordering_cost(self, order, positive_only = True)
 
     # print(fixed_ordering_cost_step.shape)
 
     # print("pipeline becfore: ", self.order_pipeline)
 
     if self.use_order_pipeline:
-
-        if self.lead_time_stochastic:
-            orders_arriving = get_orders_arriving_stochastic(self, order)
-
-        else:
-            orders_arriving = self.order_pipeline[:,-1].copy()
-            # print("orders_arriving: ", orders_arriving)
-            #Move elements one slot to the right in order_pipeline
-            self.order_pipeline[:, 1:] = self.order_pipeline[:, :-1]
-            product_indices = np.arange(self.num_products)
-            insert_indices = -self.lead_time
-            self.order_pipeline[product_indices, insert_indices] = order
+        orders_arriving = self.order_pipeline[:,-1].copy()
+        # print("orders_arriving: ", orders_arriving)
+        #Move elements one slot to the right in order_pipeline
+        self.order_pipeline[:, 1:] = self.order_pipeline[:, :-1]
+        product_indices = np.arange(self.num_products)
+        insert_indices = -self.lead_time
+        self.order_pipeline[product_indices, insert_indices] = order
     else:
         orders_arriving = order
 
     # print("pipeline after: ", self.order_pipeline)
 
     # print(np.round(self.order_pipeline,0))
 
@@ -320,15 +236,15 @@
             fixed_ordering = fixed_ordering_cost_step,
     )
 
     self.period += 1
 
     return reward_norm, info
 
-# %% ../../nbs/environments/10_calculation_functions.ipynb 13
+# %% ../../nbs/environments/10_calculation_functions.ipynb 12
 def mpfc_calculations_ss_action(self, action):
 
     # TODO Think about naming of the function
 
     if len(action.shape) == 1:
         s = action[0]
         S = action[1]
@@ -394,23 +310,18 @@
             fixed_ordering = fixed_ordering_cost_step,
     )
 
     self.period += 1
 
     return reward_norm, info
 
-# %% ../../nbs/environments/10_calculation_functions.ipynb 14
+# %% ../../nbs/environments/10_calculation_functions.ipynb 13
 def nv_calculations(self, action):
-    
-    if self.full_demand:
-        demand = self.demand[self.period+self.full_additional_context, :]
-    else:
-        demand = self.demand[self.period, :]
 
-    # assert that action is not nan
+    demand = self.demand[self.period, :]
 
     if self.mask is not None:
         mask = self.mask.copy()
         if len(self.mask.shape)==1:
             mask = mask.reshape(-1,1)
         mask = mask[self.period, :]
         action = action*mask
@@ -426,30 +337,26 @@
     cost = np.where(remaining_demand > 0, underage_cost * remaining_demand, 0)
     cost += np.where(remaining_demand < 0, overage_cost * np.abs(remaining_demand), 0)
     # cost[remaining_demand > 0] = self.underage_cost * remaining_demand[remaining_demand > 0]
     # cost[remaining_demand < 0] = self.overage_cost * np.abs(remaining_demand[remaining_demand < 0])
 
     reward = -cost.sum()
 
-    # print("demand:", demand, "action:", action, "reward: ", reward)
-
     reward_norm = normalize_reward_NV(self, reward)
-
-    # print(demand[32], action[32])
     
     info = dict(
         demand = demand,
         cost = cost
     )
 
     self.period += 1
 
     return reward_norm, info
 
-# %% ../../nbs/environments/10_calculation_functions.ipynb 16
+# %% ../../nbs/environments/10_calculation_functions.ipynb 15
 def get_fixed_ordering_cost(self, action, positive_only = True):
     """ 
     Returns the fixed ordering cost for the period.
 
     Parameters
     ----------
     action : array
```

### Comparing `RL_OM-0.7.80/RL_OM/environments/data_generators.py` & `RL_OM-0.7.9/RL_OM/environments/data_generators.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/environments/feature_converters.py` & `RL_OM-0.7.9/RL_OM/environments/feature_converters.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.7.80/RL_OM/experiment_functions/run_experiment.py` & `RL_OM-0.7.9/RL_OM/experiment_functions/run_experiment.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,23 +219,21 @@
 
         R_hist.append(R)
         
     return R_hist
 
 # %% ../../nbs/experiment_functions/01_run_experiment.ipynb 8
 def test_agent(agent, mdp, core, logger, artifact, path, run_id, n_episodes_test, n, log_wandb=True, val=False, return_J_R=False, dataset_log_freq = None):
-    
+
     # TODO: Make this into a class to avoid passing the same arguments over and over again
 
+    print("testing agent")
     got_nan = False
 
-    mdp.reset()
-
     dataset, dataset_info = core.evaluate(n_episodes=n_episodes_test, render=False, quiet = True, get_env_info=True)
-
     info_keys = dataset_info.keys()
 
     s, *_ = parse_dataset(dataset)
 
     J = np.mean(compute_J(dataset, mdp.info.gamma))
     R = np.mean(compute_J(dataset))
 
@@ -247,15 +245,15 @@
         E = agent.policy.entropy(s)
 
         if log_wandb:
             if val:
                 wandb.log({"val/J": J, "val/R": R, "val/entropy": E})
             else:
                 wandb.log({"test/J": J, "test/R": R, "test/entropy": E})
-
+    
     else:
         E = None
         if log_wandb:
             if val:
                 wandb.log({"val/J": J, "val/R": R})
             else:
                 wandb.log({"test/J": J, "test/R": R})
@@ -269,22 +267,14 @@
             step_info = dict()
 
             for key in info_keys:
                 step_info[key] = dataset_info[key][i]
 
             dataset[i] = dataset[i] + (step_info,)
 
-        if not mdp.record_state:
-            for i, step_data in enumerate(dataset):
-                # Convert the tuple to a list to modify it
-                modified_step_data = list(step_data)[1:]  # Creates a new list without the first element of the tuple
-                del modified_step_data[2]
-
-                dataset[i] = tuple(modified_step_data)
-        
         # check if n is string:
         if isinstance(n, str):
             logger.log_dataset(dataset, name_addition = f"_{n}")
             if log_wandb:
                 artifact.add_file(f"{path}/{agent.name}_{run_id}/dataset_{n}.pkl", name=f"dataset_{n}")
 
         elif (n) % dataset_log_freq == 0:
@@ -303,15 +293,14 @@
 
     # check class of agent
 
     if hasattr(agent, "agent"):
         agent_class = agent.agent.__class__.__name__
     else:
         agent_class = agent.__class__.__name__
-    
 
     networks = []
 
     if agent_class == "SAC" or agent_class == "TD3":
 
         ensemble_critic = agent._critic_approximator._impl.model
 
@@ -325,15 +314,15 @@
 
     if agent_class == "SAC":
         networks.append(agent.policy._mu_approximator._impl.model.network)
         networks.append(agent.policy._sigma_approximator._impl.model.network)
     elif agent_class == "TD3":
         networks.append(agent.policy._approximator._impl.model.network)
     
-    if ((agent_class == "MLPsgdAgent") or (agent_class == "LagLlamasgdMetaAgent")):
+    if agent_class == "MLPsgdAgent":
         networks.append(agent.model)
  
     path_full = f"{path}/parameters"
     os.makedirs(path_full, exist_ok=True)
 
     for i, network in enumerate(networks):
         network_path = "{}/parameters/network_{}_run_{}.pt".format(path, i, run_id)
@@ -363,23 +352,20 @@
     if agent_class == "SAC":
         networks.append(agent.policy._mu_approximator._impl.model.network)
         networks.append(agent.policy._sigma_approximator._impl.model.network)   
     
     elif agent_class == "TD3":
         networks.append(agent.policy._approximator._impl.model.network)
     
-    if ((agent_class == "MLPsgdAgent") or (agent_class == "LagLlamasgdMetaAgent")):
+    if agent_class == "MLPsgdAgent":
         networks.append(agent.model)
 
     for i, network in enumerate(networks):
-        if run_id is not None:
-            network_path = "{}/parameters/network_{}_run_{}.pt".format(path, i, run_id)
-        else:
-            network_path = path
-        network.load_state_dict(torch.load(network_path, map_location=torch.device(agent.device)))
+        network_path = "{}/parameters/network_{}_run_{}.pt".format(path, i, run_id)
+        network.load_state_dict(torch.load(network_path))
         print("loaded parameters")
 
     # for i, network in enumerate(ensemble_critic):
     #     network_path = "{}/parameters/network_{}_run_{}.pt".format(path, i, run_id)
     #     network.network.load_state_dict(torch.load(network_path))
 
     # _mu_approximator = agent.policy._mu_approximator._impl.model.network
@@ -425,16 +411,14 @@
                         early_stopping_patience = None,
                         early_stopping_warmup = 100,
                         save_best=True,
 
                         num_reruns_nan = 10,
 
                         create_agent_function = None,
-
-                        agent_weights_path = None,
                         
                         ):
 
     """
     # TODO: update docstring
     """
 
@@ -489,15 +473,15 @@
         core_train = Core(agent, mdp_train)
 
         if test_provided:
             core_test = Core(agent, mdp_test)
             core_val = Core(agent, mdp_val) # will use same as test set if no validation set provided
 
         artifact = wandb.Artifact("transitions_dataset", type='dataset')
-        
+
         ### Initial evaluation
         if test_provided:
             # will be implicitly test set, if no validation set provided
             nan = test_agent(agent, mdp_val, core_val, logger, artifact, path, run_id, n_episodes_test, 0, log_wandb=True, val = val_provided, dataset_log_freq = dataset_log_freq)
         else:
             nan = test_agent(agent, mdp_train, core_train, logger, artifact, path, run_id, n_episodes_test, 0, log_wandb=True, dataset_log_freq = dataset_log_freq) 
 
@@ -506,158 +490,149 @@
             continue
         
         stopped_early=False
         J_history = []
 
         ### Training loop outside mushroom_rl env:
 
-        if agent_weights_path is None: # if weights already provided skip training and test with loaded weights
-
-            print("starting training")
-            if hasattr(agent, 'train_directly') and agent.train_directly:
-                if agent.train_mode == "direct":
-                    print("fitting")
-                    agent.fit(features=mdp_train.features, demand=mdp_train.demand, mask=mdp_train.mask)
-                    print("fitted")
-                    if not hasattr(agent, 'skip_val') or not agent.skip_val:
-                        for n in trange(n_epochs):
-                            if n==0:
-                                if test_provided:
-                                    # will be implicitly test set, if no validation set provided
-                                    J, R, nan = test_agent(agent, mdp_val, core_val, logger, artifact, path, run_id, n_episodes_test, 1, log_wandb=True, val = val_provided, return_J_R=True, dataset_log_freq = dataset_log_freq)
-                                else:
-                                    J, R, nan  = test_agent(agent, mdp_train, core_train, logger, artifact, path, run_id, n_episodes_test, 1, log_wandb=True, return_J_R=True, dataset_log_freq = dataset_log_freq) 
-                            else:
-                                if val_provided:
-                                    wandb.log({"val/J": J, "val/R": R})
-                                else:
-                                    wandb.log({"test/J": J, "test/R": R})
-
-                elif agent.train_mode == "epochs":
+        print("starting training")
+        if hasattr(agent, 'train_directly') and agent.train_directly:
+            if agent.train_mode == "direct":
+                print("fitting")
+                agent.fit(features=mdp_train.features, demand=mdp_train.demand, mask=mdp_train.mask)
+                print("fitted")
+                if not hasattr(agent, 'skip_val') or not agent.skip_val:
                     for n in trange(n_epochs):
-
-                        if stopped_early:
-                            wandb.log({"val/J": J, "val/R": R})
-                            continue
-
-                        agent.fit_epoch(mdp_train.features, mdp_train.demand, mask=mdp_train.mask)
-                        
-                        agent.eval()
-                        
-                        if test_provided:
-                            # will be implicitly test set, if no validation set provided
-                            J, R, nan = test_agent(agent, mdp_val, core_val, logger, artifact, path, run_id, n_episodes_test, n+1, log_wandb=True, val = val_provided, dataset_log_freq = dataset_log_freq, return_J_R=True)
+                        if n==0:
+                            if test_provided:
+                                # will be implicitly test set, if no validation set provided
+                                J, R, nan = test_agent(agent, mdp_val, core_val, logger, artifact, path, run_id, n_episodes_test, 1, log_wandb=True, val = val_provided, return_J_R=True, dataset_log_freq = dataset_log_freq)
+                            else:
+                                J, R, nan  = test_agent(agent, mdp_train, core_train, logger, artifact, path, run_id, n_episodes_test, 1, log_wandb=True, return_J_R=True, dataset_log_freq = dataset_log_freq) 
                         else:
-                            J, R, nan = test_agent(agent, mdp_train, core_train, logger, artifact, path, run_id, n_episodes_test, n+1, log_wandb=True, dataset_log_freq = dataset_log_freq, return_J_R=True)   
-                        
-                        agent.train()
-                        
-                        J_history.append(J)
-
-                        if save_best:
-                            if J >= np.max(J_history):
-                                print("saving networks")
-                                save_networks(agent, path, run_id)
-
-                        if early_stopping_patience is not None:
-                            if n > early_stopping_warmup and n > 2*early_stopping_patience:
-                                if np.mean(J_history[-early_stopping_patience:]) <= np.mean(J_history[-2*early_stopping_patience:-early_stopping_patience]):
-                                    print("early stopping")
-                                    stopped_early = True
-                else:
-                    raise ValueError("train_mode not recognized")
-                    
-            else:
-                ### Training
-                if hasattr(agent.policy, 'train'):
-                    agent.policy.train()
-
-                if hasattr(agent, "_replay_memory"):
-                    initial_replay_size = agent._replay_memory._initial_size
-                    core_train.learn(n_steps=initial_replay_size, n_steps_per_fit=initial_replay_size, quiet=True)
+                            if val_provided:
+                                wandb.log({"val/J": J, "val/R": R})
+                            else:
+                                wandb.log({"test/J": J, "test/R": R})
 
-                for n in trange(n_epochs, leave=False):
+            elif agent.train_mode == "epochs":
+                for n in trange(n_epochs):
 
                     if stopped_early:
                         wandb.log({"val/J": J, "val/R": R})
                         continue
 
-                    try:
-
-                        core_train.learn(n_steps=n_steps, n_steps_per_fit=n_steps_per_fit, quiet = True)
-                        if hasattr(agent.policy, 'eval'):
-                            agent.policy.eval()
-                        if test_provided:
-                            # will be implicitly test set, if no validation set provided
-                            J, R, nan = test_agent(agent, mdp_val, core_val, logger, artifact, path, run_id, n_episodes_test, n+1, log_wandb=True, val = val_provided, return_J_R=True, dataset_log_freq = dataset_log_freq)
-                        else:
-                            J, R, nan = test_agent(agent, mdp_train, core_train, logger, artifact, path, run_id, n_episodes_test, n+1, log_wandb=True, return_J_R=True, dataset_log_freq = dataset_log_freq)  
-
-                    except Exception as e:
-
-                                # exit gracefully, so wandb logs the problem
-                        print(traceback.print_exc(), file=sys.stderr)
-                        exit(1)
-                        
-                    if nan:
-                        break
-
-                    J_history.append(J)
+                    agent.fit_epoch(mdp_train.features, mdp_train.demand, mask=mdp_train.mask)
+                    
+                    agent.eval()
                     
-                    if hasattr(agent.policy, 'train'):
-                        agent.policy.train()
+                    if test_provided:
+                        # will be implicitly test set, if no validation set provided
+                        J, R, nan = test_agent(agent, mdp_val, core_val, logger, artifact, path, run_id, n_episodes_test, n+1, log_wandb=True, val = val_provided, dataset_log_freq = dataset_log_freq, return_J_R=True)
+                    else:
+                        J, R, nan = test_agent(agent, mdp_train, core_train, logger, artifact, path, run_id, n_episodes_test, n+1, log_wandb=True, dataset_log_freq = dataset_log_freq, return_J_R=True)   
                     
+                    agent.train()
+                    
+                    J_history.append(J)
+
                     if save_best:
                         if J >= np.max(J_history):
                             save_networks(agent, path, run_id)
 
                     if early_stopping_patience is not None:
                         if n > early_stopping_warmup and n > 2*early_stopping_patience:
                             if np.mean(J_history[-early_stopping_patience:]) <= np.mean(J_history[-2*early_stopping_patience:-early_stopping_patience]):
                                 print("early stopping")
                                 stopped_early = True
+            else:
+                raise ValueError("train_mode not recognized")
+                
+        else:
+            print("starting training")
+            ### Training
+            if hasattr(agent.policy, 'train'):
+                agent.policy.train()
+                print("setting train flag")
+
+            if hasattr(agent, "_replay_memory"):
+                initial_replay_size = agent._replay_memory._initial_size
+                core_train.learn(n_steps=initial_replay_size, n_steps_per_fit=initial_replay_size, quiet=True)
+
+            for n in trange(n_epochs, leave=False):
+
+                if stopped_early:
+                    wandb.log({"val/J": J, "val/R": R})
+                    continue
+
+                try:
+
+                    core_train.learn(n_steps=n_steps, n_steps_per_fit=n_steps_per_fit, quiet = True)
+                    if hasattr(agent.policy, 'eval'):
+                        agent.policy.eval()
+                    if test_provided:
+                        # will be implicitly test set, if no validation set provided
+                        J, R, nan = test_agent(agent, mdp_val, core_val, logger, artifact, path, run_id, n_episodes_test, n+1, log_wandb=True, val = val_provided, return_J_R=True, dataset_log_freq = dataset_log_freq)
+                    else:
+                        J, R, nan = test_agent(agent, mdp_train, core_train, logger, artifact, path, run_id, n_episodes_test, n+1, log_wandb=True, return_J_R=True, dataset_log_freq = dataset_log_freq)  
+
+                except Exception as e:
+
+                            # exit gracefully, so wandb logs the problem
+                    print(traceback.print_exc(), file=sys.stderr)
+                    exit(1)
                     
-        ### Final evaluation
+                if nan:
+                    break
+
+                J_history.append(J)
+                
+                if hasattr(agent.policy, 'train'):
+                    agent.policy.train()
+                
+                if save_best:
+                    if J >= np.max(J_history):
+                        save_networks(agent, path, run_id)
+
+                if early_stopping_patience is not None:
+                    if n > early_stopping_warmup and n > 2*early_stopping_patience:
+                        if np.mean(J_history[-early_stopping_patience:]) <= np.mean(J_history[-2*early_stopping_patience:-early_stopping_patience]):
+                            print("early stopping")
+                            stopped_early = True
+                
+            ### Final evaluation
         
         if nan:
             print("got nan, rerunning with num_re-runs = ", num_runs)
             continue
 
         print("doing final evaluation with last model on test set")
         if hasattr(agent.policy, 'eval'):
             agent.policy.eval()
 
-        if agent_weights_path is not None:
-
-            load_networks(agent, path = agent_weights_path, run_id=None)
-
-            nan = test_agent(agent, mdp_test, core_test, logger, artifact, path, run_id, n_episodes_test, "test_best", log_wandb=True, val = False, return_J_R=False, dataset_log_freq = dataset_log_freq)
-
+        if test_provided:
+            # will always use test set
+            nan = test_agent(agent, mdp_test, core_test, logger, artifact, path, run_id, n_episodes_test, "test_last", log_wandb=True, val = False, return_J_R=False, dataset_log_freq = dataset_log_freq)
         else:
+            nan = test_agent(agent, mdp_train, core_train, logger, artifact, path, run_id, n_episodes_test, "train_last", log_wandb=True, return_J_R=False, dataset_log_freq = dataset_log_freq)   
+
+        if save_best and (not hasattr(agent, 'train_directly') or agent.train_mode == "epochs"):
+            print("doing final evaluation with best model on test set")
+            # load saved networks
+            
+            load_networks(agent, path, run_id)
 
+            if hasattr(agent.policy, 'eval'):
+                agent.policy.eval()
+        
             if test_provided:
                 # will always use test set
-                nan = test_agent(agent, mdp_test, core_test, logger, artifact, path, run_id, n_episodes_test, "test_last", log_wandb=True, val = False, return_J_R=False, dataset_log_freq = dataset_log_freq)
+                nan = test_agent(agent, mdp_test, core_test, logger, artifact, path, run_id, n_episodes_test, "test_best", log_wandb=True, val = False, return_J_R=False, dataset_log_freq = dataset_log_freq)
             else:
-                nan = test_agent(agent, mdp_train, core_train, logger, artifact, path, run_id, n_episodes_test, "train_last", log_wandb=True, return_J_R=False, dataset_log_freq = dataset_log_freq)   
-
-            if save_best and (not hasattr(agent, 'train_directly') or agent.train_mode == "epochs"):
-                print("doing final evaluation with best model on test set")
-                # load saved networks
-                
-                load_networks(agent, path, run_id)
-
-                if hasattr(agent.policy, 'eval'):
-                    agent.policy.eval()
-            
-                if test_provided:
-                    # will always use test set
-                    nan = test_agent(agent, mdp_test, core_test, logger, artifact, path, run_id, n_episodes_test, "test_best", log_wandb=True, val = False, return_J_R=False, dataset_log_freq = dataset_log_freq)
-                else:
-                    nan = test_agent(agent, mdp_train, core_train, logger, artifact, path, run_id, n_episodes_test, "train_best", log_wandb=True, return_J_R=False, dataset_log_freq = dataset_log_freq) 
+                nan = test_agent(agent, mdp_train, core_train, logger, artifact, path, run_id, n_episodes_test, "train_best", log_wandb=True, return_J_R=False, dataset_log_freq = dataset_log_freq) 
         
         if nan:
             print("got nan, rerunning with num_re-runs = ", num_runs)
         else:
             break
         
     wandb.log_artifact(artifact)
```

### Comparing `RL_OM-0.7.80/RL_OM/utils/utils.py` & `RL_OM-0.7.9/RL_OM/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# AUTOGENERATED! DO NOT EDIT! File to edit: ../../nbs/utils/01_utils.ipynb.
+# AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/utils/01_utils.ipynb.
 
 # %% auto 0
 __all__ = ['combine_dict', 'convert_str_none_to_none', 'load_agent_function', 'merge_with_namespace',
            'delete_lag_window_from_config', 'get_git_revision_hash', 'get_version', 'init_pipeline',
            'prepare_hyperparameter_opt', 'prepare_lag_window', 'prepare_calculation_function',
            'get_actions_per_product', 'track_normalization', 'create_env_agent']
 
-# %% ../../nbs/utils/01_utils.ipynb 4
+# %% ../nbs/utils/01_utils.ipynb 4
 # General libraries:
 # import numpy as np
 # import pickle
 import yaml
 # import os
 # from tqdm import tqdm, trange
 import wandb
 import datetime
 import torch
 import pkg_resources
 # import sys,traceback
 
-# %% ../../nbs/utils/01_utils.ipynb 6
+# %% ../nbs/utils/01_utils.ipynb 6
 def combine_dict(dict1, dict2):
 
     """
     Combines two dictionaries. Raises error if there are overlapping keys.
 
     Args:
         dict1 (dict): First dictionary
@@ -154,15 +154,15 @@
         version = pkg_resources.get_distribution(library_name).version
         return version
     except pkg_resources.DistributionNotFound:
         print(f"Library '{library_name}' not found.")
         return "Not Installed"
     
 
-# %% ../../nbs/utils/01_utils.ipynb 8
+# %% ../nbs/utils/01_utils.ipynb 8
 def init_pipeline(config_env, config_train, config_agent, project_name):
 
     torch.set_num_threads(1)
 
     try:
         sweep_config = wandb.config
     except:
@@ -205,14 +205,15 @@
             pass
     
     if not success:
         experiment_hash = None
     
     return config_env, config_train, config_agent, sweep_config, rl_om_hash, mushroom_fork_hash, experiment_hash
 
+
 def prepare_hyperparameter_opt():
         
     if 'hyperparameter_opt' in wandb.config._items:
         hyperparameter_opt = wandb.config._items['hyperparameter_opt']
     else:
         hyperparameter_opt = None
```

### Comparing `RL_OM-0.7.80/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.7.9/RL_OM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.7.80
+Version: 0.7.9
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.7.80/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.7.9/RL_OM.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 settings.ini
 setup.py
-RL_OM/MLtools.py
 RL_OM/__init__.py
 RL_OM/_modidx 2.py
 RL_OM/_modidx.py
 RL_OM/core.py
 RL_OM/utils.py
 RL_OM.egg-info/PKG-INFO
 RL_OM.egg-info/SOURCES.txt
@@ -22,15 +21,14 @@
 RL_OM/agents/benchmark_agents/__init__.py
 RL_OM/agents/benchmark_agents/cbs.py
 RL_OM/agents/benchmark_agents/eoq.py
 RL_OM/agents/benchmark_agents/mp_agents_ERM.py
 RL_OM/agents/benchmark_agents/nv_agents.py
 RL_OM/agents/benchmark_agents/nv_agents_ERM.py
 RL_OM/agents/benchmark_agents/nv_agents_SAA.py
-RL_OM/agents/benchmark_agents/nv_agents_gradient_boosting.py
 RL_OM/agents/benchmark_agents/qr.py
 RL_OM/agents/benchmark_agents/saa.py
 RL_OM/agents/benchmark_agents/ss.py
 RL_OM/agents/networks/__init__.py
 RL_OM/agents/networks/actors.py
 RL_OM/agents/networks/base.py
 RL_OM/agents/networks/critics.py
@@ -60,11 +58,8 @@
 RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
 RL_OM/environments/__init__.py
 RL_OM/environments/calculation_functions.py
 RL_OM/environments/data_generators.py
 RL_OM/environments/feature_converters.py
 RL_OM/environments/multi_period_inventory.py
 RL_OM/experiment_functions/__init__.py
-RL_OM/experiment_functions/run_experiment.py
-RL_OM/utils/MLtools.py
-RL_OM/utils/__init__.py
-RL_OM/utils/utils.py
+RL_OM/experiment_functions/run_experiment.py
```

### Comparing `RL_OM-0.7.80/settings.ini` & `RL_OM-0.7.9/settings.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.7.80
+version = 0.7.9
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.7.80/setup.py` & `RL_OM-0.7.9/setup.py`

 * *Files identical despite different names*

