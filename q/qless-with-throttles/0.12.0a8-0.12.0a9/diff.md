# Comparing `tmp/qless-with-throttles-0.12.0a8.tar.gz` & `tmp/qless-with-throttles-0.12.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qless-with-throttles-0.12.0a8.tar", last modified: Thu Dec 28 22:35:13 2023, max compression
+gzip compressed data, was "qless-with-throttles-0.12.0a9.tar", last modified: Mon Jan  8 17:40:54 2024, max compression
```

## Comparing `qless-with-throttles-0.12.0a8.tar` & `qless-with-throttles-0.12.0a9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 22:35:13.628366 qless-with-throttles-0.12.0a8/
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    25985 2023-12-28 22:35:13.628366 qless-with-throttles-0.12.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23406 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 22:35:13.616366 qless-with-throttles-0.12.0a8/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3362 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/bin/qless-py-worker
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 22:35:13.616366 qless-with-throttles-0.12.0a8/qless/
--rw-r--r--   0 runner    (1001) docker     (127)     8204 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 22:35:13.620366 qless-with-throttles-0.12.0a8/qless/abstract/
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_job.py
--rw-r--r--   0 runner    (1001) docker     (127)      297 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_job_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_job_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2901 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_queue_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_queues.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_throttles.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/abstract/abstract_workers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16484 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/listener.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 22:35:13.620366 qless-with-throttles-0.12.0a8/qless/lua/
--rw-r--r--   0 runner    (1001) docker     (127)    97685 2023-12-28 22:35:04.000000 qless-with-throttles-0.12.0a8/qless/lua/qless-lib.lua
--rw-r--r--   0 runner    (1001) docker     (127)    71833 2023-12-28 22:35:04.000000 qless-with-throttles-0.12.0a8/qless/lua/qless.lua
--rw-r--r--   0 runner    (1001) docker     (127)      318 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/proctitle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/profile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8925 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 22:35:13.620366 qless-with-throttles-0.12.0a8/qless/queue_resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/queue_resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4219 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/queue_resolvers/transforming_queue_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 22:35:13.620366 qless-with-throttles-0.12.0a8/qless/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4996 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/workers/forking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/workers/greenlet.py
--rw-r--r--   0 runner    (1001) docker     (127)     2051 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/workers/serial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/workers/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6410 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qless/workers/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 22:35:13.624366 qless-with-throttles-0.12.0a8/qless_with_throttles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25985 2023-12-28 22:35:13.000000 qless-with-throttles-0.12.0a8/qless_with_throttles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2023-12-28 22:35:13.000000 qless-with-throttles-0.12.0a8/qless_with_throttles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 22:35:13.000000 qless-with-throttles-0.12.0a8/qless_with_throttles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      559 2023-12-28 22:35:13.000000 qless-with-throttles-0.12.0a8/qless_with_throttles.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-12-28 22:35:13.000000 qless-with-throttles-0.12.0a8/qless_with_throttles.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 22:35:13.624366 qless-with-throttles-0.12.0a8/qmore/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qmore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qmore/client.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/qmore/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-28 22:35:13.628366 qless-with-throttles-0.12.0a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2023-12-28 22:33:46.000000 qless-with-throttles-0.12.0a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:40:54.644206 qless-with-throttles-0.12.0a9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-01-08 17:40:54.644206 qless-with-throttles-0.12.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23406 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:40:54.628206 qless-with-throttles-0.12.0a9/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3362 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/bin/qless-py-worker
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:40:54.632206 qless-with-throttles-0.12.0a9/qless/
+-rw-r--r--   0 runner    (1001) docker     (127)     8204 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:40:54.632206 qless-with-throttles-0.12.0a9/qless/abstract/
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_job_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_job_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2901 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_queue_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_queues.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_throttles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/abstract/abstract_workers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16484 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:40:54.636206 qless-with-throttles-0.12.0a9/qless/lua/
+-rw-r--r--   0 runner    (1001) docker     (127)    97685 2024-01-08 17:40:46.000000 qless-with-throttles-0.12.0a9/qless/lua/qless-lib.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    71833 2024-01-08 17:40:46.000000 qless-with-throttles-0.12.0a9/qless/lua/qless.lua
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/proctitle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8925 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:40:54.636206 qless-with-throttles-0.12.0a9/qless/queue_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/queue_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/queue_resolvers/transforming_queue_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:40:54.636206 qless-with-throttles-0.12.0a9/qless/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4996 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/workers/forking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/workers/greenlet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2051 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/workers/serial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/workers/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6410 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qless/workers/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:40:54.636206 qless-with-throttles-0.12.0a9/qless_with_throttles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-01-08 17:40:54.000000 qless-with-throttles-0.12.0a9/qless_with_throttles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-01-08 17:40:54.000000 qless-with-throttles-0.12.0a9/qless_with_throttles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 17:40:54.000000 qless-with-throttles-0.12.0a9/qless_with_throttles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-01-08 17:40:54.000000 qless-with-throttles-0.12.0a9/qless_with_throttles.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-08 17:40:54.000000 qless-with-throttles-0.12.0a9/qless_with_throttles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 17:40:54.636206 qless-with-throttles-0.12.0a9/qmore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qmore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qmore/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/qmore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-01-08 17:40:54.644206 qless-with-throttles-0.12.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-01-08 17:39:52.000000 qless-with-throttles-0.12.0a9/setup.py
```

### Comparing `qless-with-throttles-0.12.0a8/LICENSE` & `qless-with-throttles-0.12.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/PKG-INFO` & `qless-with-throttles-0.12.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qless-with-throttles
-Version: 0.12.0a8
+Version: 0.12.0a9
 Summary: Redis-based Queue Management
 Home-page: http://github.com/tdg5/qless-py
 Author: Danny Guinther
 Author-email: dannyguinther@gmail.com
 License: MIT License
 Keywords: redis,qless,job
 Classifier: Intended Audience :: Developers
