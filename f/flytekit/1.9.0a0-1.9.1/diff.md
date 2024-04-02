# Comparing `tmp/flytekit-1.9.0a0.tar.gz` & `tmp/flytekit-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekit-1.9.0a0.tar", last modified: Thu Jul 20 18:58:06 2023, max compression
+gzip compressed data, was "flytekit-1.9.1.tar", last modified: Mon Aug 28 16:42:54 2023, max compression
```

## Comparing `flytekit-1.9.0a0.tar` & `flytekit-1.9.1.tar`

### file list

```diff
@@ -1,254 +1,266 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.864495 flytekit-1.9.0a0/
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-20 18:58:06.864495 flytekit-1.9.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.828494 flytekit-1.9.0a0/flytekit/
--rw-r--r--   0 runner    (1001) docker     (123)     7877 2023-07-20 18:58:04.000000 flytekit-1.9.0a0/flytekit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22767 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/bin/entrypoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit/clients/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13495 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/auth_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9984 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/default_html.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/keyring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth/token_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/auth_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    50793 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/friendly.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit/clients/grpc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/grpc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/grpc_utils/auth_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    28489 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clients/raw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit/clis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit/clis/flyte_cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/flyte_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/flyte_cli/example.config
--rw-r--r--   0 runner    (1001) docker     (123)    81925 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/flyte_cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.836495 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/build.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/launchplan.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/pyflyte.py
--rw-r--r--   0 runner    (1001) docker     (123)     5930 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/register.py
--rw-r--r--   0 runner    (1001) docker     (123)    31410 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/clis/sdk_in_container/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.836495 flytekit-1.9.0a0/flytekit/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    36184 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/configuration/default_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/configuration/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/configuration/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     7371 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/configuration/internal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.844495 flytekit-1.9.0a0/flytekit/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/base_sql_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    31127 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/base_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5580 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/class_based_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    36181 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    12743 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/data_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/dynamic_workflow_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/gate.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)    20645 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    20508 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/local_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/map_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/mock_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/node_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/notification.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/pod_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    46418 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/promise.py
--rw-r--r--   0 runner    (1001) docker     (123)    14072 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/python_auto_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    12399 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/python_customized_container_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    14498 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/python_function_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/reference_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/shim_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15613 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/tracked_abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9668 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    77132 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/type_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/type_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    12005 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    41135 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/core/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.844495 flytekit-1.9.0a0/flytekit/deck/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/deck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/deck/deck.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.844495 flytekit-1.9.0a0/flytekit/deck/html/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/deck/html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/deck/html/template.html
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/deck/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/exceptions/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/exceptions/scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/exceptions/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extend/
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extend/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extend/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extend/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extend/backend/base_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extend/backend/external_plugin_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/cloud_pickle_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extras/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/pytorch/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/pytorch/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extras/sklearn/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/sklearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/sklearn/native.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extras/sqlite3/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/sqlite3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/sqlite3/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extras/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15405 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/tasks/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.848495 flytekit-1.9.0a0/flytekit/extras/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/tensorflow/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7664 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/extras/tensorflow/record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.852495 flytekit-1.9.0a0/flytekit/image_spec/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/image_spec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6086 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/image_spec/image_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.852495 flytekit-1.9.0a0/flytekit/interaction/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interaction/parse_stdin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.852495 flytekit-1.9.0a0/flytekit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6441 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interfaces/cli_identifiers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interfaces/random.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.852495 flytekit-1.9.0a0/flytekit/interfaces/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interfaces/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interfaces/stats/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/interfaces/stats/taggable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.852495 flytekit-1.9.0a0/flytekit/lazy_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/lazy_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/lazy_import/lazy_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/loggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.856495 flytekit-1.9.0a0/flytekit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.856495 flytekit-1.9.0a0/flytekit/models/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/admin/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/admin/task_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/admin/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/array_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    14187 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.856495 flytekit-1.9.0a0/flytekit/models/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2561 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    32176 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/core/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3938 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/dynamic_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    25993 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    14502 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/launch_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    11777 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/matchable_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/named_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    10667 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/node_execution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/presto.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/qubole.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/task.py
--rw-r--r--   0 runner    (1001) docker     (123)    15678 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/models/workflow_closure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/remote/
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/backfill.py
--rw-r--r--   0 runner    (1001) docker     (123)    30588 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/executions.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/lazy_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    86908 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/remote/remote_callable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/fast_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4355 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/module_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10803 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/script_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/serialize_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    32141 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/tools/translator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/types/directory/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/directory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/directory/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/types/file/
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23852 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/file/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/types/numpy/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/numpy/ndarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.860495 flytekit-1.9.0a0/flytekit/types/pickle/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/pickle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/pickle/pickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.864495 flytekit-1.9.0a0/flytekit/types/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18377 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/schema/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/schema/types_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.864495 flytekit-1.9.0a0/flytekit/types/structured/
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/structured/basic_dfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3917 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/structured/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)    44537 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit/types/structured/structured_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.832494 flytekit-1.9.0a0/flytekit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-07-20 18:58:06.000000 flytekit-1.9.0a0/flytekit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-20 18:58:06.000000 flytekit-1.9.0a0/flytekit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 18:58:06.000000 flytekit-1.9.0a0/flytekit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-20 18:58:06.000000 flytekit-1.9.0a0/flytekit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-07-20 18:58:06.000000 flytekit-1.9.0a0/flytekit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-20 18:58:06.000000 flytekit-1.9.0a0/flytekit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 18:58:06.864495 flytekit-1.9.0a0/flytekit_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit_scripts/Readme.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     3006 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit_scripts/flytekit_build_image.sh
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/flytekit_scripts/flytekit_venv
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-20 18:57:54.000000 flytekit-1.9.0a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-20 18:58:06.864495 flytekit-1.9.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-07-20 18:58:04.000000 flytekit-1.9.0a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.138104 flytekit-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (999)    11341 2023-08-28 16:42:38.000000 flytekit-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (999)     1039 2023-08-28 16:42:38.000000 flytekit-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (999)     4315 2023-08-28 16:42:54.138104 flytekit-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     3367 2023-08-28 16:42:38.000000 flytekit-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.102104 flytekit-1.9.1/flytekit/
+-rw-r--r--   0 runner    (1001) docker     (999)     8066 2023-08-28 16:42:51.000000 flytekit-1.9.1/flytekit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.106104 flytekit-1.9.1/flytekit/bin/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    24000 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/bin/entrypoint.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.106104 flytekit-1.9.1/flytekit/clients/
+-rw-r--r--   0 runner    (1001) docker     (999)      335 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.106104 flytekit-1.9.1/flytekit/clients/auth/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13495 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/auth/auth_client.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10281 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/auth/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (999)      411 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/auth/default_html.py
+-rw-r--r--   0 runner    (1001) docker     (999)      420 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/auth/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2053 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/auth/keyring.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5979 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/auth/token_client.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8232 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/auth_helper.py
+-rw-r--r--   0 runner    (1001) docker     (999)    50793 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/friendly.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.106104 flytekit-1.9.1/flytekit/clients/grpc_utils/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/grpc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3045 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/grpc_utils/auth_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1870 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2868 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (999)    28489 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clients/raw.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.106104 flytekit-1.9.1/flytekit/clis/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.106104 flytekit-1.9.1/flytekit/clis/flyte_cli/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/flyte_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      336 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/flyte_cli/example.config
+-rw-r--r--   0 runner    (1001) docker     (999)    81925 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/flyte_cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5900 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.110104 flytekit-1.9.1/flytekit/clis/sdk_in_container/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5269 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4612 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/build.py
+-rw-r--r--   0 runner    (1001) docker     (999)      833 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/constants.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2889 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1330 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/init.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2099 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/launchplan.py
+-rw-r--r--   0 runner    (1001) docker     (999)      395 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6734 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4344 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/package.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5482 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/pyflyte.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5930 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/register.py
+-rw-r--r--   0 runner    (1001) docker     (999)    32732 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/run.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8136 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1419 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/serve.py
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/clis/sdk_in_container/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.110104 flytekit-1.9.1/flytekit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (999)    36637 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1483 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/configuration/default_images.py
+-rw-r--r--   0 runner    (1001) docker     (999)      536 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/configuration/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11221 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/configuration/file.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7371 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/configuration/internal.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.118104 flytekit-1.9.1/flytekit/core/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      793 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16224 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/array_node_map_task.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2946 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/base_sql_task.py
+-rw-r--r--   0 runner    (1001) docker     (999)    33317 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/base_task.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5580 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1631 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/class_based_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (999)    22170 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1516 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6390 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/container_task.py
+-rw-r--r--   0 runner    (1001) docker     (999)    36721 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12882 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/data_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (999)      914 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2539 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/dynamic_workflow_task.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8366 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/gate.py
+-rw-r--r--   0 runner    (1001) docker     (999)      504 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/hash.py
+-rw-r--r--   0 runner    (1001) docker     (999)    18491 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (999)    20508 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2902 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/local_cache.py
+-rw-r--r--   0 runner    (1001) docker     (999)    18181 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/map_task.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2052 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/mock_stats.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6633 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/node.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8006 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/node_creation.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5173 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/notification.py
+-rw-r--r--   0 runner    (1001) docker     (999)      912 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/pod_template.py
+-rw-r--r--   0 runner    (1001) docker     (999)    42451 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/promise.py
+-rw-r--r--   0 runner    (1001) docker     (999)    13775 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/python_auto_container.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12399 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/python_customized_container_task.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15117 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/python_function_task.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2260 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/reference.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10861 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/reference_entity.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2979 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/resources.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8401 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8445 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/shim_task.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15723 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/task.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2496 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/testing.py
+-rw-r--r--   0 runner    (1001) docker     (999)      435 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/tracked_abc.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12604 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (999)    80132 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/type_engine.py
+-rw-r--r--   0 runner    (1001) docker     (999)      724 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/type_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (999)    12005 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (999)    38637 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/core/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.118104 flytekit-1.9.1/flytekit/deck/
+-rw-r--r--   0 runner    (1001) docker     (999)      256 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/deck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6839 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/deck/deck.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.118104 flytekit-1.9.1/flytekit/deck/html/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/deck/html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3775 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/deck/html/template.html
+-rw-r--r--   0 runner    (1001) docker     (999)     1321 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/deck/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.118104 flytekit-1.9.1/flytekit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)      328 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/exceptions/base.py
+-rw-r--r--   0 runner    (1001) docker     (999)     8994 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/exceptions/scopes.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1579 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/exceptions/system.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3028 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.118104 flytekit-1.9.1/flytekit/experimental/
+-rw-r--r--   0 runner    (1001) docker     (999)      182 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    22207 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/experimental/eager_function.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.118104 flytekit-1.9.1/flytekit/extend/
+-rw-r--r--   0 runner    (1001) docker     (999)     1446 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extend/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.122104 flytekit-1.9.1/flytekit/extend/backend/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extend/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4287 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extend/backend/agent_service.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7909 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extend/backend/base_agent.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.122104 flytekit-1.9.1/flytekit/extras/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1695 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/cloud_pickle_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.122104 flytekit-1.9.1/flytekit/extras/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (999)      895 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5164 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/pytorch/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3619 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/pytorch/native.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.122104 flytekit-1.9.1/flytekit/extras/sklearn/
+-rw-r--r--   0 runner    (1001) docker     (999)      660 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/sklearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3225 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/sklearn/native.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.122104 flytekit-1.9.1/flytekit/extras/sqlite3/
+-rw-r--r--   0 runner    (1001) docker     (999)      228 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/sqlite3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5244 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/sqlite3/task.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.122104 flytekit-1.9.1/flytekit/extras/tasks/
+-rw-r--r--   0 runner    (1001) docker     (999)      225 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    16445 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/tasks/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.122104 flytekit-1.9.1/flytekit/extras/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (999)     1058 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2763 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/tensorflow/model.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7672 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/extras/tensorflow/record.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.122104 flytekit-1.9.1/flytekit/image_spec/
+-rw-r--r--   0 runner    (1001) docker     (999)       34 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/image_spec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6910 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/image_spec/image_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.122104 flytekit-1.9.1/flytekit/interaction/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1595 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/interaction/parse_stdin.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.126104 flytekit-1.9.1/flytekit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6441 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/interfaces/cli_identifiers.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1118 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/interfaces/random.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.126104 flytekit-1.9.1/flytekit/interfaces/stats/
+-rw-r--r--   0 runner    (1001) docker     (999)      208 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/interfaces/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5068 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/interfaces/stats/client.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3062 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/interfaces/stats/taggable.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.126104 flytekit-1.9.1/flytekit/lazy_import/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/lazy_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1044 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/lazy_import/lazy_module.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3448 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/loggers.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.130104 flytekit-1.9.1/flytekit/models/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.130104 flytekit-1.9.1/flytekit/models/admin/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2054 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/admin/common.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5597 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/admin/task_execution.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4307 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/admin/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1371 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3843 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/array_job.py
+-rw-r--r--   0 runner    (1001) docker     (999)    14187 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/common.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.130104 flytekit-1.9.1/flytekit/models/core/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2561 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/core/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6056 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/core/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6918 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/core/condition.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2512 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/core/errors.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7152 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/core/execution.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7549 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/core/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2058 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (999)    33681 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/core/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3293 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3938 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/dynamic_job.py
+-rw-r--r--   0 runner    (1001) docker     (999)    26282 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/execution.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3890 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/filters.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7179 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/interface.py
+-rw-r--r--   0 runner    (1001) docker     (999)    14502 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/launch_plan.py
+-rw-r--r--   0 runner    (1001) docker     (999)    28383 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/literals.py
+-rw-r--r--   0 runner    (1001) docker     (999)    11777 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/matchable_resource.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2749 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/named_entity.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10667 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/node_execution.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2009 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/presto.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2256 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4558 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/qubole.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5149 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (999)     6482 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (999)    32711 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (999)    15678 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/types.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1581 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/models/workflow_closure.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.130104 flytekit-1.9.1/flytekit/remote/
+-rw-r--r--   0 runner    (1001) docker     (999)     2328 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4038 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/remote/backfill.py
+-rw-r--r--   0 runner    (1001) docker     (999)    31261 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/remote/entities.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7896 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/remote/executions.py
+-rw-r--r--   0 runner    (1001) docker     (999)      340 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/remote/interface.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2169 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/remote/lazy_entity.py
+-rw-r--r--   0 runner    (1001) docker     (999)    90250 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/remote/remote.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3764 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/remote/remote_callable.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.130104 flytekit-1.9.1/flytekit/sensor/
+-rw-r--r--   0 runner    (1001) docker     (999)      112 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/sensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2233 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/sensor/base_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (999)      626 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/sensor/file_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2267 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/sensor/sensor_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.130104 flytekit-1.9.1/flytekit/testing/
+-rw-r--r--   0 runner    (1001) docker     (999)      572 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.134104 flytekit-1.9.1/flytekit/tools/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4648 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/tools/fast_registration.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4355 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/tools/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (999)      413 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/tools/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1492 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/tools/module_loader.py
+-rw-r--r--   0 runner    (1001) docker     (999)    10803 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/tools/repo.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5763 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/tools/script_mode.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4468 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/tools/serialize_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (999)     1071 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/tools/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (999)    33778 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/tools/translator.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.134104 flytekit-1.9.1/flytekit/types/
+-rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.134104 flytekit-1.9.1/flytekit/types/directory/
+-rw-r--r--   0 runner    (1001) docker     (999)     1219 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/directory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    19461 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/directory/types.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.134104 flytekit-1.9.1/flytekit/types/file/
+-rw-r--r--   0 runner    (1001) docker     (999)     4699 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    23934 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/file/file.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.134104 flytekit-1.9.1/flytekit/types/iterator/
+-rw-r--r--   0 runner    (1001) docker     (999)      228 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/iterator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     2360 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/iterator/iterator.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.134104 flytekit-1.9.1/flytekit/types/numpy/
+-rw-r--r--   0 runner    (1001) docker     (999)       43 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3585 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/numpy/ndarray.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.134104 flytekit-1.9.1/flytekit/types/pickle/
+-rw-r--r--   0 runner    (1001) docker     (999)      231 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/pickle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     4101 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/pickle/pickle.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.134104 flytekit-1.9.1/flytekit/types/schema/
+-rw-r--r--   0 runner    (1001) docker     (999)      266 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)    18377 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/schema/types.py
+-rw-r--r--   0 runner    (1001) docker     (999)     5424 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/schema/types_pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.138104 flytekit-1.9.1/flytekit/types/structured/
+-rw-r--r--   0 runner    (1001) docker     (999)     2600 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (999)     7233 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/structured/basic_dfs.py
+-rw-r--r--   0 runner    (1001) docker     (999)     3917 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/structured/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (999)    44578 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit/types/structured/structured_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.106104 flytekit-1.9.1/flytekit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (999)     4315 2023-08-28 16:42:54.000000 flytekit-1.9.1/flytekit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (999)     7043 2023-08-28 16:42:54.000000 flytekit-1.9.1/flytekit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 16:42:54.000000 flytekit-1.9.1/flytekit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      319 2023-08-28 16:42:54.000000 flytekit-1.9.1/flytekit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (999)      873 2023-08-28 16:42:54.000000 flytekit-1.9.1/flytekit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (999)        9 2023-08-28 16:42:54.000000 flytekit-1.9.1/flytekit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 16:42:54.138104 flytekit-1.9.1/flytekit_scripts/
+-rw-r--r--   0 runner    (1001) docker     (999)      138 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit_scripts/Readme.rst
+-rwxr-xr-x   0 runner    (1001) docker     (999)     3006 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit_scripts/flytekit_build_image.sh
+-rw-r--r--   0 runner    (1001) docker     (999)      221 2023-08-28 16:42:38.000000 flytekit-1.9.1/flytekit_scripts/flytekit_venv
+-rw-r--r--   0 runner    (1001) docker     (999)      379 2023-08-28 16:42:38.000000 flytekit-1.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (999)      416 2023-08-28 16:42:54.138104 flytekit-1.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (999)     3728 2023-08-28 16:42:51.000000 flytekit-1.9.1/setup.py
```

### Comparing `flytekit-1.9.0a0/LICENSE` & `flytekit-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/MANIFEST.in` & `flytekit-1.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/PKG-INFO` & `flytekit-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.9.0a0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.9.1 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.9.0a0/README.md` & `flytekit-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/__init__.py` & `flytekit-1.9.1/flytekit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,17 +25,18 @@
    FlyteContext
    map_task
    ~core.workflow.ImperativeWorkflow
    ~core.node_creation.create_node
    ~core.promise.NodeOutput
    FlyteContextManager
 
-Running Locally
-------------------
-Tasks and Workflows can both be locally run (assuming the relevant tasks are capable of local execution). This is useful for unit testing.
+.. important::
+
+   Tasks and Workflows can both be locally run, assuming the relevant tasks are capable of local execution.
+   This is useful for unit testing.
 
 
 Branching and Conditionals
 ==========================
 
 Branches and conditionals can be expressed explicitly in Flyte. These conditions are evaluated
 in the flyte engine and hence should be used for control flow. ``dynamic workflows`` can be used to perform custom conditional logic not supported by flytekit
@@ -188,14 +189,15 @@
    :toctree: generated/
 
    Description
    Documentation
    SourceCode
 
 """
+import os
 import sys
 from typing import Generator
 
 from rich import traceback
 
 from flytekit.lazy_import.lazy_module import lazy_module
 
@@ -219,34 +221,36 @@
 from flytekit.core.pod_template import PodTemplate
 from flytekit.core.python_function_task import PythonFunctionTask, PythonInstanceTask
 from flytekit.core.reference import get_reference_entity
 from flytekit.core.reference_entity import LaunchPlanReference, TaskReference, WorkflowReference
 from flytekit.core.resources import Resources
 from flytekit.core.schedule import CronSchedule, FixedRate
 from flytekit.core.task import Secret, reference_task, task
+from flytekit.core.type_engine import BatchSize
 from flytekit.core.workflow import ImperativeWorkflow as Workflow
 from flytekit.core.workflow import WorkflowFailurePolicy, reference_workflow, workflow
 from flytekit.deck import Deck
 from flytekit.image_spec import ImageSpec
-from flytekit.loggers import logger
+from flytekit.loggers import LOGGING_RICH_FMT_ENV_VAR, logger
 from flytekit.models.common import Annotations, AuthRole, Labels
 from flytekit.models.core.execution import WorkflowExecutionPhase
 from flytekit.models.core.types import BlobType
 from flytekit.models.documentation import Description, Documentation, SourceCode
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
-from flytekit.types import directory, file
+from flytekit.sensor.sensor_engine import SensorEngine
+from flytekit.types import directory, file, iterator
 from flytekit.types.structured.structured_dataset import (
     StructuredDataset,
     StructuredDatasetFormat,
     StructuredDatasetTransformerEngine,
     StructuredDatasetType,
 )
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 
 def current_context() -> ExecutionParameters:
     """
     Use this method to get a handle of specific parameters available in a flyte task.
 
     Usage
@@ -299,8 +303,9 @@
         p.load()
 
 
 # Load all implicit plugins
 load_implicit_plugins()
 
 # Pretty-print exception messages
-traceback.install(width=None, extra_lines=0)
+if os.environ.get(LOGGING_RICH_FMT_ENV_VAR) != "0":
+    traceback.install(width=None, extra_lines=0)
```

### Comparing `flytekit-1.9.0a0/flytekit/bin/entrypoint.py` & `flytekit-1.9.1/flytekit/bin/entrypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import asyncio
 import contextlib
 import datetime as _datetime
+import inspect
 import os
 import pathlib
+import signal
 import subprocess
 import tempfile
 import traceback as _traceback
 from typing import List, Optional
 
 import click as _click
 from flyteidl.core import literals_pb2 as _literals_pb2
@@ -14,20 +17,22 @@
     SERIALIZED_CONTEXT_ENV_VAR,
     FastSerializationSettings,
     SerializationSettings,
     StatsConfig,
 )
 from flytekit.core import constants as _constants
 from flytekit.core import utils
+from flytekit.core.array_node_map_task import ArrayNodeMapTaskResolver
 from flytekit.core.base_task import IgnoreOutputs, PythonTask
 from flytekit.core.checkpointer import SyncCheckpoint
 from flytekit.core.context_manager import ExecutionParameters, ExecutionState, FlyteContext, FlyteContextManager
 from flytekit.core.data_persistence import FileAccessProvider
 from flytekit.core.map_task import MapTaskResolver
 from flytekit.core.promise import VoidPromise
+from flytekit.deck.deck import _output_deck
 from flytekit.exceptions import scopes as _scoped_exceptions
 from flytekit.exceptions import scopes as _scopes
 from flytekit.interfaces.stats.taggable import get_stats as _get_stats
 from flytekit.loggers import entrypoint_logger as logger
 from flytekit.loggers import user_space_logger
 from flytekit.models import dynamic_job as _dynamic_job
 from flytekit.models import literals as _literal_models
@@ -84,14 +89,19 @@
         input_proto = utils.load_proto_from_file(_literals_pb2.LiteralMap, local_inputs_file)
         idl_input_literals = _literal_models.LiteralMap.from_flyte_idl(input_proto)
 
         # Step2
         # Decorate the dispatch execute function before calling it, this wraps all exceptions into one
         # of the FlyteScopedExceptions
         outputs = _scoped_exceptions.system_entry_point(task_def.dispatch_execute)(ctx, idl_input_literals)
+        if inspect.iscoroutine(outputs):
+            # Handle eager-mode (async) tasks
+            logger.info("Output is a coroutine")
+            outputs = asyncio.run(outputs)
+
         # Step3a
         if isinstance(outputs, VoidPromise):
             logger.warning("Task produces no outputs")
             output_file_dict = {_constants.OUTPUT_FILE_NAME: _literal_models.LiteralMap(literals={})}
         elif isinstance(outputs, _literal_models.LiteralMap):
             output_file_dict = {_constants.OUTPUT_FILE_NAME: outputs}
         elif isinstance(outputs, _dynamic_job.DynamicJobSpec):
@@ -154,14 +164,18 @@
         logger.error("!! End Error Captured by Flyte !!")
 
     for k, v in output_file_dict.items():
         utils.write_proto_to_file(v.to_flyte_idl(), os.path.join(ctx.execution_state.engine_dir, k))
 
     ctx.file_access.put_data(ctx.execution_state.engine_dir, output_prefix, is_multipart=True)
     logger.info(f"Engine folder written successfully to the output prefix {output_prefix}")
+
+    if not getattr(task_def, "disable_deck", True):
+        _output_deck(task_def.name.split(".")[-1], ctx.user_space_params)
+
     logger.debug("Finished _dispatch_execute")
 
     if os.environ.get("FLYTE_FAIL_ON_ERROR", "").lower() == "true" and _constants.ERROR_FILE_NAME in output_file_dict:
         # This env is set by the flytepropeller
         # AWS batch job get the status from the exit code, so once we catch the error,
         # we should return the error code here
         exit(1)
@@ -179,22 +193,24 @@
             return os.environ[k]
     return ""
 
 
 @contextlib.contextmanager
 def setup_execution(
     raw_output_data_prefix: str,
+    output_metadata_prefix: Optional[str] = None,
     checkpoint_path: Optional[str] = None,
     prev_checkpoint: Optional[str] = None,
     dynamic_addl_distro: Optional[str] = None,
     dynamic_dest_dir: Optional[str] = None,
 ):
     """
 
-    :param raw_output_data_prefix:
+    :param raw_output_data_prefix: Where to write offloaded data (files, directories, dataframes).
+    :param output_metadata_prefix: Where to write primitive outputs.
     :param checkpoint_path:
     :param prev_checkpoint:
     :param dynamic_addl_distro: Works in concert with the other dynamic arg. If present, indicates that if a dynamic
       task were to run, it should set fast serialize to true and use these values in FastSerializationSettings
     :param dynamic_dest_dir: See above.
     :return:
     """
@@ -243,14 +259,15 @@
                 "exec_launchplan": exe_lp,
                 "api_version": _api_version,
             },
         ),
         logging=user_space_logger,
         tmp_dir=user_workspace_dir,
         raw_output_prefix=raw_output_data_prefix,
