# Comparing `tmp/ev2gym-0.0.12.tar.gz` & `tmp/ev2gym-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ev2gym-0.0.12.tar", last modified: Sun Mar 17 23:51:31 2024, max compression
+gzip compressed data, was "ev2gym-1.0.0.tar", last modified: Tue Apr  2 15:00:21 2024, max compression
```

## Comparing `ev2gym-0.0.12.tar` & `ev2gym-1.0.0.tar`

### file list

```diff
@@ -1,92 +1,82 @@
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.852784 ev2gym-0.0.12/
--rw-rw-rw-   0        0        0     1098 2024-03-17 23:49:34.000000 ev2gym-0.0.12/LICENSE
--rw-rw-rw-   0        0        0     2792 2024-03-17 23:51:31.851783 ev2gym-0.0.12/PKG-INFO
--rw-rw-rw-   0        0        0     2174 2024-03-17 23:39:48.000000 ev2gym-0.0.12/README.md
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.753766 ev2gym-0.0.12/ev2gym/
--rw-rw-rw-   0        0        0      214 2024-03-17 23:42:56.000000 ev2gym-0.0.12/ev2gym/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.767269 ev2gym-0.0.12/ev2gym/baselines/
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.771770 ev2gym-0.0.12/ev2gym/baselines/DDPG/
--rw-rw-rw-   0        0        0        0 2024-01-20 21:41:01.000000 ev2gym-0.0.12/ev2gym/baselines/DDPG/__init__.py
--rw-rw-rw-   0        0        0    10184 2024-03-17 23:37:54.000000 ev2gym-0.0.12/ev2gym/baselines/DDPG/ddpg.py
--rw-rw-rw-   0        0        0     3220 2024-01-23 14:58:15.000000 ev2gym-0.0.12/ev2gym/baselines/DDPG/nets.py
--rw-rw-rw-   0        0        0     3239 2024-01-08 19:41:53.000000 ev2gym-0.0.12/ev2gym/baselines/DDPG/noise.py
--rw-rw-rw-   0        0        0      884 2024-01-08 19:41:53.000000 ev2gym-0.0.12/ev2gym/baselines/DDPG/replay_memory.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.772770 ev2gym-0.0.12/ev2gym/baselines/DT/
--rw-rw-rw-   0        0        0        0 2024-01-20 21:41:11.000000 ev2gym-0.0.12/ev2gym/baselines/DT/__init__.py
--rw-rw-rw-   0        0        0        0 2024-01-20 21:33:22.000000 ev2gym-0.0.12/ev2gym/baselines/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.775271 ev2gym-0.0.12/ev2gym/baselines/gurobi_models/
--rw-rw-rw-   0        0        0       57 2024-01-08 19:41:53.000000 ev2gym-0.0.12/ev2gym/baselines/gurobi_models/__init__.py
--rw-rw-rw-   0        0        0    17708 2024-02-28 14:30:56.000000 ev2gym-0.0.12/ev2gym/baselines/gurobi_models/profit_max.py
--rw-rw-rw-   0        0        0    21519 2024-03-14 15:20:30.000000 ev2gym-0.0.12/ev2gym/baselines/gurobi_models/tracking_error.py
--rw-rw-rw-   0        0        0     7730 2024-03-14 22:33:10.000000 ev2gym-0.0.12/ev2gym/baselines/heuristics.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.807277 ev2gym-0.0.12/ev2gym/data/
--rw-rw-rw-   0        0        0  4515614 2023-11-09 21:56:28.000000 ev2gym-0.0.12/ev2gym/data/Netherlands_day-ahead-2015-2023.csv
--rw-rw-rw-   0        0        0        0 2024-01-20 22:10:37.000000 ev2gym-0.0.12/ev2gym/data/__init__.py
--rw-rw-rw-   0        0        0     1677 2023-10-10 08:55:57.000000 ev2gym-0.0.12/ev2gym/data/development-in-power-dem.csv
--rw-rw-rw-   0        0        0     4277 2023-10-10 08:55:57.000000 ev2gym-0.0.12/ev2gym/data/distribution-of-arrival-weekend.csv
--rw-rw-rw-   0        0        0     5900 2023-10-10 08:55:57.000000 ev2gym-0.0.12/ev2gym/data/distribution-of-arrival.csv
--rw-rw-rw-   0        0        0      808 2023-10-10 08:55:57.000000 ev2gym-0.0.12/ev2gym/data/distribution-of-charging.csv
--rw-rw-rw-   0        0        0     1699 2023-10-16 11:41:24.000000 ev2gym-0.0.12/ev2gym/data/distribution-of-connection-time.csv
--rw-rw-rw-   0        0        0     1762 2023-10-16 11:41:24.000000 ev2gym-0.0.12/ev2gym/data/distribution-of-energy-demand.csv
--rw-rw-rw-   0        0        0     2625 2024-02-15 18:40:19.000000 ev2gym-0.0.12/ev2gym/data/eda_day-ahead_prices.py
--rw-rw-rw-   0        0        0     4632 2024-02-14 20:09:08.000000 ev2gym-0.0.12/ev2gym/data/elaad_data_eda.py
--rw-rw-rw-   0        0        0     4555 2024-03-14 15:07:25.000000 ev2gym-0.0.12/ev2gym/data/ev_specs.json
--rw-rw-rw-   0        0        0     2573 2024-02-06 19:47:09.000000 ev2gym-0.0.12/ev2gym/data/loads_eda.py
--rw-rw-rw-   0        0        0     2499 2024-02-11 12:26:09.000000 ev2gym-0.0.12/ev2gym/data/mean-demand-per-arrival.csv
--rw-rw-rw-   0        0        0      938 2024-02-11 13:01:21.000000 ev2gym-0.0.12/ev2gym/data/mean-session-length-per.csv
--rw-rw-rw-   0        0        0   341513 2024-02-15 18:40:19.000000 ev2gym-0.0.12/ev2gym/data/pv_netherlands.csv
--rw-rw-rw-   0        0        0  5182017 2024-02-06 19:47:09.000000 ev2gym-0.0.12/ev2gym/data/residential_loads.csv
--rw-rw-rw-   0        0        0     9344 2023-10-16 11:41:24.000000 ev2gym-0.0.12/ev2gym/data/time_of_connection_vs_hour.npy
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.815278 ev2gym-0.0.12/ev2gym/example_config_files/
--rw-rw-rw-   0        0        0     5278 2024-03-14 15:19:23.000000 ev2gym-0.0.12/ev2gym/example_config_files/BusinessPST.yaml
--rw-rw-rw-   0        0        0     5336 2024-03-10 09:57:45.000000 ev2gym-0.0.12/ev2gym/example_config_files/PublicPST.yaml
--rw-rw-rw-   0        0        0     5240 2024-03-06 22:50:47.000000 ev2gym-0.0.12/ev2gym/example_config_files/V2GProfitMax.yaml
--rw-rw-rw-   0        0        0     5332 2024-03-10 09:58:08.000000 ev2gym-0.0.12/ev2gym/example_config_files/V2GProfitPlusLoads.yaml
--rw-rw-rw-   0        0        0     1468 2024-03-17 22:53:34.000000 ev2gym-0.0.12/ev2gym/example_config_files/V2G_MPC.yaml
--rw-rw-rw-   0        0        0     1466 2024-03-16 07:23:08.000000 ev2gym-0.0.12/ev2gym/example_config_files/V2G_MPC2.yaml
--rw-rw-rw-   0        0        0        0 2024-01-20 22:03:16.000000 ev2gym-0.0.12/ev2gym/example_config_files/__init__.py
--rw-rw-rw-   0        0        0     2614 2024-02-25 08:34:56.000000 ev2gym-0.0.12/ev2gym/example_config_files/charging_topology_10.json
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.822779 ev2gym-0.0.12/ev2gym/models/
--rw-rw-rw-   0        0        0        0 2024-01-20 10:42:21.000000 ev2gym-0.0.12/ev2gym/models/__init__.py
--rw-rw-rw-   0        0        0    17415 2024-03-10 09:35:29.000000 ev2gym-0.0.12/ev2gym/models/ev.py
--rw-rw-rw-   0        0        0    24222 2024-03-17 23:40:46.000000 ev2gym-0.0.12/ev2gym/models/ev2gym_env.py
--rw-rw-rw-   0        0        0    11737 2024-02-23 23:13:20.000000 ev2gym-0.0.12/ev2gym/models/ev_charger.py
--rw-rw-rw-   0        0        0     5666 2024-01-13 12:10:07.000000 ev2gym-0.0.12/ev2gym/models/grid.py
--rw-rw-rw-   0        0        0     9595 2024-03-17 23:37:54.000000 ev2gym-0.0.12/ev2gym/models/replay.py
--rw-rw-rw-   0        0        0    13019 2024-03-06 23:39:33.000000 ev2gym-0.0.12/ev2gym/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.826279 ev2gym-0.0.12/ev2gym/rl_agent/
--rw-rw-rw-   0        0        0        0 2024-01-20 21:32:54.000000 ev2gym-0.0.12/ev2gym/rl_agent/__init__.py
--rw-rw-rw-   0        0        0     8752 2024-03-04 22:29:20.000000 ev2gym-0.0.12/ev2gym/rl_agent/reward.py
--rw-rw-rw-   0        0        0     8560 2024-02-28 09:59:32.000000 ev2gym-0.0.12/ev2gym/rl_agent/state.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.831280 ev2gym-0.0.12/ev2gym/utilities/
--rw-rw-rw-   0        0        0        0 2024-01-20 21:46:43.000000 ev2gym-0.0.12/ev2gym/utilities/__init__.py
--rw-rw-rw-   0        0        0     3255 2024-03-17 23:39:48.000000 ev2gym-0.0.12/ev2gym/utilities/arg_parser.py
--rw-rw-rw-   0        0        0    19041 2024-03-17 23:39:48.000000 ev2gym-0.0.12/ev2gym/utilities/loaders.py
--rw-rw-rw-   0        0        0    21051 2024-03-17 23:37:54.000000 ev2gym-0.0.12/ev2gym/utilities/utils.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.837782 ev2gym-0.0.12/ev2gym/vizuals/
--rw-rw-rw-   0        0        0        0 2024-01-20 21:36:12.000000 ev2gym-0.0.12/ev2gym/vizuals/__init__.py
--rw-rw-rw-   0        0        0    29073 2024-03-17 23:40:48.000000 ev2gym-0.0.12/ev2gym/vizuals/evaluator_plot.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.847783 ev2gym-0.0.12/ev2gym/vizuals/icons/
--rw-rw-rw-   0        0        0        0 2024-01-21 22:33:26.000000 ev2gym-0.0.12/ev2gym/vizuals/icons/__init__.py
--rw-rw-rw-   0        0        0    35984 2024-01-08 19:41:53.000000 ev2gym-0.0.12/ev2gym/vizuals/icons/algorithm.png
--rw-rw-rw-   0        0        0    13646 2024-01-08 19:41:53.000000 ev2gym-0.0.12/ev2gym/vizuals/icons/charger_wallbox.png
--rw-rw-rw-   0        0        0    12744 2024-01-08 19:41:53.000000 ev2gym-0.0.12/ev2gym/vizuals/icons/charging-station_1_port.png
--rw-rw-rw-   0        0        0    11172 2024-01-08 19:41:53.000000 ev2gym-0.0.12/ev2gym/vizuals/icons/charging-station_2_ports.png
--rw-rw-rw-   0        0        0    30600 2024-01-08 19:41:53.000000 ev2gym-0.0.12/ev2gym/vizuals/icons/cpo.png
--rw-rw-rw-   0        0        0    18138 2024-01-08 19:41:53.000000 ev2gym-0.0.12/ev2gym/vizuals/icons/ev.png
--rw-rw-rw-   0        0        0    31261 2024-01-08 19:41:53.000000 ev2gym-0.0.12/ev2gym/vizuals/icons/ev2.png
--rw-rw-rw-   0        0        0    18679 2024-01-08 19:41:53.000000 ev2gym-0.0.12/ev2gym/vizuals/icons/logo.png
--rw-rw-rw-   0        0        0    13236 2024-01-08 19:41:53.000000 ev2gym-0.0.12/ev2gym/vizuals/icons/transformer.png
--rw-rw-rw-   0        0        0    24674 2024-03-16 07:24:50.000000 ev2gym-0.0.12/ev2gym/vizuals/plots.py
--rw-rw-rw-   0        0        0    13232 2024-03-17 23:39:48.000000 ev2gym-0.0.12/ev2gym/vizuals/render.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.850784 ev2gym-0.0.12/ev2gym.egg-info/
--rw-rw-rw-   0        0        0     2792 2024-03-17 23:51:31.000000 ev2gym-0.0.12/ev2gym.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2483 2024-03-17 23:51:31.000000 ev2gym-0.0.12/ev2gym.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-17 23:51:31.000000 ev2gym-0.0.12/ev2gym.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-03-17 23:51:31.000000 ev2gym-0.0.12/ev2gym.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-03-17 23:51:31.000000 ev2gym-0.0.12/ev2gym.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-17 23:51:31.852784 ev2gym-0.0.12/setup.cfg
--rw-rw-rw-   0        0        0     1244 2024-03-17 23:39:48.000000 ev2gym-0.0.12/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-17 23:51:31.849784 ev2gym-0.0.12/tests/
--rw-rw-rw-   0        0        0     9731 2024-03-17 23:37:54.000000 ev2gym-0.0.12/tests/test_degradation.py
--rw-rw-rw-   0        0        0    18300 2024-03-17 23:40:48.000000 ev2gym-0.0.12/tests/test_ev_behavior.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:00:21.796309 ev2gym-1.0.0/
+-rw-rw-rw-   0        0        0     1098 2024-03-18 00:03:15.000000 ev2gym-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0    13984 2024-04-02 15:00:21.795309 ev2gym-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    13359 2024-04-02 14:57:42.000000 ev2gym-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-02 15:00:21.536225 ev2gym-1.0.0/ev2gym/
+-rw-rw-rw-   0        0        0      214 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:00:21.554106 ev2gym-1.0.0/ev2gym/baselines/
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/baselines/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:00:21.556105 ev2gym-1.0.0/ev2gym/baselines/gurobi_models/
+-rw-rw-rw-   0        0        0       57 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/baselines/gurobi_models/__init__.py
+-rw-rw-rw-   0        0        0    17708 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/baselines/gurobi_models/profit_max.py
+-rw-rw-rw-   0        0        0    21519 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/baselines/gurobi_models/tracking_error.py
+-rw-rw-rw-   0        0        0     7730 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/baselines/heuristics.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:00:21.689555 ev2gym-1.0.0/ev2gym/data/
+-rw-rw-rw-   0        0        0  4515614 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/Netherlands_day-ahead-2015-2023.csv
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/__init__.py
+-rw-rw-rw-   0        0        0     1677 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/development-in-power-dem.csv
+-rw-rw-rw-   0        0        0     4277 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/distribution-of-arrival-weekend.csv
+-rw-rw-rw-   0        0        0     5900 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/distribution-of-arrival.csv
+-rw-rw-rw-   0        0        0      808 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/distribution-of-charging.csv
+-rw-rw-rw-   0        0        0     1699 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/distribution-of-connection-time.csv
+-rw-rw-rw-   0        0        0     1762 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/distribution-of-energy-demand.csv
+-rw-rw-rw-   0        0        0     2625 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/eda_day-ahead_prices.py
+-rw-rw-rw-   0        0        0     4632 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/elaad_data_eda.py
+-rw-rw-rw-   0        0        0     4555 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/ev_specs.json
+-rw-rw-rw-   0        0        0     2573 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/loads_eda.py
+-rw-rw-rw-   0        0        0     2547 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/mean-demand-per-arrival.csv
+-rw-rw-rw-   0        0        0      986 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/mean-session-length-per.csv
+-rw-rw-rw-   0        0        0   341513 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/pv_netherlands.csv
+-rw-rw-rw-   0        0        0  5182017 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/residential_loads.csv
+-rw-rw-rw-   0        0        0     9344 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/data/time_of_connection_vs_hour.npy
+drwxrwxrwx   0        0        0        0 2024-04-02 15:00:21.739108 ev2gym-1.0.0/ev2gym/example_config_files/
+-rw-rw-rw-   0        0        0     5304 2024-03-26 09:12:08.000000 ev2gym-1.0.0/ev2gym/example_config_files/BusinessPST.yaml
+-rw-rw-rw-   0        0        0     5337 2024-03-26 17:22:30.000000 ev2gym-1.0.0/ev2gym/example_config_files/PublicPST.yaml
+-rw-rw-rw-   0        0        0     5240 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/example_config_files/V2GProfitMax.yaml
+-rw-rw-rw-   0        0        0     5332 2024-03-18 19:28:37.000000 ev2gym-1.0.0/ev2gym/example_config_files/V2GProfitPlusLoads.yaml
+-rw-rw-rw-   0        0        0     1468 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/example_config_files/V2G_MPC.yaml
+-rw-rw-rw-   0        0        0     1466 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/example_config_files/V2G_MPC2.yaml
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/example_config_files/__init__.py
+-rw-rw-rw-   0        0        0     2614 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/example_config_files/charging_topology_10.json
+-rw-rw-rw-   0        0        0     5335 2024-04-02 14:57:42.000000 ev2gym-1.0.0/ev2gym/example_config_files/simplePST.yaml
+drwxrwxrwx   0        0        0        0 2024-04-02 15:00:21.744109 ev2gym-1.0.0/ev2gym/models/
+-rw-rw-rw-   0        0        0        0 2024-01-20 10:42:21.000000 ev2gym-1.0.0/ev2gym/models/__init__.py
+-rw-rw-rw-   0        0        0    17415 2024-03-10 09:35:29.000000 ev2gym-1.0.0/ev2gym/models/ev.py
+-rw-rw-rw-   0        0        0    24671 2024-04-02 14:57:42.000000 ev2gym-1.0.0/ev2gym/models/ev2gym_env.py
+-rw-rw-rw-   0        0        0    11737 2024-02-23 23:13:20.000000 ev2gym-1.0.0/ev2gym/models/ev_charger.py
+-rw-rw-rw-   0        0        0     5666 2024-01-13 12:10:07.000000 ev2gym-1.0.0/ev2gym/models/grid.py
+-rw-rw-rw-   0        0        0     9595 2024-03-17 23:37:54.000000 ev2gym-1.0.0/ev2gym/models/replay.py
+-rw-rw-rw-   0        0        0    13019 2024-03-06 23:39:33.000000 ev2gym-1.0.0/ev2gym/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:00:21.746609 ev2gym-1.0.0/ev2gym/rl_agent/
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/rl_agent/__init__.py
+-rw-rw-rw-   0        0        0     8752 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/rl_agent/reward.py
+-rw-rw-rw-   0        0        0     8560 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/rl_agent/state.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:00:21.749110 ev2gym-1.0.0/ev2gym/utilities/
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/utilities/__init__.py
+-rw-rw-rw-   0        0        0     3262 2024-04-02 14:57:42.000000 ev2gym-1.0.0/ev2gym/utilities/arg_parser.py
+-rw-rw-rw-   0        0        0    19045 2024-03-26 17:19:23.000000 ev2gym-1.0.0/ev2gym/utilities/loaders.py
+-rw-rw-rw-   0        0        0    21051 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/utilities/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:00:21.752110 ev2gym-1.0.0/ev2gym/visuals/
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/__init__.py
+-rw-rw-rw-   0        0        0    29073 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/evaluator_plot.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:00:21.793808 ev2gym-1.0.0/ev2gym/visuals/icons/
+-rw-rw-rw-   0        0        0        0 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/icons/__init__.py
+-rw-rw-rw-   0        0        0    35984 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/icons/algorithm.png
+-rw-rw-rw-   0        0        0    13646 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/icons/charger_wallbox.png
+-rw-rw-rw-   0        0        0    12744 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/icons/charging-station_1_port.png
+-rw-rw-rw-   0        0        0    11172 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/icons/charging-station_2_ports.png
+-rw-rw-rw-   0        0        0    30600 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/icons/cpo.png
+-rw-rw-rw-   0        0        0    18138 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/icons/ev.png
+-rw-rw-rw-   0        0        0    31261 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/icons/ev2.png
+-rw-rw-rw-   0        0        0    18679 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/icons/logo.png
+-rw-rw-rw-   0        0        0    13236 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/icons/transformer.png
+-rw-rw-rw-   0        0        0    24674 2024-03-18 00:03:15.000000 ev2gym-1.0.0/ev2gym/visuals/plots.py
+-rw-rw-rw-   0        0        0    13316 2024-03-26 09:07:34.000000 ev2gym-1.0.0/ev2gym/visuals/render.py
+drwxrwxrwx   0        0        0        0 2024-04-02 15:00:21.794808 ev2gym-1.0.0/ev2gym.egg-info/
+-rw-rw-rw-   0        0        0    13984 2024-04-02 15:00:21.000000 ev2gym-1.0.0/ev2gym.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2278 2024-04-02 15:00:21.000000 ev2gym-1.0.0/ev2gym.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-02 15:00:21.000000 ev2gym-1.0.0/ev2gym.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-04-02 15:00:21.000000 ev2gym-1.0.0/ev2gym.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-02 15:00:21.000000 ev2gym-1.0.0/ev2gym.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-02 15:00:21.796309 ev2gym-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1253 2024-04-02 14:58:45.000000 ev2gym-1.0.0/setup.py
```

### Comparing `ev2gym-0.0.12/LICENSE` & `ev2gym-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/baselines/gurobi_models/profit_max.py` & `ev2gym-1.0.0/ev2gym/baselines/gurobi_models/profit_max.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/baselines/gurobi_models/tracking_error.py` & `ev2gym-1.0.0/ev2gym/baselines/gurobi_models/tracking_error.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/baselines/heuristics.py` & `ev2gym-1.0.0/ev2gym/baselines/heuristics.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/Netherlands_day-ahead-2015-2023.csv` & `ev2gym-1.0.0/ev2gym/data/Netherlands_day-ahead-2015-2023.csv`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/development-in-power-dem.csv` & `ev2gym-1.0.0/ev2gym/data/development-in-power-dem.csv`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/distribution-of-arrival-weekend.csv` & `ev2gym-1.0.0/ev2gym/data/distribution-of-arrival-weekend.csv`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/distribution-of-arrival.csv` & `ev2gym-1.0.0/ev2gym/data/distribution-of-arrival.csv`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/distribution-of-charging.csv` & `ev2gym-1.0.0/ev2gym/data/distribution-of-charging.csv`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/distribution-of-connection-time.csv` & `ev2gym-1.0.0/ev2gym/data/distribution-of-connection-time.csv`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/distribution-of-energy-demand.csv` & `ev2gym-1.0.0/ev2gym/data/distribution-of-energy-demand.csv`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/eda_day-ahead_prices.py` & `ev2gym-1.0.0/ev2gym/data/eda_day-ahead_prices.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/elaad_data_eda.py` & `ev2gym-1.0.0/ev2gym/data/elaad_data_eda.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/ev_specs.json` & `ev2gym-1.0.0/ev2gym/data/ev_specs.json`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/loads_eda.py` & `ev2gym-1.0.0/ev2gym/data/loads_eda.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/mean-demand-per-arrival.csv` & `ev2gym-1.0.0/ev2gym/data/mean-demand-per-arrival.csv`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-﻿"Arrival Time","home","public","work"
-"00:00",30.8297799511002,20.8705986179664
-"05:00",22.0435135135135,20.2595417709451,10.8555097087379
-"00:30",32.0270384615385,20.894369779523
-"05:30",21.0539655172414,19.7498010971903,13.5385333333333
-"01:00",32.4321327967807,21.0355386961029
-"06:00",20.6445652173913,19.1001881870259,12.2773303249097
-"01:30",32.504872611465,21.4336501128668
-"06:30",21.4597902097902,18.6876522134765,13.5467311178248
-"02:00",29.508,21.6300245220831
-"07:00",17.5342777777778,16.6522399668831,11.9299762859051
-"02:30",26.4673456790123,21.2612758882766
-"07:30",18.5670903010033,15.2372158312939,14.9624647058824
-"03:00",25.5109868421053,21.5867240009928
-"08:00",14.6170186335404,13.5239781446692,15.5212659069326
-"03:30",24.0668932038835,20.9675673801628
-"08:30",11.9508457711443,12.51936726662,15.5015342203044
-"04:00",20.741935483871,19.5440361578802
-"09:00",14.6515178571429,12.2825301037311,14.8664171615202
-"04:30",21.8844444444444,20.5736627750337
-"09:30",14.2556723716381,12.7185987265251,14.6552436532508
-"10:00",15.2543318965517,12.5175843184934,14.3999800796813
-"10:30",13.9940733590734,12.8292169687832,14.7523503800968
-"11:00",14.5494482758621,12.7073268167037,14.5278352272727
-"11:30",14.96,12.962767348338,13.9883110328638
-"12:00",15.4663074712644,12.8498847984186,14.3375231092437
-"12:30",15.4995989650712,13.0149138892309,15.2775230202578
-"13:00",15.9256538461538,12.9705010402643,13.9605015948963
-"13:30",16.4996695226438,13.4206320002747,13.6947259858443
-"14:00",17.5761047835991,13.8197522131234,12.8379856287425
-"14:30",18.2843021032505,14.5824257545294,12.294854517611
-"15:00",19.1103674540682,15.1397130475545,12.5210486223663
-"15:30",19.9887250996016,15.9356384370689,12.2010671378092
-"16:00",21.7328698412698,16.3541246052123,11.4978145956607
-"16:30",22.088358291736,16.6677228815799,11.4904512195122
-"17:00",22.2276568670469,16.6894238471996,12.5883872053872
-"17:30",22.475650815689,16.389596399192,15.1986052631579
-"18:00",24.4175852182224,16.1815682683545,12.7401105527638
-"18:30",24.8914479495268,16.8275300538981,12.0279777777778
-"19:00",26.9854277797021,17.3369007149821
-"19:30",27.8613100961538,18.0725522231033
-"20:00",28.6581786185658,18.6578304604925
-"20:30",29.5004693289419,19.5963049829675
-"21:00",28.6974755700326,20.2645584524877
-"21:30",29.4559831223629,20.5896655165116
-"22:00",29.9467628607277,20.4503061258468
-"22:30",30.3777458136539,20.3341998387897
-"23:00",30.489440433213,20.4142983779764
+﻿"Arrival Time","home","public","work"
+"00:00",30.8297799511002,20.8705986179664
+"05:00",22.0435135135135,20.2595417709451,10.8555097087379
+"00:30",32.0270384615385,20.894369779523
+"05:30",21.0539655172414,19.7498010971903,13.5385333333333
+"01:00",32.4321327967807,21.0355386961029
+"06:00",20.6445652173913,19.1001881870259,12.2773303249097
+"01:30",32.504872611465,21.4336501128668
+"06:30",21.4597902097902,18.6876522134765,13.5467311178248
+"02:00",29.508,21.6300245220831
+"07:00",17.5342777777778,16.6522399668831,11.9299762859051
+"02:30",26.4673456790123,21.2612758882766
+"07:30",18.5670903010033,15.2372158312939,14.9624647058824
+"03:00",25.5109868421053,21.5867240009928
+"08:00",14.6170186335404,13.5239781446692,15.5212659069326
+"03:30",24.0668932038835,20.9675673801628
+"08:30",11.9508457711443,12.51936726662,15.5015342203044
+"04:00",20.741935483871,19.5440361578802
+"09:00",14.6515178571429,12.2825301037311,14.8664171615202
+"04:30",21.8844444444444,20.5736627750337
+"09:30",14.2556723716381,12.7185987265251,14.6552436532508
+"10:00",15.2543318965517,12.5175843184934,14.3999800796813
+"10:30",13.9940733590734,12.8292169687832,14.7523503800968
+"11:00",14.5494482758621,12.7073268167037,14.5278352272727
+"11:30",14.96,12.962767348338,13.9883110328638
+"12:00",15.4663074712644,12.8498847984186,14.3375231092437
+"12:30",15.4995989650712,13.0149138892309,15.2775230202578
+"13:00",15.9256538461538,12.9705010402643,13.9605015948963
+"13:30",16.4996695226438,13.4206320002747,13.6947259858443
+"14:00",17.5761047835991,13.8197522131234,12.8379856287425
+"14:30",18.2843021032505,14.5824257545294,12.294854517611
+"15:00",19.1103674540682,15.1397130475545,12.5210486223663
+"15:30",19.9887250996016,15.9356384370689,12.2010671378092
+"16:00",21.7328698412698,16.3541246052123,11.4978145956607
+"16:30",22.088358291736,16.6677228815799,11.4904512195122
+"17:00",22.2276568670469,16.6894238471996,12.5883872053872
+"17:30",22.475650815689,16.389596399192,15.1986052631579
+"18:00",24.4175852182224,16.1815682683545,12.7401105527638
+"18:30",24.8914479495268,16.8275300538981,12.0279777777778
+"19:00",26.9854277797021,17.3369007149821
+"19:30",27.8613100961538,18.0725522231033
+"20:00",28.6581786185658,18.6578304604925
+"20:30",29.5004693289419,19.5963049829675
+"21:00",28.6974755700326,20.2645584524877
+"21:30",29.4559831223629,20.5896655165116
+"22:00",29.9467628607277,20.4503061258468
+"22:30",30.3777458136539,20.3341998387897
+"23:00",30.489440433213,20.4142983779764
 "23:30",31.0691849710983,20.570283619716
```

