# Comparing `tmp/eth-monitor-0.8.8.tar.gz` & `tmp/eth-monitor-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-monitor-0.8.8.tar", last modified: Sat Aug 19 10:07:12 2023, max compression
+gzip compressed data, was "eth-monitor-0.8.9.tar", last modified: Tue Apr  2 11:32:25 2024, max compression
```

## Comparing `eth-monitor-0.8.8.tar` & `eth-monitor-0.8.9.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.452473 eth-monitor-0.8.8/
--rw-r--r--   0 lash      (1000) lash      (1000)     2562 2023-08-19 10:05:46.000000 eth-monitor-0.8.8/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:56:11.000000 eth-monitor-0.8.8/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      110 2023-05-13 20:45:22.000000 eth-monitor-0.8.8/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-19 10:07:12.452473 eth-monitor-0.8.8/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     9706 2023-05-13 20:42:58.000000 eth-monitor-0.8.8/README.md
--rw-r--r--   0 lash      (1000) lash      (1000)      871 2022-11-14 07:52:42.000000 eth-monitor-0.8.8/WAIVER
--rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:55:49.000000 eth-monitor-0.8.8/WAIVER.asc
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.445807 eth-monitor-0.8.8/eth_monitor/
--rw-r--r--   0 lash      (1000) lash      (1000)      902 2022-11-11 05:56:27.000000 eth-monitor-0.8.8/eth_monitor/callback.py
--rw-r--r--   0 lash      (1000) lash      (1000)      849 2023-08-13 15:18:52.000000 eth-monitor-0.8.8/eth_monitor/chain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.449140 eth-monitor-0.8.8/eth_monitor/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)       65 2022-10-13 07:08:18.000000 eth-monitor-0.8.8/eth_monitor/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3624 2023-08-19 10:05:46.000000 eth-monitor-0.8.8/eth_monitor/cli/arg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2129 2023-08-19 10:05:46.000000 eth-monitor-0.8.8/eth_monitor/cli/config.py
--rw-r--r--   0 lash      (1000) lash      (1000)      518 2022-11-14 07:56:11.000000 eth-monitor-0.8.8/eth_monitor/cli/log.py
--rw-r--r--   0 lash      (1000) lash      (1000)      269 2023-08-08 07:54:29.000000 eth-monitor-0.8.8/eth_monitor/cli/rules.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1327 2022-04-20 19:19:25.000000 eth-monitor-0.8.8/eth_monitor/config.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.442473 eth-monitor-0.8.8/eth_monitor/data/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.449140 eth-monitor-0.8.8/eth_monitor/data/config/
--rw-r--r--   0 lash      (1000) lash      (1000)       40 2022-10-13 07:08:18.000000 eth-monitor-0.8.8/eth_monitor/data/config/cache.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-08-06 15:43:41.000000 eth-monitor-0.8.8/eth_monitor/data/config/filter.ini
--rw-r--r--   0 lash      (1000) lash      (1000)      271 2023-08-19 10:05:46.000000 eth-monitor-0.8.8/eth_monitor/data/config/monitor.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       22 2022-04-20 19:19:25.000000 eth-monitor-0.8.8/eth_monitor/data/config/renderer.ini
--rw-r--r--   0 lash      (1000) lash      (1000)       36 2023-08-19 10:05:46.000000 eth-monitor-0.8.8/eth_monitor/error.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.449140 eth-monitor-0.8.8/eth_monitor/filters/
--rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-01-30 14:12:19.000000 eth-monitor-0.8.8/eth_monitor/filters/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      580 2023-08-07 11:19:10.000000 eth-monitor-0.8.8/eth_monitor/filters/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)      304 2023-08-19 10:05:46.000000 eth-monitor-0.8.8/eth_monitor/filters/block.py
--rw-r--r--   0 lash      (1000) lash      (1000)      732 2023-08-06 16:03:10.000000 eth-monitor-0.8.8/eth_monitor/filters/cache.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2121 2023-08-06 16:02:35.000000 eth-monitor-0.8.8/eth_monitor/filters/out.py
--rw-r--r--   0 lash      (1000) lash      (1000)      301 2023-08-19 10:05:46.000000 eth-monitor-0.8.8/eth_monitor/filters/run.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.449140 eth-monitor-0.8.8/eth_monitor/importers/
--rw-r--r--   0 lash      (1000) lash      (1000)     1521 2022-11-11 05:56:27.000000 eth-monitor-0.8.8/eth_monitor/importers/etherscan.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1450 2022-04-20 19:19:25.000000 eth-monitor-0.8.8/eth_monitor/index.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.449140 eth-monitor-0.8.8/eth_monitor/mock/
--rw-r--r--   0 lash      (1000) lash      (1000)      274 2022-01-30 14:12:19.000000 eth-monitor-0.8.8/eth_monitor/mock/filter_plain.py
--rw-r--r--   0 lash      (1000) lash      (1000)      417 2022-01-30 14:12:19.000000 eth-monitor-0.8.8/eth_monitor/mock/filter_ruled.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6068 2023-08-19 10:05:46.000000 eth-monitor-0.8.8/eth_monitor/rules.py
--rw-r--r--   0 lash      (1000) lash      (1000)      363 2023-08-19 10:05:46.000000 eth-monitor-0.8.8/eth_monitor/run.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.452473 eth-monitor-0.8.8/eth_monitor/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     5735 2022-04-20 19:19:25.000000 eth-monitor-0.8.8/eth_monitor/runnable/import.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3877 2022-04-20 19:19:25.000000 eth-monitor-0.8.8/eth_monitor/runnable/list.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3440 2023-08-19 10:05:46.000000 eth-monitor-0.8.8/eth_monitor/runnable/sync.py
--rw-r--r--   0 lash      (1000) lash      (1000)     5125 2022-01-30 14:12:19.000000 eth-monitor-0.8.8/eth_monitor/runnable/sync_thread_range.py
--rw-r--r--   0 lash      (1000) lash      (1000)    14322 2023-08-19 10:05:46.000000 eth-monitor-0.8.8/eth_monitor/settings.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.445807 eth-monitor-0.8.8/eth_monitor.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)    10473 2023-08-19 10:07:12.000000 eth-monitor-0.8.8/eth_monitor.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)     1304 2023-08-19 10:07:12.000000 eth-monitor-0.8.8/eth_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-08-19 10:07:12.000000 eth-monitor-0.8.8/eth_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      113 2023-08-19 10:07:12.000000 eth-monitor-0.8.8/eth_monitor.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-19 10:07:12.000000 eth-monitor-0.8.8/eth_monitor.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       12 2023-08-19 10:07:12.000000 eth-monitor-0.8.8/eth_monitor.egg-info/top_level.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.442473 eth-monitor-0.8.8/man/
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.452473 eth-monitor-0.8.8/man/build/
--rw-r--r--   0 lash      (1000) lash      (1000)     6781 2023-08-08 18:16:36.000000 eth-monitor-0.8.8/man/build/eth-monitor-import.1
--rw-r--r--   0 lash      (1000) lash      (1000)     6392 2023-08-08 18:16:36.000000 eth-monitor-0.8.8/man/build/eth-monitor-list.1
--rw-r--r--   0 lash      (1000) lash      (1000)    11342 2023-08-08 18:16:36.000000 eth-monitor-0.8.8/man/build/eth-monitor-sync.1
--rw-r--r--   0 lash      (1000) lash      (1000)    11342 2023-08-08 18:16:36.000000 eth-monitor-0.8.8/man/build/eth-monitor.1
--rw-r--r--   0 lash      (1000) lash      (1000)      103 2023-08-14 08:44:48.000000 eth-monitor-0.8.8/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)     1002 2023-08-19 10:07:12.452473 eth-monitor-0.8.8/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      852 2023-05-13 20:44:09.000000 eth-monitor-0.8.8/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)       76 2022-04-20 19:19:25.000000 eth-monitor-0.8.8/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-08-19 10:07:12.452473 eth-monitor-0.8.8/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     3524 2022-04-20 19:19:25.000000 eth-monitor-0.8.8/tests/test_basic.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2562 2023-08-19 10:05:46.000000 eth-monitor-0.8.9/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    34523 2022-11-14 07:56:11.000000 eth-monitor-0.8.9/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)      110 2023-05-13 20:45:22.000000 eth-monitor-0.8.9/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)    10666 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     9706 2023-05-13 20:42:58.000000 eth-monitor-0.8.9/README.md
+-rw-r--r--   0 lash      (1000) lash      (1000)      871 2022-11-14 07:52:42.000000 eth-monitor-0.8.9/WAIVER
+-rw-r--r--   0 lash      (1000) lash      (1000)     1634 2022-11-14 07:55:49.000000 eth-monitor-0.8.9/WAIVER.asc
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/eth_monitor/
+-rw-r--r--   0 lash      (1000) lash      (1000)      902 2022-11-11 05:56:27.000000 eth-monitor-0.8.9/eth_monitor/callback.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      849 2023-08-13 15:18:52.000000 eth-monitor-0.8.9/eth_monitor/chain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/eth_monitor/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)       65 2022-10-13 07:08:18.000000 eth-monitor-0.8.9/eth_monitor/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3624 2023-08-19 10:05:46.000000 eth-monitor-0.8.9/eth_monitor/cli/arg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2129 2023-08-19 10:05:46.000000 eth-monitor-0.8.9/eth_monitor/cli/config.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      518 2022-11-14 07:56:11.000000 eth-monitor-0.8.9/eth_monitor/cli/log.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      269 2023-08-08 07:54:29.000000 eth-monitor-0.8.9/eth_monitor/cli/rules.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1327 2022-04-20 19:19:25.000000 eth-monitor-0.8.9/eth_monitor/config.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.329575 eth-monitor-0.8.9/eth_monitor/data/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/eth_monitor/data/config/
+-rw-r--r--   0 lash      (1000) lash      (1000)       40 2022-10-13 07:08:18.000000 eth-monitor-0.8.9/eth_monitor/data/config/cache.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2023-08-06 15:43:41.000000 eth-monitor-0.8.9/eth_monitor/data/config/filter.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)      271 2023-08-19 10:05:46.000000 eth-monitor-0.8.9/eth_monitor/data/config/monitor.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       22 2022-04-20 19:19:25.000000 eth-monitor-0.8.9/eth_monitor/data/config/renderer.ini
+-rw-r--r--   0 lash      (1000) lash      (1000)       36 2023-08-19 10:05:46.000000 eth-monitor-0.8.9/eth_monitor/error.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/eth_monitor/filters/
+-rw-r--r--   0 lash      (1000) lash      (1000)       20 2022-01-30 14:12:19.000000 eth-monitor-0.8.9/eth_monitor/filters/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      580 2023-08-07 11:19:10.000000 eth-monitor-0.8.9/eth_monitor/filters/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      304 2023-08-19 10:05:46.000000 eth-monitor-0.8.9/eth_monitor/filters/block.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      732 2023-08-06 16:03:10.000000 eth-monitor-0.8.9/eth_monitor/filters/cache.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2121 2023-08-06 16:02:35.000000 eth-monitor-0.8.9/eth_monitor/filters/out.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      301 2023-08-19 10:05:46.000000 eth-monitor-0.8.9/eth_monitor/filters/run.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/eth_monitor/importers/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1521 2022-11-11 05:56:27.000000 eth-monitor-0.8.9/eth_monitor/importers/etherscan.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1450 2022-04-20 19:19:25.000000 eth-monitor-0.8.9/eth_monitor/index.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/eth_monitor/mock/
+-rw-r--r--   0 lash      (1000) lash      (1000)      274 2022-01-30 14:12:19.000000 eth-monitor-0.8.9/eth_monitor/mock/filter_plain.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      417 2022-01-30 14:12:19.000000 eth-monitor-0.8.9/eth_monitor/mock/filter_ruled.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6068 2023-08-19 10:05:46.000000 eth-monitor-0.8.9/eth_monitor/rules.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      363 2023-08-19 10:05:46.000000 eth-monitor-0.8.9/eth_monitor/run.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/eth_monitor/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5735 2022-04-20 19:19:25.000000 eth-monitor-0.8.9/eth_monitor/runnable/import.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3877 2022-04-20 19:19:25.000000 eth-monitor-0.8.9/eth_monitor/runnable/list.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3440 2023-08-19 10:05:46.000000 eth-monitor-0.8.9/eth_monitor/runnable/sync.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     5125 2022-01-30 14:12:19.000000 eth-monitor-0.8.9/eth_monitor/runnable/sync_thread_range.py
+-rw-r--r--   0 lash      (1000) lash      (1000)    14322 2023-08-19 10:05:46.000000 eth-monitor-0.8.9/eth_monitor/settings.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/eth_monitor.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)    10666 2024-04-02 11:32:25.000000 eth-monitor-0.8.9/eth_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)     1304 2024-04-02 11:32:25.000000 eth-monitor-0.8.9/eth_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2024-04-02 11:32:25.000000 eth-monitor-0.8.9/eth_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      113 2024-04-02 11:32:25.000000 eth-monitor-0.8.9/eth_monitor.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      103 2024-04-02 11:32:25.000000 eth-monitor-0.8.9/eth_monitor.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       12 2024-04-02 11:32:25.000000 eth-monitor-0.8.9/eth_monitor.egg-info/top_level.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/man/
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/man/build/
+-rw-r--r--   0 lash      (1000) lash      (1000)     6781 2023-08-08 18:16:36.000000 eth-monitor-0.8.9/man/build/eth-monitor-import.1
+-rw-r--r--   0 lash      (1000) lash      (1000)     6392 2023-08-08 18:16:36.000000 eth-monitor-0.8.9/man/build/eth-monitor-list.1
+-rw-r--r--   0 lash      (1000) lash      (1000)    11342 2023-08-08 18:16:36.000000 eth-monitor-0.8.9/man/build/eth-monitor-sync.1
+-rw-r--r--   0 lash      (1000) lash      (1000)    11342 2023-08-08 18:16:36.000000 eth-monitor-0.8.9/man/build/eth-monitor.1
+-rw-r--r--   0 lash      (1000) lash      (1000)      103 2024-04-02 11:30:27.000000 eth-monitor-0.8.9/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)     1002 2024-04-02 11:32:25.336241 eth-monitor-0.8.9/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      852 2023-05-13 20:44:09.000000 eth-monitor-0.8.9/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       77 2024-04-02 11:30:27.000000 eth-monitor-0.8.9/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2024-04-02 11:32:25.332908 eth-monitor-0.8.9/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3524 2022-04-20 19:19:25.000000 eth-monitor-0.8.9/tests/test_basic.py
```

### Comparing `eth-monitor-0.8.8/CHANGELOG` & `eth-monitor-0.8.9/CHANGELOG`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/LICENSE` & `eth-monitor-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/PKG-INFO` & `eth-monitor-0.8.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-monitor
-Version: 0.8.8
+Version: 0.8.9
 Summary: Monitor and cache transactions using match filters
 Home-page: https://git.defalsify.org/eth-monitor
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: chainlib-eth~=0.6.0
+Requires-Dist: chainlib~=0.5.2
+Requires-Dist: chainsyncer~=0.8.5
+Requires-Dist: leveldir~=0.3.0
+Requires-Dist: eth-cache~=0.4.0
+Requires-Dist: confini~=0.6.3
 
 # NAME
 
 eth-monitor - Cache, index and monitor transactions with an EVM node rpc
 
 # SYNOPSIS
```