+        output_metadata_prefix=output_metadata_prefix,
         checkpoint=checkpointer,
         task_id=_identifier.Identifier(_identifier.ResourceType.TASK, tk_project, tk_domain, tk_name, tk_version),
     )
 
     try:
         file_access = FileAccessProvider(
             local_sandbox_dir=tempfile.mkdtemp(prefix="flyte"),
@@ -333,14 +350,15 @@
     :return:
     """
     if len(resolver_args) < 1:
         raise Exception("cannot be <1")
 
     with setup_execution(
         raw_output_data_prefix,
+        output_prefix,
         checkpoint_path,
         prev_checkpoint,
         dynamic_addl_distro,
         dynamic_dest_dir,
     ) as ctx:
         resolver_obj = load_object_from_module(resolver)
         # Use the resolver to load the actual task object
@@ -362,14 +380,15 @@
     test,
     resolver: str,
     resolver_args: List[str],
     checkpoint_path: Optional[str] = None,
     prev_checkpoint: Optional[str] = None,
     dynamic_addl_distro: Optional[str] = None,
     dynamic_dest_dir: Optional[str] = None,
+    experimental: Optional[bool] = False,
 ):
     """
     This function should be called by map task and aws-batch task
     resolver should be something like:
         flytekit.core.python_auto_container.default_task_resolver
     resolver args should be something like
         task_module app.workflows task_name task_1
@@ -386,19 +405,22 @@
     """
     if len(resolver_args) < 1:
         raise Exception(f"Resolver args cannot be <1, got {resolver_args}")
 
     with setup_execution(
         raw_output_data_prefix, checkpoint_path, prev_checkpoint, dynamic_addl_distro, dynamic_dest_dir
     ) as ctx:
-        mtr = MapTaskResolver()
-        map_task = mtr.load_task(loader_args=resolver_args, max_concurrency=max_concurrency)
-
         task_index = _compute_array_job_index()
-        output_prefix = os.path.join(output_prefix, str(task_index))
+        if experimental:
+            mtr = ArrayNodeMapTaskResolver()
+        else:
+            mtr = MapTaskResolver()
+            output_prefix = os.path.join(output_prefix, str(task_index))
+
+        map_task = mtr.load_task(loader_args=resolver_args, max_concurrency=max_concurrency)
 
         if test:
             logger.info(
                 f"Test detected, returning. Inputs: {inputs} Computed task index: {task_index} "
                 f"New output prefix: {output_prefix} Raw output path: {raw_output_data_prefix} "
                 f"Resolver and args: {resolver} {resolver_args}"
             )
@@ -501,28 +523,37 @@
     for arg in task_execute_cmd:
         if arg == "--resolver":
             cmd.extend(["--dynamic-addl-distro", additional_distribution, "--dynamic-dest-dir", dest_dir])
         cmd.append(arg)
 
     # Use the commandline to run the task execute command rather than calling it directly in python code
     # since the current runtime bytecode references the older user code, rather than the downloaded distribution.
-    subprocess.run(cmd, check=True)
+    p = subprocess.Popen(cmd)
+
+    def handle_sigterm(signum, frame):
+        logger.info(f"passing signum {signum} [frame={frame}] to subprocess")
+        p.send_signal(signum)
+
+    signal.signal(signal.SIGTERM, handle_sigterm)
+    returncode = p.wait()
+    exit(returncode)
 
 
 @_pass_through.command("pyflyte-map-execute")
 @_click.option("--inputs", required=True)
 @_click.option("--output-prefix", required=True)
 @_click.option("--raw-output-data-prefix", required=False)
 @_click.option("--max-concurrency", type=int, required=False)
 @_click.option("--test", is_flag=True)
 @_click.option("--dynamic-addl-distro", required=False)
 @_click.option("--dynamic-dest-dir", required=False)
 @_click.option("--resolver", required=True)
 @_click.option("--checkpoint-path", required=False)
 @_click.option("--prev-checkpoint", required=False)
+@_click.option("--experimental", is_flag=True, default=False, required=False)
 @_click.argument(
     "resolver-args",
     type=_click.UNPROCESSED,
     nargs=-1,
 )
 def map_execute_task_cmd(
     inputs,
@@ -531,14 +562,15 @@
     max_concurrency,
     test,
     dynamic_addl_distro,
     dynamic_dest_dir,
     resolver,
     resolver_args,
     prev_checkpoint,
+    experimental,
     checkpoint_path,
 ):
     logger.info(get_version_message())
 
     raw_output_data_prefix, checkpoint_path, prev_checkpoint = normalize_inputs(
         raw_output_data_prefix, checkpoint_path, prev_checkpoint
     )
@@ -551,12 +583,13 @@
         test=test,
         dynamic_addl_distro=dynamic_addl_distro,
         dynamic_dest_dir=dynamic_dest_dir,
         resolver=resolver,
         resolver_args=resolver_args,
         checkpoint_path=checkpoint_path,
         prev_checkpoint=prev_checkpoint,
+        experimental=experimental,
     )
 
 
 if __name__ == "__main__":
     _pass_through()
```

### Comparing `flytekit-1.9.0a0/flytekit/clients/auth/auth_client.py` & `flytekit-1.9.1/flytekit/clients/auth/auth_client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clients/auth/authenticator.py` & `flytekit-1.9.1/flytekit/clients/auth/authenticator.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     token_endpoint: str
     authorization_endpoint: str
     redirect_uri: str
     client_id: str
     device_authorization_endpoint: typing.Optional[str] = None
     scopes: typing.List[str] = None
     header_key: str = "authorization"
+    audience: typing.Optional[str] = None
 
 
 class ClientConfigStore(object):
     """
     Client Config store retrieve client config. this can be done in multiple ways
     """
 
@@ -170,43 +171,52 @@
         client_id: str,
         client_secret: str,
         cfg_store: ClientConfigStore,
         header_key: typing.Optional[str] = None,
         scopes: typing.Optional[typing.List[str]] = None,
         http_proxy_url: typing.Optional[str] = None,
         verify: typing.Optional[typing.Union[bool, str]] = None,
+        audience: typing.Optional[str] = None,
     ):
         if not client_id or not client_secret:
             raise ValueError("Client ID and Client SECRET both are required.")
         cfg = cfg_store.get_client_config()
         self._token_endpoint = cfg.token_endpoint
         # Use scopes from `flytekit.configuration.PlatformConfig` if passed
         self._scopes = scopes or cfg.scopes
         self._client_id = client_id
         self._client_secret = client_secret
+        self._audience = audience or cfg.audience
         super().__init__(endpoint, cfg.header_key or header_key, http_proxy_url=http_proxy_url, verify=verify)
 
     def refresh_credentials(self):
         """
         This function is used by the _handle_rpc_error() decorator, depending on the AUTH_MODE config object. This handler
         is meant for SDK use-cases of auth (like pyflyte, or when users call SDK functions that require access to Admin,
         like when waiting for another workflow to complete from within a task). This function uses basic auth, which means
         the credentials for basic auth must be present from wherever this code is running.
 
         """
         token_endpoint = self._token_endpoint
         scopes = self._scopes
+        audience = self._audience
 
         # Note that unlike the Pkce flow, the client ID does not come from Admin.
         logging.debug(f"Basic authorization flow with client id {self._client_id} scope {scopes}")
         authorization_header = token_client.get_basic_authorization_header(self._client_id, self._client_secret)
 
         token, expires_in = token_client.get_token(
-            token_endpoint, scopes, authorization_header, http_proxy_url=self._http_proxy_url, verify=self._verify
+            token_endpoint=token_endpoint,
+            authorization_header=authorization_header,
+            http_proxy_url=self._http_proxy_url,
+            verify=self._verify,
+            scopes=scopes,
+            audience=audience,
         )
+
         logging.info("Retrieved new token, expires in {}".format(expires_in))
         self._creds = Credentials(token)
 
 
 class DeviceCodeAuthenticator(Authenticator):
     """
     This Authenticator implements the Device Code authorization flow useful for headless user authentication.
```

### Comparing `flytekit-1.9.0a0/flytekit/clients/auth/keyring.py` & `flytekit-1.9.1/flytekit/clients/auth/keyring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clients/auth/token_client.py` & `flytekit-1.9.1/flytekit/clients/auth/token_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 
 def get_token(
     token_endpoint: str,
     scopes: typing.Optional[typing.List[str]] = None,
     authorization_header: typing.Optional[str] = None,
     client_id: typing.Optional[str] = None,
     device_code: typing.Optional[str] = None,
+    audience: typing.Optional[str] = None,
     grant_type: GrantType = GrantType.CLIENT_CREDS,
     http_proxy_url: typing.Optional[str] = None,
     verify: typing.Optional[typing.Union[bool, str]] = None,
 ) -> typing.Tuple[str, int]:
     """
     :rtype: (Text,Int) The first element is the access token retrieved from the IDP, the second is the expiration
             in seconds
@@ -94,17 +95,20 @@
     }
     if client_id:
         body["client_id"] = client_id
     if device_code:
         body["device_code"] = device_code
     if scopes is not None:
         body["scope"] = ",".join(scopes)
+    if audience:
+        body["audience"] = audience
 
     proxies = {"https": http_proxy_url, "http": http_proxy_url} if http_proxy_url else None
     response = requests.post(token_endpoint, data=body, headers=headers, proxies=proxies, verify=verify)
+
     if not response.ok:
         j = response.json()
         if "error" in j:
             err = j["error"]
             if err == error_auth_pending or err == error_slow_down:
                 raise AuthenticationPending(f"Token not yet available, try again in some time {err}")
         logging.error("Status Code ({}) received from IDP: {}".format(response.status_code, response.text))
```

### Comparing `flytekit-1.9.0a0/flytekit/clients/auth_helper.py` & `flytekit-1.9.1/flytekit/clients/auth_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             token_endpoint=oauth2_metadata.token_endpoint,
             authorization_endpoint=oauth2_metadata.authorization_endpoint,
             redirect_uri=public_client_config.redirect_uri,
             client_id=public_client_config.client_id,
             scopes=public_client_config.scopes,
             header_key=public_client_config.authorization_metadata_key or None,
             device_authorization_endpoint=oauth2_metadata.device_authorization_endpoint,
+            audience=public_client_config.audience,
         )
 
 
 def get_authenticator(cfg: PlatformConfig, cfg_store: ClientConfigStore) -> Authenticator:
     """
     Returns a new authenticator based on the platform config.
     """
@@ -69,14 +70,15 @@
     elif cfg_auth == AuthType.BASIC or cfg_auth == AuthType.CLIENT_CREDENTIALS or cfg_auth == AuthType.CLIENTSECRET:
         return ClientCredentialsAuthenticator(
             endpoint=cfg.endpoint,
             client_id=cfg.client_id,
             client_secret=cfg.client_credentials_secret,
             cfg_store=cfg_store,
             scopes=cfg.scopes,
+            audience=cfg.audience,
             http_proxy_url=cfg.http_proxy_url,
             verify=verify,
         )
     elif cfg_auth == AuthType.EXTERNAL_PROCESS or cfg_auth == AuthType.EXTERNALCOMMAND:
         client_cfg = None
         if cfg_store:
             client_cfg = cfg_store.get_client_config()
@@ -172,15 +174,17 @@
         return grpc.insecure_channel(cfg.endpoint, **kwargs)
 
     credentials = None
     if "credentials" not in kwargs:
         if cfg.insecure_skip_verify:
             credentials = bootstrap_creds_from_server(cfg.endpoint)
         elif cfg.ca_cert_file_path:
-            credentials = grpc.ssl_channel_credentials(load_cert(cfg.ca_cert_file_path))
+            credentials = grpc.ssl_channel_credentials(
+                crypto.dump_certificate(crypto.FILETYPE_PEM, load_cert(cfg.ca_cert_file_path))
+            )
         else:
             credentials = grpc.ssl_channel_credentials(
                 root_certificates=kwargs.get("root_certificates", None),
                 private_key=kwargs.get("private_key", None),
                 certificate_chain=kwargs.get("certificate_chain", None),
             )
     else:
```

### Comparing `flytekit-1.9.0a0/flytekit/clients/friendly.py` & `flytekit-1.9.1/flytekit/clients/friendly.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clients/grpc_utils/auth_interceptor.py` & `flytekit-1.9.1/flytekit/clients/grpc_utils/auth_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clients/grpc_utils/wrap_exception_interceptor.py` & `flytekit-1.9.1/flytekit/clients/grpc_utils/wrap_exception_interceptor.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clients/helpers.py` & `flytekit-1.9.1/flytekit/clients/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clients/raw.py` & `flytekit-1.9.1/flytekit/clients/raw.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clis/flyte_cli/main.py` & `flytekit-1.9.1/flytekit/clis/flyte_cli/main.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clis/helpers.py` & `flytekit-1.9.1/flytekit/clis/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/backfill.py` & `flytekit-1.9.1/flytekit/clis/sdk_in_container/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/build.py` & `flytekit-1.9.1/flytekit/clis/sdk_in_container/build.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     """
 
     def __init__(self, filename: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._filename = pathlib.Path(filename).resolve()
 
     def list_commands(self, ctx):
-        entities = get_entities_in_file(self._filename.__str__())
+        entities = get_entities_in_file(self._filename.__str__(), False)
         return entities.all()
 
     def get_command(self, ctx, exe_entity):
         """
         This command uses the filename with which this command was created, and the string name of the entity passed
           after the Python filename on the command line, to load the Python object, and then return the Command that
           click should run.
```

### Comparing `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/constants.py` & `flytekit-1.9.1/flytekit/clis/sdk_in_container/constants.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 CTX_PACKAGES = "pkgs"
 CTX_NOTIFICATIONS = "notifications"
 CTX_CONFIG_FILE = "config_file"
 CTX_PROJECT_ROOT = "project_root"
 CTX_MODULE = "module"
 CTX_VERBOSE = "verbose"
 CTX_COPY_ALL = "copy_all"
+CTX_FILE_NAME = "file_name"
 
 
 project_option = _click.option(
     "-p",
     "--project",
     required=True,
     type=str,
```

### Comparing `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/helpers.py` & `flytekit-1.9.1/flytekit/clis/sdk_in_container/helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/init.py` & `flytekit-1.9.1/flytekit/clis/sdk_in_container/init.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/launchplan.py` & `flytekit-1.9.1/flytekit/clis/sdk_in_container/launchplan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/metrics.py` & `flytekit-1.9.1/flytekit/clis/sdk_in_container/metrics.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/package.py` & `flytekit-1.9.1/flytekit/clis/sdk_in_container/package.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/pyflyte.py` & `flytekit-1.9.1/flytekit/clis/sdk_in_container/pyflyte.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import typing
 
 import grpc
 import rich_click as click
 from google.protobuf.json_format import MessageToJson
 
 from flytekit import configuration
@@ -13,14 +14,15 @@
 from flytekit.clis.sdk_in_container.local_cache import local_cache
 from flytekit.clis.sdk_in_container.metrics import metrics
 from flytekit.clis.sdk_in_container.package import package
 from flytekit.clis.sdk_in_container.register import register
 from flytekit.clis.sdk_in_container.run import run
 from flytekit.clis.sdk_in_container.serialize import serialize
 from flytekit.clis.sdk_in_container.serve import serve
+from flytekit.configuration.file import FLYTECTL_CONFIG_ENV_VAR, FLYTECTL_CONFIG_ENV_VAR_OVERRIDE
 from flytekit.configuration.internal import LocalSDK
 from flytekit.exceptions.base import FlyteException
 from flytekit.exceptions.user import FlyteInvalidInputException
 from flytekit.loggers import cli_logger
 
 
 def validate_package(ctx, param, values):
@@ -77,18 +79,18 @@
 
 class ErrorHandlingCommand(click.RichGroup):
     def invoke(self, ctx: click.Context) -> typing.Any:
         try:
             return super().invoke(ctx)
         except Exception as e:
             if CTX_VERBOSE in ctx.obj and ctx.obj[CTX_VERBOSE]:
-                print("Verbose mode on")
+                click.secho("Verbose mode on")
                 raise e
             pretty_print_exception(e)
-            raise SystemExit(e)
+            raise SystemExit(e) from e
 
 
 @click.group("pyflyte", invoke_without_command=True, cls=ErrorHandlingCommand)
 @click.option(
     "--verbose", required=False, default=False, is_flag=True, help="Show verbose messages and exception traces"
 )
 @click.option(
@@ -116,14 +118,20 @@
     ctx.obj = dict()
 
     # Handle package management - get from the command line, the environment variables, then the config file.
     pkgs = pkgs or LocalSDK.WORKFLOW_PACKAGES.read() or []
     if config:
         ctx.obj[CTX_CONFIG_FILE] = config
         cfg = configuration.ConfigFile(config)
+        # Set here so that if someone has Config.auto() in their user code, the config here will get used.
+        if FLYTECTL_CONFIG_ENV_VAR in os.environ:
+            cli_logger.info(
+                f"Config file arg {config} will override env var {FLYTECTL_CONFIG_ENV_VAR}: {os.environ[FLYTECTL_CONFIG_ENV_VAR]}"
+            )
+        os.environ[FLYTECTL_CONFIG_ENV_VAR_OVERRIDE] = config
         if not pkgs:
             pkgs = LocalSDK.WORKFLOW_PACKAGES.read(cfg)
             if pkgs is None:
                 pkgs = []
     ctx.obj[CTX_PACKAGES] = pkgs
     ctx.obj[CTX_VERBOSE] = verbose
```

### Comparing `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/register.py` & `flytekit-1.9.1/flytekit/clis/sdk_in_container/register.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/run.py` & `flytekit-1.9.1/flytekit/clis/sdk_in_container/run.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import asyncio
 import datetime
 import functools
 import importlib
+import inspect
 import json
 import logging
 import os
 import pathlib
 import typing
 from dataclasses import dataclass
 from typing import cast
@@ -17,14 +19,15 @@
 from typing_extensions import get_args
 
 from flytekit import BlobType, Literal, Scalar
 from flytekit.clis.sdk_in_container.constants import (
     CTX_CONFIG_FILE,
     CTX_COPY_ALL,
     CTX_DOMAIN,
+    CTX_FILE_NAME,
     CTX_MODULE,
     CTX_PROJECT,
     CTX_PROJECT_ROOT,
 )
 from flytekit.clis.sdk_in_container.helpers import (
     FLYTE_REMOTE_INSTANCE_KEY,
     get_and_save_remote_with_click_context,
@@ -39,14 +42,15 @@
 from flytekit.core.type_engine import TypeEngine
 from flytekit.core.workflow import PythonFunctionWorkflow, WorkflowBase
 from flytekit.models import literals
 from flytekit.models.interface import Variable
 from flytekit.models.literals import Blob, BlobMetadata, LiteralCollection, LiteralMap, Primitive, Union
 from flytekit.models.types import LiteralType, SimpleType
 from flytekit.remote.executions import FlyteWorkflowExecution
+from flytekit.remote.remote import FlyteRemote
 from flytekit.tools import module_loader, script_mode
 from flytekit.tools.script_mode import _find_project_root
 from flytekit.tools.translator import Options
 from flytekit.types.pickle.pickle import FlytePickleTransformer
 
 REMOTE_FLAG_KEY = "remote"
 RUN_LEVEL_PARAMS_KEY = "run_level_params"
@@ -107,21 +111,23 @@
 
 class PickleParamType(click.ParamType):
     name = "pickle"
 
     def convert(
         self, value: typing.Any, param: typing.Optional[click.Parameter], ctx: typing.Optional[click.Context]
     ) -> typing.Any:
+
         uri = FlyteContextManager.current_context().file_access.get_random_local_path()
         with open(uri, "w+b") as outfile:
             cloudpickle.dump(value, outfile)
         return FileParam(filepath=str(pathlib.Path(uri).resolve()))
 
 
 class DateTimeType(click.DateTime):
+
     _NOW_FMT = "now"
     _ADDITONAL_FORMATS = [_NOW_FMT]
 
     def __init__(self):
         super().__init__()
         self.formats.extend(self._ADDITONAL_FORMATS)
 
@@ -270,14 +276,15 @@
             uri = native_url[: -len(remote_filename)]
 
         return uri
 
     def convert_to_structured_dataset(
         self, ctx: typing.Optional[click.Context], param: typing.Optional[click.Parameter], value: Directory
     ) -> Literal:
+
         uri = self.get_uri_for_dir(ctx, value, "00000.parquet")
 
         lit = Literal(
             scalar=Scalar(
                 structured_dataset=literals.StructuredDataset(
                     uri=uri,
                     metadata=literals.StructuredDatasetMetadata(
@@ -331,15 +338,15 @@
             )
             try:
                 # Here we use click converter to convert the input in command line to native python type,
                 # and then use flyte converter to convert it to literal.
                 python_val = converter._click_type.convert(value, param, ctx)
                 literal = converter.convert_to_literal(ctx, param, python_val)
                 return Literal(scalar=Scalar(union=Union(literal, variant)))
-            except Exception or AttributeError as e:
+            except (Exception or AttributeError) as e:
                 logging.debug(f"Failed to convert python type {python_type} to literal type {variant}", e)
         raise ValueError(f"Failed to convert python type {self._python_type} to literal type {lt}")
 
     def convert_to_list(
         self, ctx: typing.Optional[click.Context], param: typing.Optional[click.Parameter], value: list
     ) -> Literal:
         """
@@ -392,18 +399,15 @@
         param: typing.Optional[click.Parameter],
         value: typing.Union[dict, typing.Any],
     ) -> Literal:
         """
         Convert the loaded json object to a Flyte Literal struct type.
         """
         if type(value) != self._python_type:
-            if is_pydantic_basemodel(self._python_type):
-                o = self._python_type.parse_raw(json.dumps(value))  # type: ignore
-            else:
-                o = cast(DataClassJsonMixin, self._python_type).from_json(json.dumps(value))
+            o = cast(DataClassJsonMixin, self._python_type).from_json(json.dumps(value))
         else:
             o = value
         return TypeEngine.to_literal(self._flyte_ctx, o, self._python_type, self._literal_type)
 
     def convert_to_literal(
         self, ctx: typing.Optional[click.Context], param: typing.Optional[click.Parameter], value: typing.Any
     ) -> Literal:
@@ -442,23 +446,14 @@
             return lit
         except click.BadParameter:
             raise
         except Exception as e:
             raise click.BadParameter(f"Failed to convert param {param}, {value} to {self._python_type}") from e
 
 
-def is_pydantic_basemodel(python_type: typing.Type) -> bool:
-    try:
-        import pydantic
-    except ImportError:
-        return False
-    else:
-        return issubclass(python_type, pydantic.BaseModel)
-
-
 def to_click_option(
     ctx: click.Context,
     flyte_ctx: FlyteContext,
     input_name: str,
     literal_var: Variable,
     python_type: typing.Type,
     default_val: typing.Any,
@@ -586,14 +581,21 @@
         ),
         click.Option(
             param_decls=["--envs", "envs"],
             required=False,
             type=JsonParamType(),
             help="Environment variables to set in the container",
         ),
+        click.Option(
+            param_decls=["--tag", "tag"],
+            required=False,
+            multiple=True,
+            type=str,
+            help="Tags to set for the execution",
+        ),
     ]
 
 
 def load_naive_entity(module_name: str, entity_name: str, project_root: str) -> typing.Union[WorkflowBase, PythonTask]:
     """
     Load the workflow of a script file.
     N.B.: it assumes that the file is self-contained, in other words, there are no relative imports.
@@ -631,15 +633,15 @@
     def all(self) -> typing.List[str]:
         e = []
         e.extend(self.workflows)
         e.extend(self.tasks)
         return e
 
 
-def get_entities_in_file(filename: str) -> Entities:
+def get_entities_in_file(filename: pathlib.Path, should_delete: bool) -> Entities:
     """
     Returns a list of flyte workflow names and list of Flyte tasks in a file.
     """
     flyte_ctx = context_manager.FlyteContextManager.current_context().new_builder()
     module_name = os.path.splitext(os.path.relpath(filename))[0].replace(os.path.sep, ".")
     with context_manager.FlyteContextManager.with_context(flyte_ctx):
         with module_loader.add_sys_path(os.getcwd()):
@@ -651,14 +653,16 @@
     for name in dir(module):
         o = module.__dict__[name]
         if isinstance(o, WorkflowBase):
             workflows.append(name)
         elif isinstance(o, PythonTask):
             tasks.append(name)
 
+    if should_delete and os.path.exists(filename):
+        os.remove(filename)
     return Entities(workflows, tasks)
 
 
 def run_command(ctx: click.Context, entity: typing.Union[PythonFunctionWorkflow, PythonTask]):
     """
     Returns a function that is used to implement WorkflowCommand and execute a flyte workflow.
     """
@@ -670,18 +674,23 @@
         project, domain = run_level_params.get("project"), run_level_params.get("domain")
         inputs = {}
         for input_name, _ in entity.python_interface.inputs.items():
             inputs[input_name] = kwargs.get(input_name)
 
         if not ctx.obj[REMOTE_FLAG_KEY]:
             output = entity(**inputs)
+            if inspect.iscoroutine(output):
+                # TODO: make eager mode workflows run with local-mode
+                output = asyncio.run(output)
             click.echo(output)
+            if ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_FILE_NAME):
+                os.remove(ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_FILE_NAME))
             return
 
-        remote = ctx.obj[FLYTE_REMOTE_INSTANCE_KEY]
+        remote: FlyteRemote = ctx.obj[FLYTE_REMOTE_INSTANCE_KEY]
         config_file = ctx.obj.get(CTX_CONFIG_FILE)
 
         image_config = run_level_params.get("image_config")
         image_config = patch_image_config(config_file, image_config)
 
         remote_entity = remote.register_script(
             entity,
@@ -708,49 +717,66 @@
             domain=domain,
             name=run_level_params.get("name"),
             wait=run_level_params.get("wait_execution"),
             options=options,
             type_hints=entity.python_interface.inputs,
             overwrite_cache=run_level_params.get("overwrite_cache"),
             envs=run_level_params.get("envs"),
+            tags=run_level_params.get("tag"),
         )
 
         console_url = remote.generate_console_url(execution)
         click.secho(f"Go to {console_url} to see execution in the console.")
 
         if run_level_params.get("dump_snippet"):
             dump_flyte_remote_snippet(execution, project, domain)
 
+        if ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_FILE_NAME):
+            os.remove(ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_FILE_NAME))
+
     return _run
 
 
 class WorkflowCommand(click.RichGroup):
     """
     click multicommand at the python file layer, subcommands should be all the workflows in the file.
     """
 
     def __init__(self, filename: str, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        self._filename = pathlib.Path(filename).resolve()
+
+        ctx = context_manager.FlyteContextManager.current_context()
+        if ctx.file_access.is_remote(filename):
+            local_path = os.path.join(os.path.curdir, filename.rsplit("/", 1)[1])
+            ctx.file_access.download(filename, local_path)
+            self._filename = pathlib.Path(local_path).resolve()
+            self._should_delete = True
+        else:
+            self._filename = pathlib.Path(filename).resolve()
+            self._should_delete = False
+        self._entities = None
 
     def list_commands(self, ctx):
-        entities = get_entities_in_file(self._filename)
+        entities = get_entities_in_file(self._filename, self._should_delete)
+        self._entities = entities
         return entities.all()
 
     def get_command(self, ctx, exe_entity):
         """
         This command uses the filename with which this command was created, and the string name of the entity passed
           after the Python filename on the command line, to load the Python object, and then return the Command that
           click should run.
         :param ctx: The click Context object.
         :param exe_entity: string of the flyte entity provided by the user. Should be the name of a workflow, or task
           function.
         :return:
         """
-
+        is_workflow = False
+        if self._entities:
+            is_workflow = exe_entity in self._entities.workflows
         rel_path = os.path.relpath(self._filename)
         if rel_path.startswith(".."):
             raise ValueError(
                 f"You must call pyflyte from the same or parent dir, {self._filename} not under {os.getcwd()}"
             )
 
         project_root = _find_project_root(self._filename)
@@ -759,15 +785,16 @@
         # N.B.: by construction project_root will necessarily be an ancestor of the filename passed in as
         # a parameter.
         rel_path = self._filename.relative_to(project_root)
         module = os.path.splitext(rel_path)[0].replace(os.path.sep, ".")
 
         ctx.obj[RUN_LEVEL_PARAMS_KEY][CTX_PROJECT_ROOT] = project_root
         ctx.obj[RUN_LEVEL_PARAMS_KEY][CTX_MODULE] = module
-
+        if self._should_delete:
+            ctx.obj[RUN_LEVEL_PARAMS_KEY][CTX_FILE_NAME] = self._filename
         entity = load_naive_entity(module, exe_entity, project_root)
 
         # If this is a remote execution, which we should know at this point, then create the remote object
         p = ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_PROJECT)
         d = ctx.obj[RUN_LEVEL_PARAMS_KEY].get(CTX_DOMAIN)
         r = get_and_save_remote_with_click_context(ctx, p, d)
         get_upload_url_fn = functools.partial(r.client.get_upload_signed_url, project=p, domain=d)
@@ -778,19 +805,24 @@
         params = []
         for input_name, input_type_val in entity.python_interface.inputs_with_defaults.items():
             literal_var = entity.interface.inputs.get(input_name)
             python_type, default_val = input_type_val
             params.append(
                 to_click_option(ctx, flyte_ctx, input_name, literal_var, python_type, default_val, get_upload_url_fn)
             )
-        cmd = click.Command(
+
+        entity_type = "Workflow" if is_workflow else "Task"
+        h = f"{click.style(entity_type, bold=True)} ({module}.{exe_entity})"
+        if entity.__doc__:
+            h = h + click.style(f"{entity.__doc__}", dim=True)
+        cmd = click.RichCommand(
             name=exe_entity,
             params=params,
             callback=run_command(ctx, entity),
-            help=f"Run {module}.{exe_entity} in script mode",
+            help=h,
         )
         return cmd
 
 
 class RunCommand(click.RichGroup):
     """
     A click command group for registering and executing flyte workflows & tasks in a file.
@@ -802,23 +834,22 @@
 
     def list_commands(self, ctx):
         return [str(p) for p in pathlib.Path(".").glob("*.py") if str(p) != "__init__.py"]
 
     def get_command(self, ctx, filename):
         if ctx.obj:
             ctx.obj[RUN_LEVEL_PARAMS_KEY] = ctx.params
-        return WorkflowCommand(filename, name=filename, help="Run a [workflow|task] in a file using script mode")
+        return WorkflowCommand(filename, name=filename, help=f"Run a [workflow|task] from {filename}")
 
 
 _run_help = """
-This command can execute either a workflow or a task from the command line, for fully self-contained scripts.
-Tasks and workflows cannot be imported from other files currently. Please use ``pyflyte package`` or
-``pyflyte register`` to handle those and then launch from the Flyte UI or ``flytectl``.
+This command can execute either a workflow or a task from the command line, allowing for fully self-contained scripts.
+Tasks and workflows can be imported from other files.
 
-Note: This command only works on regular Python packages, not namespace packages. When determining
-the root of your project, it finds the first folder that does not have an ``__init__.py`` file.
+Note: This command is compatible with regular Python packages, but not with namespace packages.
+When determining the root of your project, it identifies the first folder without an ``__init__.py`` file.
 """
 
 run = RunCommand(
     name="run",
     help=_run_help,
 )
```

### Comparing `flytekit-1.9.0a0/flytekit/clis/sdk_in_container/serialize.py` & `flytekit-1.9.1/flytekit/clis/sdk_in_container/serialize.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 @system_entry_point
 def serialize_all(
     pkgs: typing.List[str] = None,
     local_source_root: typing.Optional[str] = None,
     folder: typing.Optional[str] = None,
     mode: typing.Optional[SerializationMode] = None,
-    image: typing.Optional[str] = None,
+    image_config: typing.Optional[ImageConfig] = None,
     flytekit_virtualenv_root: typing.Optional[str] = None,
     python_interpreter: typing.Optional[str] = None,
     config_file: typing.Optional[str] = None,
 ):
     """
     This function will write to the folder specified the following protobuf types ::
         flyteidl.admin.launch_plan_pb2.LaunchPlan
@@ -45,40 +45,48 @@
 
     See :py:class:`flytekit.models.core.identifier.ResourceType` to match the trailing index in the file name with the
     entity type.
     :param pkgs: Dot-delimited Python packages/subpackages to look into for serialization.
     :param local_source_root: Where to start looking for the code.
     :param folder: Where to write the output protobuf files
     :param mode: Regular vs fast
-    :param image: The fully qualified and versioned default image to use
+    :param image_config: ImageConfig object to use
     :param flytekit_virtualenv_root: The full path of the virtual env in the container.
     """
 
     if not (mode == SerializationMode.DEFAULT or mode == SerializationMode.FAST):
         raise AssertionError(f"Unrecognized serialization mode: {mode}")
 
     serialization_settings = SerializationSettings(
-        image_config=ImageConfig.auto(config_file, img_name=image),
+        image_config=image_config or ImageConfig.auto(config_file),
         fast_serialization_settings=FastSerializationSettings(
             enabled=mode == SerializationMode.FAST,
             # TODO: if we want to move the destination dir as a serialization argument, we should initialize it here
         ),
         flytekit_virtualenv_root=flytekit_virtualenv_root,
         python_interpreter=python_interpreter,
     )
 
     serialize_to_folder(pkgs, serialization_settings, local_source_root, folder)
 
 
 @click.group("serialize", cls=click.RichGroup)
 @click.option(
+    "-i",
     "--image",
+    "image_config",
     required=False,
-    default=lambda: os.environ.get("FLYTE_INTERNAL_IMAGE", ""),
-    help="Text tag, for example ``somedocker.com/myimage:someversion123``",
+    multiple=True,
+    type=click.UNPROCESSED,
+    callback=ImageConfig.validate_image,
+    help="A fully qualified tag for an docker image, for example ``somedocker.com/myimage:someversion123``. This is a "
+    "multi-option and can be of the form ``--image xyz.io/docker:latest"
+    " --image my_image=xyz.io/docker2:latest``. Note, the ``name=image_uri``. The name is optional, if not "
+    "provided the image will be used as the default image. All the names have to be unique, and thus "
+    "there can only be one ``--image`` option with no name.",
 )
 @click.option(
     "--local-source-root",
     required=False,
     default=lambda: os.getcwd(),
     help="Root dir for Python code containing workflow definitions to operate on when not the current working directory. "
     "Optional when running ``pyflyte serialize`` in out-of-container-mode and your code lies outside of your working directory.",
@@ -95,25 +103,27 @@
     required=False,
     help="DEPRECATED: This flag is ignored! This is the root of the flytekit virtual env in your container. "
     "The reason it needs to be a separate option is because this pyflyte utility cannot know where flytekit is "
     "installed inside your container. Required for running `pyflyte serialize` in out of container mode when "
     "your container installs the flytekit virtualenv outside of the default `/opt/venv`",
 )
 @click.pass_context
-def serialize(ctx, image, local_source_root, in_container_config_path, in_container_virtualenv_root):
+def serialize(
+    ctx, image_config: ImageConfig, local_source_root, in_container_config_path, in_container_virtualenv_root
+):
     """
     This command produces protobufs for tasks and templates.
     For tasks, one pb file is produced for each task, representing one TaskTemplate object.
     For workflows, one pb file is produced for each workflow, representing a WorkflowClosure object. The closure
     object contains the WorkflowTemplate, along with the relevant tasks for that workflow. In lieu of Admin,
     this serialization step will set the URN of the tasks to the fully qualified name of the task function.
     """
-    ctx.obj[CTX_IMAGE] = image
+    ctx.obj[CTX_IMAGE] = image_config
     ctx.obj[CTX_LOCAL_SRC_ROOT] = local_source_root
-    click.echo("Serializing Flyte elements with image {}".format(image))
+    click.echo(f"Serializing Flyte elements with image {image_config}")
 
     if in_container_virtualenv_root:
         ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT] = in_container_virtualenv_root
         ctx.obj[CTX_PYTHON_INTERPRETER] = os.path.join(in_container_virtualenv_root, "/bin/python3")
     else:
         # For in container serialize we make sure to never accept an override the entrypoint path and determine it here
         # instead.
@@ -137,15 +147,15 @@
     pkgs = ctx.obj[CTX_PACKAGES]
     dir = ctx.obj[CTX_LOCAL_SRC_ROOT]
     serialize_all(
         pkgs,
         dir,
         folder,
         SerializationMode.DEFAULT,
-        image=ctx.obj[CTX_IMAGE],
+        image_config=ctx.obj[CTX_IMAGE],
         flytekit_virtualenv_root=ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT],
         python_interpreter=ctx.obj[CTX_PYTHON_INTERPRETER],
         config_file=ctx.obj.get(constants.CTX_CONFIG_FILE, None),
     )
 
 
 @click.group("fast", cls=click.RichGroup)
@@ -176,15 +186,15 @@
     pkgs = ctx.obj[CTX_PACKAGES]
     dir = ctx.obj[CTX_LOCAL_SRC_ROOT]
     serialize_all(
         pkgs,
         dir,
         folder,
         SerializationMode.FAST,
-        image=ctx.obj[CTX_IMAGE],
+        image_config=ctx.obj[CTX_IMAGE],
         flytekit_virtualenv_root=ctx.obj[CTX_FLYTEKIT_VIRTUALENV_ROOT],
         python_interpreter=ctx.obj[CTX_PYTHON_INTERPRETER],
         config_file=ctx.obj.get(constants.CTX_CONFIG_FILE, None),
     )
 
 
 fast.add_command(fast_workflows)
```

### Comparing `flytekit-1.9.0a0/flytekit/configuration/__init__.py` & `flytekit-1.9.1/flytekit/configuration/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,15 +140,15 @@
 import tempfile
 import typing
 from dataclasses import dataclass, field
 from io import BytesIO
 from typing import Dict, List, Optional
 
 import yaml
-from dataclasses_json import dataclass_json
+from dataclasses_json import DataClassJsonMixin
 
 from flytekit.configuration import internal as _internal
 from flytekit.configuration.default_images import DefaultImages
 from flytekit.configuration.file import ConfigEntry, ConfigFile, get_config_file, read_file_if_exists, set_if_exists
 from flytekit.image_spec import ImageSpec
 from flytekit.image_spec.image_spec import ImageBuildEngine
 from flytekit.loggers import logger
@@ -160,17 +160,16 @@
 DEFAULT_FLYTEKIT_ENTRYPOINT_FILELOC = "bin/entrypoint.py"
 DEFAULT_IMAGE_NAME = "default"
 DEFAULT_IN_CONTAINER_SRC_PATH = "/root"
 _IMAGE_FQN_TAG_REGEX = re.compile(r"([^:]+)(?=:.+)?")
 SERIALIZED_CONTEXT_ENV_VAR = "_F_SS_C"
 
 
-@dataclass_json
 @dataclass(init=True, repr=True, eq=True, frozen=True)
-class Image(object):
+class Image(DataClassJsonMixin):
     """
     Image is a structured wrapper for task container images used in object serialization.
 
     Attributes:
         name (str): A user-provided name to identify this image.
         fqn (str): Fully qualified image name. This consists of
             #. a registry location
@@ -193,18 +192,19 @@
 
     @staticmethod
     def look_up_image_info(name: str, tag: str, optional_tag: bool = False) -> Image:
         """
         Looks up the image tag from environment variable (should be set from the Dockerfile).
             FLYTE_INTERNAL_IMAGE should be the environment variable.
 
-        This function is used when registering tasks/workflows with Admin.
-        When using the canonical Python-based development cycle, the version that is used to register workflows
-        and tasks with Admin should be the version of the image itself, which should ideally be something unique
-        like the sha of the latest commit.
+        This function is used when registering tasks/workflows with Admin. When using
+        the canonical Python-based development cycle, the version that is used to
+        register workflows and tasks with Admin should be the version of the image
+        itself, which should ideally be something unique like the git revision SHA1 of
+        the latest commit.
 
         :param optional_tag:
         :param name:
         :param Text tag: e.g. somedocker.com/myimage:someversion123
         :rtype: Text
         """
         from docker_image import reference
@@ -219,23 +219,25 @@
         ref = reference.Reference.parse(tag)
         if not optional_tag and ref["tag"] is None:
             raise AssertionError(f"Incorrectly formatted image {tag}, missing tag value")
         else:
             return Image(name=name, fqn=ref["name"], tag=ref["tag"])
 
 
-@dataclass_json
 @dataclass(init=True, repr=True, eq=True, frozen=True)
-class ImageConfig(object):
+class ImageConfig(DataClassJsonMixin):
     """
+    We recommend you to use ImageConfig.auto(img_name=None) to create an ImageConfig.
+    For example, ImageConfig.auto(img_name=""ghcr.io/flyteorg/flytecookbook:v1.0.0"") will create an ImageConfig.
+
     ImageConfig holds available images which can be used at registration time. A default image can be specified
     along with optional additional images. Each image in the config must have a unique name.
 
     Attributes:
-        default_image (str): The default image to be used as a container for task serialization.
+        default_image (Optional[Image]): The default image to be used as a container for task serialization.
         images (List[Image]): Optional, additional images which can be used in task container definitions.
     """
 
     default_image: Optional[Image] = None
     images: Optional[List[Image]] = None
 
     def find_image(self, name) -> Optional[Image]:
@@ -278,14 +280,17 @@
                     f"Only one default image can be specified. Received multiple {default_image} & {img} for {param}"
                 )
             if img.name == DEFAULT_IMAGE_NAME:
                 default_image = img
             else:
                 images.append(img)
 
+        if default_image is None:
+            default_image_str = os.environ.get("FLYTE_INTERNAL_IMAGE", DefaultImages.default_image())
+            default_image = Image.look_up_image_info(DEFAULT_IMAGE_NAME, default_image_str, False)
         return ImageConfig.create_from(default_image=default_image, other_images=images)
 
     @classmethod
     def create_from(
         cls, default_image: Optional[Image], other_images: typing.Optional[typing.List[Image]] = None
     ) -> ImageConfig:
         if default_image and not isinstance(default_image, Image):
@@ -424,14 +429,15 @@
             "client_credentials_secret",
             client_credentials_secret,
         )
         kwargs = set_if_exists(kwargs, "scopes", _internal.Credentials.SCOPES.read(config_file))
         kwargs = set_if_exists(kwargs, "auth_mode", _internal.Credentials.AUTH_MODE.read(config_file))
         kwargs = set_if_exists(kwargs, "endpoint", _internal.Platform.URL.read(config_file))
         kwargs = set_if_exists(kwargs, "console_endpoint", _internal.Platform.CONSOLE_ENDPOINT.read(config_file))
+
         kwargs = set_if_exists(kwargs, "http_proxy_url", _internal.Platform.HTTP_PROXY_URL.read(config_file))
         return PlatformConfig(**kwargs)
 
     @classmethod
     def for_endpoint(cls, endpoint: str, insecure: bool = False) -> PlatformConfig:
         return PlatformConfig(endpoint=endpoint, insecure=insecure)
 
@@ -659,44 +665,41 @@
         :param config_file: -> Optional config file in the flytekit config format.
         :return: Config
         """
         c = cls.auto(config_file)
         return c.with_params(platform=PlatformConfig.for_endpoint(endpoint, insecure), data_config=data_config)
 
 
-@dataclass_json
 @dataclass
-class EntrypointSettings(object):
+class EntrypointSettings(DataClassJsonMixin):
     """
     This object carries information about the path of the entrypoint command that will be invoked at runtime.
     This is where `pyflyte-execute` code can be found. This is useful for cases like pyspark execution.
     """
 
     path: Optional[str] = None
 
 
-@dataclass_json
 @dataclass
-class FastSerializationSettings(object):
+class FastSerializationSettings(DataClassJsonMixin):
     """
     This object hold information about settings necessary to serialize an object so that it can be fast-registered.
     """
 
     enabled: bool = False
     # This is the location that the code should be copied into.
     destination_dir: Optional[str] = None
 
     # This is the zip file where the new code was uploaded to.
     distribution_location: Optional[str] = None
 
 
 # TODO: ImageConfig, python_interpreter, venv_root, fast_serialization_settings.destination_dir should be combined.
-@dataclass_json
-@dataclass()
-class SerializationSettings(object):
+@dataclass
+class SerializationSettings(DataClassJsonMixin):
     """
     These settings are provided while serializing a workflow and task, before registration. This is required to get
     runtime information at serialization time, as well as some defaults.
 
     Attributes:
         project (str): The project (if any) with which to register entities under.
         domain (str): The domain (if any) with which to register entities under.
```

### Comparing `flytekit-1.9.0a0/flytekit/configuration/default_images.py` & `flytekit-1.9.1/flytekit/configuration/default_images.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/configuration/feature_flags.py` & `flytekit-1.9.1/flytekit/configuration/feature_flags.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/configuration/file.py` & `flytekit-1.9.1/flytekit/configuration/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,18 @@
 import yaml
 
 from flytekit.exceptions import user as _user_exceptions
 from flytekit.loggers import logger
 
 # This is the env var that the flytectl sandbox instructions say to set
 FLYTECTL_CONFIG_ENV_VAR = "FLYTECTL_CONFIG"
+# This is an explicit override only to be used by pyflyte and takes precedence in get_config_file over the main
+# environment variable.
+# This env var should not be set by users
+FLYTECTL_CONFIG_ENV_VAR_OVERRIDE = "_FLYTECTL_CONFIG_PYFLYTE_OVERRIDE"
 
 
 def _exists(val: typing.Any) -> bool:
     """Check if a value is defined."""
     return isinstance(val, bool) or bool(val is not None and val)
 
 
@@ -33,15 +37,15 @@
         type_: Expected type of the value
     """
 
     section: str
     option: str
     type_: typing.Type = str
 
-    def get_env_name(self):
+    def get_env_name(self) -> str:
         return f"FLYTE_{self.section.upper()}_{self.option.upper()}"
 
     def read_from_env(self, transform: typing.Optional[typing.Callable] = None) -> typing.Optional[typing.Any]:
         """
         Reads the config entry from environment variable, the structure of the env var is current
         ``FLYTE_{SECTION}_{OPTION}`` all upper cased. We will change this in the future.
         :return:
@@ -89,15 +93,15 @@
                 return transform(v) if transform else v
         except Exception:
             ...
 
         return None
 
 
-def bool_transformer(config_val: typing.Any):
+def bool_transformer(config_val: typing.Any) -> bool:
     if type(config_val) is str:
         return True if config_val and not config_val.lower() in ["false", "0", "off", "no"] else False
     else:
         return config_val
 
 
 def comma_list_transformer(config_val: typing.Any):
@@ -235,33 +239,39 @@
 
 
 def get_config_file(c: typing.Union[str, ConfigFile, None]) -> typing.Optional[ConfigFile]:
     """
     Checks if the given argument is a file or a configFile and returns a loaded configFile else returns None
     """
     if c is None:
+        # Pyflyte override env var takes highest precedence
+        # Env var takes second highest precedence
+        flytectl_path_from_env = getenv(FLYTECTL_CONFIG_ENV_VAR_OVERRIDE, getenv(FLYTECTL_CONFIG_ENV_VAR, None))
+        if flytectl_path_from_env:
+            flytectl_path = Path(flytectl_path_from_env)
+            if flytectl_path.exists():
+                logger.info(f"Using flytectl/YAML config {flytectl_path.absolute()}")
+                return ConfigFile(str(flytectl_path.absolute()))
+            else:
+                logger.warning(f"flytectl config file {flytectl_path.absolute()} does not exist, ignoring...")
+
         # See if there's a config file in the current directory where Python is being run from
         current_location_config = Path("flytekit.config")
         if current_location_config.exists():
             logger.info(f"Using configuration from Python process root {current_location_config.absolute()}")
             return ConfigFile(str(current_location_config.absolute()))
 
         # If not, see if there's a config in the user's home directory
         home_dir_config = Path(Path.home(), ".flyte", "config")  # _default_config_file_name in main.py
         if home_dir_config.exists():
             logger.info(f"Using configuration from home directory {home_dir_config.absolute()}")
             return ConfigFile(str(home_dir_config.absolute()))
 
-        # If not, see if the env var that flytectl sandbox tells the user to set is set,
-        # or see if there's something in the default home directory location
+        # If not see if there's something in the default home directory location
         flytectl_path = Path(Path.home(), ".flyte", "config.yaml")
-        flytectl_path_from_env = getenv(FLYTECTL_CONFIG_ENV_VAR, None)
-
-        if flytectl_path_from_env:
-            flytectl_path = Path(flytectl_path_from_env)
         if flytectl_path.exists():
             logger.info(f"Using flytectl/YAML config {flytectl_path.absolute()}")
             return ConfigFile(str(flytectl_path.absolute()))
 
         # If not, then return None and let caller handle
         return None
     if isinstance(c, str):
```

### Comparing `flytekit-1.9.0a0/flytekit/configuration/internal.py` & `flytekit-1.9.1/flytekit/configuration/internal.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/annotation.py` & `flytekit-1.9.1/flytekit/core/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/base_sql_task.py` & `flytekit-1.9.1/flytekit/core/base_sql_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/base_task.py` & `flytekit-1.9.1/flytekit/core/base_task.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,19 +13,21 @@
    Task
    TaskMetadata
    TaskResolverMixin
    IgnoreOutputs
 
 """
 