```

### Comparing `qless-with-throttles-0.12.0a8/README.md` & `qless-with-throttles-0.12.0a9/README.md`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/bin/qless-py-worker` & `qless-with-throttles-0.12.0a9/bin/qless-py-worker`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/pyproject.toml` & `qless-with-throttles-0.12.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/__init__.py` & `qless-with-throttles-0.12.0a9/qless/__init__.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/abstract/__init__.py` & `qless-with-throttles-0.12.0a9/qless/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/abstract/abstract_client.py` & `qless-with-throttles-0.12.0a9/qless/abstract/abstract_client.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/abstract/abstract_config.py` & `qless-with-throttles-0.12.0a9/qless/abstract/abstract_config.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/abstract/abstract_job.py` & `qless-with-throttles-0.12.0a9/qless/abstract/abstract_job.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/abstract/abstract_job_processor.py` & `qless-with-throttles-0.12.0a9/qless/abstract/abstract_job_processor.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,11 +23,11 @@
         for base in get_original_bases(cls):
             base_args = get_args(base)
             if base_args and issubclass(base_args[0], AbstractJobData):
                 data_class: Type[JD] = base_args[0]
                 return data_class
         raise RuntimeError(f"Unable to determine data class for {cls}")
 
-    @classmethod
+    @staticmethod
     @abstractmethod
-    def process(cls, job: AbstractJob) -> None:  # pragma: no cover
+    def process(job: AbstractJob) -> None:  # pragma: no cover
         ...
```

### Comparing `qless-with-throttles-0.12.0a8/qless/abstract/abstract_jobs.py` & `qless-with-throttles-0.12.0a9/qless/abstract/abstract_jobs.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/abstract/abstract_queue.py` & `qless-with-throttles-0.12.0a9/qless/abstract/abstract_queue.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/abstract/abstract_queue_jobs.py` & `qless-with-throttles-0.12.0a9/qless/abstract/abstract_queue_jobs.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/abstract/abstract_throttle.py` & `qless-with-throttles-0.12.0a9/qless/abstract/abstract_throttle.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/config.py` & `qless-with-throttles-0.12.0a9/qless/config.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/importer.py` & `qless-with-throttles-0.12.0a9/qless/importer.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/job.py` & `qless-with-throttles-0.12.0a9/qless/job.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/listener.py` & `qless-with-throttles-0.12.0a9/qless/listener.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/lua/qless-lib.lua` & `qless-with-throttles-0.12.0a9/qless/lua/qless-lib.lua`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/lua/qless.lua` & `qless-with-throttles-0.12.0a9/qless/lua/qless.lua`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/profile.py` & `qless-with-throttles-0.12.0a9/qless/profile.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/queue.py` & `qless-with-throttles-0.12.0a9/qless/queue.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/queue_resolvers/__init__.py` & `qless-with-throttles-0.12.0a9/qless/queue_resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py` & `qless-with-throttles-0.12.0a9/qless/queue_resolvers/qmore_dynamic_mapping_queue_identifiers_transformer.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py` & `qless-with-throttles-0.12.0a9/qless/queue_resolvers/qmore_dynamic_priority_queue_identifiers_transformer.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/queue_resolvers/transforming_queue_resolver.py` & `qless-with-throttles-0.12.0a9/qless/queue_resolvers/transforming_queue_resolver.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/throttle.py` & `qless-with-throttles-0.12.0a9/qless/throttle.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/workers/forking.py` & `qless-with-throttles-0.12.0a9/qless/workers/forking.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/workers/greenlet.py` & `qless-with-throttles-0.12.0a9/qless/workers/greenlet.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/workers/serial.py` & `qless-with-throttles-0.12.0a9/qless/workers/serial.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/workers/util.py` & `qless-with-throttles-0.12.0a9/qless/workers/util.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless/workers/worker.py` & `qless-with-throttles-0.12.0a9/qless/workers/worker.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless_with_throttles.egg-info/PKG-INFO` & `qless-with-throttles-0.12.0a9/qless_with_throttles.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qless-with-throttles
-Version: 0.12.0a8
+Version: 0.12.0a9
 Summary: Redis-based Queue Management
 Home-page: http://github.com/tdg5/qless-py
 Author: Danny Guinther
 Author-email: dannyguinther@gmail.com
 License: MIT License
 Keywords: redis,qless,job
 Classifier: Intended Audience :: Developers
```

### Comparing `qless-with-throttles-0.12.0a8/qless_with_throttles.egg-info/SOURCES.txt` & `qless-with-throttles-0.12.0a9/qless_with_throttles.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qless_with_throttles.egg-info/requires.txt` & `qless-with-throttles-0.12.0a9/qless_with_throttles.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/qmore/client.py` & `qless-with-throttles-0.12.0a9/qmore/client.py`

 * *Files identical despite different names*

### Comparing `qless-with-throttles-0.12.0a8/setup.py` & `qless-with-throttles-0.12.0a9/setup.py`

 * *Files identical despite different names*