### Comparing `ev2gym-0.0.12/ev2gym/data/pv_netherlands.csv` & `ev2gym-1.0.0/ev2gym/data/pv_netherlands.csv`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/residential_loads.csv` & `ev2gym-1.0.0/ev2gym/data/residential_loads.csv`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/data/time_of_connection_vs_hour.npy` & `ev2gym-1.0.0/ev2gym/data/time_of_connection_vs_hour.npy`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/example_config_files/BusinessPST.yaml` & `ev2gym-1.0.0/ev2gym/example_config_files/BusinessPST.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -23,28 +23,28 @@
 minute: 0 # Simulation starting minute (0-59)
 
 # Simulate weekdays, weekends, or both
 simulation_days: weekdays # weekdays, weekends, or both
 
 # EV Spawn Behavior
 scenario: public # public, private, or workplace
-spawn_multiplier: 5 # 1 is default, the higher the number the more EVs spawn
+spawn_multiplier: 500 # 1 is default, the higher the number the more EVs spawn
 
 ##############################################################################
 # Prices
 ##############################################################################
 discharge_price_factor: 1.2 # how many times more abs(expensive/cheaper) it is to discharge than to charge
 
 ##############################################################################
 # Charging Network
 ##############################################################################
 v2g_enabled: True # True or False