+import asyncio
 import collections
 import datetime
+import inspect
 from abc import abstractmethod
 from dataclasses import dataclass
-from typing import Any, Dict, Generic, List, Optional, OrderedDict, Tuple, Type, TypeVar, Union, cast
+from typing import Any, Coroutine, Dict, Generic, List, Optional, OrderedDict, Tuple, Type, TypeVar, Union, cast
 
 from flytekit.configuration import SerializationSettings
 from flytekit.core.context_manager import (
     ExecutionParameters,
     ExecutionState,
     FlyteContext,
     FlyteContextManager,
@@ -229,15 +231,17 @@
         """
         Returns python native types for inputs. In case this is not a python native task (base class) and hence
         returns a None. we could deduce the type from literal types, but that is not a required exercise
         # TODO we could use literal type to determine this
         """
         return None
 
-    def local_execute(self, ctx: FlyteContext, **kwargs) -> Union[Tuple[Promise], Promise, VoidPromise, None]:
+    def local_execute(
+        self, ctx: FlyteContext, **kwargs
+    ) -> Union[Tuple[Promise], Promise, VoidPromise, Coroutine, None]:
         """
         This function is used only in the local execution path and is responsible for calling dispatch execute.
         Use this function when calling a task with native values (or Promises containing Flyte literals derived from
         Python native values).
         """
         # Unwrap the kwargs values. After this, we essentially have a LiteralMap
         # The reason why we need to do this is because the inputs during local execute can be of 2 types
@@ -279,14 +283,18 @@
             else:
                 logger.info("Cache hit")
         else:
             # This code should mirror the call to `sandbox_execute` in the above cache case.
             # Code is simpler with duplication and less metaprogramming, but introduces regressions
             # if one is changed and not the other.
             outputs_literal_map = self.sandbox_execute(ctx, input_literal_map)
+
+        if inspect.iscoroutine(outputs_literal_map):
+            return outputs_literal_map
+
         outputs_literals = outputs_literal_map.literals
 
         # TODO maybe this is the part that should be done for local execution, we pass the outputs to some special
         #    location, otherwise we dont really need to right? The higher level execute could just handle literalMap
         # After running, we again have to wrap the outputs, if any, back into Promise objects
         output_names = list(self.interface.outputs.keys())  # type: ignore
         if len(output_names) != len(outputs_literals):
@@ -296,15 +304,15 @@
         # Tasks that don't return anything still return a VoidPromise
         if len(output_names) == 0:
             return VoidPromise(self.name)
 
         vals = [Promise(var, outputs_literals[var]) for var in output_names]
         return create_task_output(vals, self.python_interface)
 
-    def __call__(self, *args, **kwargs) -> Union[Tuple[Promise], Promise, VoidPromise, Tuple, None]:
+    def __call__(self, *args: object, **kwargs: object) -> Union[Tuple[Promise], Promise, VoidPromise, Tuple, None]:
         return flyte_entity_call_handler(self, *args, **kwargs)  # type: ignore
 
     def compile(self, ctx: FlyteContext, *args, **kwargs):
         raise Exception("not implemented")
 
     def get_container(self, settings: SerializationSettings) -> Optional[_task_model.Container]:
         """
@@ -333,14 +341,18 @@
     def get_config(self, settings: SerializationSettings) -> Optional[Dict[str, str]]:
         """
         Returns the task config as a serializable dictionary. This task config consists of metadata about the custom
         defined for this task.
         """
         return None
 
+    def local_execution_mode(self) -> ExecutionState.Mode:
+        """ """
+        return ExecutionState.Mode.LOCAL_TASK_EXECUTION
+
     def sandbox_execute(
         self,
         ctx: FlyteContext,
         input_literal_map: _literal_models.LiteralMap,
     ) -> _literal_models.LiteralMap:
         """
         Call dispatch_execute, in the context of a local sandbox execution. Not invoked during runtime.
@@ -480,40 +492,101 @@
         return _workflow_model.NodeMetadata(
             name=extract_obj_name(self.name),
             timeout=self.metadata.timeout,
             retries=self.metadata.retry_strategy,
             interruptible=self.metadata.interruptible,
         )
 
-    def compile(self, ctx: FlyteContext, *args, **kwargs):
+    def compile(self, ctx: FlyteContext, *args, **kwargs) -> Optional[Union[Tuple[Promise], Promise, VoidPromise]]:
         """
         Generates a node that encapsulates this task in a workflow definition.
         """
         return create_and_link_node(ctx, entity=self, **kwargs)
 
     @property
     def _outputs_interface(self) -> Dict[Any, Variable]:
         return self.interface.outputs  # type: ignore
 
+    def _output_to_literal_map(self, native_outputs, exec_ctx):
+        expected_output_names = list(self._outputs_interface.keys())
+        if len(expected_output_names) == 1:
+            # Here we have to handle the fact that the task could've been declared with a typing.NamedTuple of
+            # length one. That convention is used for naming outputs - and single-length-NamedTuples are
+            # particularly troublesome but elegant handling of them is not a high priority
+            # Again, we're using the output_tuple_name as a proxy.
+            if self.python_interface.output_tuple_name and isinstance(native_outputs, tuple):
+                native_outputs_as_map = {expected_output_names[0]: native_outputs[0]}
+            else:
+                native_outputs_as_map = {expected_output_names[0]: native_outputs}
+        elif len(expected_output_names) == 0:
+            native_outputs_as_map = {}
+        else:
+            native_outputs_as_map = {expected_output_names[i]: native_outputs[i] for i, _ in enumerate(native_outputs)}
+
+        # We manually construct a LiteralMap here because task inputs and outputs actually violate the assumption
+        # built into the IDL that all the values of a literal map are of the same type.
+        with timeit("Translate the output to literals"):
+            literals = {}
+            for i, (k, v) in enumerate(native_outputs_as_map.items()):
+                literal_type = self._outputs_interface[k].type
+                py_type = self.get_type_for_output_var(k, v)
+
+                if isinstance(v, tuple):
+                    raise TypeError(f"Output({k}) in task '{self.name}' received a tuple {v}, instead of {py_type}")
+                try:
+                    literals[k] = TypeEngine.to_literal(exec_ctx, v, py_type, literal_type)
+                except Exception as e:
+                    # only show the name of output key if it's user-defined (by default Flyte names these as "o<n>")
+                    key = k if k != f"o{i}" else i
+                    msg = f"Failed to convert outputs of task '{self.name}' at position {key}:\n  {e}"
+                    logger.error(msg)
+                    raise TypeError(msg) from e
+
+        return _literal_models.LiteralMap(literals=literals), native_outputs_as_map
+
+    def _write_decks(self, native_inputs, native_outputs_as_map, ctx, new_user_params):
+        if self._disable_deck is False:
+            from flytekit.deck.deck import Deck, _output_deck
+
+            INPUT = "input"
+            OUTPUT = "output"
+
+            input_deck = Deck(INPUT)
+            for k, v in native_inputs.items():
+                input_deck.append(TypeEngine.to_html(ctx, v, self.get_type_for_input_var(k, v)))
+
+            output_deck = Deck(OUTPUT)
+            for k, v in native_outputs_as_map.items():
+                output_deck.append(TypeEngine.to_html(ctx, v, self.get_type_for_output_var(k, v)))
+
+            if ctx.execution_state and ctx.execution_state.is_local_execution():
+                # When we run the workflow remotely, flytekit outputs decks at the end of _dispatch_execute
+                _output_deck(self.name.split(".")[-1], new_user_params)
+
+    async def _async_execute(self, native_inputs, native_outputs, ctx, exec_ctx, new_user_params):
+        native_outputs = await native_outputs
+        native_outputs = self.post_execute(new_user_params, native_outputs)
+        literals_map, native_outputs_as_map = self._output_to_literal_map(native_outputs, exec_ctx)
+        self._write_decks(native_inputs, native_outputs_as_map, ctx, new_user_params)
+        return literals_map
+
     def dispatch_execute(
         self, ctx: FlyteContext, input_literal_map: _literal_models.LiteralMap
-    ) -> Union[_literal_models.LiteralMap, _dynamic_job.DynamicJobSpec]:
+    ) -> Union[_literal_models.LiteralMap, _dynamic_job.DynamicJobSpec, Coroutine]:
         """
         This method translates Flyte's Type system based input values and invokes the actual call to the executor
         This method is also invoked during runtime.
 
         * ``VoidPromise`` is returned in the case when the task itself declares no outputs.
         * ``Literal Map`` is returned when the task returns either one more outputs in the declaration. Individual outputs
           may be none
         * ``DynamicJobSpec`` is returned when a dynamic workflow is executed
         """
-
         # Invoked before the task is executed
         new_user_params = self.pre_execute(ctx.user_space_params)
-        from flytekit.deck.deck import _output_deck
 
         # Create another execution context with the new user params, but let's keep the same working dir
         with FlyteContextManager.with_context(
             ctx.with_execution_state(
                 cast(ExecutionState, ctx.execution_state).with_params(user_space_params=new_user_params)
             )
             # type: ignore
@@ -535,82 +608,46 @@
             try:
                 with timeit("Execute user level code"):
                     native_outputs = self.execute(**native_inputs)
             except Exception as e:
                 logger.exception(f"Exception when executing {e}")
                 raise e
 
+            if inspect.iscoroutine(native_outputs):
+                # If native outputs is a coroutine, then this is an eager workflow.
+                if exec_ctx.execution_state:
+                    if exec_ctx.execution_state.mode == ExecutionState.Mode.LOCAL_TASK_EXECUTION:
+                        # Just return task outputs as a coroutine if the eager workflow is being executed locally,
+                        # outside of a workflow. This preserves the expectation that the eager workflow is an async
+                        # function.
+                        return native_outputs
+                    elif exec_ctx.execution_state.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION:
+                        # If executed inside of a workflow being executed locally, then run the coroutine to get the
+                        # actual results.
+                        return asyncio.run(
+                            self._async_execute(native_inputs, native_outputs, ctx, exec_ctx, new_user_params)
+                        )
+
+                return self._async_execute(native_inputs, native_outputs, ctx, exec_ctx, new_user_params)
+
             logger.debug("Task executed successfully in user level")
             # Lets run the post_execute method. This may result in a IgnoreOutputs Exception, which is
             # bubbled up to be handled at the callee layer.
             native_outputs = self.post_execute(new_user_params, native_outputs)
 
             # Short circuit the translation to literal map because what's returned may be a dj spec (or an
             # already-constructed LiteralMap if the dynamic task was a no-op), not python native values
             # dynamic_execute returns a literal map in local execute so this also gets triggered.
-            if isinstance(native_outputs, _literal_models.LiteralMap) or isinstance(
-                native_outputs, _dynamic_job.DynamicJobSpec
-            ):
+            if isinstance(native_outputs, (_literal_models.LiteralMap, _dynamic_job.DynamicJobSpec)):
                 return native_outputs
 
-            expected_output_names = list(self._outputs_interface.keys())
-            if len(expected_output_names) == 1:
-                # Here we have to handle the fact that the task could've been declared with a typing.NamedTuple of
-                # length one. That convention is used for naming outputs - and single-length-NamedTuples are
-                # particularly troublesome but elegant handling of them is not a high priority
-                # Again, we're using the output_tuple_name as a proxy.
-                if self.python_interface.output_tuple_name and isinstance(native_outputs, tuple):
-                    native_outputs_as_map = {expected_output_names[0]: native_outputs[0]}
-                else:
-                    native_outputs_as_map = {expected_output_names[0]: native_outputs}
-            elif len(expected_output_names) == 0:
-                native_outputs_as_map = {}
-            else:
-                native_outputs_as_map = {
-                    expected_output_names[i]: native_outputs[i] for i, _ in enumerate(native_outputs)
-                }
-
-            # We manually construct a LiteralMap here because task inputs and outputs actually violate the assumption
-            # built into the IDL that all the values of a literal map are of the same type.
-            with timeit("Translate the output to literals"):
-                literals = {}
-                for i, (k, v) in enumerate(native_outputs_as_map.items()):
-                    literal_type = self._outputs_interface[k].type
-                    py_type = self.get_type_for_output_var(k, v)
-
-                    if isinstance(v, tuple):
-                        raise TypeError(f"Output({k}) in task '{self.name}' received a tuple {v}, instead of {py_type}")
-                    try:
-                        literals[k] = TypeEngine.to_literal(exec_ctx, v, py_type, literal_type)
-                    except Exception as e:
-                        # only show the name of output key if it's user-defined (by default Flyte names these as "o<n>")
-                        key = k if k != f"o{i}" else i
-                        msg = f"Failed to convert outputs of task '{self.name}' at position {key}:\n  {e}"
-                        logger.error(msg)
-                        raise TypeError(msg) from e
-
-            if self._disable_deck is False:
-                from flytekit.deck.deck import Deck
-
-                INPUT = "input"
-                OUTPUT = "output"
-
-                input_deck = Deck(INPUT)
-                for k, v in native_inputs.items():
-                    input_deck.append(TypeEngine.to_html(ctx, v, self.get_type_for_input_var(k, v)))
-
-                output_deck = Deck(OUTPUT)
-                for k, v in native_outputs_as_map.items():
-                    output_deck.append(TypeEngine.to_html(ctx, v, self.get_type_for_output_var(k, v)))
-
-                _output_deck(self.name.split(".")[-1], new_user_params)
-
-            outputs_literal_map = _literal_models.LiteralMap(literals=literals)
+            literals_map, native_outputs_as_map = self._output_to_literal_map(native_outputs, exec_ctx)
+            self._write_decks(native_inputs, native_outputs_as_map, ctx, new_user_params)
             # After the execute has been successfully completed
-            return outputs_literal_map
+            return literals_map
 
     def pre_execute(self, user_params: Optional[ExecutionParameters]) -> Optional[ExecutionParameters]:  # type: ignore
         """
         This is the method that will be invoked directly before executing the task method and before all the inputs
         are converted. One particular case where this is useful is if the context is to be modified for the user process
         to get some user space parameters. This also ensures that things like SparkSession are already correctly
         setup before the type transformers are called
```

### Comparing `flytekit-1.9.0a0/flytekit/core/checkpointer.py` & `flytekit-1.9.1/flytekit/core/checkpointer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/class_based_resolver.py` & `flytekit-1.9.1/flytekit/core/class_based_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/condition.py` & `flytekit-1.9.1/flytekit/core/condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import datetime
 import typing
 from typing import Optional, Tuple, Union, cast
 
-from flytekit.core.context_manager import ExecutionState, FlyteContextManager
+from flytekit.core.context_manager import FlyteContextManager
 from flytekit.core.node import Node
 from flytekit.core.promise import (
     ComparisonExpression,
     ComparisonOps,
     ConjunctionExpression,
     ConjunctionOps,
     NodeOutput,
@@ -267,14 +267,21 @@
                     "Flytekit only supports Comparison (<,<=,>,>=,==,!=) or Conjunction (&/|) "
                     f"expressions, Received var {expr} in condition {cs.name}.{stmt}"
                 )
         self._expr = expr
         self._output_promise: Optional[Union[Tuple[Promise], Promise]] = None
         self._err: Optional[str] = None
         self._stmt = stmt
+        self._output_node = None
+
+    @property
+    def output_node(self) -> Optional[Node]:
+        # This is supposed to hold a pointer to the node that created this case.
+        # It is set in the then() call. but the value will not be set if it's a VoidPromise or None was returned.
+        return self._output_node
 
     @property
     def expr(self) -> Optional[Union[ComparisonExpression, ConjunctionExpression]]:
         return self._expr
 
     @property
     def output_promise(self) -> Optional[Union[Tuple[Promise], Promise]]:
@@ -285,14 +292,29 @@
         return self._err
 
     # TODO this is complicated. We do not want this to run
     def then(
         self, p: Union[Promise, Tuple[Promise]]
     ) -> Optional[Union[Condition, Promise, Tuple[Promise], VoidPromise]]:
         self._output_promise = p
+        if isinstance(p, Promise):
+            if not p.is_ready:
+                self._output_node = p.ref.node  # type: ignore
+        elif isinstance(p, VoidPromise):
+            if p.ref is not None:
+                self._output_node = p.ref.node
+        elif hasattr(p, "_fields"):
+            # This condition detects the NamedTuple case and iterates through the fields to find one that has a node
+            # which should be the first one.
+            for f in p._fields:  # type: ignore
+                prom = getattr(p, f)
+                if not prom.is_ready:
+                    self._output_node = prom.ref.node
+                    break
+
         # We can always mark branch as completed
         return self._cs.end_branch()
 
     def fail(self, err: str) -> Promise:
         self._err = err
         return cast(Promise, self._cs.end_branch())
 
@@ -411,15 +433,16 @@
         return _core_cond.BooleanExpression(conjunction=cexpr), promises
     cexpr, promises = transform_to_comp_expr(expr)
     return _core_cond.BooleanExpression(comparison=cexpr), promises
 
 
 def to_case_block(c: Case) -> Tuple[Union[_core_wf.IfBlock], typing.List[Promise]]:
     expr, promises = transform_to_boolexpr(cast(Union[ComparisonExpression, ConjunctionExpression], c.expr))
-    n = c.output_promise.ref.node  # type: ignore
+    if c.output_promise is not None:
+        n = c.output_node
     return _core_wf.IfBlock(condition=expr, then_node=n), promises
 
 
 def to_ifelse_block(node_id: str, cs: ConditionalSection) -> Tuple[_core_wf.IfElseBlock, typing.List[Binding]]:
     if len(cs.cases) == 0:
         raise AssertionError("Illegal Condition block, with no if-else cases")
     if len(cs.cases) < 2:
@@ -434,15 +457,15 @@
             case, promises = to_case_block(c)
             all_promises.extend(promises)
             other_cases.append(case)
     last_case = cs.cases[-1]
     node = None
     err = None
     if last_case.output_promise is not None:
-        node = last_case.output_promise.ref.node  # type: ignore
+        node = last_case.output_node
     else:
         err = Error(failed_node_id=node_id, message=last_case.err if last_case.err else "Condition failed")
     return (
         _core_wf.IfElseBlock(case=first_case, other=other_cases, else_node=node, error=err),
         merge_promises(*all_promises),
     )
 
@@ -484,15 +507,15 @@
         )
     """
     ctx = FlyteContextManager.current_context()
 
     if ctx.compilation_state:
         return ConditionalSection(name)
     elif ctx.execution_state:
-        if ctx.execution_state.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION:
+        if ctx.execution_state.is_local_execution():
             # In case of Local workflow execution, we will actually evaluate the expression and based on the result
             # make the branch to be active using `take_branch` method
             from flytekit.core.context_manager import BranchEvalMode
 
             if ctx.execution_state.branch_eval_mode == BranchEvalMode.BRANCH_SKIPPED:
                 return SkippedConditionalSection(name)
             return LocalExecutedConditionalSection(name)
```

### Comparing `flytekit-1.9.0a0/flytekit/core/constants.py` & `flytekit-1.9.1/flytekit/core/constants.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 INPUT_FILE_NAME = "inputs.pb"
 OUTPUT_FILE_NAME = "outputs.pb"
 FUTURES_FILE_NAME = "futures.pb"
 ERROR_FILE_NAME = "error.pb"
+REQUIREMENTS_FILE_NAME = "requirements.txt"
 
 
 class SdkTaskType(object):
     PYTHON_TASK = "python-task"
     DYNAMIC_TASK = "dynamic-task"
     CONTAINER_ARRAY_TASK = "container_array"
+    EXPERIMENTAL_ARRAY_NODE_TASK = "array_node"
     SPARK_TASK = "spark"
 
     # Hive is multi-step operation:
     #    1. a generator task that generates hive-job to be executed by the operator. Generator task is called hive task
     #       for backward compatibility (Note: it is a "batch-task" with a different name)
     #    2. hive-job is the actual set of queries to be executed. This is called hive_job
     BATCH_HIVE_TASK = "batch_hive"
```

### Comparing `flytekit-1.9.0a0/flytekit/core/container_task.py` & `flytekit-1.9.1/flytekit/core/container_task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 from typing import Any, Dict, List, Optional, Tuple, Type
 
 from flytekit.configuration import SerializationSettings
 from flytekit.core.base_task import PythonTask, TaskMetadata
+from flytekit.core.context_manager import FlyteContext
 from flytekit.core.interface import Interface
 from flytekit.core.pod_template import PodTemplate
 from flytekit.core.resources import Resources, ResourceSpec
 from flytekit.core.utils import _get_container_definition, _serialize_pod_spec
 from flytekit.models import task as _task_model
 from flytekit.models.security import Secret, SecurityContext
 
@@ -85,24 +86,16 @@
         )
         self.pod_template = pod_template
 
     @property
     def resources(self) -> ResourceSpec:
         return self._resources
 
-    def execute(self, **kwargs) -> Any:
-        print(kwargs)
-        env = ""
-        for k, v in self.environment.items():
-            env += f" -e {k}={v}"
-        print(
-            f"\ndocker run --rm -v /tmp/inputs:{self._input_data_dir} -v /tmp/outputs:{self._output_data_dir} {env}"
-            f"{self._image} {self._cmd} {self._args}"
-        )
-        return None
+    def local_execute(self, ctx: FlyteContext, **kwargs) -> Any:
+        raise RuntimeError("ContainerTask is not supported in local executions.")
 
     def get_container(self, settings: SerializationSettings) -> _task_model.Container:
         # if pod_template is specified, return None here but in get_k8s_pod, return pod_template merged with container
         if self.pod_template is not None:
             return None
 
         return self._get_container(settings)
```

### Comparing `flytekit-1.9.0a0/flytekit/core/context_manager.py` & `flytekit-1.9.1/flytekit/core/context_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
         self,
         execution_date,
         tmp_dir,
         stats,
         execution_id: typing.Optional[_identifier.WorkflowExecutionIdentifier],
         logging,
         raw_output_prefix,
+        output_metadata_prefix=None,
         checkpoint=None,
         decks=None,
         task_id: typing.Optional[_identifier.Identifier] = None,
         **kwargs,
     ):
         """
         Args:
@@ -169,14 +170,15 @@
             decks = []
         self._stats = stats
         self._execution_date = execution_date
         self._working_directory = tmp_dir
         self._execution_id = execution_id
         self._logging = logging
         self._raw_output_prefix = raw_output_prefix
+        self._output_metadata_prefix = output_metadata_prefix
         # AutoDeletingTempDir's should be used with a with block, which creates upon entry
         self._attrs = kwargs
         # It is safe to recreate the Secrets Manager
         self._secrets_manager = SecretsManager()
         self._checkpoint = checkpoint
         self._decks = decks
         self._task_id = task_id
@@ -198,14 +200,18 @@
         return self._logging
 
     @property
     def raw_output_prefix(self) -> str:
         return self._raw_output_prefix
 
     @property
+    def output_metadata_prefix(self) -> str:
+        return self._output_metadata_prefix
+
+    @property
     def working_directory(self) -> str:
         """
         A handle to a special working directory for easily producing temporary files.
         TODO: Usage examples
         """
         return self._working_directory
 
@@ -272,15 +278,15 @@
 
         time_line_deck = None
         for deck in self.decks:
             if isinstance(deck, TimeLineDeck):
                 time_line_deck = deck
                 break
         if time_line_deck is None:
-            time_line_deck = TimeLineDeck("Timeline")
+            time_line_deck = TimeLineDeck("timeline")
 
         return time_line_deck
 
     def __getattr__(self, attr_name: str) -> typing.Any:
         """
         This houses certain task specific context. For example in Spark, it houses the SparkSession, etc
         """
@@ -339,26 +345,29 @@
 
     def __getattr__(self, item: str) -> _GroupSecrets:
         """
         returns a new _GroupSecrets objects, that allows all keys within this group to be looked up like attributes
         """
         return self._GroupSecrets(item, self)
 
-    def get(self, group: str, key: Optional[str] = None, group_version: Optional[str] = None) -> str:
+    def get(
+        self, group: str, key: Optional[str] = None, group_version: Optional[str] = None, encode_mode: str = "r"
+    ) -> str:
         """
         Retrieves a secret using the resolution order -> Env followed by file. If not found raises a ValueError
+        param encode_mode, defines the mode to open files, it can either be "r" to read file, or "rb" to read binary file
         """
         self.check_group_key(group)
         env_var = self.get_secrets_env_var(group, key, group_version)
         fpath = self.get_secrets_file(group, key, group_version)
         v = os.environ.get(env_var)
         if v is not None:
             return v
         if os.path.exists(fpath):
-            with open(fpath, "r") as f:
+            with open(fpath, encode_mode) as f:
                 return f.read().strip()
         raise ValueError(
             f"Unable to find secret for key {key} in group {group} " f"in Env Var:{env_var} and FilePath: {fpath}"
         )
 
     def get_secrets_env_var(self, group: str, key: Optional[str] = None, group_version: Optional[str] = None) -> str:
         """
@@ -531,14 +540,20 @@
             working_dir=working_dir if working_dir else self.working_dir,
             mode=mode if mode else self.mode,
             engine_dir=engine_dir if engine_dir else self.engine_dir,
             branch_eval_mode=branch_eval_mode if branch_eval_mode else self.branch_eval_mode,
             user_space_params=user_space_params if user_space_params else self.user_space_params,
         )
 
+    def is_local_execution(self):
+        return (
+            self.mode == ExecutionState.Mode.LOCAL_TASK_EXECUTION
+            or self.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION
+        )
+
 
 @dataclass(frozen=True)
 class FlyteContext(object):
     """
     This is an internal-facing context object, that most users will not have to deal with. It's essentially a globally
     available grab bag of settings and objects that allows flytekit to do things like convert complex types, run and
     compile workflows, serialize Flyte entities, etc.
@@ -680,15 +695,15 @@
             Used by the condition block to indicate that a new conditional section has been started.
             """
 
             if self.compilation_state:
                 self.compilation_state = self.compilation_state.with_params(prefix=self.compilation_state.prefix)
 
             if self.execution_state:
-                if self.execution_state.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION:
+                if self.execution_state.is_local_execution():
                     if self.in_a_condition:
                         if self.execution_state.branch_eval_mode == BranchEvalMode.BRANCH_SKIPPED:
                             self.execution_state = self.execution_state.with_params()
                     else:
                         # In case of local workflow execution we should ensure a conditional section
                         # is created so that skipped branches result in tasks not being executed
                         self.execution_state = self.execution_state.with_params(
```

### Comparing `flytekit-1.9.0a0/flytekit/core/data_persistence.py` & `flytekit-1.9.1/flytekit/core/data_persistence.py`

 * *Files 9% similar despite different names*

```diff
@@ -179,49 +179,49 @@
             logger.debug(f"Error in exists checking {path} {oe}")
             anon_fs = self.get_filesystem(get_protocol(path), anonymous=True)
             if anon_fs is not None:
                 logger.debug(f"Attempting anonymous exists with {anon_fs}")
                 return anon_fs.exists(path)
             raise oe
 
-    def get(self, from_path: str, to_path: str, recursive: bool = False):
+    def get(self, from_path: str, to_path: str, recursive: bool = False, **kwargs):
         file_system = self.get_filesystem_for_path(from_path)
         if recursive:
             from_path, to_path = self.recursive_paths(from_path, to_path)
         try:
             if os.name == "nt" and file_system.protocol == "file" and recursive:
                 import shutil
 
                 return shutil.copytree(
                     self.strip_file_header(from_path), self.strip_file_header(to_path), dirs_exist_ok=True
                 )
-            return file_system.get(from_path, to_path, recursive=recursive)
+            return file_system.get(from_path, to_path, recursive=recursive, **kwargs)
         except OSError as oe:
             logger.debug(f"Error in getting {from_path} to {to_path} rec {recursive} {oe}")
             file_system = self.get_filesystem(get_protocol(from_path), anonymous=True)
             if file_system is not None:
                 logger.debug(f"Attempting anonymous get with {file_system}")
-                return file_system.get(from_path, to_path, recursive=recursive)
+                return file_system.get(from_path, to_path, recursive=recursive, **kwargs)
             raise oe
 
-    def put(self, from_path: str, to_path: str, recursive: bool = False):
+    def put(self, from_path: str, to_path: str, recursive: bool = False, **kwargs):
         file_system = self.get_filesystem_for_path(to_path)
         from_path = self.strip_file_header(from_path)
         if recursive:
             # Only check this for the local filesystem
             if file_system.protocol == "file" and not file_system.isdir(from_path):
                 raise FlyteAssertion(f"Source path {from_path} is not a directory")
             if os.name == "nt" and file_system.protocol == "file":
                 import shutil
 
                 return shutil.copytree(
                     self.strip_file_header(from_path), self.strip_file_header(to_path), dirs_exist_ok=True
                 )
             from_path, to_path = self.recursive_paths(from_path, to_path)
-        return file_system.put(from_path, to_path, recursive=recursive)
+        return file_system.put(from_path, to_path, recursive=recursive, **kwargs)
 
     def get_random_remote_path(self, file_path_or_file_name: typing.Optional[str] = None) -> str:
         """
         Constructs a randomized path on the configured raw_output_prefix (persistence layer). the random bit is a UUID
         and allows for disambiguating paths within the same directory.
 
         Use file_path_or_file_name, when you want a random directory, but want to preserve the leaf file name
@@ -283,44 +283,43 @@
     def upload_directory(self, local_path: str, remote_path: str):
         """
         :param Text local_path:
         :param Text remote_path:
         """
         return self.put_data(local_path, remote_path, is_multipart=True)
 
-    @timeit("Download data to local from remote")
-    def get_data(self, remote_path: str, local_path: str, is_multipart: bool = False):
+    def get_data(self, remote_path: str, local_path: str, is_multipart: bool = False, **kwargs):
         """
         :param remote_path:
         :param local_path:
         :param is_multipart:
         """
         try:
             pathlib.Path(local_path).parent.mkdir(parents=True, exist_ok=True)
-            self.get(remote_path, to_path=local_path, recursive=is_multipart)
+            with timeit(f"Download data to local from {remote_path}"):
+                self.get(remote_path, to_path=local_path, recursive=is_multipart, **kwargs)
         except Exception as ex:
             raise FlyteAssertion(
                 f"Failed to get data from {remote_path} to {local_path} (recursive={is_multipart}).\n\n"
                 f"Original exception: {str(ex)}"
             )
 
-    @timeit("Upload data to remote")
-    def put_data(self, local_path: Union[str, os.PathLike], remote_path: str, is_multipart: bool = False):
+    def put_data(self, local_path: Union[str, os.PathLike], remote_path: str, is_multipart: bool = False, **kwargs):
         """
         The implication here is that we're always going to put data to the remote location, so we .remote to ensure
         we don't use the true local proxy if the remote path is a file://
 
         :param local_path:
         :param remote_path:
         :param is_multipart:
         """
         try:
             local_path = str(local_path)
-
-            self.put(cast(str, local_path), remote_path, recursive=is_multipart)
+            with timeit(f"Upload data to {remote_path}"):
+                self.put(cast(str, local_path), remote_path, recursive=is_multipart, **kwargs)
         except Exception as ex:
             raise FlyteAssertion(
                 f"Failed to put data from {local_path} to {remote_path} (recursive={is_multipart}).\n\n"
                 f"Original exception: {str(ex)}"
             ) from ex
```

### Comparing `flytekit-1.9.0a0/flytekit/core/docstring.py` & `flytekit-1.9.1/flytekit/core/docstring.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/dynamic_workflow_task.py` & `flytekit-1.9.1/flytekit/core/dynamic_workflow_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/gate.py` & `flytekit-1.9.1/flytekit/core/gate.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import datetime
 import typing
 from typing import Tuple, Union
 
 import click
 
 from flytekit.core import interface as flyte_interface
-from flytekit.core.context_manager import FlyteContext, FlyteContextManager
+from flytekit.core.context_manager import ExecutionState, FlyteContext, FlyteContextManager
 from flytekit.core.promise import Promise, VoidPromise, flyte_entity_call_handler
 from flytekit.core.type_engine import TypeEngine
 from flytekit.exceptions.user import FlyteDisapprovalException
 from flytekit.interaction.parse_stdin import parse_stdin_to_literal
 from flytekit.models.core import workflow as _workflow_model
 from flytekit.models.types import LiteralType
 
@@ -112,14 +112,17 @@
             # Only one element should be in this map. Rely on kwargs instead of the stored _upstream_item even though
             # they should be the same to be cleaner
             output_name = list(kwargs.keys())[0]
             return kwargs[output_name]
         else:
             raise FlyteDisapprovalException(f"User did not approve the transaction for gate node {self.name}")
 
+    def local_execution_mode(self):
+        return ExecutionState.Mode.LOCAL_TASK_EXECUTION
+
 
 def wait_for_input(name: str, timeout: datetime.timedelta, expected_type: typing.Type):
     """Create a Gate object that waits for user input of the specified type.
 
     Create a Gate object. This object will function like a task. Note that unlike a task,
     each time this function is called, a new Python object is created. If a workflow
     calls a subworkflow twice, and the subworkflow has a signal, then two Gate
```

### Comparing `flytekit-1.9.0a0/flytekit/core/interface.py` & `flytekit-1.9.1/flytekit/core/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 import collections
 import copy
 import inspect
 import typing
 from collections import OrderedDict
 from typing import Any, Dict, Generator, List, Optional, Tuple, Type, TypeVar, Union, cast
 
-from typing_extensions import Annotated, get_args, get_origin, get_type_hints
+from typing_extensions import get_args, get_origin, get_type_hints
 
 from flytekit.core import context_manager
 from flytekit.core.docstring import Docstring
 from flytekit.core.type_engine import TypeEngine
 from flytekit.exceptions.user import FlyteValidationException
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
 from flytekit.models.literals import Void
-from flytekit.types.pickle import FlytePickle
 
 T = typing.TypeVar("T")
 
 
 def repr_kv(k: str, v: Union[Type, Tuple[Type, Any]]) -> str:
     if isinstance(v, tuple):
         if v[1]:
@@ -246,18 +245,20 @@
         )
 
     inputs_map = transform_variable_map(interface.inputs, input_descriptions)
     outputs_map = transform_variable_map(interface.outputs, output_descriptions)
     return _interface_models.TypedInterface(inputs_map, outputs_map)
 
 
-def transform_types_to_list_of_type(m: Dict[str, type], bound_inputs: typing.Set[str]) -> Dict[str, type]:
+def transform_types_to_list_of_type(
+    m: Dict[str, type], bound_inputs: typing.Set[str], list_as_optional: bool = False
+) -> Dict[str, type]:
     """
-    Converts a given variables to be collections of their type. This is useful for array jobs / map style code.
-    It will create a collection of types even if any one these types is not a collection type
+    Converts unbound inputs into the equivalent (optional) collections. This is useful for array jobs / map style code.
+    It will create a collection of types even if any one these types is not a collection type.
     """
     if m is None:
         return {}
 
     all_types_are_collection = True
     for k, v in m.items():
         if k in bound_inputs:
@@ -273,77 +274,54 @@
         return m
 
     om = {}
     for k, v in m.items():
         if k in bound_inputs:
             om[k] = v
         else:
-            om[k] = typing.List[v]  # type: ignore
+            om[k] = typing.List[typing.Optional[v] if list_as_optional else v]  # type: ignore
     return om  # type: ignore
 
 
-def transform_interface_to_list_interface(interface: Interface, bound_inputs: typing.Set[str]) -> Interface:
+def transform_interface_to_list_interface(
+    interface: Interface, bound_inputs: typing.Set[str], optional_outputs: bool = False
+) -> Interface:
     """
     Takes a single task interface and interpolates it to an array interface - to allow performing distributed python map
     like functions
-    :param interface: Interface to be upgraded toa list interface
+    :param interface: Interface to be upgraded to a list interface
     :param bound_inputs: fixed inputs that should not upgraded to a list and will be maintained as scalars.
     """
     map_inputs = transform_types_to_list_of_type(interface.inputs, bound_inputs)
-    map_outputs = transform_types_to_list_of_type(interface.outputs, set())
+    map_outputs = transform_types_to_list_of_type(interface.outputs, set(), optional_outputs)
 
     return Interface(inputs=map_inputs, outputs=map_outputs)
 
 
-def _change_unrecognized_type_to_pickle(t: Type[T]) -> typing.Union[Tuple[Type[T]], Type[T]]:
-    try:
-        if hasattr(t, "__origin__") and hasattr(t, "__args__"):
-            ot = get_origin(t)
-            args = getattr(t, "__args__")
-            if ot is list:
-                return typing.List[_change_unrecognized_type_to_pickle(args[0])]  # type: ignore
-            elif ot is dict and args[0] == str:
-                return typing.Dict[str, _change_unrecognized_type_to_pickle(args[1])]  # type: ignore
-            elif ot is typing.Union:
-                return typing.Union[tuple(_change_unrecognized_type_to_pickle(v) for v in get_args(t))]  # type: ignore
-            elif ot is Annotated:
-                base_type, *config = get_args(t)
-                return Annotated[(_change_unrecognized_type_to_pickle(base_type), *config)]  # type: ignore
-        TypeEngine.get_transformer(t)
-    except ValueError:
-        logger.warning(
-            f"Unsupported Type {t} found, Flyte will default to use PickleFile as the transport. "
-            f"Pickle can only be used to send objects between the exact same version of Python, "
-            f"and we strongly recommend to use python type that flyte support."
-        )
-        return FlytePickle[t]
-    return t
-
-
 def transform_function_to_interface(fn: typing.Callable, docstring: Optional[Docstring] = None) -> Interface:
     """
     From the annotations on a task function that the user should have provided, and the output names they want to use
     for each output parameter, construct the TypedInterface object
 
     For now the fancy object, maybe in the future a dumb object.
 
     """
     type_hints = get_type_hints(fn, include_extras=True)
     signature = inspect.signature(fn)
     return_annotation = type_hints.get("return", None)
 
     outputs = extract_return_annotation(return_annotation)
     for k, v in outputs.items():