### Comparing `eth-monitor-0.8.8/README.md` & `eth-monitor-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/WAIVER` & `eth-monitor-0.8.9/WAIVER`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/WAIVER.asc` & `eth-monitor-0.8.9/WAIVER.asc`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/callback.py` & `eth-monitor-0.8.9/eth_monitor/callback.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/chain.py` & `eth-monitor-0.8.9/eth_monitor/chain.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/cli/arg.py` & `eth-monitor-0.8.9/eth_monitor/cli/arg.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/cli/config.py` & `eth-monitor-0.8.9/eth_monitor/cli/config.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/cli/log.py` & `eth-monitor-0.8.9/eth_monitor/cli/log.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/config.py` & `eth-monitor-0.8.9/eth_monitor/config.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/filters/base.py` & `eth-monitor-0.8.9/eth_monitor/filters/base.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/filters/cache.py` & `eth-monitor-0.8.9/eth_monitor/filters/cache.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/filters/out.py` & `eth-monitor-0.8.9/eth_monitor/filters/out.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/importers/etherscan.py` & `eth-monitor-0.8.9/eth_monitor/importers/etherscan.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/index.py` & `eth-monitor-0.8.9/eth_monitor/index.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/rules.py` & `eth-monitor-0.8.9/eth_monitor/rules.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/runnable/import.py` & `eth-monitor-0.8.9/eth_monitor/runnable/import.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/runnable/list.py` & `eth-monitor-0.8.9/eth_monitor/runnable/list.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/runnable/sync.py` & `eth-monitor-0.8.9/eth_monitor/runnable/sync.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/runnable/sync_thread_range.py` & `eth-monitor-0.8.9/eth_monitor/runnable/sync_thread_range.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor/settings.py` & `eth-monitor-0.8.9/eth_monitor/settings.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/eth_monitor.egg-info/PKG-INFO` & `eth-monitor-0.8.9/eth_monitor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-monitor
-Version: 0.8.8
+Version: 0.8.9
 Summary: Monitor and cache transactions using match filters
 Home-page: https://git.defalsify.org/eth-monitor
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: AGPLv3+
 Keywords: dlt,blockchain,cryptocurrency,ethereum
 Classifier: Programming Language :: Python :: 3