-number_of_charging_stations: 3
-number_of_transformers: 1
-number_of_ports_per_cs: 1
+number_of_charging_stations: 15
+number_of_transformers: 3
+number_of_ports_per_cs: 2
 # Provide path if you want to load a specific charging topology,
 # else write None for a randomized one with the above parameters
 charging_network_topology: None #./config_files/charging_topology_10.json
 
 ##############################################################################
 # Power Setpoints Settings
 ##############################################################################
@@ -52,14 +52,16 @@
 # The higher the number the easier it is to meet the power setpoints, the opposite for negative numbers
 power_setpoint_flexiblity: 20 # (in percentage +/- %)
 
 ##############################################################################
 # Inflexible Loads, Solar Generation, and Demand Response
 ##############################################################################
 # Whether to include inflexible loads in the transformer power limit, such as residential loads
+tr_seed: -1 # Seed for the transformer loads, -1 for random
+
 inflexible_loads:
   include: False # True or False
   inflexible_loads_capacity_multiplier_mean: 0.8 # 1 is default, the higher the number the more inflexible loads
   forecast_mean: 100 # in percentage of load at time t%
   forecast_std: 0 # in percentage of load at time t%
 
 # PV solar Power
@@ -90,15 +92,14 @@
 # such as battery capacity, charging rate, etc.
 
 ##############################################################################
 # Default Model values
 ##############################################################################
 # These values are used if not using a charging network topology file or 
 # if the EV specifications are not provided