-        outputs[k] = _change_unrecognized_type_to_pickle(v)  # type: ignore
+        outputs[k] = v  # type: ignore
     inputs: Dict[str, Tuple[Type, Any]] = OrderedDict()
     for k, v in signature.parameters.items():  # type: ignore
         annotation = type_hints.get(k, None)
         default = v.default if v.default is not inspect.Parameter.empty else None
         # Inputs with default values are currently ignored, we may want to look into that in the future
-        inputs[k] = (_change_unrecognized_type_to_pickle(annotation), default)  # type: ignore
+        inputs[k] = (annotation, default)  # type: ignore
 
     # This is just for typing.NamedTuples - in those cases, the user can select a name to call the NamedTuple. We
     # would like to preserve that name in our custom collections.namedtuple.
     custom_name = None
     if hasattr(return_annotation, "__bases__"):
         bases = return_annotation.__bases__
         if len(bases) == 1 and bases[0] == tuple and hasattr(return_annotation, "_fields"):
@@ -361,28 +339,14 @@
     Given a map of str (names of inputs for instance) to their Python native types, return a map of the name to a
     Flyte Variable object with that type.
     """
     res = OrderedDict()
     if variable_map:
         for k, v in variable_map.items():
             res[k] = transform_type(v, descriptions.get(k, k))
-            sub_type: type = v
-            if hasattr(v, "__origin__") and hasattr(v, "__args__"):
-                if getattr(v, "__origin__") is list:
-                    sub_type = getattr(v, "__args__")[0]
-                elif getattr(v, "__origin__") is dict:
-                    sub_type = getattr(v, "__args__")[1]
-            if hasattr(sub_type, "__origin__") and getattr(sub_type, "__origin__") is FlytePickle:
-                original_type = cast(FlytePickle, sub_type).python_type()
-                if hasattr(original_type, "__name__"):
-                    res[k].type.metadata = {"python_class_name": original_type.__name__}
-                elif hasattr(original_type, "_name"):
-                    # If the class doesn't have the __name__ attribute, like typing.Sequence, use _name instead.
-                    res[k].type.metadata = {"python_class_name": original_type._name}
-
     return res
 
 
 def transform_type(x: type, description: Optional[str] = None) -> _interface_models.Variable:
     return _interface_models.Variable(type=TypeEngine.to_literal_type(x), description=description)
```

### Comparing `flytekit-1.9.0a0/flytekit/core/launch_plan.py` & `flytekit-1.9.1/flytekit/core/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/local_cache.py` & `flytekit-1.9.1/flytekit/core/local_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 
 # Location on the filesystem where serialized objects will be stored
 # TODO: read from config
 CACHE_LOCATION = "~/.flyte/local-cache"
 
 
 def _recursive_hash_placement(literal: Literal) -> Literal:
-    if literal.collection is not None:
-        literals = [_recursive_hash_placement(literal) for literal in literal.collection.literals]
+    # Base case, hash gets passed through always if set
+    if literal.hash is not None:
+        return Literal(hash=literal.hash)
+    elif literal.collection is not None:
+        literals = [_recursive_hash_placement(lit) for lit in literal.collection.literals]
         return Literal(collection=LiteralCollection(literals=literals))
     elif literal.map is not None:
         literal_map = {}
-        for key, literal in literal.map.literals.items():
-            literal_map[key] = _recursive_hash_placement(literal)
+        for key, literal_value in literal.map.literals.items():
+            literal_map[key] = _recursive_hash_placement(literal_value)
         return Literal(map=LiteralMap(literal_map))
-
-    # Base case
-    if literal.hash is not None:
-        return Literal(hash=literal.hash)
     else:
         return literal
 
 
 def _calculate_cache_key(task_name: str, cache_version: str, input_literal_map: LiteralMap) -> str:
     # Traverse the literals and replace the literal with a new literal that only contains the hash
     literal_map_overridden = {}
```

### Comparing `flytekit-1.9.0a0/flytekit/core/map_task.py` & `flytekit-1.9.1/flytekit/core/map_task.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 from flytekit.configuration import SerializationSettings
 from flytekit.core import tracker
 from flytekit.core.base_task import PythonTask, Task, TaskResolverMixin
 from flytekit.core.constants import SdkTaskType
 from flytekit.core.context_manager import ExecutionState, FlyteContext, FlyteContextManager
 from flytekit.core.interface import transform_interface_to_list_interface
-from flytekit.core.python_function_task import PythonFunctionTask
+from flytekit.core.python_function_task import PythonFunctionTask, PythonInstanceTask
 from flytekit.core.tracker import TrackedInstance
 from flytekit.core.utils import timeit
 from flytekit.exceptions import scopes as exception_scopes
 from flytekit.models.array_job import ArrayJob
 from flytekit.models.interface import Variable
 from flytekit.models.task import Container, K8sPod, Sql
 from flytekit.tools.module_loader import load_object_from_module
@@ -30,15 +30,15 @@
     """
     A MapPythonTask defines a :py:class:`flytekit.PythonTask` which specifies how to run
     an inner :py:class:`flytekit.PythonFunctionTask` across a range of inputs in parallel.
     """
 
     def __init__(
         self,
-        python_function_task: typing.Union[PythonFunctionTask, functools.partial],
+        python_function_task: typing.Union[PythonFunctionTask, PythonInstanceTask, functools.partial],
         concurrency: Optional[int] = None,
         min_success_ratio: Optional[float] = None,
         bound_inputs: Optional[Set[str]] = None,
         **kwargs,
     ):
         """
         Wrapper that creates a MapPythonTask
@@ -61,26 +61,39 @@
                     raise ValueError("Map tasks do not support partial tasks with lists as inputs. ")
             self._partial = python_function_task
             actual_task = self._partial.func
         else:
             actual_task = python_function_task
 
         if not isinstance(actual_task, PythonFunctionTask):
-            raise ValueError("Map tasks can only compose of Python Functon Tasks currently")
+            if isinstance(actual_task, PythonInstanceTask):
+                pass
+            else:
+                raise ValueError("Map tasks can only compose of PythonFuncton and PythonInstanceTasks currently")
 
-        if len(actual_task.python_interface.outputs.keys()) > 1:
+        n_outputs = len(actual_task.python_interface.outputs.keys())
+        if n_outputs > 1:
             raise ValueError("Map tasks only accept python function tasks with 0 or 1 outputs")
 
         self._bound_inputs: typing.Set[str] = set(bound_inputs) if bound_inputs else set()
         if self._partial:
             self._bound_inputs = set(self._partial.keywords.keys())
 
-        collection_interface = transform_interface_to_list_interface(actual_task.python_interface, self._bound_inputs)
-        self._run_task: PythonFunctionTask = actual_task
-        _, mod, f, _ = tracker.extract_task_module(actual_task.task_function)
+        # Transform the interface to List[Optional[T]] in case `min_success_ratio` is set
+        output_as_list_of_optionals = min_success_ratio is not None and min_success_ratio != 1 and n_outputs == 1
+        collection_interface = transform_interface_to_list_interface(
+            actual_task.python_interface, self._bound_inputs, output_as_list_of_optionals
+        )
+
+        self._run_task: typing.Union[PythonFunctionTask, PythonInstanceTask] = actual_task  # type: ignore
+        if isinstance(actual_task, PythonInstanceTask):
+            mod = actual_task.task_type
+            f = actual_task.lhs
+        else:
+            _, mod, f, _ = tracker.extract_task_module(typing.cast(PythonFunctionTask, actual_task).task_function)
         h = hashlib.md5(collection_interface.__str__().encode("utf-8")).hexdigest()
         name = f"{mod}.map_{f}_{h}"
 
         self._cmd_prefix: typing.Optional[typing.List[str]] = None
         self._max_concurrency: typing.Optional[int] = concurrency
         self._min_success_ratio: typing.Optional[float] = min_success_ratio
         self._array_task_interface = actual_task.python_interface
@@ -130,14 +143,15 @@
 
     def set_command_prefix(self, cmd: typing.Optional[typing.List[str]]):
         self._cmd_prefix = cmd
 
     @contextmanager
     def prepare_target(self):
         """
+        TODO: why do we do this?
         Alters the underlying run_task command to modify it for map task execution and then resets it after.
         """
         self._run_task.set_command_fn(self.get_command)
         try:
             yield
         finally:
             self._run_task.reset_command_fn()
@@ -157,15 +171,15 @@
     def get_custom(self, settings: SerializationSettings) -> Dict[str, Any]:
         return ArrayJob(parallelism=self._max_concurrency, min_success_ratio=self._min_success_ratio).to_dict()
 
     def get_config(self, settings: SerializationSettings) -> Optional[Dict[str, str]]:
         return self._run_task.get_config(settings)
 
     @property
-    def run_task(self) -> PythonFunctionTask:
+    def run_task(self) -> typing.Union[PythonFunctionTask, PythonInstanceTask]:
         return self._run_task
 
     def __call__(self, *args, **kwargs):
         """
         This call method modifies the kwargs and adds kwargs from partial.
         This is mostly done in the local_execute and compilation only.
         At runtime, the map_task is created with all the inputs filled in. to support this, we have modified
@@ -200,28 +214,28 @@
         We override this method from PythonTask because the dispatch_execute method uses this
         interface to construct outputs. Each instance of an container_array task will however produce outputs
         according to the underlying run_task interface and the array plugin handler will actually create a collection
         from these individual outputs as the final output value.
         """
 
         ctx = FlyteContextManager.current_context()
-        if ctx.execution_state is not None and ctx.execution_state.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION:
+        if ctx.execution_state and ctx.execution_state.is_local_execution():
             # In workflow execution mode we actually need to use the parent (mapper) task output interface.
             return self.interface.outputs
         return self._run_task.interface.outputs
 
     def get_type_for_output_var(self, k: str, v: Any) -> type:
         """
         We override this method from flytekit.core.base_task Task because the dispatch_execute method uses this
         interface to construct outputs. Each instance of an container_array task will however produce outputs
         according to the underlying run_task interface and the array plugin handler will actually create a collection
         from these individual outputs as the final output value.
         """
         ctx = FlyteContextManager.current_context()
-        if ctx.execution_state is not None and ctx.execution_state.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION:
+        if ctx.execution_state and ctx.execution_state.is_local_execution():
             # In workflow execution mode we actually need to use the parent (mapper) task output interface.
             return self._python_interface.outputs[k]
         return self._run_task._python_interface.outputs[k]
 
     def _execute_map_task(self, _: FlyteContext, **kwargs) -> Any:
         """
         This is called during ExecutionState.Mode.TASK_EXECUTION executions, that is executions orchestrated by the
@@ -267,15 +281,15 @@
             if outputs_expected:
                 outputs.append(o)
 
         return outputs
 
 
 def map_task(
-    task_function: typing.Union[PythonFunctionTask, functools.partial],
+    task_function: typing.Union[PythonFunctionTask, PythonInstanceTask, functools.partial],
     concurrency: int = 0,
     min_success_ratio: float = 1.0,
     **kwargs,
 ):
     """
     Use a map task for parallelizable tasks that run across a list of an input type. A map task can be composed of
     any individual :py:class:`flytekit.PythonFunctionTask`.
```

### Comparing `flytekit-1.9.0a0/flytekit/core/mock_stats.py` & `flytekit-1.9.1/flytekit/core/mock_stats.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/node.py` & `flytekit-1.9.1/flytekit/core/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,14 +124,16 @@
             self._metadata._name = kwargs["name"]
         if "task_config" in kwargs:
             logger.warning("This override is beta. We may want to revisit this in the future.")
             new_task_config = kwargs["task_config"]
             if not isinstance(new_task_config, type(self.flyte_entity._task_config)):
                 raise ValueError("can't change the type of the task config")
             self.flyte_entity._task_config = new_task_config
+        if "container_image" in kwargs:
+            self.flyte_entity._container_image = kwargs["container_image"]
         return self
 
 
 def _convert_resource_overrides(
     resources: typing.Optional[Resources], resource_name: str
 ) -> typing.List[_resources_model.ResourceEntry]:
     if resources is None:
```

### Comparing `flytekit-1.9.0a0/flytekit/core/node_creation.py` & `flytekit-1.9.1/flytekit/core/node_creation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Union
 
 from flytekit.core.base_task import PythonTask
-from flytekit.core.context_manager import BranchEvalMode, ExecutionState, FlyteContext
+from flytekit.core.context_manager import BranchEvalMode, FlyteContext
 from flytekit.core.launch_plan import LaunchPlan
 from flytekit.core.node import Node
 from flytekit.core.promise import VoidPromise
 from flytekit.core.workflow import WorkflowBase
 from flytekit.exceptions import user as _user_exceptions
 from flytekit.loggers import logger
 
@@ -140,18 +140,15 @@
                 node.outputs[output_names[0]] = outputs
 
         return node
 
     # Handling local execution
     # Note: execution state is set to TASK_EXECUTION when running dynamic task locally
     # https://github.com/flyteorg/flytekit/blob/0815345faf0fae5dc26746a43d4bda4cc2cdf830/flytekit/core/python_function_task.py#L262
-    elif ctx.execution_state is not None and (
-        ctx.execution_state.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION
-        or ctx.execution_state.mode == ExecutionState.Mode.TASK_EXECUTION
-    ):
+    elif ctx.execution_state and ctx.execution_state.is_local_execution():
         if isinstance(entity, RemoteEntity):
             raise AssertionError(f"Remote entities are not yet runnable locally {entity.name}")
 
         if ctx.execution_state.branch_eval_mode == BranchEvalMode.BRANCH_SKIPPED:
             logger.warning(f"Manual node creation cannot be used in branch logic {entity.name}")
             raise Exception("Being more restrictive for now and disallowing manual node creation in branch logic")
```

### Comparing `flytekit-1.9.0a0/flytekit/core/notification.py` & `flytekit-1.9.1/flytekit/core/notification.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/pod_template.py` & `flytekit-1.9.1/flytekit/core/pod_template.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/promise.py` & `flytekit-1.9.1/flytekit/core/promise.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import collections
+import inspect
 from enum import Enum
-from typing import Any, Dict, List, Optional, Set, Tuple, Union, cast
+from typing import Any, Coroutine, Dict, List, Optional, Set, Tuple, Union, cast
 
 from typing_extensions import Protocol, get_args
 
 from flytekit.core import constants as _common_constants
 from flytekit.core import context_manager as _flyte_context
 from flytekit.core import interface as flyte_interface
 from flytekit.core import type_engine
@@ -19,29 +20,28 @@
 )
 from flytekit.core.interface import Interface
 from flytekit.core.node import Node
 from flytekit.core.type_engine import DictTransformer, ListTransformer, TypeEngine, TypeTransformerFailedError
 from flytekit.exceptions import user as _user_exceptions
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
-from flytekit.models import literals as _literal_models
 from flytekit.models import literals as _literals_models
 from flytekit.models import types as _type_models
 from flytekit.models import types as type_models
 from flytekit.models.core import workflow as _workflow_model
 from flytekit.models.literals import Primitive
 from flytekit.models.types import SimpleType
 
 
 def translate_inputs_to_literals(
     ctx: FlyteContext,
     incoming_values: Dict[str, Any],
     flyte_interface_types: Dict[str, _interface_models.Variable],
     native_types: Dict[str, type],
-) -> Dict[str, _literal_models.Literal]:
+) -> Dict[str, _literals_models.Literal]:
     """
     The point of this function is to extract out Literals from a collection of either Python native values (which would
     be converted into Flyte literals) or Promises (the literals in which would just get extracted).
 
     When calling a task inside a workflow, a user might do something like this.
 
         def my_wf(in1: int) -> int:
@@ -65,95 +65,25 @@
     This helper function is used both when sorting out inputs to a task, as well as outputs of a function.
 
     :param ctx: Context needed in case a non-primitive literal needs to be translated to a Flyte literal (like a file)
     :param incoming_values: This is a map of your task's input or wf's output kwargs basically
     :param flyte_interface_types: One side of an :py:class:`flytekit.models.interface.TypedInterface` basically.
     :param native_types: Map to native Python type.
     """
-
-    def extract_value(
-        ctx: FlyteContext,
-        input_val: Any,
-        val_type: type,
-        flyte_literal_type: _type_models.LiteralType,
-    ) -> _literal_models.Literal:
-        if isinstance(input_val, list):
-            lt = flyte_literal_type
-            python_type = val_type
-            if flyte_literal_type.union_type:
-                for i in range(len(flyte_literal_type.union_type.variants)):
-                    variant = flyte_literal_type.union_type.variants[i]
-                    if variant.collection_type:
-                        lt = variant
-                        python_type = get_args(val_type)[i]
-            if lt.collection_type is None:
-                raise TypeError(f"Not a collection type {flyte_literal_type} but got a list {input_val}")
-            try:
-                sub_type: type = ListTransformer.get_sub_type(python_type)
-            except ValueError:
-                if len(input_val) == 0:
-                    raise
-                sub_type = type(input_val[0])
-            # To maintain consistency between translate_inputs_to_literals and ListTransformer.to_literal for batchable types,
-            # directly call ListTransformer.to_literal to batch process the list items. This is necessary because processing
-            # each list item separately could lead to errors since ListTransformer.to_python_value may treat the literal
-            # as it is batched for batchable types.
-            if ListTransformer.is_batchable(python_type):
-                return TypeEngine.to_literal(ctx, input_val, python_type, lt)
-            literal_list = [extract_value(ctx, v, sub_type, lt.collection_type) for v in input_val]
-            return _literal_models.Literal(collection=_literal_models.LiteralCollection(literals=literal_list))
-        elif isinstance(input_val, dict):
-            lt = flyte_literal_type
-            python_type = val_type
-            if flyte_literal_type.union_type:
-                for i in range(len(flyte_literal_type.union_type.variants)):
-                    variant = flyte_literal_type.union_type.variants[i]
-                    if variant.map_value_type:
-                        lt = variant
-                        python_type = get_args(val_type)[i]
-                    if variant.simple == _type_models.SimpleType.STRUCT:
-                        lt = variant
-                        python_type = get_args(val_type)[i]
-            if lt.map_value_type is None and lt.simple != _type_models.SimpleType.STRUCT:
-                raise TypeError(f"Not a map type {lt} but got a map {input_val}")
-            if lt.simple == _type_models.SimpleType.STRUCT:
-                return TypeEngine.to_literal(ctx, input_val, type(input_val), lt)
-            else:
-                k_type, sub_type = DictTransformer.get_dict_types(python_type)  # type: ignore
-                literal_map = {k: extract_value(ctx, v, sub_type, lt.map_value_type) for k, v in input_val.items()}
-                return _literal_models.Literal(map=_literal_models.LiteralMap(literals=literal_map))
-        elif isinstance(input_val, Promise):
-            # In the example above, this handles the "in2=a" type of argument
-            return input_val.val
-        elif isinstance(input_val, VoidPromise):
-            raise AssertionError(
-                f"Outputs of a non-output producing task {input_val.task_name} cannot be passed to another task."
-            )
-        elif isinstance(input_val, tuple):
-            raise AssertionError(
-                "Tuples are not a supported type for individual values in Flyte - got a tuple -"
-                f" {input_val}. If using named tuple in an inner task, please, de-reference the"
-                "actual attribute that you want to use. For example, in NamedTuple('OP', x=int) then"
-                "return v.x, instead of v, even if this has a single element"
-            )
-        else:
-            # This handles native values, the 5 example
-            return TypeEngine.to_literal(ctx, input_val, val_type, flyte_literal_type)
-
     if incoming_values is None:
         raise ValueError("Incoming values cannot be None, must be a dict")
 
     result = {}  # So as to not overwrite the input_kwargs
     for k, v in incoming_values.items():
         if k not in flyte_interface_types:
             raise ValueError(f"Received unexpected keyword argument {k}")
         var = flyte_interface_types[k]
         t = native_types[k]
         try:
-            result[k] = extract_value(ctx, v, t, var.type)
+            result[k] = TypeEngine.to_literal(ctx, v, t, var.type)
         except TypeTransformerFailedError as exc:
             raise TypeTransformerFailedError(f"Failed argument '{k}': {exc}") from exc
 
     return result
 
 
 def get_primitive_val(prim: Primitive) -> Any:
@@ -215,19 +145,19 @@
                     raise ValueError("Only primitive values can be used in comparison")
         if self._lhs is None:
             self._lhs = type_engine.TypeEngine.to_literal(FlyteContextManager.current_context(), lhs, type(lhs), None)
         if self._rhs is None:
             self._rhs = type_engine.TypeEngine.to_literal(FlyteContextManager.current_context(), rhs, type(rhs), None)
 
     @property
-    def rhs(self) -> Union["Promise", _literal_models.Literal]:
+    def rhs(self) -> Union["Promise", _literals_models.Literal]:
         return self._rhs
 
     @property
-    def lhs(self) -> Union["Promise", _literal_models.Literal]:
+    def lhs(self) -> Union["Promise", _literals_models.Literal]:
         return self._lhs
 
     @property
     def op(self) -> ComparisonOps:
         return self._op
 
     def eval(self) -> bool:
@@ -347,15 +277,15 @@
        If the task returns an integer or a ``(int, str)`` tuple like ``t1`` above, calling ``with_overrides`` on the
        result would throw an error. This Promise object adds that.
     #. Assorted handling for conditionals.
     """
 
     # TODO: Currently, NodeOutput we're creating is the slimmer core package Node class, but since only the
     #  id is used, it's okay for now. Let's clean all this up though.
-    def __init__(self, var: str, val: Union[NodeOutput, _literal_models.Literal]):
+    def __init__(self, var: str, val: Union[NodeOutput, _literals_models.Literal]):
         self._var = var
         self._promise_ready = True
         self._val = val
         if val and isinstance(val, NodeOutput):
             self._ref = val
             self._promise_ready = False
             self._val = None
@@ -384,15 +314,15 @@
                 print(p.val)
            else:
                 print(p.ref)
         """
         return self._promise_ready
 
     @property
-    def val(self) -> _literal_models.Literal:
+    def val(self) -> _literals_models.Literal:
         """
         If the promise is ready then this holds the actual evaluate value in Flyte's type system
         """
         return self._val
 
     @property
     def ref(self) -> NodeOutput:
@@ -566,21 +496,14 @@
     # Should this class be part of the Interface?
     class Output(collections.namedtuple(named_tuple_name, variables)):  # type: ignore
         def with_overrides(self, *args, **kwargs):
             val = self.__getattribute__(self._fields[0])
             val.with_overrides(*args, **kwargs)
             return self
 
-        @property
-        def ref(self):
-            for p in promises:
-                if p.ref:
-                    return p.ref
-            return None
-
         def runs_before(self, other: Any):
             """
             This function is just here to allow local workflow execution to run. See the corresponding function in
             flytekit.core.node.Node for more information. Local workflow execution in the manual ``create_node``
             paradigm is already determined by the order in which the nodes were created.
             """
             # TODO: If possible, add a check and raise an Exception if create_node was not called in the correct order.
@@ -589,59 +512,52 @@
         def __rshift__(self, other: Any):
             # See comment for runs_before
             return other
 
     return Output(*promises)  # type: ignore
 
 
-def binding_from_flyte_std(
-    ctx: _flyte_context.FlyteContext,
-    var_name: str,
-    expected_literal_type: _type_models.LiteralType,
-    t_value: Any,
-) -> _literals_models.Binding:
-    binding_data = binding_data_from_python_std(ctx, expected_literal_type, t_value, t_value_type=None)
-    return _literals_models.Binding(var=var_name, binding=binding_data)
-
-
 def binding_data_from_python_std(
     ctx: _flyte_context.FlyteContext,
     expected_literal_type: _type_models.LiteralType,
     t_value: Any,
-    t_value_type: Optional[type] = None,
+    t_value_type: type,
+    nodes: List[Node],
 ) -> _literals_models.BindingData:
     # This handles the case where the given value is the output of another task
     if isinstance(t_value, Promise):
         if not t_value.is_ready:
+            nodes.append(t_value.ref.node)  # keeps track of upstream nodes
             return _literals_models.BindingData(promise=t_value.ref)
 
     elif isinstance(t_value, VoidPromise):
         raise AssertionError(
             f"Cannot pass output from task {t_value.task_name} that produces no outputs to a downstream task"
         )
 
-    elif expected_literal_type.union_type is not None:
+    elif t_value is not None and expected_literal_type.union_type is not None:
         for i in range(len(expected_literal_type.union_type.variants)):
             try:
                 lt_type = expected_literal_type.union_type.variants[i]
                 python_type = get_args(t_value_type)[i] if t_value_type else None
-                return binding_data_from_python_std(ctx, lt_type, t_value, python_type)
+                return binding_data_from_python_std(ctx, lt_type, t_value, python_type, nodes)
             except Exception:
                 logger.debug(
                     f"failed to bind data {t_value} with literal type {expected_literal_type.union_type.variants[i]}."
                 )
         raise AssertionError(
             f"Failed to bind data {t_value} with literal type {expected_literal_type.union_type.variants}."
         )
 
     elif isinstance(t_value, list):