@@ -14,14 +14,20 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: chainlib-eth~=0.6.0
+Requires-Dist: chainlib~=0.5.2
+Requires-Dist: chainsyncer~=0.8.5
+Requires-Dist: leveldir~=0.3.0
+Requires-Dist: eth-cache~=0.4.0
+Requires-Dist: confini~=0.6.3
 
 # NAME
 
 eth-monitor - Cache, index and monitor transactions with an EVM node rpc
 
 # SYNOPSIS
```

### Comparing `eth-monitor-0.8.8/eth_monitor.egg-info/SOURCES.txt` & `eth-monitor-0.8.9/eth_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/man/build/eth-monitor-import.1` & `eth-monitor-0.8.9/man/build/eth-monitor-import.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/man/build/eth-monitor-list.1` & `eth-monitor-0.8.9/man/build/eth-monitor-list.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/man/build/eth-monitor-sync.1` & `eth-monitor-0.8.9/man/build/eth-monitor-sync.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/man/build/eth-monitor.1` & `eth-monitor-0.8.9/man/build/eth-monitor.1`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/setup.cfg` & `eth-monitor-0.8.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-monitor
-version = 0.8.8
+version = 0.8.9
 description = Monitor and cache transactions using match filters
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/eth-monitor
 keywords = 
 	dlt
 	blockchain
```

### Comparing `eth-monitor-0.8.8/setup.py` & `eth-monitor-0.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `eth-monitor-0.8.8/tests/test_basic.py` & `eth-monitor-0.8.9/tests/test_basic.py`

 * *Files identical despite different names*