-tr_seed: -1 # Seed for the transformer
 
 # Default Transformer model
 transformer:
   max_power: 100 # in kW
 
 # Default Charging Station model
 charging_station:
```

### Comparing `ev2gym-0.0.12/ev2gym/example_config_files/PublicPST.yaml` & `ev2gym-1.0.0/ev2gym/example_config_files/PublicPST.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This yml file is used to configure the evsim simulation
 
 ##############################################################################
 # Simulation Parameters
 ##############################################################################
 timescale: 15 # in minutes per step
-simulation_length: 85 #90 # in steps per simulation
+simulation_length: 112 #90 # in steps per simulation
 
 ##############################################################################
 # Date and Time
 ##############################################################################
 # Year, month, 
 year: 2022 # 2015-2023
 month: 1 # 1-12
```

### Comparing `ev2gym-0.0.12/ev2gym/example_config_files/V2GProfitMax.yaml` & `ev2gym-1.0.0/ev2gym/example_config_files/V2GProfitMax.yaml`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/example_config_files/V2GProfitPlusLoads.yaml` & `ev2gym-1.0.0/ev2gym/example_config_files/V2GProfitPlusLoads.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # This yml file is used to configure the evsim simulation
 
 ##############################################################################
 # Simulation Parameters
 ##############################################################################
 timescale: 15 # in minutes per step
-simulation_length: 55 #90 # in steps per simulation
+simulation_length: 85 #90 # in steps per simulation
 
 ##############################################################################
 # Date and Time
 ##############################################################################
 # Year, month, 
 year: 2022 # 2015-2023
 month: 1 # 1-12
 day: 17 # 1-31
 # Whether to get a random date every time the environment is reset
 random_day: True # True or False
 
 # Simulation Starting Time
 # Hour and minute do not change after the environment has been reset
-hour: 7 # Simulation starting hour (24 hour format)
+hour: 5 # Simulation starting hour (24 hour format)
 minute: 0 # Simulation starting minute (0-59)
 
 # Simulate weekdays, weekends, or both
 simulation_days: weekdays # weekdays, weekends, or both
 
 # EV Spawn Behavior
 scenario: workplace # public, private, or workplace
```