-        sub_type: Optional[type] = ListTransformer.get_sub_type(t_value_type) if t_value_type else None
+        sub_type: type = ListTransformer.get_sub_type(t_value_type)
         collection = _literals_models.BindingDataCollection(
             bindings=[
-                binding_data_from_python_std(ctx, expected_literal_type.collection_type, t, sub_type) for t in t_value
+                binding_data_from_python_std(ctx, expected_literal_type.collection_type, t, sub_type, nodes)
+                for t in t_value
             ]
         )
 
         return _literals_models.BindingData(collection=collection)
 
     elif isinstance(t_value, dict):
         if (
@@ -651,21 +567,20 @@
             raise AssertionError(
                 f"this should be a Dictionary type and it is not: {type(t_value)} vs {expected_literal_type}"
             )
         if expected_literal_type.simple == _type_models.SimpleType.STRUCT:
             lit = TypeEngine.to_literal(ctx, t_value, type(t_value), expected_literal_type)
             return _literals_models.BindingData(scalar=lit.scalar)
         else:
-            _, v_type = (
-                DictTransformer.get_dict_types(t_value_type) if t_value_type else None,
-                None,
-            )
+            _, v_type = DictTransformer.get_dict_types(t_value_type)
             m = _literals_models.BindingDataMap(
                 bindings={
-                    k: binding_data_from_python_std(ctx, expected_literal_type.map_value_type, v, v_type)
+                    k: binding_data_from_python_std(
+                        ctx, expected_literal_type.map_value_type, v, v_type or type(v), nodes
+                    )
                     for k, v in t_value.items()
                 }
             )
         return _literals_models.BindingData(map=m)
 
     elif isinstance(t_value, tuple):
         raise AssertionError(
@@ -682,17 +597,18 @@
 
 def binding_from_python_std(
     ctx: _flyte_context.FlyteContext,
     var_name: str,
     expected_literal_type: _type_models.LiteralType,
     t_value: Any,
     t_value_type: type,
-) -> _literals_models.Binding:
-    binding_data = binding_data_from_python_std(ctx, expected_literal_type, t_value, t_value_type)
-    return _literals_models.Binding(var=var_name, binding=binding_data)
+) -> Tuple[_literals_models.Binding, List[Node]]:
+    nodes: List[Node] = []
+    binding_data = binding_data_from_python_std(ctx, expected_literal_type, t_value, t_value_type, nodes)
+    return _literals_models.Binding(var=var_name, binding=binding_data), nodes
 
 
 def to_binding(p: Promise) -> _literals_models.Binding:
     return _literals_models.Binding(var=p.var, binding=_literals_models.BindingData(promise=p.ref))
 
 
 class VoidPromise(object):
@@ -872,15 +788,15 @@
 
     if _inputs_not_allowed:
         inputs_not_allowed_specified = _inputs_not_allowed.intersection(kwargs.keys())
         if inputs_not_allowed_specified:
             raise _user_exceptions.FlyteAssertion(
                 f"Fixed inputs cannot be specified. Please remove the following inputs - {inputs_not_allowed_specified}"
             )
-
+    nodes = []
     for k in sorted(typed_interface.inputs):
         var = typed_interface.inputs[k]
         if k not in kwargs:
             if _inputs_not_allowed and _ignorable_inputs:
                 if k in _ignorable_inputs or k in _inputs_not_allowed:
                     continue
             # TODO to improve the error message, should we show python equivalent types for var.type?
@@ -891,44 +807,37 @@
         # into the function.
         if isinstance(v, tuple):
             raise AssertionError(
                 f"Variable({k}) for function({entity.name}) cannot receive a multi-valued tuple {v}."
                 f" Check if the predecessor function returning more than one value?"
             )
         try:
-            bindings.append(
-                binding_from_flyte_std(
-                    ctx,
-                    var_name=k,
-                    expected_literal_type=var.type,
-                    t_value=v,
-                )
+            b, n = binding_from_python_std(
+                ctx,
+                var_name=k,
+                expected_literal_type=var.type,
+                t_value=v,
+                t_value_type=type(v),  # since we don't have the python type available
             )
+            bindings.append(b)
+            nodes.extend(n)
             used_inputs.add(k)
         except Exception as e:
             raise AssertionError(f"Failed to Bind variable {k} for function {entity.name}.") from e
 
     extra_inputs = used_inputs ^ set(kwargs.keys())
     if len(extra_inputs) > 0:
         raise _user_exceptions.FlyteAssertion(
             f"Too many inputs for [{entity.name}] Expected inputs: {typed_interface.inputs.keys()} "
             f"- extra inputs: {extra_inputs}"
         )
 
     # Detect upstream nodes
     # These will be our core Nodes until we can amend the Promise to use NodeOutputs that reference our Nodes
-    upstream_nodes = list(
-        set(
-            [
-                input_val.ref.node
-                for input_val in kwargs.values()
-                if isinstance(input_val, Promise) and input_val.ref.node_id != _common_constants.GLOBAL_INPUT_NODE_ID
-            ]
-        )
-    )
+    upstream_nodes = list(set([n for n in nodes if n.id != _common_constants.GLOBAL_INPUT_NODE_ID]))
 
     flytekit_node = Node(
         id=f"{ctx.compilation_state.prefix}n{len(ctx.compilation_state.nodes)}",
         metadata=entity.construct_node_metadata(),
         bindings=sorted(bindings, key=lambda b: b.var),
         upstream_nodes=upstream_nodes,
         flyte_entity=entity,
@@ -961,14 +870,15 @@
     :return:  Optional[Union[Tuple[Promise], Promise, VoidPromise]]
     """
     if ctx.compilation_state is None:
         raise _user_exceptions.FlyteAssertion("Cannot create node when not compiling...")
 
     used_inputs = set()
     bindings = []
+    nodes = []
 
     interface = entity.python_interface
     typed_interface = flyte_interface.transform_interface_to_typed_interface(interface)
     # Mypy needs some extra help to believe that `typed_interface` will not be `None`
     assert typed_interface is not None
 
     for k in sorted(interface.inputs):
@@ -994,44 +904,36 @@
         # into the function.
         if isinstance(v, tuple):
             raise AssertionError(
                 f"Variable({k}) for function({entity.name}) cannot receive a multi-valued tuple {v}."
                 f" Check if the predecessor function returning more than one value?"
             )
         try:
-            bindings.append(
-                binding_from_python_std(
-                    ctx,
-                    var_name=k,
-                    expected_literal_type=var.type,
-                    t_value=v,
-                    t_value_type=interface.inputs[k],
-                )
+            b, n = binding_from_python_std(
+                ctx,
+                var_name=k,
+                expected_literal_type=var.type,
+                t_value=v,
+                t_value_type=interface.inputs[k],
             )
+            bindings.append(b)
+            nodes.extend(n)
             used_inputs.add(k)
         except Exception as e:
             raise AssertionError(f"Failed to Bind variable {k} for function {entity.name}.") from e
 
     extra_inputs = used_inputs ^ set(kwargs.keys())
     if len(extra_inputs) > 0:
         raise _user_exceptions.FlyteAssertion(
             "Too many inputs were specified for the interface.  Extra inputs were: {}".format(extra_inputs)
         )
 
     # Detect upstream nodes
     # These will be our core Nodes until we can amend the Promise to use NodeOutputs that reference our Nodes
-    upstream_nodes = list(
-        set(
-            [
-                input_val.ref.node
-                for input_val in kwargs.values()
-                if isinstance(input_val, Promise) and input_val.ref.node_id != _common_constants.GLOBAL_INPUT_NODE_ID
-            ]
-        )
-    )
+    upstream_nodes = list(set([n for n in nodes if n.id != _common_constants.GLOBAL_INPUT_NODE_ID]))
 
     flytekit_node = Node(
         # TODO: Better naming, probably a derivative of the function name.
         id=f"{ctx.compilation_state.prefix}n{len(ctx.compilation_state.nodes)}",
         metadata=entity.construct_node_metadata(),
         bindings=sorted(bindings, key=lambda b: b.var),
         upstream_nodes=upstream_nodes,
@@ -1051,18 +953,21 @@
     return create_task_output(node_outputs, interface)
 
 
 class LocallyExecutable(Protocol):
     def local_execute(self, ctx: FlyteContext, **kwargs) -> Union[Tuple[Promise], Promise, VoidPromise, None]:
         ...
 
+    def local_execution_mode(self) -> ExecutionState.Mode:
+        ...
+
 
 def flyte_entity_call_handler(
     entity: SupportsNodeCreation, *args, **kwargs
-) -> Union[Tuple[Promise], Promise, VoidPromise, Tuple, None]:
+) -> Union[Tuple[Promise], Promise, VoidPromise, Tuple, Coroutine, None]:
     """
     This function is the call handler for tasks, workflows, and launch plans (which redirects to the underlying
     workflow). The logic is the same for all three, but we did not want to create base class, hence this separate
     method. When one of these entities is () aka __called__, there are three things we may do:
     #. Compilation Mode - this happens when the function is called as part of a workflow (potentially
        dynamic task?). Instead of running the user function, produce promise objects and create a node.
     #. Workflow Execution Mode - when a workflow is being run locally. Even though workflows are functions
@@ -1084,46 +989,60 @@
     for k, v in kwargs.items():
         if k not in cast(SupportsNodeCreation, entity).python_interface.inputs:
             raise ValueError(
                 f"Received unexpected keyword argument '{k}' in function '{cast(SupportsNodeCreation, entity).name}'"
             )
 
     ctx = FlyteContextManager.current_context()
+    if ctx.execution_state and (
+        ctx.execution_state.mode == ExecutionState.Mode.TASK_EXECUTION
+        or ctx.execution_state.mode == ExecutionState.Mode.LOCAL_TASK_EXECUTION
+    ):
+        logger.error("You are not supposed to nest @Task/@Workflow inside a @Task!")
     if ctx.compilation_state is not None and ctx.compilation_state.mode == 1:
         return create_and_link_node(ctx, entity=entity, **kwargs)
-    elif ctx.execution_state is not None and ctx.execution_state.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION:
-        if ctx.execution_state.branch_eval_mode == BranchEvalMode.BRANCH_SKIPPED:
+    if ctx.execution_state and ctx.execution_state.is_local_execution():
+        mode = cast(LocallyExecutable, entity).local_execution_mode()
+        with FlyteContextManager.with_context(
+            ctx.with_execution_state(ctx.execution_state.with_params(mode=mode))
+        ) as child_ctx:
             if (
-                len(cast(SupportsNodeCreation, entity).python_interface.inputs) > 0
-                or len(cast(SupportsNodeCreation, entity).python_interface.outputs) > 0
+                child_ctx.execution_state
+                and child_ctx.execution_state.branch_eval_mode == BranchEvalMode.BRANCH_SKIPPED
             ):
-                output_names = list(cast(SupportsNodeCreation, entity).python_interface.outputs.keys())
-                if len(output_names) == 0:
-                    return VoidPromise(entity.name)
-                vals = [Promise(var, None) for var in output_names]
-                return create_task_output(vals, cast(SupportsNodeCreation, entity).python_interface)
-            else:
-                return None
-        return cast(LocallyExecutable, entity).local_execute(ctx, **kwargs)
+                if (
+                    len(cast(SupportsNodeCreation, entity).python_interface.inputs) > 0
+                    or len(cast(SupportsNodeCreation, entity).python_interface.outputs) > 0
+                ):
+                    output_names = list(cast(SupportsNodeCreation, entity).python_interface.outputs.keys())
+                    if len(output_names) == 0:
+                        return VoidPromise(entity.name)
+                    vals = [Promise(var, None) for var in output_names]
+                    return create_task_output(vals, cast(SupportsNodeCreation, entity).python_interface)
+                else:
+                    return None
+            return cast(LocallyExecutable, entity).local_execute(ctx, **kwargs)
     else:
+        mode = cast(LocallyExecutable, entity).local_execution_mode()
         with FlyteContextManager.with_context(
-            ctx.with_execution_state(
-                ctx.new_execution_state().with_params(mode=ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION)
-            )
+            ctx.with_execution_state(ctx.new_execution_state().with_params(mode=mode))
         ) as child_ctx:
             cast(ExecutionParameters, child_ctx.user_space_params)._decks = []
             result = cast(LocallyExecutable, entity).local_execute(child_ctx, **kwargs)
 
         expected_outputs = len(cast(SupportsNodeCreation, entity).python_interface.outputs)
         if expected_outputs == 0:
             if result is None or isinstance(result, VoidPromise):
                 return None
             else:
                 raise Exception(f"Received an output when workflow local execution expected None. Received: {result}")
 
+        if inspect.iscoroutine(result):
+            return result
+
         if (1 < expected_outputs == len(cast(Tuple[Promise], result))) or (
             result is not None and expected_outputs == 1
         ):
             return create_native_named_tuple(ctx, result, cast(SupportsNodeCreation, entity).python_interface)
 
         raise ValueError(
             f"Expected outputs and actual outputs do not match."
```

### Comparing `flytekit-1.9.0a0/flytekit/core/python_auto_container.py` & `flytekit-1.9.1/flytekit/core/python_auto_container.py`

 * *Files 3% similar despite different names*

```diff
@@ -233,22 +233,16 @@
         _, task_module, _, task_name, *_ = loader_args
 
         task_module = importlib.import_module(name=task_module)  # type: ignore
         task_def = getattr(task_module, task_name)
         return task_def
 
     def loader_args(self, settings: SerializationSettings, task: PythonAutoContainerTask) -> List[str]:  # type:ignore
-        from flytekit.core.python_function_task import PythonFunctionTask
-
-        if isinstance(task, PythonFunctionTask):
-            _, m, t, _ = extract_task_module(task.task_function)
-            return ["task-module", m, "task-name", t]
-        if isinstance(task, TrackedInstance):
-            _, m, t, _ = extract_task_module(task)
-            return ["task-module", m, "task-name", t]
+        _, m, t, _ = extract_task_module(task)
+        return ["task-module", m, "task-name", t]
 
     def get_all_tasks(self) -> List[PythonAutoContainerTask]:  # type: ignore
         raise Exception("should not be needed")
 
 
 default_task_resolver = DefaultTaskResolver()
```

### Comparing `flytekit-1.9.0a0/flytekit/core/python_customized_container_task.py` & `flytekit-1.9.1/flytekit/core/python_customized_container_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/python_function_task.py` & `flytekit-1.9.1/flytekit/core/python_function_task.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
    :toctree: generated/
 
    PythonFunctionTask
    PythonInstanceTask
 
 """
 
-
 from abc import ABC
 from collections import OrderedDict
 from enum import Enum
 from typing import Any, Callable, List, Optional, TypeVar, Union, cast
 
 from flytekit.core.base_task import Task, TaskResolverMixin
 from flytekit.core.context_manager import ExecutionState, FlyteContext, FlyteContextManager
@@ -89,14 +88,15 @@
     In the above code, the name of the function, the module, and the interface (inputs = int and outputs = str) will be
     auto detected.
     """
 
     class ExecutionBehavior(Enum):
         DEFAULT = 1
         DYNAMIC = 2
+        EAGER = 3
 
     def __init__(
         self,
         task_config: T,
         task_function: Callable,
         task_type="python-task",
         ignore_input_vars: Optional[List[str]] = None,
@@ -151,21 +151,35 @@
     def execution_mode(self) -> ExecutionBehavior:
         return self._execution_mode
 
     @property
     def task_function(self):
         return self._task_function
 
+    @property
+    def name(self) -> str:
+        """
+        Returns the name of the task.
+        """
+        if self.instantiated_in and self.instantiated_in not in self._name:
+            return f"{self.instantiated_in}.{self._name}"
+        return self._name
+
     def execute(self, **kwargs) -> Any:
         """
         This method will be invoked to execute the task. If you do decide to override this method you must also
         handle dynamic tasks or you will no longer be able to use the task as a dynamic task generator.
         """
         if self.execution_mode == self.ExecutionBehavior.DEFAULT:
             return exception_scopes.user_entry_point(self._task_function)(**kwargs)
+        elif self.execution_mode == self.ExecutionBehavior.EAGER:
+            # if the task is a coroutine function, inject the context object so that the async_entity
+            # has access to the FlyteContext.
+            kwargs["async_ctx"] = FlyteContextManager.current_context()
+            return exception_scopes.user_entry_point(self._task_function)(**kwargs)
         elif self.execution_mode == self.ExecutionBehavior.DYNAMIC:
             return self.dynamic_execute(self._task_function, **kwargs)
 
     def _create_and_cache_dynamic_workflow(self):
         if self._wf is None:
             workflow_meta = WorkflowMetadata(on_failure=WorkflowFailurePolicy.FAIL_IMMEDIATELY)
             defaults = WorkflowMetadataDefaults(
@@ -254,15 +268,15 @@
         Since the user code within a dynamic task constitute a workflow, we have to first compile the workflow, and
         then execute that workflow.
 
         When running for real in production, the task would stop after the compilation step, and then create a file
         representing that newly generated workflow, instead of executing it.
         """
         ctx = FlyteContextManager.current_context()
-        if ctx.execution_state and ctx.execution_state.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION:
+        if ctx.execution_state and ctx.execution_state.is_local_execution():
             # The rest of this function mimics the local_execute of the workflow. We can't use the workflow
             # local_execute directly though since that converts inputs into Promises.
             logger.debug(f"Executing Dynamic workflow, using raw inputs {kwargs}")
             self._create_and_cache_dynamic_workflow()
             function_outputs = cast(PythonFunctionWorkflow, self._wf).execute(**kwargs)
 
             if isinstance(function_outputs, VoidPromise) or function_outputs is None:
```

### Comparing `flytekit-1.9.0a0/flytekit/core/reference.py` & `flytekit-1.9.1/flytekit/core/reference.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/reference_entity.py` & `flytekit-1.9.1/flytekit/core/reference_entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,14 +178,17 @@
         # Tasks that don't return anything still return a VoidPromise
         if len(output_names) == 0:
             return VoidPromise(self.name)
 
         vals = [Promise(var, outputs_literals[var]) for var in output_names]
         return create_task_output(vals, self.python_interface)
 
+    def local_execution_mode(self):
+        return ExecutionState.Mode.LOCAL_TASK_EXECUTION
+
     def construct_node_metadata(self) -> _workflow_model.NodeMetadata:
         return _workflow_model.NodeMetadata(name=extract_obj_name(self.name))
 
     def compile(self, ctx: FlyteContext, *args, **kwargs):
         return create_and_link_node(ctx, entity=self, **kwargs)
 
     def __call__(self, *args, **kwargs):
@@ -203,17 +206,15 @@
             raise _user_exceptions.FlyteAssertion(
                 f"Cannot call reference entity with args - detected {len(args)} positional args {args}"
             )
 
         ctx = FlyteContext.current_context()
         if ctx.compilation_state is not None and ctx.compilation_state.mode == 1:
             return self.compile(ctx, *args, **kwargs)
-        elif (
-            ctx.execution_state is not None and ctx.execution_state.mode == ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION
-        ):
+        elif ctx.execution_state and ctx.execution_state.is_local_execution():
             if ctx.execution_state.branch_eval_mode == BranchEvalMode.BRANCH_SKIPPED:
                 return
             return self.local_execute(ctx, **kwargs)
         else:
             logger.debug("Reference entity - running raw execute")
             return self.execute(**kwargs)
```

### Comparing `flytekit-1.9.0a0/flytekit/core/resources.py` & `flytekit-1.9.1/flytekit/core/resources.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/schedule.py` & `flytekit-1.9.1/flytekit/core/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/shim_task.py` & `flytekit-1.9.1/flytekit/core/shim_task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/task.py` & `flytekit-1.9.1/flytekit/core/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         if plugin_config_type in cls._PYTHONFUNCTION_TASK_PLUGINS:
             return cls._PYTHONFUNCTION_TASK_PLUGINS[plugin_config_type]
         # Defaults to returning Base PythonFunctionTask
         return PythonFunctionTask
 
 
 T = TypeVar("T")
+FuncOut = TypeVar("FuncOut")
 
 
 @overload
 def task(
     _task_function: None = ...,
     task_config: Optional[T] = ...,
     cache: bool = ...,
@@ -96,21 +97,21 @@
     secret_requests: Optional[List[Secret]] = ...,
     execution_mode: PythonFunctionTask.ExecutionBehavior = ...,
     task_resolver: Optional[TaskResolverMixin] = ...,
     docs: Optional[Documentation] = ...,
     disable_deck: bool = ...,
     pod_template: Optional["PodTemplate"] = ...,
     pod_template_name: Optional[str] = ...,
-) -> Callable[[Callable[..., Any]], PythonFunctionTask[T]]:
+) -> Callable[[Callable[..., FuncOut]], PythonFunctionTask[T]]:
     ...
 
 
 @overload
 def task(
-    _task_function: Callable[..., Any],
+    _task_function: Callable[..., FuncOut],
     task_config: Optional[T] = ...,
     cache: bool = ...,
     cache_serialize: bool = ...,
     cache_version: str = ...,
     retries: int = ...,
     interruptible: Optional[bool] = ...,
     deprecated: str = ...,
@@ -122,20 +123,20 @@
     secret_requests: Optional[List[Secret]] = ...,
     execution_mode: PythonFunctionTask.ExecutionBehavior = ...,
     task_resolver: Optional[TaskResolverMixin] = ...,
     docs: Optional[Documentation] = ...,
     disable_deck: bool = ...,
     pod_template: Optional["PodTemplate"] = ...,
     pod_template_name: Optional[str] = ...,
-) -> PythonFunctionTask[T]:
+) -> Union[PythonFunctionTask[T], Callable[..., FuncOut]]:
     ...
 
 
 def task(
-    _task_function: Optional[Callable[..., Any]] = None,
+    _task_function: Optional[Callable[..., FuncOut]] = None,
     task_config: Optional[T] = None,
     cache: bool = False,
     cache_serialize: bool = False,
     cache_version: str = "",
     retries: int = 0,
     interruptible: Optional[bool] = None,
     deprecated: str = "",
@@ -147,21 +148,21 @@
     secret_requests: Optional[List[Secret]] = None,
     execution_mode: PythonFunctionTask.ExecutionBehavior = PythonFunctionTask.ExecutionBehavior.DEFAULT,
     task_resolver: Optional[TaskResolverMixin] = None,
     docs: Optional[Documentation] = None,
     disable_deck: bool = True,
     pod_template: Optional["PodTemplate"] = None,
     pod_template_name: Optional[str] = None,
-) -> Union[Callable[[Callable[..., Any]], PythonFunctionTask[T]], PythonFunctionTask[T]]:
+) -> Union[Callable[[Callable[..., FuncOut]], PythonFunctionTask[T]], PythonFunctionTask[T], Callable[..., FuncOut]]:
     """
     This is the core decorator to use for any task type in flytekit.
 
     Tasks are the building blocks of Flyte. They represent users code. Tasks have the following properties
 
-    * Versioned (usually tied to the git sha)
+    * Versioned (usually tied to the git revision SHA1)
     * Strong interfaces (specified inputs and outputs)
     * Declarative
     * Independently executable
     * Unit testable
 
     For a simple python task,
```

### Comparing `flytekit-1.9.0a0/flytekit/core/testing.py` & `flytekit-1.9.1/flytekit/core/testing.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/tracker.py` & `flytekit-1.9.1/flytekit/core/tracker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,87 @@
 import importlib
-import importlib as _importlib
 import inspect
-import inspect as _inspect
 import os
+import sys
 import typing
+from pathlib import Path
 from types import ModuleType
-from typing import Callable, Tuple, Union
+from typing import Callable, Optional, Tuple, Union
 
 from flytekit.configuration.feature_flags import FeatureFlags
 from flytekit.exceptions import system as _system_exceptions
 from flytekit.loggers import logger
 
 
+def import_module_from_file(module_name, file):
+    try:
+        spec = importlib.util.spec_from_file_location(module_name, file)
+        module = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(module)
+        return module
+    except AssertionError:
+        # handle where we can't determine the module of functions within the module
+        return importlib.import_module(module_name)
+    except Exception as exc:
+        raise ModuleNotFoundError(f"Module from file {file} cannot be loaded") from exc
+
+
 class InstanceTrackingMeta(type):
     """
     Please see the original class :py:class`flytekit.common.mixins.registerable._InstanceTracker` also and also look
     at the tests in the ``tests/flytekit/unit/core/tracker/test_tracking/`` folder to see how it's used.
 
     Basically, this will make instances of classes that use this metaclass aware of the module (the .py file) that
     caused the instance to be created. This is useful because it means that we can then (at least try to) find the
     variable that the instance was assigned to.
     """
 
     @staticmethod
+    def _get_module_from_main(globals) -> Optional[str]:
+        curdir = Path.cwd()
+        file = globals.get("__file__")
+        if file is None:
+            return None
+
+        file = Path(file)
+        try:
+            file_relative = file.relative_to(curdir)
+        except ValueError:
+            return None
+
+        module_components = [*file_relative.with_suffix("").parts]
+        module_name = ".".join(module_components)
+        if len(module_components) == 0:
+            return None
+
+        # make sure current directory is in the PYTHONPATH.
+        sys.path.insert(0, str(curdir))
+        return import_module_from_file(module_name, file)
+
+    @staticmethod
     def _find_instance_module():
-        frame = _inspect.currentframe()
+        frame = inspect.currentframe()
         while frame:
             if frame.f_code.co_name == "<module>" and "__name__" in frame.f_globals:
-                return frame.f_globals["__name__"]
+                if frame.f_globals["__name__"] != "__main__":
+                    return frame.f_globals["__name__"], frame.f_globals["__file__"]
+                # if the remote_deploy command is invoked in the same module as where
+                # the app is defined, get the module from the file name
+                mod = InstanceTrackingMeta._get_module_from_main(frame.f_globals)
+                if mod is None:
+                    return None, None
+                return mod.__name__, mod.__file__
             frame = frame.f_back
-        return None
+        return None, None
 
     def __call__(cls, *args, **kwargs):
         o = super(InstanceTrackingMeta, cls).__call__(*args, **kwargs)
-        o._instantiated_in = InstanceTrackingMeta._find_instance_module()
+        mod_name, mod_file = InstanceTrackingMeta._find_instance_module()
+        o._instantiated_in = mod_name
+        o._module_file = mod_file
         return o
 
 
 class TrackedInstance(metaclass=InstanceTrackingMeta):
     """
     Please see the notes for the metaclass above first.
 
@@ -47,14 +91,15 @@
     * Task resolvers, because task resolvers are instances of :py:class:`flytekit.core.python_auto_container.TaskResolverMixin`
       classes, not the classes themselves, which means we need to look on the left hand side of them to see how to
       find them at task execution time.
     """
 
     def __init__(self, *args, **kwargs):
         self._instantiated_in = None
+        self._module_file = None
         self._lhs = None
         super().__init__(*args, **kwargs)
 
     @property
     def instantiated_in(self) -> str:
         return self._instantiated_in
 
@@ -73,29 +118,52 @@
         if self._lhs is not None:
             return self._lhs
 
         if self._instantiated_in is None or self._instantiated_in == "":
             raise _system_exceptions.FlyteSystemException(f"Object {self} does not have an _instantiated in")
 
         logger.debug(f"Looking for LHS for {self} from {self._instantiated_in}")
-        m = _importlib.import_module(self._instantiated_in)
+        m = importlib.import_module(self._instantiated_in)
         for k in dir(m):
             try:
                 if getattr(m, k) is self:
                     logger.debug(f"Found LHS for {self}, {k}")
                     self._lhs = k
                     return k
             except ValueError as err:
                 # Empty pandas dataframes behave weirdly here such that calling `m.df` raises:
                 # ValueError: The truth value of a {type(self).__name__} is ambiguous. Use a.empty, a.bool(), a.item(),
                 #   a.any() or a.all()
                 # Since dataframes aren't registrable entities to begin with we swallow any errors they raise and
                 # continue looping through m.
                 logger.warning("Caught ValueError {} while attempting to auto-assign name".format(err))
 
+        # try to find object in module when the tracked instance is defined in the __main__ module
+        module = import_module_from_file(self._instantiated_in, self._module_file)
+
+        def _candidate_name_matches(candidate) -> bool:
+            if not hasattr(candidate, "name") or not hasattr(self, "name"):
+                return False
+            return candidate.name == self.name
+
+        for k in dir(module):
+            try:
+                candidate = getattr(module, k)
+                # consider the variable equivalent to self if it's of the same type, name
+                if (
+                    type(candidate) == type(self)
+                    and _candidate_name_matches(candidate)
+                    and candidate.instantiated_in == self.instantiated_in
+                ):
+                    self._lhs = k
+                    return k
+            except ValueError as err:
+                logger.warning(f"Caught ValueError {err} while attempting to auto-assign name")
+                pass
+
         logger.error(f"Could not find LHS for {self} in {self._instantiated_in}")
         raise _system_exceptions.FlyteSystemException(f"Error looking for LHS in {self._instantiated_in}")
 
 
 def isnested(func: Callable) -> bool:
     """
     Returns true if a function is local to another function and is not accessible through a module
@@ -212,37 +280,43 @@
         """
         return self._resolve_abs_module_name(path, package_root)
 
 
 _mod_sanitizer = _ModuleSanitizer()
 
 
+def _task_module_from_callable(f: Callable):
+    mod = inspect.getmodule(f)
+    mod_name = getattr(mod, "__name__", f.__module__)
+    name = f.__name__.split(".")[-1]
+    return mod, mod_name, name
+
+
 def extract_task_module(f: Union[Callable, TrackedInstance]) -> Tuple[str, str, str, str]:
     """
     Returns the task-name, absolute module and the string name of the callable.
     :param f: A task or any other callable
     :return: [name to use: str, module_name: str, function_name: str, full_path: str]
     """
 
     if isinstance(f, TrackedInstance):
-        mod = importlib.import_module(f.instantiated_in)
-        mod_name = mod.__name__
-        name = f.lhs
-        # We cannot get the sourcefile for an instance, so we replace it with the module
-        g = mod
-        inspect_file = inspect.getfile(g)
+        if f.instantiated_in:
+            mod = importlib.import_module(f.instantiated_in)
+            mod_name = mod.__name__
+            name = f.lhs
+        elif hasattr(f, "task_function"):
+            mod, mod_name, name = _task_module_from_callable(f.task_function)
     else:
-        mod = inspect.getmodule(f)  # type: ignore
-        if mod is None:
-            raise AssertionError(f"Unable to determine module of {f}")
-        mod_name = mod.__name__
-        name = f.__name__.split(".")[-1]
-        inspect_file = inspect.getfile(f)
+        mod, mod_name, name = _task_module_from_callable(f)
+
+    if mod is None:
+        raise AssertionError(f"Unable to determine module of {f}")
 
     if mod_name == "__main__":
+        inspect_file = inspect.getfile(f)  # type: ignore
         return name, "", name, os.path.abspath(inspect_file)
 
     mod_name = get_full_module_path(mod, mod_name)
     return f"{mod_name}.{name}", mod_name, name, os.path.abspath(inspect.getfile(mod))
 
 
 def get_full_module_path(mod: ModuleType, mod_name: str) -> str:
```

### Comparing `flytekit-1.9.0a0/flytekit/core/type_engine.py` & `flytekit-1.9.1/flytekit/core/type_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import inspect
 import json as _json
 import mimetypes
 import textwrap
 import typing
 from abc import ABC, abstractmethod
 from functools import lru_cache
-from typing import Dict, NamedTuple, Optional, Type, cast
+from typing import Any, Dict, List, NamedTuple, Optional, Tuple, Type, cast
 
 from dataclasses_json import DataClassJsonMixin, dataclass_json
 from google.protobuf import json_format as _json_format
 from google.protobuf import struct_pb2 as _struct
 from google.protobuf.json_format import MessageToDict as _MessageToDict
 from google.protobuf.json_format import ParseDict as _ParseDict
 from google.protobuf.message import Message
@@ -51,14 +51,45 @@
 )
 from flytekit.models.types import LiteralType, SimpleType, StructuredDatasetType, TypeStructure, UnionType
 
 T = typing.TypeVar("T")
 DEFINITIONS = "definitions"
 
 
+class BatchSize:
+    """
+    This is used to annotate a FlyteDirectory when we want to download/upload the contents of the directory in batches. For example,
+
+    @task
+    def t1(directory: Annotated[FlyteDirectory, BatchSize(10)]) -> Annotated[FlyteDirectory, BatchSize(100)]:
+        ...
+        return FlyteDirectory(...)
+
+    In the above example flytekit will download all files from the input `directory` in chunks of 10, i.e. first it
+    downloads 10 files, loads them to memory, then writes those 10 to local disk, then it loads the next 10, so on
+    and so forth. Similarly, for outputs, in this case flytekit is going to upload the resulting directory in chunks of
+    100.
+    """
+
+    def __init__(self, val: int):
+        self._val = val
+
+    @property
+    def val(self) -> int:
+        return self._val
+
+
+def get_batch_size(t: Type) -> Optional[int]:
+    if is_annotated(t):
+        for annotation in get_args(t)[1:]:
+            if isinstance(annotation, BatchSize):
+                return annotation.val
+    return None
+
+
 class TypeTransformerFailedError(TypeError, AssertionError, ValueError):
     ...
 
 
 class TypeTransformer(typing.Generic[T]):
     """
     Base transformer type that should be implemented for every python native type that can be handled by flytekit
@@ -169,16 +200,15 @@
         if type(python_val) != self._type:
             raise TypeTransformerFailedError(
                 f"Expected value of type {self._type} but got '{python_val}' of type {type(python_val)}"
             )
         return self._to_literal_transformer(python_val)
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> T:
-        if get_origin(expected_python_type) is Annotated:
-            expected_python_type = get_args(expected_python_type)[0]
+        expected_python_type = get_underlying_type(expected_python_type)
 
         if expected_python_type != self._type:
             raise TypeTransformerFailedError(
                 f"Cannot convert to type {expected_python_type}, only {self._type} is supported"
             )
 
         try:  # todo(maximsmol): this is quite ugly and each transformer should really check their Literal
@@ -217,30 +247,28 @@
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> T:
         raise RestrictedTypeError(f"Transformer for type {self.python_type} is restricted currently")
 
 
 class DataclassTransformer(TypeTransformer[object]):
     """
-    The Dataclass Transformer, provides a type transformer for arbitrary Python dataclasses, that have
-    @dataclass and @dataclass_json decorators.
+    The Dataclass Transformer provides a type transformer for dataclasses_json dataclasses.
 
     The Dataclass is converted to and from json and is transported between tasks using the proto.Structpb representation
     Also the type declaration will try to extract the JSON Schema for the object if possible and pass it with the
     definition.
 
     For Json Schema, we use https://github.com/fuhrysteve/marshmallow-jsonschema library.
 
     Example
 
     .. code-block:: python
 
-        @dataclass_json
         @dataclass
-        class Test():
+        class Test(DataClassJsonMixin):
            a: int
            b: str
 
         from marshmallow_jsonschema import JSONSchema
         t = Test(a=10,b="e")
         JSONSchema().dump(t.schema())
 
@@ -267,17 +295,16 @@
         super().__init__("Object-Dataclass-Transformer", object)
 
     def assert_type(self, expected_type: Type[DataClassJsonMixin], v: T):
         # Skip iterating all attributes in the dataclass if the type of v already matches the expected_type
         if type(v) == expected_type:
             return
 
-        # @dataclass_json
         # @dataclass
-        # class Foo(object):
+        # class Foo(DataClassJsonMixin):
         #     a: int = 0
         #
         # @task
         # def t1(a: Foo):
         #     ...
         #
         # In above example, the type of v may not equal to the expected_type in some cases
@@ -307,23 +334,24 @@
                 raise TypeTransformerFailedError(f"Type of Val '{original_type}' is not an instance of {expected_type}")
 
     def get_literal_type(self, t: Type[T]) -> LiteralType:
         """
         Extracts the Literal type definition for a Dataclass and returns a type Struct.
         If possible also extracts the JSONSchema for the dataclass.
         """
-        if get_origin(t) is Annotated:
+        if is_annotated(t):
             raise ValueError(
                 "Flytekit does not currently have support for FlyteAnnotations applied to Dataclass."
                 f"Type {t} cannot be parsed."
             )
 
         if not issubclass(t, DataClassJsonMixin):
             raise AssertionError(
-                f"Dataclass {t} should be decorated with @dataclass_json to be " f"serialized correctly"
+                f"Dataclass {t} should be decorated with @dataclass_json or be a subclass of DataClassJsonMixin to be "
+                "serialized correctly"
             )
         schema = None
         try:
             s = cast(DataClassJsonMixin, self._get_origin_type_in_annotation(t)).schema()
             for _, v in s.fields.items():
                 # marshmallow-jsonschema only supports enums loaded by name.
                 # https://github.com/fuhrysteve/marshmallow-jsonschema/blob/81eada1a0c42ff67de216923968af0a6b54e5dcb/marshmallow_jsonschema/base.py#L228
@@ -346,15 +374,16 @@
         if not dataclasses.is_dataclass(python_val):
             raise TypeTransformerFailedError(
                 f"{type(python_val)} is not of type @dataclass, only Dataclasses are supported for "
                 f"user defined datatypes in Flytekit"
             )
         if not issubclass(type(python_val), DataClassJsonMixin):
             raise TypeTransformerFailedError(
-                f"Dataclass {python_type} should be decorated with @dataclass_json to be " f"serialized correctly"
+                f"Dataclass {python_type} should be decorated with @dataclass_json or be a subclass of "
+                "DataClassJsonMixin to be serialized correctly"
             )
         self._serialize_flyte_type(python_val, python_type)
         return Literal(
             scalar=Scalar(generic=_json_format.Parse(cast(DataClassJsonMixin, python_val).to_json(), _struct.Struct()))
         )
 
     def _get_origin_type_in_annotation(self, python_type: Type[T]) -> Type[T]:
@@ -364,15 +393,15 @@
         if get_origin(python_type) is list:
             return typing.List[self._get_origin_type_in_annotation(get_args(python_type)[0])]  # type: ignore
         elif get_origin(python_type) is dict:
             return typing.Dict[  # type: ignore
                 self._get_origin_type_in_annotation(get_args(python_type)[0]),
                 self._get_origin_type_in_annotation(get_args(python_type)[1]),
             ]
-        elif get_origin(python_type) is Annotated:
+        elif is_annotated(python_type):
             return get_args(python_type)[0]
         elif dataclasses.is_dataclass(python_type):
             for field in dataclasses.fields(copy.deepcopy(python_type)):
                 field.type = self._get_origin_type_in_annotation(field.type)
         return python_type
 
     def _fix_structured_dataset_type(self, python_type: Type[T], python_val: typing.Any) -> T:
@@ -426,18 +455,18 @@
         if inspect.isclass(python_type) and (
             issubclass(python_type, FlyteSchema)
             or issubclass(python_type, FlyteFile)
             or issubclass(python_type, FlyteDirectory)
             or issubclass(python_type, StructuredDataset)
         ):
             lv = TypeEngine.to_literal(FlyteContext.current_context(), python_val, python_type, None)
-            # dataclass_json package will extract the "path" from FlyteFile, FlyteDirectory, and write it to a
+            # dataclasses_json package will extract the "path" from FlyteFile, FlyteDirectory, and write it to a
             # JSON which will be stored in IDL. The path here should always be a remote path, but sometimes the
             # path in FlyteFile and FlyteDirectory could be a local path. Therefore, reset the python value here,
-            # so that dataclass_json can always get a remote path.
+            # so that dataclasses_json can always get a remote path.
             # In other words, the file transformer has special code that handles the fact that if remote_source is
             # set, then the real uri in the literal should be the remote source, not the path (which may be an
             # auto-generated random local path). To be sure we're writing the right path to the json, use the uri
             # as determined by the transformer.
             if issubclass(python_type, FlyteFile) or issubclass(python_type, FlyteDirectory):
                 return python_type(path=lv.scalar.blob.uri)
             elif issubclass(python_type, StructuredDataset):
@@ -593,20 +622,20 @@
             dc.__setattr__(f.name, self._fix_val_int(f.type, val))
         return dc
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> T:
         if not dataclasses.is_dataclass(expected_python_type):
             raise TypeTransformerFailedError(
                 f"{expected_python_type} is not of type @dataclass, only Dataclasses are supported for "
-                f"user defined datatypes in Flytekit"
+                "user defined datatypes in Flytekit"
             )
         if not issubclass(expected_python_type, DataClassJsonMixin):
             raise TypeTransformerFailedError(
-                f"Dataclass {expected_python_type} should be decorated with @dataclass_json to be "
-                f"serialized correctly"
+                f"Dataclass {expected_python_type} should be decorated with @dataclass_json or be a subclass of "
+                "DataClassJsonMixin to be serialized correctly"
             )
         json_str = _json_format.MessageToJson(lv.scalar.generic)
         dc = cast(DataClassJsonMixin, expected_python_type).from_json(json_str)
         dc = self._fix_structured_dataset_type(expected_python_type, dc)
         return self._fix_dataclass_int(expected_python_type, self._deserialize_flyte_type(dc, expected_python_type))
 
     # This ensures that calls with the same literal type returns the same dataclass. For example, `pyflyte run``
@@ -706,15 +735,15 @@
 
     @classmethod
     def register_additional_type(cls, transformer: TypeTransformer, additional_type: Type, override=False):
         if additional_type not in cls._REGISTRY or override:
             cls._REGISTRY[additional_type] = transformer
 
     @classmethod
-    def get_transformer(cls, python_type: Type[T]) -> TypeTransformer[T]:
+    def get_transformer(cls, python_type: Type) -> TypeTransformer[T]:
         """
         The TypeEngine hierarchy for flyteKit. This method looksup and selects the type transformer. The algorithm is
         as follows
 
           d = dictionary of registered transformers, where is a python `type`
           v = lookup type
         Step 1:
@@ -733,30 +762,30 @@
             TODO lets make this deterministic by using an ordered dict
 
         Step 5:
             if v is of type data class, use the dataclass transformer
         """
         cls.lazy_import_transformers()
         # Step 1
-        if get_origin(python_type) is Annotated:
+        if is_annotated(python_type):
             args = get_args(python_type)
             for annotation in args:
                 if isinstance(annotation, TypeTransformer):
                     return annotation
 
             python_type = args[0]
 
         if python_type in cls._REGISTRY:
             return cls._REGISTRY[python_type]
 
         # Step 2
         if hasattr(python_type, "__origin__"):
             # Handling of annotated generics, eg:
             # Annotated[typing.List[int], 'foo']
-            if get_origin(python_type) is Annotated:
+            if is_annotated(python_type):
                 return cls.get_transformer(get_args(python_type)[0])
 
             if python_type.__origin__ in cls._REGISTRY:
                 return cls._REGISTRY[python_type.__origin__]
 
             raise ValueError(f"Generic Type {python_type.__origin__} not supported currently in Flytekit.")
 
@@ -776,15 +805,19 @@
                 # is the case for one of the restricted types, namely NamedTuple.
                 logger.debug(f"Invalid base type {base_type} in call to isinstance", exc_info=True)
 
         # Step 4
         if dataclasses.is_dataclass(python_type):
             return cls._DATACLASS_TRANSFORMER
 
-        raise ValueError(f"Type {python_type} not supported currently in Flytekit. Please register a new transformer")
+        # Step 5
+        display_pickle_warning(str(python_type))
+        from flytekit.types.pickle.pickle import FlytePickleTransformer
+
+        return FlytePickleTransformer()
 
     @classmethod
     def lazy_import_transformers(cls):
         """
         Only load the transformers if needed.
         """
         if cls.has_lazy_import:
@@ -819,15 +852,15 @@
     def to_literal_type(cls, python_type: Type) -> LiteralType:
         """
         Converts a python type into a flyte specific ``LiteralType``
         """
         transformer = cls.get_transformer(python_type)
         res = transformer.get_literal_type(python_type)
         data = None
-        if get_origin(python_type) is Annotated:
+        if is_annotated(python_type):
             for x in get_args(python_type)[1:]:
                 if not isinstance(x, FlyteAnnotation):
                     continue
                 if data is not None:
                     raise ValueError(
                         f"More than one FlyteAnnotation used within {python_type} typehint. Flytekit requires a max of one."
                     )
@@ -839,25 +872,41 @@
         return res
 
     @classmethod
     def to_literal(cls, ctx: FlyteContext, python_val: typing.Any, python_type: Type, expected: LiteralType) -> Literal:
         """
         Converts a python value of a given type and expected ``LiteralType`` into a resolved ``Literal`` value.
         """
+        from flytekit.core.promise import Promise, VoidPromise
+
+        if isinstance(python_val, Promise):
+            # In the example above, this handles the "in2=a" type of argument
+            return python_val.val
+        if isinstance(python_val, VoidPromise):
+            raise AssertionError(
+                f"Outputs of a non-output producing task {python_val.task_name} cannot be passed to another task."
+            )
+        if isinstance(python_val, tuple):
+            raise AssertionError(
+                "Tuples are not a supported type for individual values in Flyte - got a tuple -"
+                f" {python_val}. If using named tuple in an inner task, please, de-reference the"
+                "actual attribute that you want to use. For example, in NamedTuple('OP', x=int) then"
+                "return v.x, instead of v, even if this has a single element"
+            )
         if python_val is None and expected.union_type is None:
             raise TypeTransformerFailedError(f"Python value cannot be None, expected {python_type}/{expected}")
         transformer = cls.get_transformer(python_type)
         if transformer.type_assertions_enabled:
             transformer.assert_type(python_type, python_val)
 
         # In case the value is an annotated type we inspect the annotations and look for hash-related annotations.
         hash = None
-        if get_origin(python_type) is Annotated:
+        if is_annotated(python_type):
             # We are now dealing with one of two cases:
-            # 1. The annotated type is a `HashMethod`, which indicates that we should we should produce the hash using
+            # 1. The annotated type is a `HashMethod`, which indicates that we should produce the hash using
             #    the method indicated in the annotation.
             # 2. The annotated type is being used for a different purpose other than calculating hash values, in which case
             #    we should just continue.
             for annotation in get_args(python_type)[1:]:
                 if not isinstance(annotation, HashMethod):
                     continue
                 hash = annotation.calculate(python_val)
@@ -876,15 +925,15 @@
         """
         transformer = cls.get_transformer(expected_python_type)
         return transformer.to_python_value(ctx, lv, expected_python_type)
 
     @classmethod
     def to_html(cls, ctx: FlyteContext, python_val: typing.Any, expected_python_type: Type[typing.Any]) -> str:
         transformer = cls.get_transformer(expected_python_type)
-        if get_origin(expected_python_type) is Annotated:
+        if is_annotated(expected_python_type):
             expected_python_type, *annotate_args = get_args(expected_python_type)
             from flytekit.deck.renderer import Renderable
 
             for arg in annotate_args:
                 if isinstance(arg, Renderable):
                     return arg.to_html(python_val)
         return transformer.to_html(ctx, python_val, expected_python_type)
@@ -1000,15 +1049,15 @@
     def get_sub_type(t: Type[T]) -> Type[T]:
         """
         Return the generic Type T of the List
         """
         if hasattr(t, "__origin__"):
             # Handle annotation on list generic, eg:
             # Annotated[typing.List[int], 'foo']
-            if get_origin(t) is Annotated:
+            if is_annotated(t):
                 return ListTransformer.get_sub_type(get_args(t)[0])
 
             if getattr(t, "__origin__") is list and hasattr(t, "__args__"):
                 return getattr(t, "__args__")[0]
 
         raise ValueError("Only generic univariate typing.List[T] type is supported.")
 
@@ -1026,15 +1075,15 @@
     def is_batchable(t: Type):
         """
         This function evaluates whether the provided type is batchable or not.
         It returns True only if the type is either List or Annotated(List) and the List subtype is FlytePickle.
         """
         from flytekit.types.pickle import FlytePickle
 
-        if get_origin(t) is Annotated:
+        if is_annotated(t):
             return ListTransformer.is_batchable(get_args(t)[0])
         if get_origin(t) is list:
             subtype = get_args(t)[0]
             if subtype == FlytePickle or (hasattr(subtype, "__origin__") and subtype.__origin__ == FlytePickle):
                 return True
         return False
 
@@ -1043,15 +1092,15 @@
             raise TypeTransformerFailedError("Expected a list")
 
         if ListTransformer.is_batchable(python_type):
             from flytekit.types.pickle.pickle import BatchSize, FlytePickle
 
             batch_size = len(python_val)  # default batch size
             # parse annotated to get the number of items saved in a pickle file.
-            if get_origin(python_type) is Annotated:
+            if is_annotated(python_type):
                 for annotation in get_args(python_type)[1:]:
                     if isinstance(annotation, BatchSize):
                         batch_size = annotation.val
                         break
             if batch_size > 0:
                 lit_list = [TypeEngine.to_literal(ctx, python_val[i : i + batch_size], FlytePickle, expected.collection_type) for i in range(0, len(python_val), batch_size)]  # type: ignore
             else:
@@ -1082,14 +1131,24 @@
     def guess_python_type(self, literal_type: LiteralType) -> list:  # type: ignore
         if literal_type.collection_type:
             ct: Type = TypeEngine.guess_python_type(literal_type.collection_type)
             return typing.List[ct]  # type: ignore
         raise ValueError(f"List transformer cannot reverse {literal_type}")
 
 
+@lru_cache
+def display_pickle_warning(python_type: str):
+    # This is a warning that is only displayed once per python type
+    logger.warning(
+        f"Unsupported Type {python_type} found, Flyte will default to use PickleFile as the transport. "
+        f"Pickle can only be used to send objects between the exact same version of Python, "
+        f"and we strongly recommend to use python type that flyte support."
+    )
+
+
 def _add_tag_to_type(x: LiteralType, tag: str) -> LiteralType:
     x._structure = TypeStructure(tag=tag)
     return x
 
 
 def _type_essence(x: LiteralType) -> LiteralType:
     if x.metadata is not None or x.structure is not None or x.annotation is not None:
@@ -1187,40 +1246,38 @@
     def get_sub_type_in_optional(t: Type[T]) -> Type[T]:
         """
         Return the generic Type T of the Optional type
         """
         return get_args(t)[0]
 
     def get_literal_type(self, t: Type[T]) -> Optional[LiteralType]:
-        if get_origin(t) is Annotated:
-            t = get_args(t)[0]
+        t = get_underlying_type(t)
 
         try:
             trans: typing.List[typing.Tuple[TypeTransformer, typing.Any]] = [
                 (TypeEngine.get_transformer(x), x) for x in get_args(t)
             ]
             # must go through TypeEngine.to_literal_type instead of trans.get_literal_type
             # to handle Annotated
             variants = [_add_tag_to_type(TypeEngine.to_literal_type(x), t.name) for (t, x) in trans]
             return _type_models.LiteralType(union_type=UnionType(variants))
         except Exception as e:
             raise ValueError(f"Type of Generic Union type is not supported, {e}")
 
     def to_literal(self, ctx: FlyteContext, python_val: T, python_type: Type[T], expected: LiteralType) -> Literal:
-        if get_origin(python_type) is Annotated:
-            python_type = get_args(python_type)[0]
+        python_type = get_underlying_type(python_type)
 
         found_res = False
         res = None
         res_type = None
-        for t in get_args(python_type):
+        for i in range(len(get_args(python_type))):
             try:
+                t = get_args(python_type)[i]
                 trans: TypeTransformer[T] = TypeEngine.get_transformer(t)
-
-                res = trans.to_literal(ctx, python_val, t, expected)
+                res = trans.to_literal(ctx, python_val, t, expected.union_type.variants[i])
                 res_type = _add_tag_to_type(trans.get_literal_type(t), trans.name)
                 if found_res:
                     # Should really never happen, sanity check
                     raise TypeError("Ambiguous choice of variant for union type")
                 found_res = True
             except (TypeTransformerFailedError, AttributeError, ValueError, AssertionError) as e:
                 logger.debug(f"Failed to convert from {python_val} to {t}", e)
@@ -1228,16 +1285,15 @@
 
         if found_res:
             return Literal(scalar=Scalar(union=Union(value=res, stored_type=res_type)))
 
         raise TypeTransformerFailedError(f"Cannot convert from {python_val} to {python_type}")
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> Optional[typing.Any]:
-        if get_origin(expected_python_type) is Annotated:
-            expected_python_type = get_args(expected_python_type)[0]
+        expected_python_type = get_underlying_type(expected_python_type)
 
         union_tag = None
         union_type = None
         if lv.scalar is not None and lv.scalar.union is not None:
             union_type = lv.scalar.union.stored_type
             if union_type.structure is not None:
                 union_tag = union_type.structure.tag
@@ -1464,15 +1520,15 @@
     Enables converting a python type enum.Enum to LiteralType.EnumType
     """
 
     def __init__(self):
         super().__init__(name="DefaultEnumTransformer", t=enum.Enum)
 
     def get_literal_type(self, t: Type[T]) -> LiteralType:
-        if get_origin(t) is Annotated:
+        if is_annotated(t):
             raise ValueError(
                 f"Flytekit does not currently have support \
                     for FlyteAnnotations applied to enums. {t} cannot be \
                     parsed."
             )
 
         values = [v.value for v in t]  # type: ignore
@@ -1490,40 +1546,40 @@
 
         return Literal(scalar=Scalar(primitive=Primitive(string_value=python_val.value)))  # type: ignore
 
     def to_python_value(self, ctx: FlyteContext, lv: Literal, expected_python_type: Type[T]) -> T:
         return expected_python_type(lv.scalar.primitive.string_value)  # type: ignore
 
 
-def convert_json_schema_to_python_class(schema: dict, schema_name) -> Type[dataclasses.dataclass()]:  # type: ignore
+def convert_json_schema_to_python_class(schema: Dict[str, Any], schema_name: str) -> Type[Any]:
     """
     Generate a model class based on the provided JSON Schema
     :param schema: dict representing valid JSON schema
     :param schema_name: dataclass name of return type
     """
-    attribute_list = []
+    attribute_list: List[Tuple[str, type]] = []
     for property_key, property_val in schema[schema_name]["properties"].items():
         property_type = property_val["type"]
         # Handle list
         if property_val["type"] == "array":
-            attribute_list.append((property_key, typing.List[_get_element_type(property_val["items"])]))  # type: ignore
+            attribute_list.append((property_key, List[_get_element_type(property_val["items"])]))  # type: ignore[misc,index]
         # Handle dataclass and dict
         elif property_type == "object":
             if property_val.get("$ref"):
                 name = property_val["$ref"].split("/")[-1]
                 attribute_list.append((property_key, convert_json_schema_to_python_class(schema, name)))
             elif property_val.get("additionalProperties"):
                 attribute_list.append(
-                    (property_key, typing.Dict[str, _get_element_type(property_val["additionalProperties"])])  # type: ignore
+                    (property_key, Dict[str, _get_element_type(property_val["additionalProperties"])])  # type: ignore[misc,index]
                 )
             else:
-                attribute_list.append((property_key, typing.Dict[str, _get_element_type(property_val)]))  # type: ignore
+                attribute_list.append((property_key, Dict[str, _get_element_type(property_val)]))  # type: ignore[misc,index]
         # Handle int, float, bool or str
         else:
-            attribute_list.append([property_key, _get_element_type(property_val)])  # type: ignore
+            attribute_list.append((property_key, _get_element_type(property_val)))
 
     return dataclass_json(dataclasses.make_dataclass(schema_name, attribute_list))
 
 
 def _get_element_type(element_property: typing.Dict[str, str]) -> Type:
     element_type = element_property["type"]
     element_format = element_property["format"] if "format" in element_property else None
@@ -1635,14 +1691,26 @@
             lambda x: Literal(scalar=Scalar(primitive=Primitive(duration=x))),
             lambda x: x.scalar.primitive.duration,
         )
     )
 
     TypeEngine.register(
         SimpleTransformer(
+            "date",
+            _datetime.date,
+            _type_models.LiteralType(simple=_type_models.SimpleType.DATETIME),
+            lambda x: Literal(
+                scalar=Scalar(primitive=Primitive(datetime=_datetime.datetime.combine(x, _datetime.time.min)))
+            ),  # convert datetime to date
+            lambda x: x.scalar.primitive.datetime.date(),  # get date from datetime
+        )
+    )
+
+    TypeEngine.register(
+        SimpleTransformer(
             "none",
             type(None),
             _type_models.LiteralType(simple=_type_models.SimpleType.NONE),
             lambda x: Literal(scalar=Scalar(none_type=Void())),
             lambda x: _check_and_convert_void(x),
         ),
         [None],
@@ -1778,7 +1846,18 @@
             self._ctx or FlyteContext.current_context(), self._literals[attr], cast(Type, as_type)
         )
         self._native_values[attr] = val
         return val
 
 
 _register_default_type_transformers()
+
+
+def is_annotated(t: Type) -> bool:
+    return get_origin(t) is Annotated
+
+
+def get_underlying_type(t: Type) -> Type:
+    """Return the underlying type for annotated types or the type itself"""
+    if is_annotated(t):
+        return get_args(t)[0]
+    return t
```

### Comparing `flytekit-1.9.0a0/flytekit/core/type_helpers.py` & `flytekit-1.9.1/flytekit/core/type_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/utils.py` & `flytekit-1.9.1/flytekit/core/utils.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/core/workflow.py` & `flytekit-1.9.1/flytekit/core/workflow.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from __future__ import annotations
 
+import asyncio
+import inspect
 import typing
 from dataclasses import dataclass
 from enum import Enum
 from functools import update_wrapper
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, Union, cast, overload
-
-from typing_extensions import get_args
+from typing import Any, Callable, Coroutine, Dict, List, Optional, Tuple, Type, Union, cast, overload
 
 from flytekit.core import constants as _common_constants
 from flytekit.core.base_task import PythonTask
 from flytekit.core.class_based_resolver import ClassStorageTaskResolver
 from flytekit.core.condition import ConditionalSection
-from flytekit.core.context_manager import CompilationState, FlyteContext, FlyteContextManager, FlyteEntities
+from flytekit.core.context_manager import (
+    CompilationState,
+    ExecutionState,
+    FlyteContext,
+    FlyteContextManager,
+    FlyteEntities,
+)
 from flytekit.core.docstring import Docstring
 from flytekit.core.interface import (
     Interface,
     transform_function_to_interface,
     transform_inputs_to_parameters,
     transform_interface_to_typed_interface,
 )
@@ -31,34 +37,33 @@
     extract_obj_name,
     flyte_entity_call_handler,
     translate_inputs_to_literals,
 )
 from flytekit.core.python_auto_container import PythonAutoContainerTask
 from flytekit.core.reference_entity import ReferenceEntity, WorkflowReference
 from flytekit.core.tracker import extract_task_module
-from flytekit.core.type_engine import TypeEngine, TypeTransformerFailedError, UnionTransformer
+from flytekit.core.type_engine import TypeEngine
 from flytekit.exceptions import scopes as exception_scopes
 from flytekit.exceptions.user import FlyteValidationException, FlyteValueException
 from flytekit.loggers import logger
 from flytekit.models import interface as _interface_models
 from flytekit.models import literals as _literal_models
-from flytekit.models import types as type_models
 from flytekit.models.core import workflow as _workflow_model
 from flytekit.models.documentation import Description, Documentation
-from flytekit.models.types import TypeStructure
 
 GLOBAL_START_NODE = Node(
     id=_common_constants.GLOBAL_INPUT_NODE_ID,
     metadata=None,
     bindings=[],
     upstream_nodes=[],
     flyte_entity=None,
 )
 
 T = typing.TypeVar("T")
+FuncOut = typing.TypeVar("FuncOut")
 
 
 class WorkflowFailurePolicy(Enum):
     """
     Defines the behavior for a workflow execution in the case of an observed node execution failure. By default, a
     workflow execution will immediately enter a failed state if a component node fails.
     """
@@ -255,15 +260,15 @@
 
     def construct_node_metadata(self) -> _workflow_model.NodeMetadata:
         return _workflow_model.NodeMetadata(
             name=extract_obj_name(self.name),
             interruptible=self.workflow_metadata_defaults.interruptible,
         )
 
-    def __call__(self, *args, **kwargs) -> Union[Tuple[Promise], Promise, VoidPromise, Tuple, None]:
+    def __call__(self, *args, **kwargs) -> Union[Tuple[Promise], Promise, VoidPromise, Tuple, Coroutine, None]:
         """
         Workflow needs to fill in default arguments before invoking the call handler.
         """
         # Get default arguments and override with kwargs passed in
         input_kwargs = self.python_interface.default_inputs_as_kwargs
         input_kwargs.update(kwargs)
         self.compile()
@@ -275,71 +280,31 @@
 
     def execute(self, **kwargs):
         raise Exception("Should not be called")
 
     def compile(self, **kwargs):
         pass
 
-    def ensure_literal(
-        self, ctx, py_type: Type[T], input_type: type_models.LiteralType, python_value: Any
-    ) -> _literal_models.Literal:
-        """
-        This function will attempt to convert a python value to a literal. If the python value is a promise, it will
-        return the promise's value.
-        """
-        if input_type.union_type is not None:
-            if python_value is None and UnionTransformer.is_optional_type(py_type):
-                return _literal_models.Literal(scalar=_literal_models.Scalar(none_type=_literal_models.Void()))
-            for i in range(len(input_type.union_type.variants)):
-                lt_type = input_type.union_type.variants[i]
-                python_type = get_args(py_type)[i]
-                try:
-                    final_lt = self.ensure_literal(ctx, python_type, lt_type, python_value)
-                    lt_type._structure = TypeStructure(tag=TypeEngine.get_transformer(python_type).name)
-                    return _literal_models.Literal(
-                        scalar=_literal_models.Scalar(union=_literal_models.Union(value=final_lt, stored_type=lt_type))
-                    )
-                except Exception as e:
-                    logger.debug(f"Failed to convert {python_value} to {lt_type} with error {e}")
-            raise TypeError(f"Failed to convert {python_value} to {input_type}")
-        if isinstance(python_value, list) and input_type.collection_type:
-            collection_lit_type = input_type.collection_type
-            collection_py_type = get_args(py_type)[0]
-            xx = [self.ensure_literal(ctx, collection_py_type, collection_lit_type, pv) for pv in python_value]
-            return _literal_models.Literal(collection=_literal_models.LiteralCollection(literals=xx))
-        elif isinstance(python_value, dict) and input_type.map_value_type:
-            mapped_lit_type = input_type.map_value_type
-            mapped_py_type = get_args(py_type)[1]
-            xx = {k: self.ensure_literal(ctx, mapped_py_type, mapped_lit_type, v) for k, v in python_value.items()}  # type: ignore
-            return _literal_models.Literal(map=_literal_models.LiteralMap(literals=xx))
-        # It is a scalar, convert to Promise if necessary.
-        else:
-            if isinstance(python_value, Promise):
-                return python_value.val
-            if not isinstance(python_value, Promise):
-                try:
-                    res = TypeEngine.to_literal(ctx, python_value, py_type, input_type)
-                    return res
-                except TypeTransformerFailedError as exc:
-                    raise TypeError(
-                        f"Failed to convert input '{python_value}' of workflow '{self.name}':\n  {exc}"
-                    ) from exc
-
     def local_execute(self, ctx: FlyteContext, **kwargs) -> Union[Tuple[Promise], Promise, VoidPromise, None]:
         # This is done to support the invariant that Workflow local executions always work with Promise objects
         # holding Flyte literal values. Even in a wf, a user can call a sub-workflow with a Python native value.
-        for k, v in kwargs.items():
-            py_type = self.python_interface.inputs[k]
-            lit_type = self.interface.inputs[k].type
-            kwargs[k] = Promise(var=k, val=self.ensure_literal(ctx, py_type, lit_type, v))
-
-            # The output of this will always be a combination of Python native values and Promises containing Flyte
-            # Literals.
+        literal_map = translate_inputs_to_literals(
+            ctx,
+            incoming_values=kwargs,
+            flyte_interface_types=self.interface.inputs,
+            native_types=self.python_interface.inputs,
+        )
+        kwargs_literals = {k: Promise(var=k, val=v) for k, v in literal_map.items()}
         self.compile()
-        function_outputs = self.execute(**kwargs)
+        function_outputs = self.execute(**kwargs_literals)
+
+        if inspect.iscoroutine(function_outputs):
+            # handle coroutines for eager workflows
+            function_outputs = asyncio.run(function_outputs)
+
         # First handle the empty return case.
         # A workflow function may return a task that doesn't return anything
         #   def wf():
         #       return t1()
         # or it may not return at all
         #   def wf():
         #       t1()
@@ -378,14 +343,18 @@
             native_types=self.python_interface.outputs,
         )
         # Recreate new promises that use the workflow's output names.
         new_promises = [Promise(var, wf_outputs_as_literal_dict[var]) for var in expected_output_names]
 
         return create_task_output(new_promises, self.python_interface)
 
