# Comparing `tmp/apify_client-1.6.5b1.tar.gz` & `tmp/apify_client-1.6.5b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_client-1.6.5b1.tar", last modified: Tue Feb 27 13:14:38 2024, max compression
+gzip compressed data, was "apify_client-1.6.5b2.tar", last modified: Tue Apr  2 12:59:59 2024, max compression
```

## Comparing `apify_client-1.6.5b1.tar` & `apify_client-1.6.5b2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:14:38.228031 apify_client-1.6.5b1/
--rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-02-27 13:14:38.228031 apify_client-1.6.5b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-02-27 13:14:35.000000 apify_client-1.6.5b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 13:14:38.228031 apify_client-1.6.5b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:14:38.220031 apify_client-1.6.5b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:14:38.220031 apify_client-1.6.5b1/src/apify_client/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/_http_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:14:38.220031 apify_client-1.6.5b1/src/apify_client/clients/
--rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:14:38.224031 apify_client-1.6.5b1/src/apify_client/clients/base/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/base/actor_job_base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/base/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/base/resource_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/base/resource_collection_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:14:38.228031 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33049 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/actor.py
--rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/actor_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/actor_env_var.py
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/actor_env_var_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/actor_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/actor_version_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/build_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    46556 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/dataset_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/key_value_store_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    21378 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/request_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/request_queue_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    17783 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/run_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/schedule_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/store_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    23412 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/task_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/webhook_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/webhook_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 13:14:09.000000 apify_client-1.6.5b1/src/apify_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 13:14:38.228031 apify_client-1.6.5b1/src/apify_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-02-27 13:14:38.000000 apify_client-1.6.5b1/src/apify_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-02-27 13:14:38.000000 apify_client-1.6.5b1/src/apify_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 13:14:38.000000 apify_client-1.6.5b1/src/apify_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-02-27 13:14:38.000000 apify_client-1.6.5b1/src/apify_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-27 13:14:38.000000 apify_client-1.6.5b1/src/apify_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:59:59.063034 apify_client-1.6.5b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11355 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-02 12:59:59.063034 apify_client-1.6.5b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-02 12:59:56.000000 apify_client-1.6.5b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:59:59.063034 apify_client-1.6.5b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:59:59.051034 apify_client-1.6.5b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:59:59.051034 apify_client-1.6.5b2/src/apify_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2833 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10561 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4611 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18652 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:59:59.055034 apify_client-1.6.5b2/src/apify_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     3545 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:59:59.055034 apify_client-1.6.5b2/src/apify_client/clients/base/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/base/actor_job_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4477 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/base/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/base/resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/base/resource_collection_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:59:59.059034 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33049 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/actor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10572 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/actor_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4484 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/actor_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/actor_env_var_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10124 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/actor_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7645 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/actor_version_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2994 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46556 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15551 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4793 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5315 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21378 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4279 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17783 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7862 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/schedule_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3960 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23412 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/task_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10662 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8299 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/webhook_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:59:29.000000 apify_client-1.6.5b2/src/apify_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:59:59.059034 apify_client-1.6.5b2/src/apify_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-02 12:59:59.000000 apify_client-1.6.5b2/src/apify_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-02 12:59:59.000000 apify_client-1.6.5b2/src/apify_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:59:59.000000 apify_client-1.6.5b2/src/apify_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-02 12:59:59.000000 apify_client-1.6.5b2/src/apify_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 12:59:59.000000 apify_client-1.6.5b2/src/apify_client.egg-info/top_level.txt
```

### Comparing `apify_client-1.6.5b1/LICENSE` & `apify_client-1.6.5b2/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/PKG-INFO` & `apify_client-1.6.5b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_client
-Version: 1.6.5b1
+Version: 1.6.5b2
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.6.5b1/README.md` & `apify_client-1.6.5b2/README.md`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/pyproject.toml` & `apify_client-1.6.5b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "apify_client"
-version = "1.6.5b1"
+version = "1.6.5b2"
 description = "Apify API client for Python"
 readme = "README.md"
 license = { text = "Apache Software License" }
 authors = [{ name = "Apify Technologies s.r.o.", email = "support@apify.com" }]
 keywords = ["apify", "api", "client", "scraping", "automation"]
 
 classifiers = [
```

### Comparing `apify_client-1.6.5b1/src/apify_client/_errors.py` & `apify_client-1.6.5b2/src/apify_client/_errors.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/_http_client.py` & `apify_client-1.6.5b2/src/apify_client/_http_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/_logging.py` & `apify_client-1.6.5b2/src/apify_client/_logging.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/_utils.py` & `apify_client-1.6.5b2/src/apify_client/_utils.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/client.py` & `apify_client-1.6.5b2/src/apify_client/client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/__init__.py` & `apify_client-1.6.5b2/src/apify_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/base/__init__.py` & `apify_client-1.6.5b2/src/apify_client/clients/base/__init__.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/base/actor_job_base_client.py` & `apify_client-1.6.5b2/src/apify_client/clients/base/actor_job_base_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/base/base_client.py` & `apify_client-1.6.5b2/src/apify_client/clients/base/base_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/base/resource_client.py` & `apify_client-1.6.5b2/src/apify_client/clients/base/resource_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/base/resource_collection_client.py` & `apify_client-1.6.5b2/src/apify_client/clients/base/resource_collection_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/__init__.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/__init__.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/actor.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/actor.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/actor_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/actor_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/actor_env_var.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/actor_env_var.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/actor_env_var_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/actor_env_var_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/actor_version.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/actor_version.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/actor_version_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/actor_version_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/build.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/build.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/build_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/build_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/dataset.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/dataset.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/dataset_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/dataset_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/key_value_store.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/key_value_store.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/key_value_store_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/key_value_store_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/log.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/log.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/request_queue.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/request_queue.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/request_queue_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/request_queue_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/run.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/run.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/run_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/run_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/schedule.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/schedule.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/schedule_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/schedule_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/store_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/store_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/task.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/task.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/task_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/task_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/user.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/user.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/webhook.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/webhook.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/webhook_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/webhook_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/webhook_dispatch.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/webhook_dispatch.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py` & `apify_client-1.6.5b2/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client/consts.py` & `apify_client-1.6.5b2/src/apify_client/consts.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.6.5b1/src/apify_client.egg-info/PKG-INFO` & `apify_client-1.6.5b2/src/apify_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_client
-Version: 1.6.5b1
+Version: 1.6.5b2
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.6.5b1/src/apify_client.egg-info/SOURCES.txt` & `apify_client-1.6.5b2/src/apify_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