### Comparing `ev2gym-0.0.12/ev2gym/example_config_files/V2G_MPC.yaml` & `ev2gym-1.0.0/ev2gym/example_config_files/V2G_MPC.yaml`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/example_config_files/V2G_MPC2.yaml` & `ev2gym-1.0.0/ev2gym/example_config_files/V2G_MPC2.yaml`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/example_config_files/charging_topology_10.json` & `ev2gym-1.0.0/ev2gym/example_config_files/charging_topology_10.json`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/models/ev.py` & `ev2gym-1.0.0/ev2gym/models/ev.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/models/ev2gym_env.py` & `ev2gym-1.0.0/ev2gym/models/ev2gym_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 import random
 from copy import deepcopy
 import yaml
 import json
 
 # from .grid import Grid
 from ev2gym.models.replay import EvCityReplay
-from ev2gym.vizuals.plots import ev_city_plot, visualize_step
+from ev2gym.visuals.plots import ev_city_plot, visualize_step
 from ev2gym.utilities.utils import get_statistics, print_statistics, calculate_charge_power_potential
 from ev2gym.utilities.loaders import load_ev_spawn_scenarios, load_power_setpoints, load_transformers, load_ev_charger_profiles, load_ev_profiles, load_electricity_prices
-from ev2gym.vizuals.render import Renderer
+from ev2gym.visuals.render import Renderer
 
 from ev2gym.rl_agent.reward import SquaredTrackingErrorReward
 from ev2gym.rl_agent.state import PublicPST
 
 
 class EV2Gym(gym.Env):
 