+    def local_execution_mode(self) -> ExecutionState.Mode:
+        """ """
+        return ExecutionState.Mode.LOCAL_WORKFLOW_EXECUTION
+
 
 class ImperativeWorkflow(WorkflowBase):
     """
     An imperative workflow is a programmatic analogue to the typical ``@workflow`` function-based workflow and is
     better suited to programmatic applications.
 
     Assuming you have some tasks like so
@@ -606,15 +575,15 @@
 
         flyte_type = TypeEngine.to_literal_type(python_type=python_type)
 
         ctx = FlyteContext.current_context()
         if ctx.compilation_state is not None:
             raise Exception("Can't already be compiling")
         with FlyteContextManager.with_context(ctx.with_compilation_state(self.compilation_state)) as ctx:
-            b = binding_from_python_std(
+            b, _ = binding_from_python_std(
                 ctx, output_name, expected_literal_type=flyte_type, t_value=p, t_value_type=python_type
             )
             self._output_bindings.append(b)
             self._python_interface = self._python_interface.with_outputs(extra_outputs={output_name: python_type})
             self._interface = transform_interface_to_typed_interface(self._python_interface)
 
     def add_task(self, task: PythonTask, **kwargs) -> Node:
@@ -729,15 +698,15 @@
                     )
                 if self.python_interface.output_tuple_name is None:
                     raise AssertionError(
                         "Outputs specification for Workflow does not define a tuple, but return value is a tuple"
                     )
                 workflow_outputs = workflow_outputs[0]
             t = self.python_interface.outputs[output_names[0]]
-            b = binding_from_python_std(
+            b, _ = binding_from_python_std(
                 ctx,
                 output_names[0],
                 self.interface.outputs[output_names[0]].type,
                 workflow_outputs,
                 t,
             )
             bindings.append(b)
@@ -746,15 +715,15 @@
                 raise AssertionError("The Workflow specification indicates multiple return values, received only one")
             if len(output_names) != len(workflow_outputs):
                 raise Exception(f"Length mismatch {len(output_names)} vs {len(workflow_outputs)}")
             for i, out in enumerate(output_names):
                 if isinstance(workflow_outputs[i], ConditionalSection):
                     raise AssertionError("A Conditional block (if-else) should always end with an `else_()` clause")
                 t = self.python_interface.outputs[out]
-                b = binding_from_python_std(
+                b, _ = binding_from_python_std(
                     ctx,
                     out,
                     self.interface.outputs[out].type,
                     workflow_outputs[i],
                     t,
                 )
                 bindings.append(b)
@@ -779,34 +748,34 @@
 
 @overload
 def workflow(
     _workflow_function: None = ...,
     failure_policy: Optional[WorkflowFailurePolicy] = ...,
     interruptible: bool = ...,
     docs: Optional[Documentation] = ...,
-) -> Callable[[Callable[..., Any]], PythonFunctionWorkflow]:
+) -> Callable[[Callable[..., FuncOut]], PythonFunctionWorkflow]:
     ...
 
 
 @overload
 def workflow(
-    _workflow_function: Callable[..., Any],
+    _workflow_function: Callable[..., FuncOut],
     failure_policy: Optional[WorkflowFailurePolicy] = ...,
     interruptible: bool = ...,
     docs: Optional[Documentation] = ...,
-) -> PythonFunctionWorkflow:
+) -> Union[PythonFunctionWorkflow, Callable[..., FuncOut]]:
     ...
 
 
 def workflow(
     _workflow_function: Optional[Callable[..., Any]] = None,
     failure_policy: Optional[WorkflowFailurePolicy] = None,
     interruptible: bool = False,
     docs: Optional[Documentation] = None,
-) -> Union[Callable[[Callable[..., Any]], PythonFunctionWorkflow], PythonFunctionWorkflow]:
+) -> Union[Callable[[Callable[..., FuncOut]], PythonFunctionWorkflow], PythonFunctionWorkflow, Callable[..., FuncOut]]:
     """
     This decorator declares a function to be a Flyte workflow. Workflows are declarative entities that construct a DAG
     of tasks using the data flow between tasks.
 
     Unlike a task, the function body of a workflow is evaluated at serialization-time (aka compile-time). This is
     because while we can determine the entire structure of a task by looking at the function's signature, workflows need
     to run through the function itself because the body of the function is what expresses the workflow structure. It's
```

### Comparing `flytekit-1.9.0a0/flytekit/deck/deck.py` & `flytekit-1.9.1/flytekit/deck/deck.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     MarkdownRenderer can convert Markdown string to HTML
 
     Flyte context saves a list of deck objects, and we use renderers in those decks to render
     the data and create an HTML file when those tasks are executed
 
     Each task has a least three decks (input, output, default). Input/output decks are
     used to render tasks' input/output data, and the default deck is used to render line plots,
-    scatter plots or markdown text. In addition, users can create new decks to render
+    scatter plots or Markdown text. In addition, users can create new decks to render
     their data with custom renderers.
 
     .. warning::
 
         This feature is in beta.
 
     .. code-block:: python
@@ -51,15 +51,14 @@
         def t2() -> Annotated[pd.DataFrame, TopFrameRenderer(10)]:
             return iris_df
 
     """
 
     def __init__(self, name: str, html: Optional[str] = ""):
         self._name = name
-        # self.renderers = renderers if isinstance(renderers, list) else [renderers]
         self._html = html
         FlyteContextManager.current_context().user_space_params.decks.append(self)
 
     def append(self, html: str) -> "Deck":
         assert isinstance(html, str)
         self._html = self._html + "\n" + html
         return self
@@ -111,20 +110,18 @@
                 <li>For accurate execution time measurements, users should refer to wall time and process time.</li>
             </ol>
         """
         # set the accuracy to microsecond
         df["ProcessTime"] = df["ProcessTime"].apply(lambda time: "{:.6f}".format(time))
         df["WallTime"] = df["WallTime"].apply(lambda time: "{:.6f}".format(time))
 
-        width = 1400
-        gantt_chart_html = GanttChartRenderer().to_html(df, chart_width=width)
+        gantt_chart_html = GanttChartRenderer().to_html(df)
         time_table_html = TableRenderer().to_html(
             df[["Name", "WallTime", "ProcessTime"]],
             header_labels=["Name", "Wall Time(s)", "Process Time(s)"],
-            table_width=width,
         )
         return gantt_chart_html + time_table_html + note
 
 
 def _get_deck(
     new_user_params: ExecutionParameters, ignore_jupyter: bool = False
 ) -> typing.Union[str, "IPython.core.display.HTML"]:  # type:ignore
@@ -141,22 +138,30 @@
             ...
         return HTML(raw_html)
     return raw_html
 
 
 def _output_deck(task_name: str, new_user_params: ExecutionParameters):
     ctx = FlyteContext.current_context()
-    if ctx.execution_state.mode == ExecutionState.Mode.TASK_EXECUTION:
-        output_dir = ctx.execution_state.engine_dir
-    else:
-        output_dir = ctx.file_access.get_random_local_directory()
-    deck_path = os.path.join(output_dir, DECK_FILE_NAME)
-    with open(deck_path, "w") as f:
-        f.write(_get_deck(new_user_params, ignore_jupyter=True))
-    logger.info(f"{task_name} task creates flyte deck html to file://{deck_path}")
+    local_dir = ctx.file_access.get_random_local_directory()
+    local_path = f"{local_dir}{os.sep}{DECK_FILE_NAME}"
+    try:
+        with open(local_path, "w", encoding="utf-8") as f:
+            f.write(_get_deck(new_user_params, ignore_jupyter=True))
+        logger.info(f"{task_name} task creates flyte deck html to file://{local_path}")
+        if ctx.execution_state.mode == ExecutionState.Mode.TASK_EXECUTION:
+            fs = ctx.file_access.get_filesystem_for_path(new_user_params.output_metadata_prefix)
+            remote_path = f"{new_user_params.output_metadata_prefix}{ctx.file_access.sep(fs)}{DECK_FILE_NAME}"
+            kwargs: typing.Dict[str, str] = {
+                "ContentType": "text/html",  # For s3
+                "content_type": "text/html",  # For gcs
+            }
+            ctx.file_access.put_data(local_path, remote_path, **kwargs)
+    except Exception as e:
+        logger.error(f"Failed to write flyte deck html with error {e}.")
 
 
 def get_deck_template() -> "Template":
     from jinja2 import Environment, FileSystemLoader, select_autoescape
 
     root = os.path.dirname(os.path.abspath(__file__))
     templates_dir = os.path.join(root, "html")
```

### Comparing `flytekit-1.9.0a0/flytekit/deck/html/template.html` & `flytekit-1.9.1/flytekit/deck/html/template.html`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/deck/renderer.py` & `flytekit-1.9.1/flytekit/deck/renderer.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/exceptions/scopes.py` & `flytekit-1.9.1/flytekit/exceptions/scopes.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/exceptions/system.py` & `flytekit-1.9.1/flytekit/exceptions/system.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/exceptions/user.py` & `flytekit-1.9.1/flytekit/exceptions/user.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/extend/__init__.py` & `flytekit-1.9.1/flytekit/extend/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/extras/cloud_pickle_resolver.py` & `flytekit-1.9.1/flytekit/extras/cloud_pickle_resolver.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/extras/pytorch/__init__.py` & `flytekit-1.9.1/flytekit/extras/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/extras/pytorch/checkpoint.py` & `flytekit-1.9.1/flytekit/extras/pytorch/checkpoint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 import typing
 from dataclasses import asdict, dataclass, fields, is_dataclass
 from typing import Any, Callable, Dict, NamedTuple, Optional, Type, Union
 
 import torch
-from dataclasses_json import dataclass_json
+from dataclasses_json import DataClassJsonMixin
 from typing_extensions import Protocol
 
 from flytekit.core.context_manager import FlyteContext
 from flytekit.core.type_engine import TypeEngine, TypeTransformer, TypeTransformerFailedError
 from flytekit.models.core import types as _core_types
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
@@ -16,17 +16,16 @@
 
 class IsDataclass(Protocol):
     __dataclass_fields__: Dict
     __dataclass_params__: Dict
     __post_init__: Optional[Callable]
 
 
-@dataclass_json
 @dataclass
-class PyTorchCheckpoint:
+class PyTorchCheckpoint(DataClassJsonMixin):
     """
     This class is helpful to save a checkpoint.
     """
 
     module: Optional[torch.nn.Module] = None
     hyperparameters: Optional[Union[Dict[str, Any], NamedTuple, IsDataclass]] = None
     optimizer: Optional[torch.optim.Optimizer] = None
```

### Comparing `flytekit-1.9.0a0/flytekit/extras/pytorch/native.py` & `flytekit-1.9.1/flytekit/extras/pytorch/native.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/extras/sklearn/__init__.py` & `flytekit-1.9.1/flytekit/extras/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/extras/sklearn/native.py` & `flytekit-1.9.1/flytekit/extras/sklearn/native.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import pathlib
-from typing import Generic, Type, TypeVar
+from typing import Type, TypeVar
 
 import joblib
 import sklearn
 
 from flytekit.core.context_manager import FlyteContext
 from flytekit.core.type_engine import TypeEngine, TypeTransformer, TypeTransformerFailedError
 from flytekit.models.core import types as _core_types
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
 
 T = TypeVar("T")
 
 
-class SklearnTypeTransformer(TypeTransformer, Generic[T]):
+class SklearnTypeTransformer(TypeTransformer[T]):
     def get_literal_type(self, t: Type[T]) -> LiteralType:
         return LiteralType(
             blob=_core_types.BlobType(
                 format=self.SKLEARN_FORMAT,
                 dimensionality=_core_types.BlobType.BlobDimensionality.SINGLE,
             )
         )
@@ -71,9 +71,19 @@
 
 class SklearnEstimatorTransformer(SklearnTypeTransformer[sklearn.base.BaseEstimator]):
     SKLEARN_FORMAT = "SklearnEstimator"
 
     def __init__(self):
         super().__init__(name="Sklearn Estimator", t=sklearn.base.BaseEstimator)
 
+    def guess_python_type(self, literal_type: LiteralType) -> Type[sklearn.base.BaseEstimator]:
+        if (
+            literal_type.blob is not None
+            and literal_type.blob.dimensionality == _core_types.BlobType.BlobDimensionality.SINGLE
+            and literal_type.blob.format == self.SKLEARN_FORMAT
+        ):
+            return sklearn.base.BaseEstimator
+
+        raise ValueError(f"Transformer {self} cannot reverse {literal_type}")
+
 
 TypeEngine.register(SklearnEstimatorTransformer())
```

### Comparing `flytekit-1.9.0a0/flytekit/extras/sqlite3/task.py` & `flytekit-1.9.1/flytekit/extras/sqlite3/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/extras/tasks/shell.py` & `flytekit-1.9.1/flytekit/extras/tasks/shell.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from dataclasses import dataclass
 
 import flytekit
 from flytekit.core.context_manager import ExecutionParameters
 from flytekit.core.interface import Interface
 from flytekit.core.python_function_task import PythonInstanceTask
 from flytekit.core.task import TaskPlugins
+from flytekit.exceptions.user import FlyteRecoverableException
 from flytekit.loggers import logger
 from flytekit.types.directory import FlyteDirectory
 from flytekit.types.file import FlyteFile
 
 
 @dataclass
 class OutputLocation:
@@ -94,14 +95,38 @@
         except KeyError as e:
             raise ValueError(f"Variable {e} in Query not found in inputs {consolidated_args.keys()}")
 
 
 T = typing.TypeVar("T")
 
 