@@ -297,15 +297,17 @@
         # f'{datetime.datetime.now().strftime("%Y-%m-%d_%H-%M")}'
 
         self.init_statistic_variables()
 
         return self._get_observation(), {}
 
     def init_statistic_variables(self):
-        
+        '''
+        Initializes the variables used for keeping simulation statistics
+        '''
         self.current_step = 0
         self.total_evs_spawned = 0
         self.total_reward = 0
 
         self.current_ev_departed = 0
         self.current_ev_arrived = 0
         self.current_evs_parked = 0
@@ -489,14 +491,15 @@
 
             if self.save_replay:
                 self._save_sim_replay()
 
             if self.save_plots:
                 #save the env as a pickle file
                 with open(f"./results/{self.sim_name}/env.pkl", 'wb') as f:
+                    self.renderer = None
                     pickle.dump(self, f)
                 ev_city_plot(self)
 
             self.done = True
             return self._get_observation(), reward, True, truncated, get_statistics(self)
         else:
             return self._get_observation(), reward, False, truncated, {'None': None}
@@ -510,14 +513,22 @@
         '''Saves the simulation data in a pickle file'''
         replay = EvCityReplay(self)
         print(f"Saving replay file at {replay.replay_path}")
         with open(replay.replay_path, 'wb') as f:
             pickle.dump(replay, f)
 
         return replay.replay_path
+    
+    def set_save_plots(self, save_plots):
+        if save_plots:
+            os.makedirs("./results", exist_ok=True)
+            print(f"Creating directory: ./results/{self.sim_name}")
+            os.makedirs(f"./results/{self.sim_name}", exist_ok=True)
+            
+        self.save_plots = save_plots
 
     def _update_power_statistics(self, departing_evs):
         '''Updates the power statistics of the simulation'''
 
         # if not self.lightweight_plots:
         for tr in self.transformers:
             # self.transformer_amps[tr.id, self.current_step] = tr.current_amps
```

### Comparing `ev2gym-0.0.12/ev2gym/models/ev_charger.py` & `ev2gym-1.0.0/ev2gym/models/ev_charger.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/models/grid.py` & `ev2gym-1.0.0/ev2gym/models/grid.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/models/replay.py` & `ev2gym-1.0.0/ev2gym/models/replay.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/models/transformer.py` & `ev2gym-1.0.0/ev2gym/models/transformer.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/rl_agent/reward.py` & `ev2gym-1.0.0/ev2gym/rl_agent/reward.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/rl_agent/state.py` & `ev2gym-1.0.0/ev2gym/rl_agent/state.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/utilities/arg_parser.py` & `ev2gym-1.0.0/ev2gym/utilities/arg_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,25 +29,25 @@
                         help="Standard deviation of the OU-Noise (default: 0.2)")
     parser.add_argument("--hidden_size", nargs=2, default=[256, 256], type=tuple,
                         help="Num. of units of the hidden layers (default: [400, 300]; OpenAI: [64, 64])")    
     parser.add_argument("--wandb", default=True, type=bool,
                         help="Enable logging to wandb (default: True)")
 
     # Environment specific arguments
-    # parser.add_argument("--config_file", default="ev2gym/example_config_files/PublicPST.yaml",
-    parser.add_argument("--config_file", default="ev2gym/example_config_files/V2G_MPC.yaml",
+    parser.add_argument("--config_file", default="ev2gym/example_config_files/PublicPST.yaml",
+    # parser.add_argument("--config_file", default="ev2gym/example_config_files/V2G_MPC.yaml",
     # parser.add_argument("--config_file", default="ev2gym/example_config_files/V2GProfitPlusLoads.yaml",
                         help="Path to the config file (default: config_files/config.yaml)")
-    parser.add_argument("--n_test_cycles", default=1, type=int,
+    parser.add_argument("--n_test_cycles", default=50, type=int,
                         help="Num. of episodes in the evaluation phases (default: 10; OpenAI: 20)")
 
     # Generate trajectories specific arguments
-    parser.add_argument("--n_trajectories", default=20, type=int,
+    parser.add_argument("--n_trajectories", default=200_000, type=int,
                         help="Num. of trajectories to generate (default: 10)")
     
     #
-    parser.add_argument("--dataset", default="-", type=str)
+    parser.add_argument("--dataset", default="RR", type=str)
     parser.add_argument("--save_opt_trajectories", default=True, type=bool,
                         help="Save Optimal trajectories (default: False)")
     
 
     return parser.parse_args()
```

### Comparing `ev2gym-0.0.12/ev2gym/utilities/loaders.py` & `ev2gym-1.0.0/ev2gym/utilities/loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             dataset_timescale/desired_timescale)].reset_index(drop=True)
 
     # duplicate the data to have two years of data
     data = pd.concat([data, data], ignore_index=True)
 
     # add a date column to the dataframe
     data['date'] = pd.date_range(
-        start=dataset_starting_date, periods=data.shape[0], freq=f'{desired_timescale}T')
+        start=dataset_starting_date, periods=data.shape[0], freq=f'{desired_timescale}min')
 
     # find year of the data
     year = int(dataset_starting_date.split('-')[0])
     # replace the year of the simulation date with the year of the data
     simulation_date = f'{year}-{simulation_date.split("-")[1]}-{simulation_date.split("-")[2]}'
 
     simulation_index = data[data['date'] == simulation_date].index[0]