+def _run_script(script) -> typing.Tuple[int, str, str]:
+    """
+    Run script as a subprocess and return the returncode, stdout, and stderr.
+
+    While executing the su process, stdout of the subprocess will be printed
+    to the current process stdout so that the subprocess execution will not appear unresponsive
+
+    :param script: script to be executed
+    :type script: str
+    :return: tuple containing the process returncode, stdout, and stderr
+    :rtype: typing.Tuple[int, str, str]
+    """
+    process = subprocess.Popen(script, stdout=subprocess.PIPE, stderr=subprocess.PIPE, bufsize=0, shell=True, text=True)
+
+    # print stdout so that long-running subprocess will not appear unresponsive
+    out = ""
+    for line in process.stdout:
+        print(line)
+        out += line
+
+    code = process.wait()
+    return code, out, process.stderr.read()
+
+
 class ShellTask(PythonInstanceTask[T]):
     """ """
 
     def __init__(
         self,
         name: str,
         debug: bool = False,
@@ -209,29 +234,31 @@
 
         gen_script = self._interpolizer.interpolate(self._script, inputs=kwargs, outputs=outputs)
         if self._debug:
             print("\n==============================================\n")
             print(gen_script)
             print("\n==============================================\n")
 
-        try:
-            if platform.system() == "Windows" and os.environ.get("ComSpec") is None:
-                # https://github.com/python/cpython/issues/101283
-                os.environ["ComSpec"] = "C:\\Windows\\System32\\cmd.exe"
-            subprocess.check_call(gen_script, shell=True)
-        except subprocess.CalledProcessError as e:
+        if platform.system() == "Windows" and os.environ.get("ComSpec") is None:
+            # https://github.com/python/cpython/issues/101283
+            os.environ["ComSpec"] = "C:\\Windows\\System32\\cmd.exe"
+
+        returncode, stdout, stderr = _run_script(gen_script)
+        if returncode != 0:
             files = os.listdir(".")
             fstr = "\n-".join(files)
-            logger.error(
-                f"Failed to Execute Script, return-code {e.returncode} \n"
-                f"StdErr: {e.stderr}\n"
-                f"StdOut: {e.stdout}\n"
-                f" Current directory contents: .\n-{fstr}"
+            error = (
+                f"Failed to Execute Script, return-code {returncode} \n"
+                f"Current directory contents: .\n-{fstr}\n"
+                f"StdOut: {stdout}\n"
+                f"StdErr: {stderr}\n"
             )
-            raise
+            logger.error(error)
+            # raise FlyteRecoverableException so that it's classified as user error and will be retried
+            raise FlyteRecoverableException(error)
 
         final_outputs = []
         for v in self._output_locs:
             if issubclass(v.var_type, FlyteFile):
                 final_outputs.append(FlyteFile(outputs[v.var]))
             if issubclass(v.var_type, FlyteDirectory):
                 final_outputs.append(FlyteDirectory(outputs[v.var]))
```

### Comparing `flytekit-1.9.0a0/flytekit/extras/tensorflow/__init__.py` & `flytekit-1.9.1/flytekit/extras/tensorflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/extras/tensorflow/model.py` & `flytekit-1.9.1/flytekit/extras/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/extras/tensorflow/record.py` & `flytekit-1.9.1/flytekit/extras/tensorflow/record.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import os
 from dataclasses import dataclass
 from typing import Optional, Tuple, Type, Union
 
 import tensorflow as tf
-from dataclasses_json import dataclass_json
+from dataclasses_json import DataClassJsonMixin
 from tensorflow.python.data.ops.readers import TFRecordDatasetV2
 from typing_extensions import Annotated, get_args, get_origin
 
 from flytekit.core.context_manager import FlyteContext
 from flytekit.core.type_engine import TypeEngine, TypeTransformer, TypeTransformerFailedError
 from flytekit.models.core import types as _core_types
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
 from flytekit.types.directory import TFRecordsDirectory
 from flytekit.types.file import TFRecordFile
 
 
-@dataclass_json
 @dataclass
-class TFRecordDatasetConfig:
+class TFRecordDatasetConfig(DataClassJsonMixin):
     """
     TFRecordDatasetConfig can be used while creating tf.data.TFRecordDataset comprising
     record of one or more TFRecord files.
 
     Args:
       compression_type: A scalar evaluating to one of "" (no compression), "ZLIB", or "GZIP".
       buffer_size: The number of bytes in the read buffer. If None, a sensible default for both local and remote file systems is used.
```

### Comparing `flytekit-1.9.0a0/flytekit/image_spec/image_spec.py` & `flytekit-1.9.1/flytekit/image_spec/image_spec.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,54 +1,63 @@
 import base64
 import hashlib
 import os
+import pathlib
 import typing
 from abc import abstractmethod
 from copy import copy
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass
 from functools import lru_cache
 from typing import List, Optional
 
 import click
 import requests
-from dataclasses_json import dataclass_json
 
 DOCKER_HUB = "docker.io"
 _F_IMG_ID = "_F_IMG_ID"
 
 
-@dataclass_json
 @dataclass
 class ImageSpec:
     """
     This class is used to specify the docker image that will be used to run the task.
 
     Args:
         name: name of the image.
         python_version: python version of the image. Use default python in the base image if None.
         builder: Type of plugin to build the image. Use envd by default.
         source_root: source root of the image.
         env: environment variables of the image.
         registry: registry of the image.
         packages: list of python packages to install.
+        requirements: path to the requirements.txt file.
         apt_packages: list of apt packages to install.
+        cuda: version of cuda to install.
+        cudnn: version of cudnn to install.
         base_image: base image of the image.
         platform: Specify the target platforms for the build output (for example, windows/amd64 or linux/amd64,darwin/arm64
+        pip_index: Specify the custom pip index url
+        registry_config: Specify the path to a JSON registry config file
     """
 
     name: str = "flytekit"
     python_version: str = None  # Use default python in the base image if None.
     builder: str = "envd"
     source_root: Optional[str] = None
     env: Optional[typing.Dict[str, str]] = None
     registry: Optional[str] = None
     packages: Optional[List[str]] = None
+    requirements: Optional[str] = None
     apt_packages: Optional[List[str]] = None
+    cuda: Optional[str] = None
+    cudnn: Optional[str] = None
     base_image: Optional[str] = None
     platform: str = "linux/amd64"
+    pip_index: Optional[str] = None
+    registry_config: Optional[str] = None
 
     def image_name(self) -> str:
         """
         return full image name with tag.
         """
         tag = calculate_hash_from_image_spec(self)
         container_image = f"{self.name}:{tag}"
@@ -100,15 +109,15 @@
                     return False
 
             click.secho(f"Failed to check if the image exists with error : {e}", fg="red")
             click.secho("Flytekit assumes that the image already exists.", fg="blue")
             return True
 
     def __hash__(self):
-        return hash(self.to_json())
+        return hash(asdict(self).__str__())
 
 
 class ImageSpecBuilder:
     @abstractmethod
     def build_image(self, image_spec: ImageSpec):
         """
         Build the docker image and push it to the registry.
@@ -121,42 +130,49 @@
 
 class ImageBuildEngine:
     """
     ImageBuildEngine contains a list of builders that can be used to build an ImageSpec.
     """
 
     _REGISTRY: typing.Dict[str, ImageSpecBuilder] = {}
+    _BUILT_IMAGES: typing.Set[str] = set()
 
     @classmethod
     def register(cls, builder_type: str, image_spec_builder: ImageSpecBuilder):
         cls._REGISTRY[builder_type] = image_spec_builder
 
     @classmethod
     def build(cls, image_spec: ImageSpec):
         if image_spec.builder not in cls._REGISTRY:
             raise Exception(f"Builder {image_spec.builder} is not registered.")
-        if not image_spec.exist():
-            click.secho(f"Image {image_spec.image_name()} not found. Building...", fg="blue")
-            cls._REGISTRY[image_spec.builder].build_image(image_spec)
+        img_name = image_spec.image_name()
+        if img_name in cls._BUILT_IMAGES or image_spec.exist():
+            click.secho(f"Image {img_name} found. Skip building.", fg="blue")
         else:
-            click.secho(f"Image {image_spec.image_name()} found. Skip building.", fg="blue")
+            click.secho(f"Image {img_name} not found. Building...", fg="blue")
+            cls._REGISTRY[image_spec.builder].build_image(image_spec)
+            cls._BUILT_IMAGES.add(img_name)
 
 
 @lru_cache
 def calculate_hash_from_image_spec(image_spec: ImageSpec):
     """
     Calculate the hash from the image spec.
     """
     # copy the image spec to avoid modifying the original image spec. otherwise, the hash will be different.
     spec = copy(image_spec)
     spec.source_root = hash_directory(image_spec.source_root) if image_spec.source_root else b""
-    image_spec_bytes = bytes(spec.to_json(), "utf-8")
+    if spec.requirements:
+        spec.requirements = hashlib.sha1(pathlib.Path(spec.requirements).read_bytes()).hexdigest()
+    # won't rebuild the image if we change the registry_config path
+    spec.registry_config = None
+    image_spec_bytes = asdict(spec).__str__().encode("utf-8")
     tag = base64.urlsafe_b64encode(hashlib.md5(image_spec_bytes).digest()).decode("ascii")
-    # replace "=" with "." to make it a valid tag
-    return tag.replace("=", ".")
+    # replace "=" with "." and replace "-" with "_" to make it a valid tag
+    return tag.replace("=", ".").replace("-", "_")
 
 
 def hash_directory(path):
     """
     Return the SHA-256 hash of the directory at the given path.
     """
     hasher = hashlib.sha256()
```

### Comparing `flytekit-1.9.0a0/flytekit/interaction/parse_stdin.py` & `flytekit-1.9.1/flytekit/interaction/parse_stdin.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/interfaces/cli_identifiers.py` & `flytekit-1.9.1/flytekit/interfaces/cli_identifiers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/interfaces/random.py` & `flytekit-1.9.1/flytekit/interfaces/random.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/interfaces/stats/client.py` & `flytekit-1.9.1/flytekit/interfaces/stats/client.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/interfaces/stats/taggable.py` & `flytekit-1.9.1/flytekit/interfaces/stats/taggable.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/lazy_import/lazy_module.py` & `flytekit-1.9.1/flytekit/lazy_import/lazy_module.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/loggers.py` & `flytekit-1.9.1/flytekit/loggers.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # The environment variable controls exposed to affect the individual loggers should be considered to be beta.
 # The ux/api may change in the future.
 # At time of writing, the code was written to preserve existing default behavior
 # For now, assume this is the environment variable whose usage will remain unchanged and controls output for all
 # loggers defined in this file.
 LOGGING_ENV_VAR = "FLYTE_SDK_LOGGING_LEVEL"
 LOGGING_FMT_ENV_VAR = "FLYTE_SDK_LOGGING_FORMAT"
+LOGGING_RICH_FMT_ENV_VAR = "FLYTE_SDK_RICH_TRACEBACKS"
 
 # By default, the root flytekit logger to debug so everything is logged, but enable fine-tuning
 logger = logging.getLogger("flytekit")
 
 # Stop propagation so that configuration is isolated to this file (so that it doesn't matter what the
 # global Python root logger is set to).
 logger.propagate = False
@@ -32,23 +33,26 @@
 auth_logger = child_loggers["auth"]
 cli_logger = child_loggers["cli"]
 remote_logger = child_loggers["remote"]
 entrypoint_logger = child_loggers["entrypoint"]
 user_space_logger = child_loggers["user_space"]
 
 # create console handler
-try:
-    handler = RichHandler(
-        rich_tracebacks=True,
-        omit_repeated_times=False,
-        keywords=["[flytekit]"],
-        log_time_format="%Y-%m-%d %H:%M:%S,%f",
-        console=Console(width=os.get_terminal_size().columns),
-    )
-except OSError:
+if os.environ.get(LOGGING_RICH_FMT_ENV_VAR) != "0":
+    try:
+        handler = RichHandler(
+            rich_tracebacks=True,
+            omit_repeated_times=False,
+            keywords=["[flytekit]"],
+            log_time_format="%Y-%m-%d %H:%M:%S,%f",
+            console=Console(width=os.get_terminal_size().columns),
+        )
+    except OSError:
+        handler = logging.StreamHandler()
+else:
     handler = logging.StreamHandler()
 
 handler.setLevel(logging.DEBUG)
 
 # Root logger control
 # Don't want to import the configuration library since that will cause all sorts of circular imports, let's
 # just use the environment variable if it's defined. Decide in the future when we implement better controls
```

### Comparing `flytekit-1.9.0a0/flytekit/models/admin/common.py` & `flytekit-1.9.1/flytekit/models/admin/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/admin/task_execution.py` & `flytekit-1.9.1/flytekit/models/admin/task_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/admin/workflow.py` & `flytekit-1.9.1/flytekit/models/admin/workflow.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/annotation.py` & `flytekit-1.9.1/flytekit/models/annotation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/array_job.py` & `flytekit-1.9.1/flytekit/models/array_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/common.py` & `flytekit-1.9.1/flytekit/models/common.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/core/catalog.py` & `flytekit-1.9.1/flytekit/models/core/catalog.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/core/compiler.py` & `flytekit-1.9.1/flytekit/models/core/compiler.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/core/condition.py` & `flytekit-1.9.1/flytekit/models/core/condition.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/core/errors.py` & `flytekit-1.9.1/flytekit/models/core/errors.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/core/execution.py` & `flytekit-1.9.1/flytekit/models/core/execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/core/identifier.py` & `flytekit-1.9.1/flytekit/models/core/identifier.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/core/types.py` & `flytekit-1.9.1/flytekit/models/core/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/core/workflow.py` & `flytekit-1.9.1/flytekit/models/core/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -336,26 +336,60 @@
         return cls(
             signal=SignalCondition.from_flyte_idl(pb2_object.signal) if pb2_object.HasField("signal") else None,
             sleep=SleepCondition.from_flyte_idl(pb2_object.sleep) if pb2_object.HasField("sleep") else None,
             approve=ApproveCondition.from_flyte_idl(pb2_object.approve) if pb2_object.HasField("approve") else None,
         )
 
 
+class ArrayNode(_common.FlyteIdlEntity):
+    def __init__(self, node: "Node", parallelism=None, min_successes=None, min_success_ratio=None) -> None:
+        """
+        TODO: docstring
+        """
+        self._node = node
+        self._parallelism = parallelism
+        # TODO either min_successes or min_success_ratio should be set
+        self._min_successes = min_successes
+        self._min_success_ratio = min_success_ratio
+
+    @property
+    def node(self) -> "Node":
+        return self._node
+
+    def to_flyte_idl(self) -> _core_workflow.ArrayNode:
+        return _core_workflow.ArrayNode(
+            node=self._node.to_flyte_idl() if self._node is not None else None,
+            parallelism=self._parallelism,
+            min_successes=self._min_successes,
+            min_success_ratio=self._min_success_ratio,
+        )
+
+    @classmethod
+    def from_flyte_idl(cls, pb2_object) -> "ArrayNode":
+        return cls(
+            Node.from_flyte_idl(pb2_object.node),
+            pb2_object.parallelism,
+            pb2_object.min_successes,
+            pb2_object.min_success_ratio,
+        )
+
+
 class Node(_common.FlyteIdlEntity):
     def __init__(
         self,
         id,
         metadata,
         inputs,
         upstream_node_ids,
         output_aliases,
         task_node=None,
         workflow_node=None,
         branch_node=None,
         gate_node: typing.Optional[GateNode] = None,
+        array_node: typing.Optional[ArrayNode] = None,
     ):
         """
         A Workflow graph Node. One unit of execution in the graph. Each node can be linked to a Task,
         a Workflow or a branch node.  One of the nodes must be specified.
 
         :param Text id: A workflow-level unique identifier that identifies this node in the workflow. "inputs" and
             "outputs" are reserved node ids that cannot be used by other nodes.
@@ -379,14 +413,15 @@
         self._upstream_node_ids = upstream_node_ids
         # TODO: For proper graph handling, we need to keep track of the node objects themselves, not just the node IDs
         self._output_aliases = output_aliases
         self._task_node = task_node
         self._workflow_node = workflow_node
         self._branch_node = branch_node
         self._gate_node = gate_node
+        self._array_node = array_node
 
     @property
     def id(self):
         """
         A workflow-level unique identifier that identifies this node in the workflow. "inputs" and
         "outputs" are reserved node ids that cannot be used by other nodes.
         :rtype: Text
@@ -455,14 +490,18 @@
         return self._branch_node
 
     @property
     def gate_node(self) -> typing.Optional[GateNode]:
         return self._gate_node
 
     @property
+    def array_node(self) -> typing.Optional[ArrayNode]:
+        return self._array_node
+
+    @property
     def target(self):
         """
         :rtype: T
         """
         return self.task_node or self.workflow_node or self.branch_node
 
     def to_flyte_idl(self):
@@ -475,14 +514,15 @@
             inputs=[i.to_flyte_idl() for i in self.inputs],
             upstream_node_ids=self.upstream_node_ids,
             output_aliases=[a.to_flyte_idl() for a in self.output_aliases],
             task_node=self.task_node.to_flyte_idl() if self.task_node is not None else None,
             workflow_node=self.workflow_node.to_flyte_idl() if self.workflow_node is not None else None,
             branch_node=self.branch_node.to_flyte_idl() if self.branch_node is not None else None,
             gate_node=self.gate_node.to_flyte_idl() if self.gate_node else None,
+            array_node=self.array_node.to_flyte_idl() if self.array_node else None,
         )
 
     @classmethod
     def from_flyte_idl(cls, pb2_object):
         """
         :param flyteidl.core.workflow_pb2.Node pb2_object:
         :rtype: Node
@@ -497,14 +537,15 @@
             workflow_node=WorkflowNode.from_flyte_idl(pb2_object.workflow_node)
             if pb2_object.HasField("workflow_node")
             else None,
             branch_node=BranchNode.from_flyte_idl(pb2_object.branch_node)
             if pb2_object.HasField("branch_node")
             else None,
             gate_node=GateNode.from_flyte_idl(pb2_object.gate_node) if pb2_object.HasField("gate_node") else None,
+            array_node=ArrayNode.from_flyte_idl(pb2_object.array_node) if pb2_object.HasField("array_node") else None,
         )
 
 
 class TaskNodeOverrides(_common.FlyteIdlEntity):
     def __init__(self, resources: typing.Optional[Resources] = None):
         self._resources = resources
```

### Comparing `flytekit-1.9.0a0/flytekit/models/documentation.py` & `flytekit-1.9.1/flytekit/models/documentation.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/dynamic_job.py` & `flytekit-1.9.1/flytekit/models/dynamic_job.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/execution.py` & `flytekit-1.9.1/flytekit/models/execution.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,14 +174,15 @@
         annotations=None,
         auth_role=None,
         raw_output_data_config=None,
         max_parallelism: Optional[int] = None,
         security_context: Optional[security.SecurityContext] = None,
         overwrite_cache: Optional[bool] = None,
         envs: Optional[_common_models.Envs] = None,
+        tags: Optional[typing.List[str]] = None,
     ):
         """
         :param flytekit.models.core.identifier.Identifier launch_plan: Launch plan unique identifier to execute
         :param ExecutionMetadata metadata: The metadata to be associated with this execution
         :param NotificationList notifications: List of notifications for this execution.
         :param bool disable_all: If true, all notifications should be disabled.
         :param flytekit.models.common.Labels labels: Labels to apply to the execution.
@@ -190,27 +191,29 @@
         :param raw_output_data_config: Optional location of offloaded data for things like S3, etc.
         :param max_parallelism int: Controls the maximum number of tasknodes that can be run in parallel for the entire
             workflow. This is useful to achieve fairness. Note: MapTasks are regarded as one unit, and
             parallelism/concurrency of MapTasks is independent from this.
         :param security_context: Optional security context to use for this execution.
         :param overwrite_cache: Optional flag to overwrite the cache for this execution.
         :param envs: flytekit.models.common.Envs environment variables to set for this execution.
+        :param tags: Optional list of tags to apply to the execution.
         """
         self._launch_plan = launch_plan
         self._metadata = metadata
         self._notifications = notifications
         self._disable_all = disable_all
         self._labels = labels or _common_models.Labels({})
         self._annotations = annotations or _common_models.Annotations({})
         self._auth_role = auth_role or _common_models.AuthRole()
         self._raw_output_data_config = raw_output_data_config
         self._max_parallelism = max_parallelism
         self._security_context = security_context
         self._overwrite_cache = overwrite_cache
         self._envs = envs
+        self._tags = tags
 
     @property
     def launch_plan(self):
         """
         If the values were too large, this is the URI where the values were offloaded.
         :rtype: flytekit.models.core.identifier.Identifier
         """
@@ -277,14 +280,18 @@
     def overwrite_cache(self) -> Optional[bool]:
         return self._overwrite_cache
 
     @property
     def envs(self) -> Optional[_common_models.Envs]:
         return self._envs
 
+    @property
+    def tags(self) -> Optional[typing.List[str]]:
+        return self._tags
+
     def to_flyte_idl(self):
         """
         :rtype: flyteidl.admin.execution_pb2.ExecutionSpec
         """
         return _execution_pb2.ExecutionSpec(
             launch_plan=self.launch_plan.to_flyte_idl(),
             metadata=self.metadata.to_flyte_idl(),
@@ -296,14 +303,15 @@
             raw_output_data_config=self._raw_output_data_config.to_flyte_idl()
             if self._raw_output_data_config
             else None,
             max_parallelism=self.max_parallelism,
             security_context=self.security_context.to_flyte_idl() if self.security_context else None,
             overwrite_cache=self.overwrite_cache,
             envs=self.envs.to_flyte_idl() if self.envs else None,
+            tags=self.tags,
         )
 
     @classmethod
     def from_flyte_idl(cls, p):
         """
         :param flyteidl.admin.execution_pb2.ExecutionSpec p:
         :return: ExecutionSpec
@@ -321,14 +329,15 @@
             else None,
             max_parallelism=p.max_parallelism,
             security_context=security.SecurityContext.from_flyte_idl(p.security_context)
             if p.security_context
             else None,
             overwrite_cache=p.overwrite_cache,
             envs=_common_models.Envs.from_flyte_idl(p.envs) if p.HasField("envs") else None,
+            tags=p.tags,
         )
 
 
 class LiteralMapBlob(_common_models.FlyteIdlEntity):
     def __init__(self, values=None, uri=None):
         """
         :param flytekit.models.literals.LiteralMap values:
```

### Comparing `flytekit-1.9.0a0/flytekit/models/filters.py` & `flytekit-1.9.1/flytekit/models/filters.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/interface.py` & `flytekit-1.9.1/flytekit/models/interface.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/launch_plan.py` & `flytekit-1.9.1/flytekit/models/launch_plan.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/literals.py` & `flytekit-1.9.1/flytekit/models/literals.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/matchable_resource.py` & `flytekit-1.9.1/flytekit/models/matchable_resource.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/named_entity.py` & `flytekit-1.9.1/flytekit/models/named_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/node_execution.py` & `flytekit-1.9.1/flytekit/models/node_execution.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/presto.py` & `flytekit-1.9.1/flytekit/models/presto.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/project.py` & `flytekit-1.9.1/flytekit/models/project.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/qubole.py` & `flytekit-1.9.1/flytekit/models/qubole.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/schedule.py` & `flytekit-1.9.1/flytekit/models/schedule.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/security.py` & `flytekit-1.9.1/flytekit/models/security.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/task.py` & `flytekit-1.9.1/flytekit/models/task.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/types.py` & `flytekit-1.9.1/flytekit/models/types.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/models/workflow_closure.py` & `flytekit-1.9.1/flytekit/models/workflow_closure.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/remote/__init__.py` & `flytekit-1.9.1/flytekit/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/remote/backfill.py` & `flytekit-1.9.1/flytekit/remote/backfill.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/remote/entities.py` & `flytekit-1.9.1/flytekit/remote/entities.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,52 +338,60 @@
 
 class FlyteGateNode(_workflow_model.GateNode):
     @classmethod
     def promote_from_model(cls, model: _workflow_model.GateNode):
         return cls(model.signal, model.sleep, model.approve)
 
 
+class FlyteArrayNode(_workflow_model.ArrayNode):
+    @classmethod
+    def promote_from_model(cls, model: _workflow_model.ArrayNode):
+        return cls(model._parallelism, model._node, model._min_success_ratio, model._min_successes)
+
+
 class FlyteNode(_hash_mixin.HashOnReferenceMixin, _workflow_model.Node):
     """A class encapsulating a remote Flyte node."""
 
     def __init__(
         self,
         id,
         upstream_nodes,
         bindings,
         metadata,
         task_node: Optional[FlyteTaskNode] = None,
         workflow_node: Optional[FlyteWorkflowNode] = None,
         branch_node: Optional[FlyteBranchNode] = None,
         gate_node: Optional[FlyteGateNode] = None,
+        array_node: Optional[FlyteArrayNode] = None,
     ):
-        if not task_node and not workflow_node and not branch_node and not gate_node:
+        if not task_node and not workflow_node and not branch_node and not gate_node and not array_node:
             raise _user_exceptions.FlyteAssertion(
-                "An Flyte node must have one of task|workflow|branch|gate entity specified at once"
+                "An Flyte node must have one of task|workflow|branch|gate|array entity specified at once"
             )
         # TODO: Revisit flyte_branch_node and flyte_gate_node, should they be another type like Condition instead
         #       of a node?
         self._flyte_task_node = task_node
         if task_node:
             self._flyte_entity = task_node.flyte_task
         elif workflow_node:
             self._flyte_entity = workflow_node.flyte_workflow or workflow_node.flyte_launch_plan
         else:
-            self._flyte_entity = branch_node or gate_node
+            self._flyte_entity = branch_node or gate_node or array_node
 
         super(FlyteNode, self).__init__(
             id=id,
             metadata=metadata,
             inputs=bindings,
             upstream_node_ids=[n.id for n in upstream_nodes],
             output_aliases=[],
             task_node=task_node,
             workflow_node=workflow_node,
             branch_node=branch_node,
             gate_node=gate_node,
+            array_node=array_node,
         )
         self._upstream = upstream_nodes
 
     @property
     def task_node(self) -> Optional[FlyteTaskNode]:
         return self._flyte_task_node
 
@@ -423,15 +431,21 @@
     ) -> Tuple[Optional[FlyteNode], Dict[id_models.Identifier, FlyteWorkflow]]:
         node_model_id = model.id
         # TODO: Consider removing
         if id in {_constants.START_NODE_ID, _constants.END_NODE_ID}:
             remote_logger.warning(f"Should not call promote from model on a start node or end node {model}")
             return None, converted_sub_workflows
 
-        flyte_task_node, flyte_workflow_node, flyte_branch_node, flyte_gate_node = None, None, None, None
+        flyte_task_node, flyte_workflow_node, flyte_branch_node, flyte_gate_node, flyte_array_node = (
+            None,
+            None,
+            None,
+            None,
+            None,
+        )
         if model.task_node is not None:
             if model.task_node.reference_id not in tasks:
                 raise RuntimeError(
                     f"Remote Workflow closure does not have task with id {model.task_node.reference_id}."
                 )
             flyte_task_node = cls._promote_task_node(tasks[model.task_node.reference_id])
         elif model.workflow_node is not None:
@@ -448,14 +462,17 @@
                 sub_workflows,
                 node_launch_plans,
                 tasks,
                 converted_sub_workflows,
             )
         elif model.gate_node is not None:
             flyte_gate_node = FlyteGateNode.promote_from_model(model.gate_node)
+        elif model.array_node is not None:
+            flyte_array_node = FlyteArrayNode.promote_from_model(model.array_node)
+            # TODO: validate task in tasks
         else:
             raise _system_exceptions.FlyteSystemException(
                 f"Bad Node model, neither task nor workflow detected, node: {model}"
             )
 
         # When WorkflowTemplate models (containing node models) are returned by Admin, they've been compiled with a
         # start node. In order to make the promoted FlyteWorkflow look the same, we strip the start-node text back out.
@@ -473,14 +490,15 @@
                 upstream_nodes=[],  # set downstream, model doesn't contain this information
                 bindings=model.inputs,
                 metadata=model.metadata,
                 task_node=flyte_task_node,
                 workflow_node=flyte_workflow_node,
                 branch_node=flyte_branch_node,
                 gate_node=flyte_gate_node,
+                array_node=flyte_array_node,
             ),
             converted_sub_workflows,
         )
 
     @property
     def upstream_nodes(self) -> List[FlyteNode]:
         return self._upstream
```

### Comparing `flytekit-1.9.0a0/flytekit/remote/executions.py` & `flytekit-1.9.1/flytekit/remote/executions.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/remote/lazy_entity.py` & `flytekit-1.9.1/flytekit/remote/lazy_entity.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/remote/remote.py` & `flytekit-1.9.1/flytekit/remote/remote.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,18 +74,19 @@
     FlyteControlPlaneEntity,
     FlyteLocalEntity,
     Options,
     get_serializable,
     get_serializable_launch_plan,
 )
 
-try:
-    from IPython.core.display import HTML
-except ImportError:
-    ...
+if typing.TYPE_CHECKING:
+    try:
+        from IPython.core.display import HTML
+    except ImportError:
+        ...
 
 ExecutionDataResponse = typing.Union[WorkflowExecutionGetDataResponse, NodeExecutionGetDataResponse]
 
 MOST_RECENT_FIRST = admin_common_models.Sort("created_at", admin_common_models.Sort.Direction.DESCENDING)
 
 
 class RegistrationSkipped(Exception):
@@ -223,46 +224,55 @@
     @property
     def file_access(self) -> FileAccessProvider:
         """File access provider to use for offloading non-literal inputs/outputs."""
         return self._file_access
 
     def get(
         self, flyte_uri: typing.Optional[str] = None
-    ) -> typing.Optional[typing.Union[LiteralsResolver, HTML, bytes]]:
+    ) -> typing.Optional[typing.Union[LiteralsResolver, Literal, HTML, bytes]]:
+        """
+        General function that works with flyte tiny urls. This can return outputs (in the form of LiteralsResolver, or
+        individual Literals for singular requests), or HTML if passed a deck link, or bytes containing HTML,
+        if ipython is not available locally.
+        """
         if flyte_uri is None:
             raise user_exceptions.FlyteUserException("flyte_uri cannot be empty")
         ctx = self._ctx or FlyteContextManager.current_context()
         try:
             data_response = self.client.get_data(flyte_uri)
 
             if data_response.HasField("literal_map"):
                 lm = LiteralMap.from_flyte_idl(data_response.literal_map)
                 return LiteralsResolver(lm.literals)
+            elif data_response.HasField("literal"):
+                return data_response.literal
             elif data_response.HasField("pre_signed_urls"):
                 if len(data_response.pre_signed_urls.signed_url) == 0:
                     raise ValueError(f"Flyte url {flyte_uri} resolved to empty download link")
                 d = data_response.pre_signed_urls.signed_url[0]
                 remote_logger.debug(f"Download link is {d}")
                 fs = ctx.file_access.get_filesystem_for_path(d)
 
                 # If the venv has IPython, then return IPython's HTML
                 if ipython_check():
+                    from IPython.core.display import HTML
+
                     remote_logger.debug(f"IPython found, returning HTML from {flyte_uri}")
                     with fs.open(d, "rb") as r:
                         html = HTML(str(r.read()))
                         return html
                 # If not return bytes
                 else:
                     remote_logger.debug(f"IPython not found, returning HTML as bytes from {flyte_uri}")
                     return fs.open(d, "rb").read()
 
         except user_exceptions.FlyteUserException as e:
             remote_logger.info(f"Error from Flyte backend when trying to fetch data: {e.__cause__}")
 
-        remote_logger.debug(f"Nothing found from {flyte_uri}")
+        remote_logger.info(f"Nothing found from {flyte_uri}")
 
     def remote_context(self):
         """Context manager with remote-specific configuration."""
         return FlyteContextManager.with_context(
             FlyteContextManager.current_context().with_file_access(self.file_access)
         )
 
@@ -776,28 +786,32 @@
         upload_location = self.client.get_upload_signed_url(
             project=project or self.default_project,
             domain=domain or self.default_domain,
             content_md5=md5_bytes,
             filename=to_upload.name,
         )
 
+        extra_headers = self.get_extra_headers_for_protocol(upload_location.native_url)
         encoded_md5 = b64encode(md5_bytes)
         with open(str(to_upload), "+rb") as local_file:
             content = local_file.read()
             content_length = len(content)
+            headers = {"Content-Length": str(content_length), "Content-MD5": encoded_md5}
+            headers.update(extra_headers)
             rsp = requests.put(
                 upload_location.signed_url,
                 data=content,
-                headers={"Content-Length": str(content_length), "Content-MD5": encoded_md5},
+                headers=headers,
                 verify=False
                 if self._config.platform.insecure_skip_verify is True
                 else self._config.platform.ca_cert_file_path,
             )
 
-            if rsp.status_code != requests.codes["OK"]:
+            # Check both HTTP 201 and 200, because some storage backends (e.g. Azure) return 201 instead of 200.
+            if rsp.status_code not in (requests.codes["OK"], requests.codes["created"]):
                 raise FlyteValueException(
                     rsp.status_code,
                     f"Request to send data {upload_location.signed_url} failed.",
                 )
 
         remote_logger.debug(
             f"Uploading {to_upload} to {upload_location.signed_url} native url {upload_location.native_url}"
@@ -935,20 +949,22 @@
 
     def _execute(
         self,
         entity: typing.Union[FlyteTask, FlyteWorkflow, FlyteLaunchPlan],
         inputs: typing.Dict[str, typing.Any],
         project: str = None,
         domain: str = None,
-        execution_name: str = None,
+        execution_name: typing.Optional[str] = None,
+        execution_name_prefix: typing.Optional[str] = None,
         options: typing.Optional[Options] = None,
         wait: bool = False,
         type_hints: typing.Optional[typing.Dict[str, typing.Type]] = None,
         overwrite_cache: typing.Optional[bool] = None,
         envs: typing.Optional[typing.Dict[str, str]] = None,
+        tags: typing.Optional[typing.List[str]] = None,
     ) -> FlyteWorkflowExecution:
         """Common method for execution across all entities.
 
         :param flyte_id: entity identifier
         :param inputs: dictionary mapping argument names to values
         :param project: project on which to execute the entity referenced by flyte_id
         :param domain: domain on which to execute the entity referenced by flyte_id
@@ -956,17 +972,21 @@
         :param wait: if True, waits for execution to complete
         :param type_hints: map of python types to inputs so that the TypeEngine knows how to convert the input values
           into Flyte Literals.
         :param overwrite_cache: Allows for all cached values of a workflow and its tasks to be overwritten
           for a single execution. If enabled, all calculations are performed even if cached results would
           be available, overwriting the stored data once execution finishes successfully.
         :param envs: Environment variables to set for the execution.
+        :param tags: Tags to set for the execution.
         :returns: :class:`~flytekit.remote.workflow_execution.FlyteWorkflowExecution`
         """
-        execution_name = execution_name or "f" + uuid.uuid4().hex[:19]
+        if execution_name is not None and execution_name_prefix is not None:
+            raise ValueError("Only one of execution_name and execution_name_prefix can be set, but got both set")
+        execution_name_prefix = execution_name_prefix + "-" if execution_name_prefix is not None else None
+        execution_name = execution_name or (execution_name_prefix or "f") + uuid.uuid4().hex[:19]
         if not options:
             options = Options()
         if options.disable_notifications is not None:
             if options.disable_notifications:
                 notifications = None
             else:
                 notifications = NotificationList(options.notifications)
@@ -1021,14 +1041,15 @@
                     labels=options.labels,
                     annotations=options.annotations,
                     raw_output_data_config=options.raw_output_data_config,
                     auth_role=None,
                     max_parallelism=options.max_parallelism,
                     security_context=options.security_context,
                     envs=common_models.Envs(envs) if envs else None,
+                    tags=tags,
                 ),
                 literal_inputs,
             )
         except user_exceptions.FlyteEntityAlreadyExistsException:
             remote_logger.warning(
                 f"Execution with Execution ID {execution_name} already exists. "
                 f"Assuming this is the same execution, returning!"
@@ -1071,21 +1092,23 @@
         self,
         entity: typing.Union[FlyteTask, FlyteLaunchPlan, FlyteWorkflow, PythonTask, WorkflowBase, LaunchPlan],
         inputs: typing.Dict[str, typing.Any],
         project: str = None,
         domain: str = None,
         name: str = None,
         version: str = None,
-        execution_name: str = None,
+        execution_name: typing.Optional[str] = None,
+        execution_name_prefix: typing.Optional[str] = None,
         image_config: typing.Optional[ImageConfig] = None,
         options: typing.Optional[Options] = None,
         wait: bool = False,
         type_hints: typing.Optional[typing.Dict[str, typing.Type]] = None,
         overwrite_cache: typing.Optional[bool] = None,
         envs: typing.Optional[typing.Dict[str, str]] = None,
+        tags: typing.Optional[typing.List[str]] = None,
     ) -> FlyteWorkflowExecution:
         """
         Execute a task, workflow, or launchplan, either something that's been declared locally, or a fetched entity.
 
         This method supports:
         - ``Flyte{Task, Workflow, LaunchPlan}`` remote module objects.
         - ``@task``-decorated functions and ``TaskTemplate`` tasks.
@@ -1115,14 +1138,15 @@
           using the type engine, and then to ``type(v)``. Providing the correct Python types is particularly important
           if the inputs are containers like lists or maps, or if the Python type is one of the more complex Flyte
           provided classes (like a StructuredDataset that's annotated with columns).
         :param overwrite_cache: Allows for all cached values of a workflow and its tasks to be overwritten
           for a single execution. If enabled, all calculations are performed even if cached results would
           be available, overwriting the stored data once execution finishes successfully.
         :param envs: Environment variables to be set for the execution.
+        :param tags: Tags to be set for the execution.
 
         .. note:
 
             The ``name`` and ``version`` arguments do not apply to ``FlyteTask``, ``FlyteLaunchPlan``, and
             ``FlyteWorkflow`` entity inputs. These values are determined by referencing the entity identifier values.
         """
         if entity.python_interface:
@@ -1130,157 +1154,177 @@
         if isinstance(entity, FlyteTask) or isinstance(entity, FlyteLaunchPlan):
             return self.execute_remote_task_lp(
                 entity=entity,
                 inputs=inputs,
                 project=project,
                 domain=domain,
                 execution_name=execution_name,
+                execution_name_prefix=execution_name_prefix,
                 options=options,
                 wait=wait,
                 type_hints=type_hints,
                 overwrite_cache=overwrite_cache,
                 envs=envs,
+                tags=tags,
             )
         if isinstance(entity, FlyteWorkflow):
             return self.execute_remote_wf(
                 entity=entity,
                 inputs=inputs,
                 project=project,
                 domain=domain,
                 execution_name=execution_name,
+                execution_name_prefix=execution_name_prefix,
                 options=options,
                 wait=wait,
                 type_hints=type_hints,
                 overwrite_cache=overwrite_cache,
                 envs=envs,
+                tags=tags,
             )
         if isinstance(entity, PythonTask):
             return self.execute_local_task(
                 entity=entity,
                 inputs=inputs,
                 project=project,
                 domain=domain,
                 name=name,
                 version=version,
                 execution_name=execution_name,
+                execution_name_prefix=execution_name_prefix,
                 image_config=image_config,
                 wait=wait,
                 overwrite_cache=overwrite_cache,
                 envs=envs,
+                tags=tags,
             )
         if isinstance(entity, WorkflowBase):
             return self.execute_local_workflow(
                 entity=entity,
                 inputs=inputs,
                 project=project,
                 domain=domain,
                 name=name,
                 version=version,
                 execution_name=execution_name,
+                execution_name_prefix=execution_name_prefix,
                 image_config=image_config,
                 options=options,
                 wait=wait,
                 overwrite_cache=overwrite_cache,
                 envs=envs,
+                tags=tags,
             )
         if isinstance(entity, LaunchPlan):
             return self.execute_local_launch_plan(
                 entity=entity,
                 inputs=inputs,
                 version=version,
                 project=project,
                 domain=domain,
                 execution_name=execution_name,
+                execution_name_prefix=execution_name_prefix,
                 options=options,
                 wait=wait,
                 overwrite_cache=overwrite_cache,
                 envs=envs,
+                tags=tags,
             )
         raise NotImplementedError(f"entity type {type(entity)} not recognized for execution")
 
     # Flyte Remote Entities
     # ---------------------
 
     def execute_remote_task_lp(
         self,
         entity: typing.Union[FlyteTask, FlyteLaunchPlan],
         inputs: typing.Dict[str, typing.Any],
         project: str = None,
         domain: str = None,
-        execution_name: str = None,
+        execution_name: typing.Optional[str] = None,
+        execution_name_prefix: typing.Optional[str] = None,
         options: typing.Optional[Options] = None,
         wait: bool = False,
         type_hints: typing.Optional[typing.Dict[str, typing.Type]] = None,
         overwrite_cache: typing.Optional[bool] = None,
         envs: typing.Optional[typing.Dict[str, str]] = None,
+        tags: typing.Optional[typing.List[str]] = None,
     ) -> FlyteWorkflowExecution:
         """Execute a FlyteTask, or FlyteLaunchplan.
 
         NOTE: the name and version arguments are currently not used and only there consistency in the function signature
         """
         return self._execute(
             entity,
             inputs,
             project=project,
             domain=domain,
             execution_name=execution_name,
+            execution_name_prefix=execution_name_prefix,
             wait=wait,
             options=options,
             type_hints=type_hints,
             overwrite_cache=overwrite_cache,
             envs=envs,
+            tags=tags,
         )
 
     def execute_remote_wf(
         self,
         entity: FlyteWorkflow,
         inputs: typing.Dict[str, typing.Any],
         project: str = None,
         domain: str = None,
-        execution_name: str = None,
+        execution_name: typing.Optional[str] = None,
+        execution_name_prefix: typing.Optional[str] = None,
         options: typing.Optional[Options] = None,
         wait: bool = False,
         type_hints: typing.Optional[typing.Dict[str, typing.Type]] = None,
         overwrite_cache: typing.Optional[bool] = None,
         envs: typing.Optional[typing.Dict[str, str]] = None,
+        tags: typing.Optional[typing.List[str]] = None,
     ) -> FlyteWorkflowExecution:
         """Execute a FlyteWorkflow.
 
         NOTE: the name and version arguments are currently not used and only there consistency in the function signature
         """
         launch_plan = self.fetch_launch_plan(entity.id.project, entity.id.domain, entity.id.name, entity.id.version)
         return self.execute_remote_task_lp(
             launch_plan,
             inputs,
             project=project,
             domain=domain,
             execution_name=execution_name,
+            execution_name_prefix=execution_name_prefix,
             options=options,
             wait=wait,
             type_hints=type_hints,
             overwrite_cache=overwrite_cache,
             envs=envs,
+            tags=tags,
         )
 
     # Flytekit Entities
     # -----------------
 
     def execute_local_task(
         self,
         entity: PythonTask,
         inputs: typing.Dict[str, typing.Any],
         project: str = None,
         domain: str = None,
         name: str = None,
         version: str = None,
-        execution_name: str = None,
+        execution_name: typing.Optional[str] = None,
+        execution_name_prefix: typing.Optional[str] = None,
         image_config: typing.Optional[ImageConfig] = None,
         wait: bool = False,
         overwrite_cache: typing.Optional[bool] = None,
         envs: typing.Optional[typing.Dict[str, str]] = None,
+        tags: typing.Optional[typing.List[str]] = None,
     ) -> FlyteWorkflowExecution:
         """
         Execute a @task-decorated function or TaskTemplate task.
 
         :param entity: local task entity.
         :param inputs: register the task, which requires compiling the task, before running it.
         :param project: The execution project, will default to the Remote's default project.
@@ -1288,14 +1332,15 @@
         :param name: specific name of the task to run.
         :param version: specific version of the task to run.
         :param execution_name: If provided, will use this name for the execution.
         :param image_config: If provided, will use this image config in the pod.
         :param wait: If True, will wait for the execution to complete before returning.
         :param overwrite_cache: If True, will overwrite the cache.
         :param envs: Environment variables to set for the execution.
+        :param tags: Tags to set for the execution.
         :return: FlyteWorkflowExecution object.
         """
         resolved_identifiers = self._resolve_identifier_kwargs(entity, project, domain, name, version)
         resolved_identifiers_dict = asdict(resolved_identifiers)
         try:
             flyte_task: FlyteTask = self.fetch_task(**resolved_identifiers_dict)
         except FlyteEntityNotExistException:
@@ -1312,34 +1357,38 @@
 
         return self.execute(
             flyte_task,
             inputs,
             project=resolved_identifiers.project,
             domain=resolved_identifiers.domain,
             execution_name=execution_name,
+            execution_name_prefix=execution_name_prefix,
             wait=wait,
             type_hints=entity.python_interface.inputs,
             overwrite_cache=overwrite_cache,
             envs=envs,
+            tags=tags,
         )
 
     def execute_local_workflow(
         self,
         entity: WorkflowBase,
         inputs: typing.Dict[str, typing.Any],
         project: str = None,
         domain: str = None,
         name: str = None,
         version: str = None,
-        execution_name: str = None,
+        execution_name: typing.Optional[str] = None,
+        execution_name_prefix: typing.Optional[str] = None,
         image_config: typing.Optional[ImageConfig] = None,
         options: typing.Optional[Options] = None,
         wait: bool = False,
         overwrite_cache: typing.Optional[bool] = None,
         envs: typing.Optional[typing.Dict[str, str]] = None,
+        tags: typing.Optional[typing.List[str]] = None,
     ) -> FlyteWorkflowExecution:
         """
         Execute an @workflow decorated function.
         :param entity:
         :param inputs:
         :param project:
         :param domain:
@@ -1347,14 +1396,15 @@
         :param version:
         :param execution_name:
         :param image_config:
         :param options:
         :param wait:
         :param overwrite_cache:
         :param envs:
+        :param tags:
         :return:
         """
         resolved_identifiers = self._resolve_identifier_kwargs(entity, project, domain, name, version)
         resolved_identifiers_dict = asdict(resolved_identifiers)
 
         ss = SerializationSettings(
             image_config=image_config,
@@ -1388,46 +1438,51 @@
 
         return self.execute(
             flyte_lp,
             inputs,
             project=project,
             domain=domain,
             execution_name=execution_name,
+            execution_name_prefix=execution_name_prefix,
             wait=wait,
             options=options,
             type_hints=entity.python_interface.inputs,
             overwrite_cache=overwrite_cache,
             envs=envs,
+            tags=tags,
         )
 
     def execute_local_launch_plan(
         self,
         entity: LaunchPlan,
         inputs: typing.Dict[str, typing.Any],
         version: str,
         project: typing.Optional[str] = None,
         domain: typing.Optional[str] = None,
         execution_name: typing.Optional[str] = None,
+        execution_name_prefix: typing.Optional[str] = None,
         options: typing.Optional[Options] = None,
         wait: bool = False,
         overwrite_cache: typing.Optional[bool] = None,
         envs: typing.Optional[typing.Dict[str, str]] = None,
+        tags: typing.Optional[typing.List[str]] = None,
     ) -> FlyteWorkflowExecution:
         """
 
         :param entity: The locally defined launch plan object
         :param inputs: Inputs to be passed into the execution as a dict with Python native values.
         :param version: The version to look up/register the launch plan (if not already exists)
         :param project: The same as version, but will default to the Remote object's project
         :param domain: The same as version, but will default to the Remote object's domain
         :param execution_name: If specified, will be used as the execution name instead of randomly generating.
         :param options: Options to be passed into the execution.
         :param wait: If True, will wait for the execution to complete before returning.
         :param overwrite_cache: If True, will overwrite the cache.
         :param envs: Environment variables to be passed into the execution.
+        :param tags: Tags to be passed into the execution.
         :return: FlyteWorkflowExecution object
         """
         try:
             flyte_launchplan: FlyteLaunchPlan = self.fetch_launch_plan(
                 project=project,
                 domain=domain,
                 name=entity.name,
@@ -1442,19 +1497,21 @@
             )
         return self.execute_remote_task_lp(
             flyte_launchplan,
             inputs,
             project=project,
             domain=domain,
             execution_name=execution_name,
+            execution_name_prefix=execution_name_prefix,
             options=options,
             wait=wait,
             type_hints=entity.python_interface.inputs,
             overwrite_cache=overwrite_cache,
             envs=envs,
+            tags=tags,
         )
 
     ###################################
     # Wait for Executions to Complete #
     ###################################
 
     def wait(
@@ -1888,7 +1945,13 @@
         )
         remote_wf = self.register_workflow(wf, serialization_settings=ss)
 
         if not execute:
             return remote_wf
 
         return self.execute(remote_wf, inputs={}, project=project, domain=domain, execution_name=execution_name)
+
+    @staticmethod
+    def get_extra_headers_for_protocol(native_url):
+        if native_url.startswith("abfs://"):
+            return {"x-ms-blob-type": "BlockBlob"}
+        return {}
```

### Comparing `flytekit-1.9.0a0/flytekit/remote/remote_callable.py` & `flytekit-1.9.1/flytekit/remote/remote_callable.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,13 +61,16 @@
         else:
             logger.debug("Fetched entity, running raw execute.")
             return self.execute(**kwargs)
 
     def local_execute(self, ctx: FlyteContext, **kwargs) -> Optional[Union[Tuple[Promise], Promise, VoidPromise]]:
         return self.execute(**kwargs)
 
+    def local_execution_mode(self) -> ExecutionState.Mode:
+        return ExecutionState.Mode.LOCAL_TASK_EXECUTION
+
     def execute(self, **kwargs) -> Any:
         raise AssertionError(f"Remotely fetched entities cannot be run locally. Please mock the {self.name}.execute.")
 
     @property
     def python_interface(self) -> Optional[Dict[str, Type]]:
         return self._python_interface
```

### Comparing `flytekit-1.9.0a0/flytekit/testing/__init__.py` & `flytekit-1.9.1/flytekit/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/tools/fast_registration.py` & `flytekit-1.9.1/flytekit/tools/fast_registration.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/tools/ignore.py` & `flytekit-1.9.1/flytekit/tools/ignore.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/tools/module_loader.py` & `flytekit-1.9.1/flytekit/tools/module_loader.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/tools/repo.py` & `flytekit-1.9.1/flytekit/tools/repo.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/tools/script_mode.py` & `flytekit-1.9.1/flytekit/tools/script_mode.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/tools/serialize_helpers.py` & `flytekit-1.9.1/flytekit/tools/serialize_helpers.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/tools/subprocess.py` & `flytekit-1.9.1/flytekit/tools/subprocess.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/tools/translator.py` & `flytekit-1.9.1/flytekit/tools/translator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from collections import OrderedDict
 from dataclasses import dataclass
 from typing import Callable, Dict, List, Optional, Tuple, Union
 
 from flytekit import PythonFunctionTask, SourceCode
 from flytekit.configuration import SerializationSettings
 from flytekit.core import constants as _common_constants
+from flytekit.core.array_node_map_task import ArrayNodeMapTask
 from flytekit.core.base_task import PythonTask
 from flytekit.core.condition import BranchNode
 from flytekit.core.container_task import ContainerTask
 from flytekit.core.gate import Gate
 from flytekit.core.launch_plan import LaunchPlan, ReferenceLaunchPlan
 from flytekit.core.map_task import MapPythonTask
 from flytekit.core.node import Node
@@ -26,14 +27,15 @@
 from flytekit.models import security
 from flytekit.models.admin import workflow as admin_workflow_models
 from flytekit.models.admin.workflow import WorkflowSpec
 from flytekit.models.core import identifier as _identifier_model
 from flytekit.models.core import workflow as _core_wf
 from flytekit.models.core import workflow as workflow_model
 from flytekit.models.core.workflow import ApproveCondition
+from flytekit.models.core.workflow import ArrayNode as ArrayNodeModel
 from flytekit.models.core.workflow import BranchNode as BranchNodeModel
 from flytekit.models.core.workflow import GateNode, SignalCondition, SleepCondition, TaskNodeOverrides
 from flytekit.models.task import TaskSpec, TaskTemplate
 
 FlyteLocalEntity = Union[
     PythonTask,
     BranchNode,
@@ -47,14 +49,15 @@
 ]
 FlyteControlPlaneEntity = Union[
     TaskSpec,
     _launch_plan_models.LaunchPlan,
     admin_workflow_models.WorkflowSpec,
     workflow_model.Node,
     BranchNodeModel,
+    ArrayNodeModel,
 ]
 
 
 @dataclass
 class Options(object):
     """
     These are options that can be configured for a launchplan during registration or overridden during an execution.
@@ -176,26 +179,26 @@
 
     container = entity.get_container(settings)
     # This pod will be incorrect when doing fast serialize
     pod = entity.get_k8s_pod(settings)
 
     if settings.should_fast_serialize():
         # This handles container tasks.
-        if container and isinstance(entity, (PythonAutoContainerTask, MapPythonTask)):
+        if container and isinstance(entity, (PythonAutoContainerTask, MapPythonTask, ArrayNodeMapTask)):
             # For fast registration, we'll need to muck with the command, but on
             # ly for certain kinds of tasks. Specifically,
             # tasks that rely on user code defined in the container. This should be encapsulated by the auto container
             # parent class
             container._args = prefix_with_fast_execute(settings, container.args)
 
         # If the pod spec is not None, we have to get it again, because the one we retrieved above will be incorrect.
         # The reason we have to call get_k8s_pod again, instead of just modifying the command in this file, is because
         # the pod spec is a K8s library object, and we shouldn't be messing around with it in this file.
         elif pod and not isinstance(entity, ContainerTask):
-            if isinstance(entity, MapPythonTask):
+            if isinstance(entity, (MapPythonTask, ArrayNodeMapTask)):
                 entity.set_command_prefix(get_command_prefix_for_fast_execute(settings))
                 pod = entity.get_k8s_pod(settings)
             else:
                 entity.set_command_fn(_fast_serialize_command_fn(settings, entity))
                 pod = entity.get_k8s_pod(settings)
                 entity.reset_command_fn()
 
@@ -412,15 +415,27 @@
             raise Exception(
                 f"Unexpected resource type for reference entity {entity.flyte_entity}: {ref_template.resource_type}"
             )
         return node_model
 
     from flytekit.remote import FlyteLaunchPlan, FlyteTask, FlyteWorkflow
 
-    if isinstance(entity.flyte_entity, PythonTask):
+    if isinstance(entity.flyte_entity, ArrayNodeMapTask):
+        node_model = workflow_model.Node(
+            id=_dnsify(entity.id),
+            metadata=entity.metadata,
+            inputs=entity.bindings,
+            upstream_node_ids=[n.id for n in upstream_nodes],
+            output_aliases=[],
+            array_node=get_serializable_array_node(entity_mapping, settings, entity, options=options),
+        )
+        # TODO: do I need this?
+        # if entity._aliases:
+        #     node_model._output_aliases = entity._aliases
+    elif isinstance(entity.flyte_entity, PythonTask):
         task_spec = get_serializable(entity_mapping, settings, entity.flyte_entity, options=options)
         node_model = workflow_model.Node(
             id=_dnsify(entity.id),
             metadata=entity.metadata,
             inputs=entity.bindings,
             upstream_node_ids=[n.id for n in upstream_nodes],
             output_aliases=[],
@@ -535,14 +550,43 @@
         )
     else:
         raise Exception(f"Node contained non-serializable entity {entity._flyte_entity}")
 
     return node_model
 
 
+def get_serializable_array_node(
+    entity_mapping: OrderedDict,
+    settings: SerializationSettings,
+    node: Node,
+    options: Optional[Options] = None,
+) -> ArrayNodeModel:
+    # TODO Add support for other flyte entities
+    entity = node.flyte_entity
+    task_spec = get_serializable(entity_mapping, settings, entity, options)
+    task_node = workflow_model.TaskNode(
+        reference_id=task_spec.template.id,
+        overrides=TaskNodeOverrides(resources=node._resources),
+    )
+    node = workflow_model.Node(
+        id=entity.name,
+        metadata=entity.construct_node_metadata(),
+        inputs=node.bindings,
+        upstream_node_ids=[],
+        output_aliases=[],
+        task_node=task_node,
+    )
+    return ArrayNodeModel(
+        node=node,
+        parallelism=entity.concurrency,
+        min_successes=entity.min_successes,
+        min_success_ratio=entity.min_success_ratio,
+    )
+
+
 def get_serializable_branch_node(
     entity_mapping: OrderedDict,
     settings: SerializationSettings,
     entity: FlyteLocalEntity,
     options: Optional[Options] = None,
 ) -> BranchNodeModel:
     # We have to iterate through the blocks to convert the nodes from the internal Node type to the Node model type.
```

### Comparing `flytekit-1.9.0a0/flytekit/types/directory/__init__.py` & `flytekit-1.9.1/flytekit/types/directory/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/types/directory/types.py` & `flytekit-1.9.1/flytekit/types/directory/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,37 +6,36 @@
 import typing
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Generator, Tuple
 from uuid import UUID
 
 import fsspec
-from dataclasses_json import config, dataclass_json
+from dataclasses_json import DataClassJsonMixin, config
 from fsspec.utils import get_protocol
 from marshmallow import fields
 
 from flytekit.core.context_manager import FlyteContext, FlyteContextManager
-from flytekit.core.type_engine import TypeEngine, TypeTransformer
+from flytekit.core.type_engine import TypeEngine, TypeTransformer, get_batch_size
 from flytekit.models import types as _type_models
 from flytekit.models.core import types as _core_types
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
 from flytekit.types.file import FileExt, FlyteFile
 
 T = typing.TypeVar("T")
 PathType = typing.Union[str, os.PathLike]
 
 
 def noop():
     ...
 
 
-@dataclass_json
 @dataclass
-class FlyteDirectory(os.PathLike, typing.Generic[T]):
+class FlyteDirectory(DataClassJsonMixin, os.PathLike, typing.Generic[T]):
     path: PathType = field(default=None, metadata=config(mm_field=fields.String()))  # type: ignore
     """
     .. warning::
 
         This class should not be used on very large datasets, as merely listing the dataset will cause
         the entire dataset to be downloaded. Listing on S3 and other backend object stores is not consistent
         and we should not need data to be downloaded to list.
@@ -318,14 +317,16 @@
         python_val: FlyteDirectory,
         python_type: typing.Type[FlyteDirectory],
         expected: LiteralType,
     ) -> Literal:
 
         remote_directory = None
         should_upload = True
+        batch_size = get_batch_size(python_type)
+
         meta = BlobMetadata(type=self._blob_type(format=self.get_format(python_type)))
 
         # There are two kinds of literals we handle, either an actual FlyteDirectory, or a string path to a directory.
         # Handle the FlyteDirectory case
         if isinstance(python_val, FlyteDirectory):
             # If the object has a remote source, then we just convert it back.
             if python_val._remote_source is not None:
@@ -354,15 +355,15 @@
         else:
             raise AssertionError(f"Expected FlyteDirectory or os.PathLike object, received {type(python_val)}")
 
         # If we're uploading something, that means that the uri should always point to the upload destination.
         if should_upload:
             if remote_directory is None:
                 remote_directory = ctx.file_access.get_random_remote_directory()
-            ctx.file_access.put_data(source_path, remote_directory, is_multipart=True)
+            ctx.file_access.put_data(source_path, remote_directory, is_multipart=True, batch_size=batch_size)
             return Literal(scalar=Scalar(blob=Blob(metadata=meta, uri=remote_directory)))
 
         # If not uploading, then we can only take the original source path as the uri.
         else:
             return Literal(scalar=Scalar(blob=Blob(metadata=meta, uri=source_path)))
 
     def to_python_value(
@@ -375,16 +376,18 @@
         # make any sense.
         if not ctx.file_access.is_remote(uri):
             return expected_python_type(uri)
 
         # For the remote case, return an FlyteDirectory object that can download
         local_folder = ctx.file_access.get_random_local_directory()
 
+        batch_size = get_batch_size(expected_python_type)
+
         def _downloader():
-            return ctx.file_access.get_data(uri, local_folder, is_multipart=True)
+            return ctx.file_access.get_data(uri, local_folder, is_multipart=True, batch_size=batch_size)
 
         expected_format = self.get_format(expected_python_type)
 
         fd = FlyteDirectory.__class_getitem__(expected_format)(local_folder, _downloader)
         fd._remote_source = uri
 
         return fd
```

### Comparing `flytekit-1.9.0a0/flytekit/types/file/__init__.py` & `flytekit-1.9.1/flytekit/types/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/types/file/file.py` & `flytekit-1.9.1/flytekit/types/file/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,37 +2,35 @@
 
 import os
 import pathlib
 import typing
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 
-from dataclasses_json import config, dataclass_json
+from dataclasses_json import DataClassJsonMixin, config
 from marshmallow import fields
-from typing_extensions import Annotated, get_args, get_origin
 
 from flytekit.core.context_manager import FlyteContext, FlyteContextManager
-from flytekit.core.type_engine import TypeEngine, TypeTransformer, TypeTransformerFailedError
+from flytekit.core.type_engine import TypeEngine, TypeTransformer, TypeTransformerFailedError, get_underlying_type
 from flytekit.loggers import logger
 from flytekit.models.core.types import BlobType
 from flytekit.models.literals import Blob, BlobMetadata, Literal, Scalar
 from flytekit.models.types import LiteralType
 from flytekit.types.pickle.pickle import FlytePickleTransformer
 
 
 def noop():
     ...
 
 
 T = typing.TypeVar("T")
 
 
-@dataclass_json
 @dataclass
-class FlyteFile(os.PathLike, typing.Generic[T]):
+class FlyteFile(DataClassJsonMixin, os.PathLike, typing.Generic[T]):
     path: typing.Union[str, os.PathLike] = field(
         default=None, metadata=config(mm_field=fields.String())
     )  # type: ignore
     """
     Since there is no native Python implementation of files and directories for the Flyte Blob type, (like how int
     exists for Flyte's Integer type) we need to create one so that users can express that their tasks take
     in or return a file. There is ``pathlib.Path`` of course, (which is usable in Flytekit as a return value, though
@@ -333,16 +331,15 @@
         remote_path = None
         should_upload = True
 
         if python_val is None:
             raise TypeTransformerFailedError("None value cannot be converted to a file.")
 
         # Correctly handle `Annotated[FlyteFile, ...]` by extracting the origin type
-        if get_origin(python_type) is Annotated:
-            python_type = get_args(python_type)[0]
+        python_type = get_underlying_type(python_type)
 
         if not (python_type is os.PathLike or issubclass(python_type, FlyteFile)):
             raise ValueError(f"Incorrect type {python_type}, must be either a FlyteFile or os.PathLike")
 
         # information used by all cases
         meta = BlobMetadata(type=self._blob_type(format=FlyteFilePathTransformer.get_format(python_type)))
 
@@ -404,19 +401,23 @@
     def to_python_value(
         self, ctx: FlyteContext, lv: Literal, expected_python_type: typing.Union[typing.Type[FlyteFile], os.PathLike]
     ) -> FlyteFile:
         try:
             uri = lv.scalar.blob.uri
         except AttributeError:
             raise TypeTransformerFailedError(f"Cannot convert from {lv} to {expected_python_type}")
+
         # In this condition, we still return a FlyteFile instance, but it's a simple one that has no downloading tricks
         # Using is instead of issubclass because FlyteFile does actually subclass it
         if expected_python_type is os.PathLike:
             return FlyteFile(uri)
 
+        # Correctly handle `Annotated[FlyteFile, ...]` by extracting the origin type
+        expected_python_type = get_underlying_type(expected_python_type)
+
         # The rest of the logic is only for FlyteFile types.
         if not issubclass(expected_python_type, FlyteFile):  # type: ignore
             raise TypeError(f"Neither os.PathLike nor FlyteFile specified {expected_python_type}")
 
         # This is a local file path, like /usr/local/my_file, don't mess with it. Certainly, downloading it doesn't
         # make any sense.
         if not ctx.file_access.is_remote(uri):
```

### Comparing `flytekit-1.9.0a0/flytekit/types/numpy/ndarray.py` & `flytekit-1.9.1/flytekit/types/numpy/ndarray.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/types/pickle/pickle.py` & `flytekit-1.9.1/flytekit/types/pickle/pickle.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,16 @@
             ctx.file_access.get_data(uri, local_path, False)
             uri = local_path
         with open(uri, "rb") as infile:
             data = cloudpickle.load(infile)
         return data
 
     def to_literal(self, ctx: FlyteContext, python_val: T, python_type: Type[T], expected: LiteralType) -> Literal:
+        if python_val is None:
+            raise AssertionError("Cannot pickle None Value.")
         meta = BlobMetadata(
             type=_core_types.BlobType(
                 format=self.PYTHON_PICKLE_FORMAT, dimensionality=_core_types.BlobType.BlobDimensionality.SINGLE
             )
         )
         # Dump the task output into pickle
         local_dir = ctx.file_access.get_random_local_directory()
@@ -98,15 +100,17 @@
             and literal_type.blob.format == FlytePickleTransformer.PYTHON_PICKLE_FORMAT
         ):
             return FlytePickle
 
         raise ValueError(f"Transformer {self} cannot reverse {literal_type}")
 
     def get_literal_type(self, t: Type[T]) -> LiteralType:
-        return LiteralType(
+        lt = LiteralType(
             blob=_core_types.BlobType(
                 format=self.PYTHON_PICKLE_FORMAT, dimensionality=_core_types.BlobType.BlobDimensionality.SINGLE
             )
         )
+        lt.metadata = {"python_class_name": str(t)}
+        return lt
 
 
 TypeEngine.register(FlytePickleTransformer())
```

### Comparing `flytekit-1.9.0a0/flytekit/types/schema/types.py` & `flytekit-1.9.1/flytekit/types/schema/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from dataclasses import dataclass, field
 from enum import Enum
 from pathlib import Path
 from typing import Type
 
 import numpy as _np
 import pandas
-from dataclasses_json import config, dataclass_json
+from dataclasses_json import DataClassJsonMixin, config
 from marshmallow import fields
 
 from flytekit.core.context_manager import FlyteContext, FlyteContextManager
 from flytekit.core.type_engine import TypeEngine, TypeTransformer, TypeTransformerFailedError
 from flytekit.loggers import logger
 from flytekit.models.literals import Literal, Scalar, Schema
 from flytekit.models.types import LiteralType, SchemaType
@@ -175,17 +175,16 @@
     @classmethod
     def get_handler(cls, t: Type) -> SchemaHandler:
         if t not in cls._SCHEMA_HANDLERS:
             raise ValueError(f"DataFrames of type {t} are not supported currently")
         return cls._SCHEMA_HANDLERS[t]
 
 
-@dataclass_json
 @dataclass
-class FlyteSchema(object):
+class FlyteSchema(DataClassJsonMixin):
     remote_path: typing.Optional[str] = field(default=None, metadata=config(mm_field=fields.String()))
     """
     This is the main schema class that users should use.
     """
 
     @classmethod
     def columns(cls) -> typing.Dict[str, typing.Type]:
```

### Comparing `flytekit-1.9.0a0/flytekit/types/schema/types_pandas.py` & `flytekit-1.9.1/flytekit/types/schema/types_pandas.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/types/structured/__init__.py` & `flytekit-1.9.1/flytekit/types/structured/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,22 @@
     StructuredDataset,
     StructuredDatasetDecoder,
     StructuredDatasetEncoder,
     StructuredDatasetTransformerEngine,
 )
 
 
+def register_csv_handlers():
+
+    from .basic_dfs import CSVToPandasDecodingHandler, PandasToCSVEncodingHandler
+
+    StructuredDatasetTransformerEngine.register(PandasToCSVEncodingHandler(), default_format_for_type=True)
+    StructuredDatasetTransformerEngine.register(CSVToPandasDecodingHandler(), default_format_for_type=True)
+
+
 def register_pandas_handlers():
     import pandas as pd
 
     from .basic_dfs import PandasToParquetEncodingHandler, ParquetToPandasDecodingHandler
 
     StructuredDatasetTransformerEngine.register(PandasToParquetEncodingHandler(), default_format_for_type=True)
     StructuredDatasetTransformerEngine.register(ParquetToPandasDecodingHandler(), default_format_for_type=True)
```

### Comparing `flytekit-1.9.0a0/flytekit/types/structured/basic_dfs.py` & `flytekit-1.9.1/flytekit/types/structured/basic_dfs.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from flytekit import FlyteContext, logger
 from flytekit.configuration import DataConfig
 from flytekit.core.data_persistence import s3_setup_args
 from flytekit.models import literals
 from flytekit.models.literals import StructuredDatasetMetadata
 from flytekit.models.types import StructuredDatasetType
 from flytekit.types.structured.structured_dataset import (
+    CSV,
     PARQUET,
     StructuredDataset,
     StructuredDatasetDecoder,
     StructuredDatasetEncoder,
 )
 
 T = TypeVar("T")
@@ -31,14 +32,62 @@
     if protocol == "s3":
         kwargs = s3_setup_args(cfg.s3, anon)
         if kwargs:
             return kwargs
     return None
 
 
+class PandasToCSVEncodingHandler(StructuredDatasetEncoder):
+    def __init__(self):
+        super().__init__(pd.DataFrame, None, CSV)
+
+    def encode(
+        self,
+        ctx: FlyteContext,
+        structured_dataset: StructuredDataset,
+        structured_dataset_type: StructuredDatasetType,
+    ) -> literals.StructuredDataset:
+        uri = typing.cast(str, structured_dataset.uri) or ctx.file_access.get_random_remote_directory()
+        if not ctx.file_access.is_remote(uri):
+            Path(uri).mkdir(parents=True, exist_ok=True)
+        path = os.path.join(uri, ".csv")
+        df = typing.cast(pd.DataFrame, structured_dataset.dataframe)
+        df.to_csv(
+            path,
+            index=False,
+            storage_options=get_storage_options(ctx.file_access.data_config, path),
+        )
+        structured_dataset_type.format = CSV
+        return literals.StructuredDataset(uri=uri, metadata=StructuredDatasetMetadata(structured_dataset_type))
+
+
+class CSVToPandasDecodingHandler(StructuredDatasetDecoder):
+    def __init__(self):
+        super().__init__(pd.DataFrame, None, CSV)
+
+    def decode(
+        self,
+        ctx: FlyteContext,
+        flyte_value: literals.StructuredDataset,
+        current_task_metadata: StructuredDatasetMetadata,
+    ) -> pd.DataFrame:
+        uri = flyte_value.uri
+        columns = None
+        kwargs = get_storage_options(ctx.file_access.data_config, uri)
+        path = os.path.join(uri, ".csv")
+        if current_task_metadata.structured_dataset_type and current_task_metadata.structured_dataset_type.columns:
+            columns = [c.name for c in current_task_metadata.structured_dataset_type.columns]
+        try:
+            return pd.read_csv(path, usecols=columns, storage_options=kwargs)
+        except NoCredentialsError:
+            logger.debug("S3 source detected, attempting anonymous S3 access")
+            kwargs = get_storage_options(ctx.file_access.data_config, uri, anon=True)
+            return pd.read_csv(path, usecols=columns, storage_options=kwargs)
+
+
 class PandasToParquetEncodingHandler(StructuredDatasetEncoder):
     def __init__(self):
         super().__init__(pd.DataFrame, None, PARQUET)
 
     def encode(
         self,
         ctx: FlyteContext,
```

### Comparing `flytekit-1.9.0a0/flytekit/types/structured/bigquery.py` & `flytekit-1.9.1/flytekit/types/structured/bigquery.py`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/flytekit/types/structured/structured_dataset.py` & `flytekit-1.9.1/flytekit/types/structured/structured_dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import types
 import typing
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Dict, Generator, Optional, Type, Union
 
 import _datetime
-from dataclasses_json import config, dataclass_json
+from dataclasses_json import DataClassJsonMixin, config
 from fsspec.utils import get_protocol
 from marshmallow import fields
 from typing_extensions import Annotated, TypeAlias, get_args, get_origin
 
 from flytekit import lazy_module
 from flytekit.core.context_manager import FlyteContext, FlyteContextManager
 from flytekit.core.type_engine import TypeEngine, TypeTransformer
@@ -34,21 +34,21 @@
 DF = typing.TypeVar("DF")  # Dataframe type
 
 # For specifying the storage formats of StructuredDatasets. It's just a string, nothing fancy.
 StructuredDatasetFormat: TypeAlias = str
 
 # Storage formats
 PARQUET: StructuredDatasetFormat = "parquet"
+CSV: StructuredDatasetFormat = "csv"
 GENERIC_FORMAT: StructuredDatasetFormat = ""
 GENERIC_PROTOCOL: str = "generic protocol"
 
 
-@dataclass_json
 @dataclass
-class StructuredDataset(object):
+class StructuredDataset(DataClassJsonMixin):
     """
     This is the user facing StructuredDataset class. Please don't confuse it with the literals.StructuredDataset
     class (that is just a model, a Python class representation of the protobuf).
     """
 
     uri: typing.Optional[str] = field(default=None, metadata=config(mm_field=fields.String()))
     file_format: typing.Optional[str] = field(default=GENERIC_FORMAT, metadata=config(mm_field=fields.String()))
@@ -386,15 +386,15 @@
 
         except KeyError:
             ...
 
         if protocol_specific_handler or fsspec_handler or single_handler:
             return protocol_specific_handler or fsspec_handler or single_handler
         else:
-            raise ValueError(f"Failed to find a handler for {df_type}, protocol {protocol}, fmt |{format}|")
+            raise ValueError(f"Failed to find a handler for {df_type}, protocol [{protocol}], fmt ['{format}']")
 
     @classmethod
     def get_encoder(cls, df_type: Type, protocol: str, format: str):
         return cls._finder(StructuredDatasetTransformerEngine.ENCODERS, df_type, protocol, format)
 
     @classmethod
     def get_decoder(cls, df_type: Type, protocol: str, format: str):
```

### Comparing `flytekit-1.9.0a0/flytekit.egg-info/PKG-INFO` & `flytekit-1.9.1/flytekit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekit
-Version: 1.9.0a0
+Version: 1.9.1
 Summary: Flyte SDK for Python
 Home-page: https://github.com/flyteorg/flytekit
 Maintainer: Flyte Contributors
 Maintainer-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flytekit Version: 1.9.0a0 Summary: Flyte SDK for
+Metadata-Version: 2.1 Name: flytekit Version: 1.9.1 Summary: Flyte SDK for
 Python Home-page: https://github.com/flyteorg/flytekit Maintainer: Flyte
 Contributors Maintainer-email: admin@flyte.org License: apache2 Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
```

### Comparing `flytekit-1.9.0a0/flytekit.egg-info/SOURCES.txt` & `flytekit-1.9.1/flytekit.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 flytekit/configuration/__init__.py
 flytekit/configuration/default_images.py
 flytekit/configuration/feature_flags.py
 flytekit/configuration/file.py
 flytekit/configuration/internal.py
 flytekit/core/__init__.py
 flytekit/core/annotation.py
+flytekit/core/array_node_map_task.py
 flytekit/core/base_sql_task.py
 flytekit/core/base_task.py
 flytekit/core/checkpointer.py
 flytekit/core/class_based_resolver.py
 flytekit/core/condition.py
 flytekit/core/constants.py
 flytekit/core/container_task.py
@@ -102,18 +103,20 @@
 flytekit/deck/html/__init__.py
 flytekit/deck/html/template.html
 flytekit/exceptions/__init__.py
 flytekit/exceptions/base.py
 flytekit/exceptions/scopes.py
 flytekit/exceptions/system.py
 flytekit/exceptions/user.py
+flytekit/experimental/__init__.py
+flytekit/experimental/eager_function.py
 flytekit/extend/__init__.py
 flytekit/extend/backend/__init__.py
-flytekit/extend/backend/base_plugin.py
-flytekit/extend/backend/external_plugin_service.py
+flytekit/extend/backend/agent_service.py
+flytekit/extend/backend/base_agent.py
 flytekit/extras/__init__.py
 flytekit/extras/cloud_pickle_resolver.py
 flytekit/extras/pytorch/__init__.py
 flytekit/extras/pytorch/checkpoint.py
 flytekit/extras/pytorch/native.py
 flytekit/extras/sklearn/__init__.py
 flytekit/extras/sklearn/native.py
@@ -175,14 +178,18 @@
 flytekit/remote/backfill.py
 flytekit/remote/entities.py
 flytekit/remote/executions.py
 flytekit/remote/interface.py
 flytekit/remote/lazy_entity.py
 flytekit/remote/remote.py
 flytekit/remote/remote_callable.py
+flytekit/sensor/__init__.py
+flytekit/sensor/base_sensor.py
+flytekit/sensor/file_sensor.py
+flytekit/sensor/sensor_engine.py
 flytekit/testing/__init__.py
 flytekit/tools/__init__.py
 flytekit/tools/fast_registration.py
 flytekit/tools/ignore.py
 flytekit/tools/interactive.py
 flytekit/tools/module_loader.py
 flytekit/tools/repo.py
@@ -191,14 +198,16 @@
 flytekit/tools/subprocess.py
 flytekit/tools/translator.py
 flytekit/types/__init__.py
 flytekit/types/directory/__init__.py
 flytekit/types/directory/types.py
 flytekit/types/file/__init__.py
 flytekit/types/file/file.py
+flytekit/types/iterator/__init__.py
+flytekit/types/iterator/iterator.py
 flytekit/types/numpy/__init__.py
 flytekit/types/numpy/ndarray.py
 flytekit/types/pickle/__init__.py
 flytekit/types/pickle/pickle.py
 flytekit/types/schema/__init__.py
 flytekit/types/schema/types.py
 flytekit/types/schema/types_pandas.py
```

### Comparing `flytekit-1.9.0a0/flytekit.egg-info/requires.txt` & `flytekit-1.9.1/flytekit.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 googleapis-common-protos>=1.57
-flyteidl>=1.5.4
+flyteidl>=1.5.14
 wheel<1.0.0,>=0.30.0
 pandas<2.0.0,>=1.0.0
 pyarrow<11.0.0,>=4.0.0
 click<9.0,>=6.6
 croniter<4.0.0,>=0.3.20
 deprecated<2.0,>=1.0
 docker<7.0.0,>=4.0.0
 python-dateutil>=2.1
-grpcio<2.0,>=1.50.0
-grpcio-status<2.0,>=1.50.0
+grpcio!=1.55.0,<1.53.1,<2.0,>=1.50.0
+grpcio-status!=1.55.0,<1.53.1,<2.0,>=1.50.0
 importlib-metadata
 fsspec>=2023.3.0
 adlfs
 s3fs>=0.6.0
 gcsfs
 pyopenssl
 joblib
 python-json-logger>=2.0.0
 pytimeparse<2.0.0,>=1.1.8
 pytz
-pyyaml
+pyyaml!=5.4.0,!=5.4.1,!=6.0.0
 keyring>=18.0.1
 requests<3.0.0,>=2.18.4
-responses>=0.10.7
 sortedcontainers<3.0.0,>=1.5.9
 statsd<4.0.0,>=3.0.0
 urllib3<2.0.0,>=1.22
 wrapt<2.0.0,>=1.0.0
-dataclasses-json>=0.5.2
+dataclasses-json<0.5.12,>=0.5.2
 marshmallow-jsonschema>=0.12.0
+marshmallow-enum
 natsort>=7.0.1
 docker-image-py>=0.1.10
 typing_extensions
 docstring-parser>=0.9.0
 diskcache>=5.2.1
 cloudpickle>=2.0.0
 cookiecutter>=1.7.3
 numpy
 gitpython
 kubernetes>=12.0.1
 rich
 rich_click
-
-[:python_version < "3.8.0"]
-singledispatchmethod
+jsonpickle
```

### Comparing `flytekit-1.9.0a0/flytekit_scripts/flytekit_build_image.sh` & `flytekit-1.9.1/flytekit_scripts/flytekit_build_image.sh`

 * *Files identical despite different names*

### Comparing `flytekit-1.9.0a0/setup.py` & `flytekit-1.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup  # noqa
 
 extras_require = {}
 
-__version__ = "1.9.0a0"
+__version__ = "1.9.1"
 
 setup(
     name="flytekit",
     version=__version__,
     maintainer="Flyte Contributors",
     maintainer_email="admin@flyte.org",
     packages=find_packages(
@@ -25,60 +25,61 @@
             "pyflyte-map-execute=flytekit.bin.entrypoint:map_execute_task_cmd",
             "pyflyte=flytekit.clis.sdk_in_container.pyflyte:main",
             "flyte-cli=flytekit.clis.flyte_cli.main:_flyte_cli",
         ]
     },
     install_requires=[
         "googleapis-common-protos>=1.57",
-        "flyteidl>=1.5.4",
+        "flyteidl>=1.5.14",
         "wheel>=0.30.0,<1.0.0",
         "pandas>=1.0.0,<2.0.0",
         "pyarrow>=4.0.0,<11.0.0",
         "click>=6.6,<9.0",
         "croniter>=0.3.20,<4.0.0",
         "deprecated>=1.0,<2.0",
         "docker>=4.0.0,<7.0.0",
         "python-dateutil>=2.1",
         # Restrict grpcio and grpcio-status.  Version 1.50.0 pulls in a version of protobuf that is not compatible
         # with the old protobuf library (as described in https://developers.google.com/protocol-buffers/docs/news/2022-05-06)
-        "grpcio>=1.50.0,<2.0",
-        "grpcio-status>=1.50.0,<2.0",
+        "grpcio>=1.50.0,!=1.55.0,<1.53.1,<2.0",
+        "grpcio-status>=1.50.0,!=1.55.0,<1.53.1,<2.0",
         "importlib-metadata",
         "fsspec>=2023.3.0",
         "adlfs",
         "s3fs>=0.6.0",
         "gcsfs",
         "pyopenssl",
         "joblib",
         "python-json-logger>=2.0.0",
         "pytimeparse>=1.1.8,<2.0.0",
         "pytz",
-        "pyyaml",
+        "pyyaml!=6.0.0,!=5.4.0,!=5.4.1",  # pyyaml is broken with cython 3: https://github.com/yaml/pyyaml/issues/601
         "keyring>=18.0.1",
         "requests>=2.18.4,<3.0.0",
-        "responses>=0.10.7",
         "sortedcontainers>=1.5.9,<3.0.0",
         "statsd>=3.0.0,<4.0.0",
         "urllib3>=1.22,<2.0.0",
         "wrapt>=1.0.0,<2.0.0",
-        "dataclasses-json>=0.5.2",
+        # TODO: remove upper-bound after fixing change in contract
+        "dataclasses-json>=0.5.2,<0.5.12",
         "marshmallow-jsonschema>=0.12.0",
+        "marshmallow-enum",
         "natsort>=7.0.1",
         "docker-image-py>=0.1.10",
-        "singledispatchmethod; python_version < '3.8.0'",
         "typing_extensions",
         "docstring-parser>=0.9.0",
         "diskcache>=5.2.1",
         "cloudpickle>=2.0.0",
         "cookiecutter>=1.7.3",
         "numpy",
         "gitpython",
         "kubernetes>=12.0.1",
         "rich",
         "rich_click",
+        "jsonpickle",
     ],
     extras_require=extras_require,
     scripts=[
         "flytekit_scripts/flytekit_build_image.sh",
         "flytekit_scripts/flytekit_venv",
         "flytekit/bin/entrypoint.py",
     ],
```