@@ -179,15 +179,15 @@
         span=60//desired_timescale, adjust=True).mean()
 
     # duplicate the data to have two years of data
     data = pd.concat([data, data], ignore_index=True)
 
     # add a date column to the dataframe
     data['date'] = pd.date_range(
-        start=dataset_starting_date, periods=data.shape[0], freq=f'{desired_timescale}T')
+        start=dataset_starting_date, periods=data.shape[0], freq=f'{desired_timescale}min')
 
     # find year of the data
     year = int(dataset_starting_date.split('-')[0])
     # replace the year of the simulation date with the year of the data
     simulation_date = f'{year}-{simulation_date.split("-")[1]}-{simulation_date.split("-")[2]}'
 
     simulation_index = data[data['date'] == simulation_date].index[0]
```

### Comparing `ev2gym-0.0.12/ev2gym/utilities/utils.py` & `ev2gym-1.0.0/ev2gym/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/vizuals/evaluator_plot.py` & `ev2gym-1.0.0/ev2gym/visuals/evaluator_plot.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/vizuals/icons/algorithm.png` & `ev2gym-1.0.0/ev2gym/visuals/icons/algorithm.png`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/vizuals/icons/charger_wallbox.png` & `ev2gym-1.0.0/ev2gym/visuals/icons/charger_wallbox.png`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/vizuals/icons/charging-station_1_port.png` & `ev2gym-1.0.0/ev2gym/visuals/icons/charging-station_1_port.png`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/vizuals/icons/charging-station_2_ports.png` & `ev2gym-1.0.0/ev2gym/visuals/icons/charging-station_2_ports.png`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/vizuals/icons/cpo.png` & `ev2gym-1.0.0/ev2gym/visuals/icons/cpo.png`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/vizuals/icons/ev.png` & `ev2gym-1.0.0/ev2gym/visuals/icons/ev.png`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/vizuals/icons/ev2.png` & `ev2gym-1.0.0/ev2gym/visuals/icons/ev2.png`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/vizuals/icons/logo.png` & `ev2gym-1.0.0/ev2gym/visuals/icons/logo.png`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/vizuals/icons/transformer.png` & `ev2gym-1.0.0/ev2gym/visuals/icons/transformer.png`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/vizuals/plots.py` & `ev2gym-1.0.0/ev2gym/visuals/plots.py`

 * *Files identical despite different names*

### Comparing `ev2gym-0.0.12/ev2gym/vizuals/render.py` & `ev2gym-1.0.0/ev2gym/visuals/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 import PIL
 import numpy as np
 import pkg_resources
 
 # Image URLs for graph nodes
 
 icons = {
-    "cpo": pkg_resources.resource_filename('ev2gym', "vizuals/icons/cpo.png"),
-    "transformer": pkg_resources.resource_filename('ev2gym', "vizuals/icons/transformer.png"),
-    "charger_1": pkg_resources.resource_filename('ev2gym', "vizuals/icons/charging-station_1_port.png"),
-    "charger_2": pkg_resources.resource_filename('ev2gym', "vizuals/icons/charging-station_2_ports.png"),
-    "charger_wallbox": pkg_resources.resource_filename('ev2gym', "vizuals/icons/charger_wallbox.png"),
-    "ev": pkg_resources.resource_filename('ev2gym', "vizuals/icons/ev.png")
+    "cpo": pkg_resources.resource_filename('ev2gym', "visuals/icons/cpo.png"),
+    "transformer": pkg_resources.resource_filename('ev2gym', "visuals/icons/transformer.png"),
+    "charger_1": pkg_resources.resource_filename('ev2gym', "visuals/icons/charging-station_1_port.png"),
+    "charger_2": pkg_resources.resource_filename('ev2gym', "visuals/icons/charging-station_2_ports.png"),
+    "charger_wallbox": pkg_resources.resource_filename('ev2gym', "visuals/icons/charger_wallbox.png"),
+    "ev": pkg_resources.resource_filename('ev2gym', "visuals/icons/ev.png")
 }
 
 
 class Renderer():
     """Class for rendering the simulation environment"""
 
     def __init__(self, env):
@@ -201,15 +201,15 @@
                 self.ev_list.append(a)
 
         # add title to top of the figure
         # self.fig.suptitle("EV Charging Network", fontsize=16)
 
         # add icon to the bottom of the figure
         image_path = pkg_resources.resource_filename(
-            'ev2gym', "vizuals/icons/logo.png")
+            'ev2gym', "visuals/icons/logo.png")
         icon = PIL.Image.open(image_path)
         icon = icon.resize((100, 50), PIL.Image.LANCZOS)
         self.fig.figimage(icon, 20, 20, alpha=1, zorder=1)
 
         # add text to a box in the bottom right corner
         text = f"Time step: {self.env.current_step}/ {self.env.simulation_length}\n" + \
                f"{self.env.sim_date}\n" \
@@ -276,11 +276,12 @@
             self.charger_labels_ax["charger_" + str(i)].set_text(
                 str(round(self.env.charging_stations[i].current_power_output, 1)) + "kW")
 
         for i in range(0, self.env.number_of_transformers):
             # append transformer current to node labels
             self.tr_labels_ax["transformer_" +
                               str(i)].set_text(str(round(self.env.transformers[i].current_amps /
-                                                         self.env.transformers[i].max_current*100, 0)) + "%")
+                                                         self.env.transformers[i].max_current[self.env.current_step-1]
+                                                         *100, 0)) + "%")
         # update ev nodes
         self.fig.canvas.draw()
         self.fig.canvas.flush_events()
```

### Comparing `ev2gym-0.0.12/setup.py` & `ev2gym-1.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='ev2gym',
-    version='0.0.12',
-    description='A realistic V2X environment using gym',
+    version='1.0.0',
+    description='A realistic V2G simulator environment',
     author='Stavros Orfanoudakis',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    keywords='gym, Reinforcement Learning, V2X, EVs, ev2gym, Electric Vehicles, Electric Vehicle Simulator',
+    keywords='gym, Reinforcement Learning, V2X, V2G, G2V, EVs, ev2gym, Electric Vehicles, Electric Vehicle Simulator',
     # package_dir = {"": "ev2gym"},
     packages=find_packages(),
     python_requires=">=3.6",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
```

