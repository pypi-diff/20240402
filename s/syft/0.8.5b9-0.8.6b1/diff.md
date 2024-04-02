# Comparing `tmp/syft-0.8.5b9.tar.gz` & `tmp/syft-0.8.6b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syft-0.8.5b9.tar", last modified: Mon Mar 18 06:47:13 2024, max compression
+gzip compressed data, was "syft-0.8.6b1.tar", last modified: Fri Mar 22 16:28:17 2024, max compression
```

## Comparing `syft-0.8.5b9.tar` & `syft-0.8.6b1.tar`

### file list

```diff
@@ -1,309 +1,311 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.352193 syft-0.8.5b9/
--rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-03-18 06:44:05.000000 syft-0.8.5b9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-18 06:44:05.000000 syft-0.8.5b9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    22897 2024-03-18 06:47:13.352193 syft-0.8.5b9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    18474 2024-03-18 06:45:05.000000 syft-0.8.5b9/PYPI.md
--rw-r--r--   0 runner    (1001) docker     (127)    17304 2024-03-18 06:44:05.000000 syft-0.8.5b9/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-18 06:44:05.000000 syft-0.8.5b9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-18 06:47:13.352193 syft-0.8.5b9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-18 06:44:05.000000 syft-0.8.5b9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.288193 syft-0.8.5b9/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.296193 syft-0.8.5b9/src/syft/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-18 06:44:35.000000 syft-0.8.5b9/src/syft/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-03-18 06:44:35.000000 syft-0.8.5b9/src/syft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/abstract_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.296193 syft-0.8.5b9/src/syft/capnp/
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/capnp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/capnp/iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/capnp/kv_iterable.capnp
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/capnp/recursive_serde.capnp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.300193 syft-0.8.5b9/src/syft/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36422 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/client/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46083 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/client/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)    18906 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/client/domain_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/client/enclave_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/client/gateway_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/client/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-03-18 06:46:14.000000 syft-0.8.5b9/src/syft/client/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/client/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/client/syncing.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/client/user_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.304193 syft-0.8.5b9/src/syft/custom_worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/custom_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/custom_worker/builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/custom_worker/builder_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/custom_worker/builder_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/custom_worker/builder_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/custom_worker/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/custom_worker/k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/custom_worker/runner_k8s.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/custom_worker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.304193 syft-0.8.5b9/src/syft/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/exceptions/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/exceptions/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.304193 syft-0.8.5b9/src/syft/external/
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.304193 syft-0.8.5b9/src/syft/external/oblv/
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/external/oblv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/external/oblv/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/external/oblv/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/external/oblv/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/external/oblv/deployment_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/external/oblv/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/external/oblv/oblv_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/external/oblv/oblv_keys_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/external/oblv/oblv_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13721 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/external/oblv/oblv_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/gevent_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.304193 syft-0.8.5b9/src/syft/img/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/img/base64.py
--rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/img/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/img/small-grid-symbol-logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.308193 syft-0.8.5b9/src/syft/node/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/node/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/node/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/node/enclave.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/node/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)    63571 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/node/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/node/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/node/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/node/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/node/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/node/worker_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.308193 syft-0.8.5b9/src/syft/protocol/
--rw-r--r--   0 runner    (1001) docker     (127)    22541 2024-03-18 06:46:14.000000 syft-0.8.5b9/src/syft/protocol/data_protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    50633 2024-03-18 06:44:56.000000 syft-0.8.5b9/src/syft/protocol/protocol_version.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.308193 syft-0.8.5b9/src/syft/protocol/releases/
--rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/protocol/releases/0.8.2.json
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/protocol/releases/0.8.3.json
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/protocol/releases/0.8.4.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.312193 syft-0.8.5b9/src/syft/serde/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/array.py
--rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/arrow.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/capnp.py
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/lib_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/lib_service_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/mock.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/recursive.py
--rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/recursive_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/signature.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/serde/third_party.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.312193 syft-0.8.5b9/src/syft/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.316193 syft-0.8.5b9/src/syft/service/action/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/action/action_data_empty.py
--rw-r--r--   0 runner    (1001) docker     (127)    16748 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/action/action_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/action/action_graph_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    71240 2024-03-18 06:45:10.000000 syft-0.8.5b9/src/syft/service/action/action_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/action/action_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)    38474 2024-03-18 06:46:14.000000 syft-0.8.5b9/src/syft/service/action/action_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/action/action_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/action/action_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/action/numpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/action/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/action/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/action/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.316193 syft-0.8.5b9/src/syft/service/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/blob_storage/remote_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/blob_storage/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/blob_storage/stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.316193 syft-0.8.5b9/src/syft/service/code/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/code/code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/code/status_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/code/unparse.py
--rw-r--r--   0 runner    (1001) docker     (127)    55598 2024-03-18 06:46:14.000000 syft-0.8.5b9/src/syft/service/code/user_code.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/code/user_code_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)    22789 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/code/user_code_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/code/user_code_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/code/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.320193 syft-0.8.5b9/src/syft/service/code_history/
--rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/code_history/code_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/code_history/code_history_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/code_history/code_history_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.320193 syft-0.8.5b9/src/syft/service/data_subject/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/data_subject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/data_subject/data_subject.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/data_subject/data_subject_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/data_subject/data_subject_member_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/data_subject/data_subject_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.320193 syft-0.8.5b9/src/syft/service/dataset/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28883 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/dataset/dataset_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/dataset/dataset_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.320193 syft-0.8.5b9/src/syft/service/enclave/
--rw-r--r--   0 runner    (1001) docker     (127)     6581 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/enclave/enclave_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.320193 syft-0.8.5b9/src/syft/service/job/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/job/job_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    22622 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/job/job_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.320193 syft-0.8.5b9/src/syft/service/log/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/log/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/log/log_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/log/log_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.320193 syft-0.8.5b9/src/syft/service/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/metadata/metadata_service.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/metadata/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/metadata/node_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.324193 syft-0.8.5b9/src/syft/service/network/
--rw-r--r--   0 runner    (1001) docker     (127)    19533 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/network/network_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/network/node_peer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/network/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.324193 syft-0.8.5b9/src/syft/service/notification/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/notification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/notification/email_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/notification/notification_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/notification/notification_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/notification/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.324193 syft-0.8.5b9/src/syft/service/notifier/
--rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/notifier/notifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/notifier/notifier_enums.py
--rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/notifier/notifier_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/notifier/notifier_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/notifier/smtp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.324193 syft-0.8.5b9/src/syft/service/object_search/
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/object_search/migration_state_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/object_search/object_migration_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.324193 syft-0.8.5b9/src/syft/service/output/
--rw-r--r--   0 runner    (1001) docker     (127)     8906 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/output/output_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.324193 syft-0.8.5b9/src/syft/service/policy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25602 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/policy/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/policy/policy_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/policy/user_policy_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.328193 syft-0.8.5b9/src/syft/service/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-03-18 06:46:14.000000 syft-0.8.5b9/src/syft/service/project/project.py
--rw-r--r--   0 runner    (1001) docker     (127)    15911 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/project/project_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/project/project_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.328193 syft-0.8.5b9/src/syft/service/queue/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/queue/base_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/queue/queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/queue/queue_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/queue/queue_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    33929 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/queue/zmq_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.328193 syft-0.8.5b9/src/syft/service/request/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49702 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/request/request.py
--rw-r--r--   0 runner    (1001) docker     (127)    11465 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/request/request_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/request/request_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.328193 syft-0.8.5b9/src/syft/service/settings/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/settings/migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/settings/settings_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/settings/settings_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.332193 syft-0.8.5b9/src/syft/service/sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29637 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/sync/diff_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/sync/sync_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/sync/sync_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/sync/sync_state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.332193 syft-0.8.5b9/src/syft/service/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/user/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/user/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/user/user_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/user/user_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/user/user_stash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.332193 syft-0.8.5b9/src/syft/service/veilid/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/veilid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/veilid/veilid_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/veilid/veilid_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.336193 syft-0.8.5b9/src/syft/service/worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/image_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/image_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/image_registry_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/image_registry_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/worker_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/worker_image_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/worker_image_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/worker_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    25667 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/worker_pool_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/worker_pool_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/worker_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/service/worker/worker_stash.py
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/stable_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.336193 syft-0.8.5b9/src/syft/store/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.336193 syft-0.8.5b9/src/syft/store/blob_storage/
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/store/blob_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/store/blob_storage/on_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/store/blob_storage/seaweedfs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/store/dict_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    25606 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/store/document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    25135 2024-03-18 06:46:14.000000 syft-0.8.5b9/src/syft/store/kv_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/store/linked_obj.py
--rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/store/locks.py
--rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/store/mongo_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/store/mongo_codecs.py
--rw-r--r--   0 runner    (1001) docker     (127)    31542 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/store/mongo_document_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    16066 2024-03-18 06:46:14.000000 syft-0.8.5b9/src/syft/store/sqlite_document_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.340193 syft-0.8.5b9/src/syft/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/dicttuple.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/grid_url.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/identity.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/syft_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/syft_migration.py
--rw-r--r--   0 runner    (1001) docker     (127)    37205 2024-03-18 06:46:14.000000 syft-0.8.5b9/src/syft/types/syft_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/syncable_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/transforms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/twin_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/types/uid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.344193 syft-0.8.5b9/src/syft/util/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/_std_stream_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/autoreload.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/experimental_flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/filterwarnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/fonts.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/jax_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.344193 syft-0.8.5b9/src/syft/util/notebook_ui/
--rw-r--r--   0 runner    (1001) docker     (127)    28420 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/notebook_ui/notebook_addons.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/trace_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)    24446 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-18 06:44:05.000000 syft-0.8.5b9/src/syft/util/version_compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 06:47:13.344193 syft-0.8.5b9/src/syft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22897 2024-03-18 06:47:13.000000 syft-0.8.5b9/src/syft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-03-18 06:47:13.000000 syft-0.8.5b9/src/syft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 06:47:13.000000 syft-0.8.5b9/src/syft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-18 06:47:13.000000 syft-0.8.5b9/src/syft.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 06:44:36.000000 syft-0.8.5b9/src/syft.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-18 06:47:13.000000 syft-0.8.5b9/src/syft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-18 06:47:13.000000 syft-0.8.5b9/src/syft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.068658 syft-0.8.6b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11843 2024-03-22 16:25:00.000000 syft-0.8.6b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-22 16:25:00.000000 syft-0.8.6b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-03-22 16:28:17.068658 syft-0.8.6b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    18569 2024-03-22 16:26:03.000000 syft-0.8.6b1/PYPI.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17399 2024-03-22 16:25:00.000000 syft-0.8.6b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-22 16:25:00.000000 syft-0.8.6b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-03-22 16:28:17.072658 syft-0.8.6b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-22 16:25:00.000000 syft-0.8.6b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.004657 syft-0.8.6b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.012657 syft-0.8.6b1/src/syft/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-22 16:25:31.000000 syft-0.8.6b1/src/syft/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)     6312 2024-03-22 16:25:31.000000 syft-0.8.6b1/src/syft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/abstract_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.016657 syft-0.8.6b1/src/syft/capnp/
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/capnp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/capnp/iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/capnp/kv_iterable.capnp
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/capnp/recursive_serde.capnp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.016657 syft-0.8.6b1/src/syft/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36986 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46083 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18906 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/domain_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7795 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/enclave_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6359 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/gateway_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14936 2024-03-22 16:27:15.000000 syft-0.8.6b1/src/syft/client/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/syncing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/client/user_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.020657 syft-0.8.6b1/src/syft/custom_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/builder_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13892 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/builder_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/builder_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7955 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/runner_k8s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/custom_worker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.020657 syft-0.8.6b1/src/syft/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/exceptions/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/exceptions/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.020657 syft-0.8.6b1/src/syft/external/
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.020657 syft-0.8.6b1/src/syft/external/oblv/
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12614 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/deployment_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/oblv_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/oblv_keys_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/oblv_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13721 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/external/oblv/oblv_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/gevent_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.024657 syft-0.8.6b1/src/syft/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/img/base64.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25535 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/img/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41764 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/img/small-grid-symbol-logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.024657 syft-0.8.6b1/src/syft/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/enclave.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60531 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8758 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/node/worker_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.024657 syft-0.8.6b1/src/syft/protocol/
+-rw-r--r--   0 runner    (1001) docker     (127)    22541 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/protocol/data_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/protocol/protocol_version.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.024657 syft-0.8.6b1/src/syft/protocol/releases/
+-rw-r--r--   0 runner    (1001) docker     (127)    21316 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/protocol/releases/0.8.2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/protocol/releases/0.8.3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/protocol/releases/0.8.4.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50490 2024-03-22 16:27:36.000000 syft-0.8.6b1/src/syft/protocol/releases/0.8.5.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.028658 syft-0.8.6b1/src/syft/serde/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3597 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/arrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/capnp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/lib_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11491 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/lib_service_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/recursive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11583 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/recursive_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/signature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/serde/third_party.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.028658 syft-0.8.6b1/src/syft/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.032657 syft-0.8.6b1/src/syft/service/action/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_data_empty.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16790 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_graph_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71240 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37785 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/service/action/action_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13954 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/action_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4875 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/action/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.032657 syft-0.8.6b1/src/syft/service/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/blob_storage/remote_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12866 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/blob_storage/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/blob_storage/stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/code/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/status_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/unparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55680 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/service/code/user_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/user_code_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24350 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/user_code_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/user_code_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/code_history/
+-rw-r--r--   0 runner    (1001) docker     (127)     4854 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code_history/code_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9177 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code_history/code_history_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/code_history/code_history_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3218 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/data_subject/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/data_subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/data_subject_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/data_subject_member_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/data_subject/data_subject_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/dataset/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28883 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/dataset/dataset_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/dataset/dataset_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/enclave/
+-rw-r--r--   0 runner    (1001) docker     (127)     6597 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/enclave/enclave_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/job/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9191 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/job/job_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22622 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/job/job_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.036658 syft-0.8.6b1/src/syft/service/log/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/log/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/log/log_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/log/log_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/metadata/metadata_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/metadata/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/metadata/node_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/network/
+-rw-r--r--   0 runner    (1001) docker     (127)    19533 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/network/network_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6564 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/network/node_peer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6027 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/network/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/notification/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14659 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/email_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10068 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/notification_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/notification_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notification/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/notifier/
+-rw-r--r--   0 runner    (1001) docker     (127)     7052 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/notifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/notifier_enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11728 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/notifier_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/notifier_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2180 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/notifier/smtp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/object_search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/object_search/migration_state_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/object_search/object_migration_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.040658 syft-0.8.6b1/src/syft/service/output/
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/output/output_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.044658 syft-0.8.6b1/src/syft/service/policy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27196 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/policy/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/policy/policy_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/policy/user_policy_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.044658 syft-0.8.6b1/src/syft/service/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49644 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/service/project/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15911 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/project/project_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/project/project_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.044658 syft-0.8.6b1/src/syft/service/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/base_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11250 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/queue_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5354 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/queue_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33929 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/queue/zmq_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.044658 syft-0.8.6b1/src/syft/service/request/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49952 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/request/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/request/request_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/request/request_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17295 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.048658 syft-0.8.6b1/src/syft/service/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/settings_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/settings/settings_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.048658 syft-0.8.6b1/src/syft/service/sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29637 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/diff_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11131 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/sync_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/sync_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/sync/sync_state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.048658 syft-0.8.6b1/src/syft/service/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/user_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/user_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/user/user_stash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.052658 syft-0.8.6b1/src/syft/service/veilid/
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/veilid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/veilid/veilid_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/veilid/veilid_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.052658 syft-0.8.6b1/src/syft/service/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/image_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/image_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/image_registry_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/image_registry_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22317 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10314 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_image_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2463 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_image_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9700 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25667 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_pool_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_pool_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11381 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3029 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/service/worker/worker_stash.py
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/stable_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.056658 syft-0.8.6b1/src/syft/store/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.056658 syft-0.8.6b1/src/syft/store/blob_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/blob_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/blob_storage/on_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/blob_storage/seaweedfs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/dict_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25674 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25135 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/store/kv_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/linked_obj.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11659 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10005 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/mongo_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/mongo_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31590 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/store/mongo_document_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15863 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/store/sqlite_document_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.060658 syft-0.8.6b1/src/syft/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11865 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/cache_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7492 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/dicttuple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/grid_url.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/identity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/syft_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/syft_migration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37205 2024-03-22 16:27:14.000000 syft-0.8.6b1/src/syft/types/syft_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/syncable_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8877 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/twin_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8245 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/types/uid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.064658 syft-0.8.6b1/src/syft/util/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9797 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/_std_stream_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/autoreload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/experimental_flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/filterwarnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/fonts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/jax_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.064658 syft-0.8.6b1/src/syft/util/notebook_ui/
+-rw-r--r--   0 runner    (1001) docker     (127)    28420 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/notebook_ui/notebook_addons.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5301 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2601 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6681 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/trace_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24446 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-22 16:25:00.000000 syft-0.8.6b1/src/syft/util/version_compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:28:17.064658 syft-0.8.6b1/src/syft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22992 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9149 2024-03-22 16:28:17.000000 syft-0.8.6b1/src/syft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:25:32.000000 syft-0.8.6b1/src/syft.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-22 16:28:16.000000 syft-0.8.6b1/src/syft.egg-info/top_level.txt
```

### Comparing `syft-0.8.5b9/LICENSE` & `syft-0.8.6b1/LICENSE`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/PKG-INFO` & `syft-0.8.6b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.5b9
+Version: 0.8.6b1
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -101,15 +101,15 @@
 Requires-Dist: coverage; extra == "test-plugins"
 Requires-Dist: faker; extra == "test-plugins"
 Requires-Dist: distro; extra == "test-plugins"
 
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://static.pepy.tech/badge/pysyft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
-<img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/title_syft_light.png" width="200px" />
+<img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/title_syft_light.png" width="200px" />
 
 Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
 ✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Podman` ✅ `Kubernetes`
 
@@ -120,49 +120,49 @@
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8.4,<0.8.5")
+sy.requires(">=0.8.5,<0.8.6")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8.4,<0.8.5")
+sy.requires(">=0.8.5,<0.8.6")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## PySyft in 10 minutes
 
-📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api">API Example Notebooks</a>
+📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api">API Example Notebooks</a>
 
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
 
 ## Deploy Kubernetes Helm Chart
 
 **Note**: Assuming we have a Kubernetes cluster already setup.
 
 #### 1. Add and update Helm repo for Syft
 
@@ -233,19 +233,20 @@
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
 - PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
 - PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
 
 # Versions
 
 `0.9.0` - Coming soon...  
-`0.8.5` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
-`0.8.4` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
+`0.8.6` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.5` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.8.4` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
 - `0.8.3` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.3/notebooks/api/0.8">API</a>
 - `0.8.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.2/notebooks/api/0.8">API</a>
 - `0.8.1` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 - `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
@@ -259,15 +260,15 @@
 PySyft (Beta): `pip install -U syft --pre`  
 PyGrid (Beta): `hagrid launch ... tag=beta`
 
 HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
 
 # What is Syft?
 
-<img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
+<img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
 
 `Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.
 
 ### Why should I use Syft?
 
 `Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.
 
@@ -277,39 +278,39 @@
 # Tutorials
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
 <p>Data Owner</p></div>
 </th>
 <th align="center">
 <img width="441" height="1">
-<div align="center"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
+<div align="center"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
 <p>Data Scientist</p></div>
 
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
 <p>Data Engineer</p>
 </div>
 </th>
 </tr>
 <tr>
 <td valign="top">
 
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/quickstart/data-owner/02-create-account-configure-pb.ipynb">Create Accounts</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/02-create-account-configure-pb.ipynb">Create Accounts</a>
 - Manage Privacy Budget</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/quickstart/data-owner/03-join-network.ipynb">Join a Network</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/03-join-network.ipynb">Join a Network</a>
 - Learn how PETs streamline Data Policies
 
 </td>
 <td valign="top">
 
 - Install Syft</a>
 - Connect to a Domain</a>
@@ -389,25 +390,25 @@
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
 
-<a href="https://slack.openmined.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
+<a href="https://slack.openmined.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
 
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
 
 <p align="left"><sub><sup>
 🎥 <a href="https://www.youtube.com/watch?v=qVf0tPBzr2k">PETs: Remote Data Science Unleashed - R gov 2021</a><br />
 🎥 <a href="https://youtu.be/sCoDWKTbh3s?list=PL_lsbAsL_o2BQKXG7mkGFA8LSApCnhljL">Introduction to Remote Data Science - PyTorch 2021</a><br />
 🎥 <a href="https://youtu.be/kzLeTz_vIeQ?list=PL_lsbAsL_o2BtOz6KUfUI_Zla6Rg5dmyc">The Future of AI Tools - PyTorch 2020</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=4zrU54VIK6k&t=1s">Privacy Preserving AI - MIT Deep Learning Series</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=Pr4erdusiW0">Privacy-Preserving Data Science - TWiML Talk #241</a><br />
@@ -418,106 +419,106 @@
 </sup></sup></p>
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
 
-<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
+<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
 
 </div>
 </th>
 </tr>
 </table>
 
 # Courses
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
+<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
+<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
 </div>
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
+<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
 </div>
 </th>
 </tr>
 </table>
 
 # Contributors
 
 OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
 
 # Supporters
 
 <table border="0">
 <tr>
 <th align="center">
-<a href="https://sloan.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_sloan.png" /></a>
+<a href="https://sloan.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_sloan.png" /></a>
 </th>
 <th align="center">
-<a href="https://opensource.fb.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_meta.png" /></a>
+<a href="https://opensource.fb.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_meta.png" /></a>
 </th>
 <th align="center">
-<a href="https://pytorch.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_torch.png" /></a>
+<a href="https://pytorch.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_torch.png" /></a>
 </th>
 <th align="center">
 <a href="https://www.dpmc.govt.nz/">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_nz_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_nz_light.png" />
 </a>
 </th>
 <th align="center">
-<a href="https://twitter.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_twitter.png" /></a>
+<a href="https://twitter.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_twitter.png" /></a>
 </th>
 <th align="center">
-<a href="https://google.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_google.png" /></a>
+<a href="https://google.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_google.png" /></a>
 </th>
 <th align="center">
-<a href="https://microsoft.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_microsoft.png" /></a>
+<a href="https://microsoft.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_microsoft.png" /></a>
 </th>
 <th align="center">
-<a href="https://omidyar.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_on.png" /></a>
+<a href="https://omidyar.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_on.png" /></a>
 </th>
 <th align="center">
-<a href="https://www.udacity.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_udacity.png" /></a>
+<a href="https://www.udacity.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_udacity.png" /></a>
 </th>
 <th align="center">
 <a href="https://www.centerfordigitalhealthinnovation.org/">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_cdhi_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_cdhi_light.png" />
 
 </a>
 </th>
 <th align="center">
 <a href="https://arkhn.org/">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_arkhn_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_arkhn_light.png" />
 </a>
 </th>
 </tr>
 </table>
 
 # Open Collective
 
 `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA. We are funded by our generous supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/opencollective_light.png" alt="Contributors" width="100%" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/opencollective_light.png" alt="Contributors" width="100%" />
 
 # Disclaimer
 
 Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.
 
 # License
```

### Comparing `syft-0.8.5b9/PYPI.md` & `syft-0.8.6b1/PYPI.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://static.pepy.tech/badge/pysyft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
-<img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/title_syft_light.png" width="200px" />
+<img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/title_syft_light.png" width="200px" />
 
 Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
 ✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Podman` ✅ `Kubernetes`
 
@@ -16,49 +16,49 @@
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8.4,<0.8.5")
+sy.requires(">=0.8.5,<0.8.6")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8.4,<0.8.5")
+sy.requires(">=0.8.5,<0.8.6")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## PySyft in 10 minutes
 
-📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api">API Example Notebooks</a>
+📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api">API Example Notebooks</a>
 
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
 
 ## Deploy Kubernetes Helm Chart
 
 **Note**: Assuming we have a Kubernetes cluster already setup.
 
 #### 1. Add and update Helm repo for Syft
 
@@ -129,19 +129,20 @@
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
 - PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
 - PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
 
 # Versions
 
 `0.9.0` - Coming soon...  
-`0.8.5` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
-`0.8.4` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
+`0.8.6` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.5` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.8.4` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
 - `0.8.3` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.3/notebooks/api/0.8">API</a>
 - `0.8.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.2/notebooks/api/0.8">API</a>
 - `0.8.1` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 - `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
@@ -155,15 +156,15 @@
 PySyft (Beta): `pip install -U syft --pre`  
 PyGrid (Beta): `hagrid launch ... tag=beta`
 
 HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
 
 # What is Syft?
 
-<img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
+<img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
 
 `Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.
 
 ### Why should I use Syft?
 
 `Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.
 
@@ -173,39 +174,39 @@
 # Tutorials
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
 <p>Data Owner</p></div>
 </th>
 <th align="center">
 <img width="441" height="1">
-<div align="center"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
+<div align="center"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
 <p>Data Scientist</p></div>
 
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
 <p>Data Engineer</p>
 </div>
 </th>
 </tr>
 <tr>
 <td valign="top">
 
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/quickstart/data-owner/02-create-account-configure-pb.ipynb">Create Accounts</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/02-create-account-configure-pb.ipynb">Create Accounts</a>
 - Manage Privacy Budget</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/quickstart/data-owner/03-join-network.ipynb">Join a Network</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/03-join-network.ipynb">Join a Network</a>
 - Learn how PETs streamline Data Policies
 
 </td>
 <td valign="top">
 
 - Install Syft</a>
 - Connect to a Domain</a>
@@ -285,25 +286,25 @@
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
 
-<a href="https://slack.openmined.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
+<a href="https://slack.openmined.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
 
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
 
 <p align="left"><sub><sup>
 🎥 <a href="https://www.youtube.com/watch?v=qVf0tPBzr2k">PETs: Remote Data Science Unleashed - R gov 2021</a><br />
 🎥 <a href="https://youtu.be/sCoDWKTbh3s?list=PL_lsbAsL_o2BQKXG7mkGFA8LSApCnhljL">Introduction to Remote Data Science - PyTorch 2021</a><br />
 🎥 <a href="https://youtu.be/kzLeTz_vIeQ?list=PL_lsbAsL_o2BtOz6KUfUI_Zla6Rg5dmyc">The Future of AI Tools - PyTorch 2020</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=4zrU54VIK6k&t=1s">Privacy Preserving AI - MIT Deep Learning Series</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=Pr4erdusiW0">Privacy-Preserving Data Science - TWiML Talk #241</a><br />
@@ -314,106 +315,106 @@
 </sup></sup></p>
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
 
-<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
+<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
 
 </div>
 </th>
 </tr>
 </table>
 
 # Courses
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
+<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
+<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
 </div>
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
+<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
 </div>
 </th>
 </tr>
 </table>
 
 # Contributors
 
 OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
 
 # Supporters
 
 <table border="0">
 <tr>
 <th align="center">
-<a href="https://sloan.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_sloan.png" /></a>
+<a href="https://sloan.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_sloan.png" /></a>
 </th>
 <th align="center">
-<a href="https://opensource.fb.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_meta.png" /></a>
+<a href="https://opensource.fb.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_meta.png" /></a>
 </th>
 <th align="center">
-<a href="https://pytorch.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_torch.png" /></a>
+<a href="https://pytorch.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_torch.png" /></a>
 </th>
 <th align="center">
 <a href="https://www.dpmc.govt.nz/">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_nz_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_nz_light.png" />
 </a>
 </th>
 <th align="center">
-<a href="https://twitter.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_twitter.png" /></a>
+<a href="https://twitter.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_twitter.png" /></a>
 </th>
 <th align="center">
-<a href="https://google.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_google.png" /></a>
+<a href="https://google.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_google.png" /></a>
 </th>
 <th align="center">
-<a href="https://microsoft.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_microsoft.png" /></a>
+<a href="https://microsoft.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_microsoft.png" /></a>
 </th>
 <th align="center">
-<a href="https://omidyar.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_on.png" /></a>
+<a href="https://omidyar.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_on.png" /></a>
 </th>
 <th align="center">
-<a href="https://www.udacity.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_udacity.png" /></a>
+<a href="https://www.udacity.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_udacity.png" /></a>
 </th>
 <th align="center">
 <a href="https://www.centerfordigitalhealthinnovation.org/">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_cdhi_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_cdhi_light.png" />
 
 </a>
 </th>
 <th align="center">
 <a href="https://arkhn.org/">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_arkhn_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_arkhn_light.png" />
 </a>
 </th>
 </tr>
 </table>
 
 # Open Collective
 
 `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA. We are funded by our generous supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/opencollective_light.png" alt="Contributors" width="100%" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/opencollective_light.png" alt="Contributors" width="100%" />
 
 # Disclaimer
 
 Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.
 
 # License
```

#### html2text {}

```diff
@@ -4,19 +4,19 @@
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_d_e_v_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_h_a_t_-_o_n_%_2_0_s_l_a_c_k_-
 _p_u_r_p_l_e_?_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_m_d_b_o_o_k_]
 
 [Syft Logo]Perform data science on `data` that remains in `someone else's`
 server # Quickstart â `Linux` â `macOS` â `Windows` â `Docker` â
 `Podman` â `Kubernetes` ## Install Client ```bash $ pip install -U syft
 [data_science] ``` ## Launch Server ```python # from Jupyter / Python import
-syft as sy sy.requires(">=0.8.4,<0.8.5") node = sy.orchestra.launch(name="my-
+syft as sy sy.requires(">=0.8.5,<0.8.6") node = sy.orchestra.launch(name="my-
 domain", port=8080, dev_mode=True, reset=True) ``` ```bash # or from the
 command line $ syft launch --name=my-domain --port=8080 --reset=True Starting
 syft-node server on 0.0.0.0:8080 ``` ## Launch Client ```python import syft as
-sy sy.requires(">=0.8.4,<0.8.5") domain_client = sy.login(port=8080,
+sy sy.requires(">=0.8.5,<0.8.6") domain_client = sy.login(port=8080,
 email="info@openmined.org", password="changethis") ``` ## PySyft in 10 minutes
 ð _A_P_I_ _E_x_a_m_p_l_e_ _N_o_t_e_b_o_o_k_s - _0_0_-_l_o_a_d_-_d_a_t_a_._i_p_y_n_b - _0_1_-_s_u_b_m_i_t_-_c_o_d_e_._i_p_y_n_b - _0_2_-
 _r_e_v_i_e_w_-_c_o_d_e_-_a_n_d_-_a_p_p_r_o_v_e_._i_p_y_n_b - _0_3_-_d_a_t_a_-_s_c_i_e_n_t_i_s_t_-_d_o_w_n_l_o_a_d_-_r_e_s_u_l_t_._i_p_y_n_b - _0_4_-
 _j_a_x_-_e_x_a_m_p_l_e_._i_p_y_n_b - _0_5_-_c_u_s_t_o_m_-_p_o_l_i_c_y_._i_p_y_n_b - _0_6_-_m_u_l_t_i_p_l_e_-_c_o_d_e_-_r_e_q_u_e_s_t_s_._i_p_y_n_b -
 _0_7_-_d_o_m_a_i_n_-_r_e_g_i_s_t_e_r_-_c_o_n_t_r_o_l_-_f_l_o_w_._i_p_y_n_b - _0_8_-_c_o_d_e_-_v_e_r_s_i_o_n_._i_p_y_n_b - _0_9_-_b_l_o_b_-
 _s_t_o_r_a_g_e_._i_p_y_n_b - _1_0_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_._i_p_y_n_b - _1_1_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_-_k_8_s_._i_p_y_n_b ##
 Deploy Kubernetes Helm Chart **Note**: Assuming we have a Kubernetes cluster
@@ -41,44 +41,44 @@
 `PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where
 `private data` lives ## Docs and Support - ð _D_o_c_s - `#support` on _S_l_a_c_k #
 Install Notes - HAGrid 0.3 Requires: ð `python` ð `git` - Run: `pip
 install -U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA Requires
 ðµ `hagrid`: - Run: `hagrid quickstart` - PySyft 0.8.1 Requires: ð `python
 3.10 - 3.12` - Run: `pip install -U syft` - PyGrid Requires: ð³ `docker`,
 ð¦¦ `podman` or â¸ï¸ `kubernetes` - Run: `hagrid launch ...` # Versions
-`0.9.0` - Coming soon... `0.8.5` (Beta) - `dev` branch ðð½ _A_P_I - Coming
-soon... `0.8.4` (Stable) - _A_P_I Deprecated: - `0.8.3` - _A_P_I - `0.8.2` - _A_P_I -
-`0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` - _C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d - `0.6.0` - _C_o_u_r_s_e_ _3
-- `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix - `0.2.0` - `0.5.0` PySyft and PyGrid use the
-same `version` and its best to match them up where possible. We release weekly
-betas which can be used in each context: PySyft (Stable): `pip install -U syft`
-PyGrid (Stable) `hagrid launch ... tag=latest` PySyft (Beta): `pip install -
-U syft --pre` PyGrid (Beta): `hagrid launch ... tag=beta` HAGrid is a cli /
-deployment tool so the latest version of `hagrid` is usually the best. # What
-is Syft? [Syft]`Syft` is OpenMined's `open source` stack that provides `secure`
-and `private` Data Science in Python. Syft decouples `private data` from model
-training, using techniques like [Federated Learning](https://ai.googleblog.com/
-2017/04/federated-learning-collaborative.html), [Differential Privacy](https://
-en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https:
-//en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-
-like interface and integration with `Deep Learning` frameworks, so that you as
-a `Data Scientist` can maintain your current workflow while using these new
-`privacy-enhancing techniques`. ### Why should I use Syft? `Syft` allows a
-`Data Scientist` to ask `questions` about a `dataset` and, within `privacy
-limits` set by the `data owner`, get `answers` to those `questions`, all
-without obtaining a `copy` of the data itself. We call this process `Remote
-Data Science`. It means in a wide variety of `domains` across society, the
-current `risks` of sharing information (`copying` data) with someone such as,
-privacy invasion, IP theft and blackmail will no longer prevent the vast
-`benefits` such as innovation, insights and scientific discovery which secure
-access will provide. No more cold calls to get `access` to a dataset. No more
-weeks of `wait times` to get a `result` on your `query`. It also means `1000x
-more data` in every domain. PySyft opens the doors to a streamlined Data
-Scientist `workflow`, all with the individual's `privacy` at its heart. #
-Terminology
+`0.9.0` - Coming soon... `0.8.6` (Beta) - `dev` branch ðð½ _A_P_I - Coming
+soon... `0.8.5` (Stable) - _A_P_I Deprecated: - `0.8.4` - _A_P_I - `0.8.3` - _A_P_I -
+`0.8.2` - _A_P_I - `0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` - _C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d -
+`0.6.0` - _C_o_u_r_s_e_ _3 - `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix - `0.2.0` - `0.5.0` PySyft
+and PyGrid use the same `version` and its best to match them up where possible.
+We release weekly betas which can be used in each context: PySyft (Stable):
+`pip install -U syft` PyGrid (Stable) `hagrid launch ... tag=latest` PySyft
+(Beta): `pip install -U syft --pre` PyGrid (Beta): `hagrid launch ... tag=beta`
+HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually
+the best. # What is Syft? [Syft]`Syft` is OpenMined's `open source` stack that
+provides `secure` and `private` Data Science in Python. Syft decouples `private
+data` from model training, using techniques like [Federated Learning](https://
+ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential
+Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted
+Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is
+done with a `numpy`-like interface and integration with `Deep Learning`
+frameworks, so that you as a `Data Scientist` can maintain your current
+workflow while using these new `privacy-enhancing techniques`. ### Why should I
+use Syft? `Syft` allows a `Data Scientist` to ask `questions` about a `dataset`
+and, within `privacy limits` set by the `data owner`, get `answers` to those
+`questions`, all without obtaining a `copy` of the data itself. We call this
+process `Remote Data Science`. It means in a wide variety of `domains` across
+society, the current `risks` of sharing information (`copying` data) with
+someone such as, privacy invasion, IP theft and blackmail will no longer
+prevent the vast `benefits` such as innovation, insights and scientific
+discovery which secure access will provide. No more cold calls to get `access`
+to a dataset. No more weeks of `wait times` to get a `result` on your `query`.
+It also means `1000x more data` in every domain. PySyft opens the doors to a
+streamlined Data Scientist `workflow`, all with the individual's `privacy` at
+its heart. # Terminology
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |                  [[IImmaaggee]]             |                 [[IImmaaggee]]              |
 |_ _ _ _ _ _ _ _ _?ð_?_?_?¨_?ð_?_?_?»_?â_?_?_?ð_?_?_?¼_ _DD_aa_tt_aa_ _OO_ww_nn_ee_rr_ss_ _ _ _|_ _ _ _ _ _?ð_?_?_?©_?ð_?_?_?½_?â_?_?_?ð_?_?_?¬_ _DD_aa_tt_aa_ _SS_cc_ii_ee_nn_tt_ii_ss_tt_ss_ _ |
 |Provide `datasets` which they would   |Are end `users` who desire to perform |
 |like to make available for `study` by |`computations` or `answer` a specific |
 |an `outside party` they may or may not|`question` using one or more data     |
 |_`_f_u_l_l_y_ _t_r_u_s_t_`_ _h_a_s_ _g_o_o_d_ _i_n_t_e_n_t_i_o_n_s_._ _ _ _ _|_o_w_n_e_r_s_'_ _`_d_a_t_a_s_e_t_s_`_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
@@ -111,15 +111,15 @@
 |_[[_II_mm_aa_gg_ee_]]_|_[[_II_mm_aa_gg_ee_]]_|_[[_II_mm_aa_gg_ee_]]|
 # Contributors OpenMined and Syft appreciates all contributors, if you would
 like to fix a bug or suggest a new feature, please see our [guidelines](https:/
 /openmined.github.io/PySyft/developer_guide/index.html).
 [Contributors]# Supporters
         _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//                  _[[_hh_tt_tt_pp_ss_::_//_//
 _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_// _rr_aa_ww_.._gg_ii_tt_hh_uu_bb_uu_ss_ee_rr_cc_oo_nn_tt_ee_nn_tt_.._cc_oo_mm_//
- _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._55_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._55_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._55_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._55_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._55_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._55_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._55_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._55_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._55_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._55_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._55_//
+ _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//    _OO_pp_ee_nn_MM_ii_nn_ee_dd_//_PP_yy_SS_yy_ff_tt_//_00_.._88_.._66_//
  _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____ss_ll_oo_aa_nn_.._pp_nn_gg_]]   _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____mm_ee_tt_aa_.._pp_nn_gg_]]    _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____tt_oo_rr_cc_hh_.._pp_nn_gg_]]          _dd_oo_cc_ss_//_ii_mm_gg_//          _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____tt_ww_ii_tt_tt_ee_rr_.._pp_nn_gg_]] _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____gg_oo_oo_gg_ll_ee_.._pp_nn_gg_]]          _dd_oo_cc_ss_//_ii_mm_gg_//            _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____oo_nn_.._pp_nn_gg_]]    _dd_oo_cc_ss_//_ii_mm_gg_//_ll_oo_gg_oo____uu_dd_aa_cc_ii_tt_yy_.._pp_nn_gg_]]         _dd_oo_cc_ss_//_ii_mm_gg_//                  _dd_oo_cc_ss_//_ii_mm_gg_//
                                                                                      _ll_oo_gg_oo____nn_zz____ll_ii_gg_hh_tt_.._pp_nn_gg_]]                                                              _ll_oo_gg_oo____mm_ii_cc_rr_oo_ss_oo_ff_tt_.._pp_nn_gg_]]                                                              _ll_oo_gg_oo____cc_dd_hh_ii____ll_ii_gg_hh_tt_.._pp_nn_gg_]]      _ll_oo_gg_oo____aa_rr_kk_hh_nn____ll_ii_gg_hh_tt_.._pp_nn_gg_]]
 # Open Collective `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA.
 We are funded by our generous supporters on _O_p_e_n_ _C_o_l_l_e_c_t_i_v_e.
 
 [Contributors]# Disclaimer Syft is under active development and is not yet
 ready for pilots on private data without our assistance. As early access
```

### Comparing `syft-0.8.5b9/README.md` & `syft-0.8.6b1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8.4,<0.8.5")
+sy.requires(">=0.8.5,<0.8.6")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8.4,<0.8.5")
+sy.requires(">=0.8.5,<0.8.6")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## PySyft in 10 minutes
 
 📝 <a href="notebooks/api">API Example Notebooks</a>
 
@@ -132,19 +132,20 @@
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
 - PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
 - PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
 
 # Versions
 
 `0.9.0` - Coming soon...  
-`0.8.5` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
-`0.8.4` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
+`0.8.6` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.5` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.8.4` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
 - `0.8.3` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.3/notebooks/api/0.8">API</a>
 - `0.8.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.2/notebooks/api/0.8">API</a>
 - `0.8.1` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 - `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
```

#### html2text {}

```diff
@@ -4,19 +4,19 @@
 _b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_d_e_v_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_h_a_t_-_o_n_%_2_0_s_l_a_c_k_-
 _p_u_r_p_l_e_?_l_o_g_o_=_s_l_a_c_k_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_r_e_a_d_-_d_o_c_s_-_y_e_l_l_o_w_?_l_o_g_o_=_m_d_b_o_o_k_]
 
 [Syft Logo]Perform data science on `data` that remains in `someone else's`
 server # Quickstart â `Linux` â `macOS` â `Windows` â `Docker` â
 `Podman` â `Kubernetes` ## Install Client ```bash $ pip install -U syft
 [data_science] ``` ## Launch Server ```python # from Jupyter / Python import
-syft as sy sy.requires(">=0.8.4,<0.8.5") node = sy.orchestra.launch(name="my-
+syft as sy sy.requires(">=0.8.5,<0.8.6") node = sy.orchestra.launch(name="my-
 domain", port=8080, dev_mode=True, reset=True) ``` ```bash # or from the
 command line $ syft launch --name=my-domain --port=8080 --reset=True Starting
 syft-node server on 0.0.0.0:8080 ``` ## Launch Client ```python import syft as
-sy sy.requires(">=0.8.4,<0.8.5") domain_client = sy.login(port=8080,
+sy sy.requires(">=0.8.5,<0.8.6") domain_client = sy.login(port=8080,
 email="info@openmined.org", password="changethis") ``` ## PySyft in 10 minutes
 ð _A_P_I_ _E_x_a_m_p_l_e_ _N_o_t_e_b_o_o_k_s - _0_0_-_l_o_a_d_-_d_a_t_a_._i_p_y_n_b - _0_1_-_s_u_b_m_i_t_-_c_o_d_e_._i_p_y_n_b - _0_2_-
 _r_e_v_i_e_w_-_c_o_d_e_-_a_n_d_-_a_p_p_r_o_v_e_._i_p_y_n_b - _0_3_-_d_a_t_a_-_s_c_i_e_n_t_i_s_t_-_d_o_w_n_l_o_a_d_-_r_e_s_u_l_t_._i_p_y_n_b - _0_4_-
 _j_a_x_-_e_x_a_m_p_l_e_._i_p_y_n_b - _0_5_-_c_u_s_t_o_m_-_p_o_l_i_c_y_._i_p_y_n_b - _0_6_-_m_u_l_t_i_p_l_e_-_c_o_d_e_-_r_e_q_u_e_s_t_s_._i_p_y_n_b -
 _0_7_-_d_o_m_a_i_n_-_r_e_g_i_s_t_e_r_-_c_o_n_t_r_o_l_-_f_l_o_w_._i_p_y_n_b - _0_8_-_c_o_d_e_-_v_e_r_s_i_o_n_._i_p_y_n_b - _0_9_-_b_l_o_b_-
 _s_t_o_r_a_g_e_._i_p_y_n_b - _1_0_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_._i_p_y_n_b - _1_1_-_c_o_n_t_a_i_n_e_r_-_i_m_a_g_e_s_-_k_8_s_._i_p_y_n_b ##
 Deploy Kubernetes Helm Chart **Note**: Assuming we have a Kubernetes cluster
@@ -41,44 +41,44 @@
 `PyGrid` = our ð³ `docker` / ð§ `vm` `Domain` & `Gateway` Servers where
 `private data` lives ## Docs and Support - ð _D_o_c_s - `#support` on _S_l_a_c_k #
 Install Notes - HAGrid 0.3 Requires: ð `python` ð `git` - Run: `pip
 install -U hagrid` - Interactive Install ð§ð½ââï¸ WizardBETA Requires
 ðµ `hagrid`: - Run: `hagrid quickstart` - PySyft 0.8.1 Requires: ð `python
 3.10 - 3.12` - Run: `pip install -U syft` - PyGrid Requires: ð³ `docker`,
 ð¦¦ `podman` or â¸ï¸ `kubernetes` - Run: `hagrid launch ...` # Versions
-`0.9.0` - Coming soon... `0.8.5` (Beta) - `dev` branch ðð½ _A_P_I - Coming
-soon... `0.8.4` (Stable) - _A_P_I Deprecated: - `0.8.3` - _A_P_I - `0.8.2` - _A_P_I -
-`0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` - _C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d - `0.6.0` - _C_o_u_r_s_e_ _3
-- `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix - `0.2.0` - `0.5.0` PySyft and PyGrid use the
-same `version` and its best to match them up where possible. We release weekly
-betas which can be used in each context: PySyft (Stable): `pip install -U syft`
-PyGrid (Stable) `hagrid launch ... tag=latest` PySyft (Beta): `pip install -
-U syft --pre` PyGrid (Beta): `hagrid launch ... tag=beta` HAGrid is a cli /
-deployment tool so the latest version of `hagrid` is usually the best. # What
-is Syft? [Syft]`Syft` is OpenMined's `open source` stack that provides `secure`
-and `private` Data Science in Python. Syft decouples `private data` from model
-training, using techniques like [Federated Learning](https://ai.googleblog.com/
-2017/04/federated-learning-collaborative.html), [Differential Privacy](https://
-en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https:
-//en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-
-like interface and integration with `Deep Learning` frameworks, so that you as
-a `Data Scientist` can maintain your current workflow while using these new
-`privacy-enhancing techniques`. ### Why should I use Syft? `Syft` allows a
-`Data Scientist` to ask `questions` about a `dataset` and, within `privacy
-limits` set by the `data owner`, get `answers` to those `questions`, all
-without obtaining a `copy` of the data itself. We call this process `Remote
-Data Science`. It means in a wide variety of `domains` across society, the
-current `risks` of sharing information (`copying` data) with someone such as,
-privacy invasion, IP theft and blackmail will no longer prevent the vast
-`benefits` such as innovation, insights and scientific discovery which secure
-access will provide. No more cold calls to get `access` to a dataset. No more
-weeks of `wait times` to get a `result` on your `query`. It also means `1000x
-more data` in every domain. PySyft opens the doors to a streamlined Data
-Scientist `workflow`, all with the individual's `privacy` at its heart. #
-Terminology
+`0.9.0` - Coming soon... `0.8.6` (Beta) - `dev` branch ðð½ _A_P_I - Coming
+soon... `0.8.5` (Stable) - _A_P_I Deprecated: - `0.8.4` - _A_P_I - `0.8.3` - _A_P_I -
+`0.8.2` - _A_P_I - `0.8.1` - _A_P_I - `0.8.0` - _A_P_I - `0.7.0` - _C_o_u_r_s_e_ _3_ _U_p_d_a_t_e_d -
+`0.6.0` - _C_o_u_r_s_e_ _3 - `0.5.1` - _C_o_u_r_s_e_ _2 + M1 Hotfix - `0.2.0` - `0.5.0` PySyft
+and PyGrid use the same `version` and its best to match them up where possible.
+We release weekly betas which can be used in each context: PySyft (Stable):
+`pip install -U syft` PyGrid (Stable) `hagrid launch ... tag=latest` PySyft
+(Beta): `pip install -U syft --pre` PyGrid (Beta): `hagrid launch ... tag=beta`
+HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually
+the best. # What is Syft? [Syft]`Syft` is OpenMined's `open source` stack that
+provides `secure` and `private` Data Science in Python. Syft decouples `private
+data` from model training, using techniques like [Federated Learning](https://
+ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential
+Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted
+Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is
+done with a `numpy`-like interface and integration with `Deep Learning`
+frameworks, so that you as a `Data Scientist` can maintain your current
+workflow while using these new `privacy-enhancing techniques`. ### Why should I
+use Syft? `Syft` allows a `Data Scientist` to ask `questions` about a `dataset`
+and, within `privacy limits` set by the `data owner`, get `answers` to those
+`questions`, all without obtaining a `copy` of the data itself. We call this
+process `Remote Data Science`. It means in a wide variety of `domains` across
+society, the current `risks` of sharing information (`copying` data) with
+someone such as, privacy invasion, IP theft and blackmail will no longer
+prevent the vast `benefits` such as innovation, insights and scientific
+discovery which secure access will provide. No more cold calls to get `access`
+to a dataset. No more weeks of `wait times` to get a `result` on your `query`.
+It also means `1000x more data` in every domain. PySyft opens the doors to a
+streamlined Data Scientist `workflow`, all with the individual's `privacy` at
+its heart. # Terminology
  _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ 
 |                  [[IImmaaggee]]             |                 [[IImmaaggee]]              |
 |_ _ _ _ _ _ _ _ _?ð_?_?_?¨_?ð_?_?_?»_?â_?_?_?ð_?_?_?¼_ _DD_aa_tt_aa_ _OO_ww_nn_ee_rr_ss_ _ _ _|_ _ _ _ _ _?ð_?_?_?©_?ð_?_?_?½_?â_?_?_?ð_?_?_?¬_ _DD_aa_tt_aa_ _SS_cc_ii_ee_nn_tt_ii_ss_tt_ss_ _ |
 |Provide `datasets` which they would   |Are end `users` who desire to perform |
 |like to make available for `study` by |`computations` or `answer` a specific |
 |an `outside party` they may or may not|`question` using one or more data     |
 |_`_f_u_l_l_y_ _t_r_u_s_t_`_ _h_a_s_ _g_o_o_d_ _i_n_t_e_n_t_i_o_n_s_._ _ _ _ _|_o_w_n_e_r_s_'_ _`_d_a_t_a_s_e_t_s_`_._ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ _ |
```

### Comparing `syft-0.8.5b9/setup.cfg` & `syft-0.8.6b1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = syft
-version = attr: "0.8.5-beta.9"
+version = attr: "0.8.6-beta.1"
 description = Perform numpy-like analysis on data that remains in someone elses server
 author = OpenMined
 author_email = info@openmined.org
 license = Apache-2.0
 long_description = file: PYPI.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 url = https://openmined.github.io/PySyft/
```

### Comparing `syft-0.8.5b9/src/syft/VERSION` & `syft-0.8.6b1/src/syft/VERSION`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Mono Repo Global Version
-__version__ = "0.8.5-beta.9"
+__version__ = "0.8.6-beta.1"
 # elsewhere we can call this file: `python VERSION` and simply take the stdout
 
 # stdlib
 import os
 import subprocess
 import sys
```

### Comparing `syft-0.8.5b9/src/syft/__init__.py` & `syft-0.8.6b1/src/syft/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.8.5-beta.9"
+__version__ = "0.8.6-beta.1"
 
 # stdlib
 from collections.abc import Callable
 import pathlib
 from pathlib import Path
 import sys
 from typing import Any
@@ -22,15 +22,15 @@
 from .client.registry import EnclaveRegistry  # noqa: F401
 from .client.registry import NetworkRegistry  # noqa: F401
 from .client.search import Search  # noqa: F401
 from .client.search import SearchResults  # noqa: F401
 from .client.user_settings import UserSettings  # noqa: F401
 from .client.user_settings import settings  # noqa: F401
 from .custom_worker.config import DockerWorkerConfig  # noqa: F401
-from .external import OBLV  # noqa: F401
+from .external import OBLV_ENABLED  # noqa: F401
 from .external import enable_external_lib  # noqa: F401
 from .node.credentials import SyftSigningKey  # noqa: F401
 from .node.domain import Domain  # noqa: F401
 from .node.enclave import Enclave  # noqa: F401
 from .node.gateway import Gateway  # noqa: F401
 from .node.server import serve_node  # noqa: F401
 from .node.server import serve_node as bind_worker  # noqa: F401
@@ -104,15 +104,15 @@
     #     \nTo switch to dark mode, please run `sy.options.color_theme = 'dark'`"
     #     )
     # )
 except:  # noqa: E722
     pass  # nosec
 
 # For server-side, to enable by environment variable
-if OBLV:
+if OBLV_ENABLED:
     enable_external_lib("oblv")
 
 
 def module_property(func: Any) -> Callable:
     """Decorator to turn module functions into properties.
     Function names must be prefixed with an underscore."""
     module = sys.modules[func.__module__]
```

### Comparing `syft-0.8.5b9/src/syft/abstract_node.py` & `syft-0.8.6b1/src/syft/abstract_node.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/client/api.py` & `syft-0.8.6b1/src/syft/client/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,23 +42,25 @@
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
 from ..service.service import UserLibConfigRegistry
 from ..service.service import UserServiceConfigRegistry
 from ..service.user.user_roles import ServiceRole
 from ..service.warnings import APIEndpointWarning
 from ..service.warnings import WarningContext
+from ..types.cache_object import CachedSyftObject
 from ..types.identity import Identity
 from ..types.syft_object import SYFT_OBJECT_VERSION_2
 from ..types.syft_object import SyftBaseObject
 from ..types.syft_object import SyftMigrationRegistry
 from ..types.syft_object import SyftObject
 from ..types.uid import LineageID
 from ..types.uid import UID
 from ..util.autoreload import autoreload_enabled
 from ..util.telemetry import instrument
+from ..util.util import prompt_warning_message
 from .connection import NodeConnection
 
 if TYPE_CHECKING:
     # relative
     from ..node import Node
     from ..service.job.job_stash import Job
 
@@ -578,14 +580,28 @@
         return annotation.copy_with(migrated_annotations_tuple)
     elif origin is not None:
         return origin[migrated_annotations_tuple]
     else:
         return migrated_annotation[0]
 
 
+def result_needs_api_update(api_call_result: Any) -> bool:
+    # relative
+    from ..service.request.request import Request
+    from ..service.request.request import UserCodeStatusChange
+
+    if isinstance(api_call_result, Request) and any(
+        isinstance(x, UserCodeStatusChange) for x in api_call_result.changes
+    ):
+        return True
+    if isinstance(api_call_result, SyftSuccess) and api_call_result.require_api_update:
+        return True
+    return False
+
+
 @instrument
 @serializable(
     attrs=[
         "endpoints",
         "node_uid",
         "node_name",
         "lib_endpoints",
@@ -735,33 +751,33 @@
         if self.connection is not None:
             signed_result = self.connection.make_call(signed_call)
         else:
             return SyftError(message="API connection is None")
 
         result = debox_signed_syftapicall_response(signed_result=signed_result)
 
+        if isinstance(result, CachedSyftObject):
+            if result.error_msg is not None:
+                prompt_warning_message(
+                    message=f"{result.error_msg}. Loading results from cache."
+                )
+            result = result.result
+
         if isinstance(result, OkErr):
             if result.is_ok():
-                res = result.ok()
-                # we update the api when we create objects that change it
-                self.update_api(res)
-                return res
+                result = result.ok()
             else:
-                return result.err()
+                result = result.err()
+        # we update the api when we create objects that change it
+        self.update_api(result)
         return result
 
     def update_api(self, api_call_result: Any) -> None:
         # TODO: hacky stuff with typing and imports to prevent circular imports
-        # relative
-        from ..service.request.request import Request
-        from ..service.request.request import UserCodeStatusChange
-
-        if isinstance(api_call_result, Request) and any(
-            isinstance(x, UserCodeStatusChange) for x in api_call_result.changes
-        ):
+        if result_needs_api_update(api_call_result):
             if self.refresh_api_callback is not None:
                 self.refresh_api_callback()
 
     @staticmethod
     def _add_route(
         api_module: APIModule, endpoint: APIEndpoint, endpoint_method: Callable
     ) -> None:
```

### Comparing `syft-0.8.5b9/src/syft/client/client.py` & `syft-0.8.6b1/src/syft/client/client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/client/connection.py` & `syft-0.8.6b1/src/syft/client/connection.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/client/deploy.py` & `syft-0.8.6b1/src/syft/client/deploy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/client/domain_client.py` & `syft-0.8.6b1/src/syft/client/domain_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/client/enclave_client.py` & `syft-0.8.6b1/src/syft/client/enclave_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/client/gateway_client.py` & `syft-0.8.6b1/src/syft/client/gateway_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/client/registry.py` & `syft-0.8.6b1/src/syft/client/registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/client/search.py` & `syft-0.8.6b1/src/syft/client/search.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/client/syncing.py` & `syft-0.8.6b1/src/syft/client/syncing.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/client/user_settings.py` & `syft-0.8.6b1/src/syft/client/user_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/custom_worker/builder.py` & `syft-0.8.6b1/src/syft/custom_worker/builder.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/custom_worker/builder_docker.py` & `syft-0.8.6b1/src/syft/custom_worker/builder_docker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/custom_worker/builder_k8s.py` & `syft-0.8.6b1/src/syft/custom_worker/builder_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/custom_worker/builder_types.py` & `syft-0.8.6b1/src/syft/custom_worker/builder_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/custom_worker/config.py` & `syft-0.8.6b1/src/syft/custom_worker/config.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/custom_worker/k8s.py` & `syft-0.8.6b1/src/syft/custom_worker/k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/custom_worker/runner_k8s.py` & `syft-0.8.6b1/src/syft/custom_worker/runner_k8s.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/custom_worker/utils.py` & `syft-0.8.6b1/src/syft/custom_worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/exceptions/exception.py` & `syft-0.8.6b1/src/syft/exceptions/exception.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/external/__init__.py` & `syft-0.8.6b1/src/syft/external/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 """This module contains all the external libraries that Syft supports.
 We lazy load the external libraries when they are needed.
 """
 
 # stdlib
 import importlib
 import os
+from typing import Any
 
 # relative
 from ..service.response import SyftError
 from ..service.response import SyftSuccess
+from ..service.service import AbstractService
 from ..util.util import str_to_bool
 
 # Contains all the external libraries that Syft supports.
 # Used to check if a library is supported
 # if the external library is not installed, we prompt the user
 # to install it with the pip package name.
 
-OBLV = str_to_bool(os.getenv("OBLV_ENABLED", "false"))
+OBLV_ENABLED = str_to_bool(os.getenv("OBLV_ENABLED", "false"))
 
 EXTERNAL_LIBS = {
     "oblv": {
         "pip_package_name": "oblv-ctl",
         "module_name": "oblv_ctl",
     }
 }
 
 
+def OblvServiceProvider(*args: Any, **kwargs: Any) -> type[AbstractService] | None:
+    if OBLV_ENABLED:
+        # relative
+        from .oblv.oblv_service import OblvService
+
+        return OblvService(*args, **kwargs)
+    return None
+
+
 def package_exists(package_name: str) -> bool:
     try:
         importlib.import_module(package_name)
         return True
     except ImportError:
         return False
```

### Comparing `syft-0.8.5b9/src/syft/external/oblv/__init__.py` & `syft-0.8.6b1/src/syft/external/oblv/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/external/oblv/deployment.py` & `syft-0.8.6b1/src/syft/external/oblv/deployment.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/external/oblv/deployment_client.py` & `syft-0.8.6b1/src/syft/external/oblv/deployment_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/external/oblv/exceptions.py` & `syft-0.8.6b1/src/syft/external/oblv/exceptions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/external/oblv/oblv_keys_stash.py` & `syft-0.8.6b1/src/syft/external/oblv/oblv_keys_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/external/oblv/oblv_proxy.py` & `syft-0.8.6b1/src/syft/external/oblv/oblv_proxy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/external/oblv/oblv_service.py` & `syft-0.8.6b1/src/syft/external/oblv/oblv_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/gevent_patch.py` & `syft-0.8.6b1/src/syft/gevent_patch.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/img/logo.png` & `syft-0.8.6b1/src/syft/img/logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/img/small-grid-symbol-logo.png` & `syft-0.8.6b1/src/syft/img/small-grid-symbol-logo.png`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/node/credentials.py` & `syft-0.8.6b1/src/syft/node/credentials.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/node/node.py` & `syft-0.8.6b1/src/syft/node/node.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # future
 from __future__ import annotations
 
 # stdlib
-import binascii
 from collections import OrderedDict
 from collections.abc import Callable
-import contextlib
 from datetime import datetime
 from functools import partial
 import hashlib
-from multiprocessing import current_process
 import os
 from pathlib import Path
+import shutil
 import subprocess  # nosec
+import tempfile
+from time import sleep
 import traceback
 from typing import Any
-import uuid
 
 # third party
 from nacl.signing import SigningKey
 from result import Err
 from result import Result
 from typing_extensions import Self
 
@@ -31,15 +30,15 @@
 from ..client.api import SignedSyftAPICall
 from ..client.api import SyftAPI
 from ..client.api import SyftAPICall
 from ..client.api import SyftAPIData
 from ..client.api import debox_signed_syftapicall_response
 from ..client.client import SyftClient
 from ..exceptions.exception import PySyftException
-from ..external import OBLV
+from ..external import OblvServiceProvider
 from ..protocol.data_protocol import PROTOCOL_TYPE
 from ..protocol.data_protocol import get_data_protocol
 from ..service.action.action_object import Action
 from ..service.action.action_object import ActionObject
 from ..service.action.action_service import ActionService
 from ..service.action.action_store import ActionStore
 from ..service.action.action_store import DictActionStore
@@ -93,15 +92,15 @@
 from ..service.settings.settings_stash import SettingsStash
 from ..service.sync.sync_service import SyncService
 from ..service.user.user import User
 from ..service.user.user import UserCreate
 from ..service.user.user_roles import ServiceRole
 from ..service.user.user_service import UserService
 from ..service.user.user_stash import UserStash
-from ..service.veilid import VEILID_ENABLED
+from ..service.veilid import VeilidServiceProvider
 from ..service.worker.image_registry_service import SyftImageRegistryService
 from ..service.worker.utils import DEFAULT_WORKER_IMAGE_TAG
 from ..service.worker.utils import DEFAULT_WORKER_POOL_NAME
 from ..service.worker.utils import create_default_image
 from ..service.worker.worker_image_service import SyftWorkerImageService
 from ..service.worker.worker_pool import WorkerPool
 from ..service.worker.worker_pool_service import SyftWorkerPoolService
@@ -120,15 +119,14 @@
 from ..types.syft_object import SYFT_OBJECT_VERSION_2
 from ..types.syft_object import SyftObject
 from ..types.uid import UID
 from ..util.experimental_flags import flags
 from ..util.telemetry import instrument
 from ..util.util import get_env
 from ..util.util import get_queue_address
-from ..util.util import get_root_data_path
 from ..util.util import random_name
 from ..util.util import str_to_bool
 from ..util.util import thread_ident
 from .credentials import SyftSigningKey
 from .credentials import SyftVerifyKey
 from .worker_settings import WorkerSettings
 
@@ -286,26 +284,25 @@
     packages: str
 
     def __init__(
         self,
         *,  # Trasterisk
         name: str | None = None,
         id: UID | None = None,
-        services: list[type[AbstractService]] | None = None,
         signing_key: SyftSigningKey | SigningKey | None = None,
         action_store_config: StoreConfig | None = None,
         document_store_config: StoreConfig | None = None,
         root_email: str | None = default_root_email,
         root_username: str | None = default_root_username,
         root_password: str | None = default_root_password,
         processes: int = 0,
         is_subprocess: bool = False,
         node_type: str | NodeType = NodeType.DOMAIN,
         local_db: bool = False,
-        sqlite_path: str | None = None,
+        reset: bool = False,
         blob_storage_config: BlobStorageConfig | None = None,
         queue_config: QueueConfig | None = None,
         queue_port: int | None = None,
         n_consumers: int = 0,
         create_producer: bool = False,
         thread_workers: bool = False,
         node_side_type: str | NodeSideType = NodeSideType.HIGH_SIDE,
@@ -318,96 +315,68 @@
         email_sender: str | None = None,
         smtp_port: int | None = None,
         smtp_host: str | None = None,
     ):
         # 🟡 TODO 22: change our ENV variable format and default init args to make this
         # less horrible or add some convenience functions
         self.dev_mode = dev_mode or get_dev_mode()
-        if node_uid_env is not None:
-            self.id = UID.from_string(node_uid_env)
-        else:
-            if id is None:
-                id = UID()
-            self.id = id
+        self.id = UID.from_string(node_uid_env) if node_uid_env else (id or UID())
         self.packages = ""
+        self.processes = processes
+        self.is_subprocess = is_subprocess
+        self.name = name or random_name()
+        self.enable_warnings = enable_warnings
+        self.in_memory_workers = in_memory_workers
+        self.node_type = NodeType(node_type)
+        self.node_side_type = NodeSideType(node_side_type)
+        self.client_cache: dict = {}
+        self.peer_client_cache: dict = {}
 
-        self.signing_key = None
-        if signing_key_env is not None:
-            self.signing_key = SyftSigningKey.from_string(signing_key_env)
+        if isinstance(node_type, str):
+            node_type = NodeType(node_type)
+        self.node_type = node_type
+
+        if isinstance(node_side_type, str):
+            node_side_type = NodeSideType(node_side_type)
+        self.node_side_type = node_side_type
+
+        skey = None
+        if signing_key_env:
+            skey = SyftSigningKey.from_string(signing_key_env)
+        elif isinstance(signing_key, SigningKey):
+            skey = SyftSigningKey(signing_key=signing_key)
         else:
-            if isinstance(signing_key, SigningKey):
-                signing_key = SyftSigningKey(signing_key=signing_key)
-            self.signing_key = signing_key
+            skey = signing_key
+        self.signing_key = skey or SyftSigningKey.generate()
 
-        if self.signing_key is None:
-            self.signing_key = SyftSigningKey.generate()
+        self.queue_config = self.create_queue_config(
+            n_consumers=n_consumers,
+            create_producer=create_producer,
+            thread_workers=thread_workers,
+            queue_port=queue_port,
+            queue_config=queue_config,
+        )
 
-        self.processes = processes
-        self.is_subprocess = is_subprocess
-        self.name = random_name() if name is None else name
-        services = (
-            [
-                UserService,
-                WorkerService,
-                SettingsService,
-                ActionService,
-                LogService,
-                DatasetService,
-                UserCodeService,
-                QueueService,
-                JobService,
-                RequestService,
-                DataSubjectService,
-                NetworkService,
-                PolicyService,
-                NotifierService,
-                NotificationService,
-                DataSubjectMemberService,
-                ProjectService,
-                EnclaveService,
-                CodeHistoryService,
-                MetadataService,
-                BlobStorageService,
-                MigrateStateService,
-                SyftWorkerImageService,
-                SyftWorkerPoolService,
-                SyftImageRegistryService,
-                SyncService,
-                OutputService,
-                UserCodeStatusService,
-            ]
-            if services is None
-            else services
-        )
-
-        self.service_config = ServiceConfigRegistry.get_registered_configs()
-        self.local_db = local_db
-        self.sqlite_path = sqlite_path
+        # must call before initializing stores
+        if reset:
+            self.remove_temp_dir()
+
+        use_sqlite = local_db or (processes > 0 and not is_subprocess)
+        document_store_config = document_store_config or self.get_default_store(
+            use_sqlite=use_sqlite
+        )
+        action_store_config = action_store_config or self.get_default_store(
+            use_sqlite=use_sqlite
+        )
         self.init_stores(
             action_store_config=action_store_config,
             document_store_config=document_store_config,
         )
 
-        if OBLV:
-            # relative
-            from ..external.oblv.oblv_service import OblvService
-
-            services += [OblvService]
-            create_oblv_key_pair(worker=self)
-
-        if VEILID_ENABLED:
-            # relative
-            from ..service.veilid.veilid_service import VeilidService
-
-            services += [VeilidService]
-
-        self.enable_warnings = enable_warnings
-        self.in_memory_workers = in_memory_workers
-
-        self.services = services
+        # construct services only after init stores
         self._construct_services()
 
         create_admin_new(  # nosec B106
             name=root_username,
             email=root_email,
             password=root_password,
             node=self,
@@ -418,34 +387,17 @@
             email_password=smtp_password,
             email_username=smtp_username,
             email_sender=email_sender,
             smtp_port=smtp_port,
             smtp_host=smtp_host,
         )
 
-        self.client_cache: dict = {}
-
-        if isinstance(node_type, str):
-            node_type = NodeType(node_type)
-        self.node_type = node_type
-
-        if isinstance(node_side_type, str):
-            node_side_type = NodeSideType(node_side_type)
-        self.node_side_type = node_side_type
-
         self.post_init()
-        self.create_initial_settings(admin_email=root_email)
 
-        self.queue_config = self.create_queue_config(
-            n_consumers=n_consumers,
-            create_producer=create_producer,
-            thread_workers=thread_workers,
-            queue_port=queue_port,
-            queue_config=queue_config,
-        )
+        self.create_initial_settings(admin_email=root_email)
 
         self.init_queue_manager(queue_config=self.queue_config)
 
         self.init_blob_storage(config=blob_storage_config)
 
         # Migrate data before any operation on db
         if migrate:
@@ -458,19 +410,29 @@
         path = "/proc/self/cgroup"
         return (
             os.path.exists("/.dockerenv")
             or os.path.isfile(path)
             and any("docker" in line for line in open(path))
         )
 
+    def get_default_store(self, use_sqlite: bool) -> StoreConfig:
+        if use_sqlite:
+            return SQLiteStoreConfig(
+                client_config=SQLiteStoreClientConfig(
+                    filename=f"{self.id}.sqlite",
+                    path=self.get_temp_dir("db"),
+                )
+            )
+        return DictStoreConfig()
+
     def init_blob_storage(self, config: BlobStorageConfig | None = None) -> None:
         if config is None:
-            root_directory = get_root_data_path()
-            base_directory = root_directory / f"{self.id}"
-            client_config = OnDiskBlobStorageClientConfig(base_directory=base_directory)
+            client_config = OnDiskBlobStorageClientConfig(
+                base_directory=self.get_temp_dir("blob")
+            )
             config_ = OnDiskBlobStorageConfig(client_config=client_config)
         else:
             config_ = config
         self.blob_store_config = config_
         self.blob_storage_client = config_.client_type(config=config_.client_config)
 
         # relative
@@ -489,17 +451,23 @@
     def stop(self) -> None:
         for consumer_list in self.queue_manager.consumers.values():
             for c in consumer_list:
                 c.close()
         for p in self.queue_manager.producers.values():
             p.close()
 
+        NodeRegistry.remove_node(self.id)
+
     def close(self) -> None:
         self.stop()
 
+    def cleanup(self) -> None:
+        self.stop()
+        self.remove_temp_dir()
+
     def create_queue_config(
         self,
         n_consumers: int,
         create_producer: bool,
         thread_workers: bool,
         queue_port: int | None,
         queue_config: QueueConfig | None,
@@ -595,102 +563,51 @@
     def named(
         cls,
         *,  # Trasterisk
         name: str,
         processes: int = 0,
         reset: bool = False,
         local_db: bool = False,
-        sqlite_path: str | None = None,
         node_type: str | NodeType = NodeType.DOMAIN,
         node_side_type: str | NodeSideType = NodeSideType.HIGH_SIDE,
         enable_warnings: bool = False,
         n_consumers: int = 0,
         thread_workers: bool = False,
         create_producer: bool = False,
         queue_port: int | None = None,
         dev_mode: bool = False,
         migrate: bool = False,
         in_memory_workers: bool = True,
     ) -> Self:
+        uid = UID.with_seed(name)
         name_hash = hashlib.sha256(name.encode("utf8")).digest()
-        name_hash_uuid = name_hash[0:16]
-        name_hash_uuid = bytearray(name_hash_uuid)
-        name_hash_uuid[6] = (
-            name_hash_uuid[6] & 0x0F
-        ) | 0x40  # Set version to 4 (uuid4)
-        name_hash_uuid[8] = (name_hash_uuid[8] & 0x3F) | 0x80  # Set variant to RFC 4122
-        name_hash_string = binascii.hexlify(bytearray(name_hash_uuid)).decode("utf-8")
-        if uuid.UUID(name_hash_string).version != 4:
-            raise Exception(f"Invalid UID: {name_hash_string} for name: {name}")
-        uid = UID(name_hash_string)
         key = SyftSigningKey(signing_key=SigningKey(name_hash))
         blob_storage_config = None
-        if reset:
-            store_config = SQLiteStoreClientConfig()
-            store_config.filename = f"{uid}.sqlite"
-
-            # stdlib
-            import sqlite3
-
-            with contextlib.closing(sqlite3.connect(store_config.file_path)) as db:
-                cursor = db.cursor()
-                cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
-                tables = cursor.fetchall()
-
-                for table_name in tables:
-                    drop_table_sql = f"DROP TABLE IF EXISTS {table_name[0]};"
-                    cursor.execute(drop_table_sql)
-
-                db.commit()
-                db.close()
-
-            # remove lock files for reading
-            # we should update this to partition locks per node
-            for f in Path("/tmp/sherlock").glob("*.json"):  # nosec
-                if f.is_file():
-                    f.unlink()
-
-            with contextlib.suppress(FileNotFoundError, PermissionError):
-                if os.path.exists(store_config.file_path):
-                    os.unlink(store_config.file_path)
-
-            # Reset blob storage
-            root_directory = get_root_data_path()
-            base_directory = root_directory / f"{uid}"
-            if base_directory.exists():
-                for file in base_directory.iterdir():
-                    file.unlink()
-            blob_client_config = OnDiskBlobStorageClientConfig(
-                base_directory=base_directory
-            )
-            blob_storage_config = OnDiskBlobStorageConfig(
-                client_config=blob_client_config
-            )
 
         node_type = NodeType(node_type)
         node_side_type = NodeSideType(node_side_type)
 
         return cls(
             name=name,
             id=uid,
             signing_key=key,
             processes=processes,
             local_db=local_db,
-            sqlite_path=sqlite_path,
             node_type=node_type,
             node_side_type=node_side_type,
             enable_warnings=enable_warnings,
             blob_storage_config=blob_storage_config,
             queue_port=queue_port,
             n_consumers=n_consumers,
             thread_workers=thread_workers,
             create_producer=create_producer,
             dev_mode=dev_mode,
             migrate=migrate,
             in_memory_workers=in_memory_workers,
+            reset=reset,
         )
 
     def is_root(self, credentials: SyftVerifyKey) -> bool:
         return credentials == self.verify_key
 
     @property
     def root_client(self) -> SyftClient:
@@ -852,80 +769,43 @@
         context = AuthedServiceContext(
             node=self, credentials=self.verify_key, role=ServiceRole.ADMIN
         )
         AuthNodeContextRegistry.set_node_context(
             node_uid=self.id, user_verify_key=self.verify_key, context=context
         )
 
-        if UserCodeService in self.services:
+        if "usercodeservice" in self.service_path_map:
             user_code_service = self.get_service(UserCodeService)
             user_code_service.load_user_code(context=context)
 
-        if self.is_subprocess or current_process().name != "MainProcess":
-            # print(f"> Starting Subprocess {self}")
-            pass
-        else:
-            pass
-            # why would we do this?
-            # print(f"> {self}")
-
         def reload_user_code() -> None:
             user_code_service.load_user_code(context=context)
 
         ti = thread_ident()
         if ti is not None:
             CODE_RELOADER[ti] = reload_user_code
 
     def init_stores(
         self,
-        document_store_config: StoreConfig | None = None,
-        action_store_config: StoreConfig | None = None,
+        document_store_config: StoreConfig,
+        action_store_config: StoreConfig,
     ) -> None:
-        if document_store_config is None:
-            if self.local_db or (self.processes > 0 and not self.is_subprocess):
-                client_config = SQLiteStoreClientConfig(path=self.sqlite_path)
-                document_store_config = SQLiteStoreConfig(client_config=client_config)
-            else:
-                document_store_config = DictStoreConfig()
-        if (
-            isinstance(document_store_config, SQLiteStoreConfig)
-            and document_store_config.client_config.filename is None
-        ):
-            document_store_config.client_config.filename = f"{self.id}.sqlite"
-            if self.dev_mode:
-                print(
-                    f"SQLite Store Path:\n!open file://{document_store_config.client_config.file_path}\n"
-                )
-        document_store = document_store_config.store_type
-        self.document_store_config = document_store_config
-
         # We add the python id of the current node in order
         # to create one connection per Node object in MongoClientCache
         # so that we avoid closing the connection from a
         # different thread through the garbage collection
-        if isinstance(self.document_store_config, MongoStoreConfig):
-            self.document_store_config.client_config.node_obj_python_id = id(self)
+        if isinstance(document_store_config, MongoStoreConfig):
+            document_store_config.client_config.node_obj_python_id = id(self)
 
-        self.document_store = document_store(
+        self.document_store_config = document_store_config
+        self.document_store = document_store_config.store_type(
             node_uid=self.id,
             root_verify_key=self.verify_key,
             store_config=document_store_config,
         )
-        if action_store_config is None:
-            if self.local_db or (self.processes > 0 and not self.is_subprocess):
-                client_config = SQLiteStoreClientConfig(path=self.sqlite_path)
-                action_store_config = SQLiteStoreConfig(client_config=client_config)
-            else:
-                action_store_config = DictStoreConfig()
-
-        if (
-            isinstance(action_store_config, SQLiteStoreConfig)
-            and action_store_config.client_config.filename is None
-        ):
-            action_store_config.client_config.filename = f"{self.id}.sqlite"
 
         if isinstance(action_store_config, SQLiteStoreConfig):
             self.action_store: ActionStore = SQLiteActionStore(
                 node_uid=self.id,
                 store_config=action_store_config,
                 root_verify_key=self.verify_key,
             )
@@ -955,67 +835,73 @@
         return self.get_service("jobservice").stash
 
     @property
     def worker_stash(self) -> WorkerStash:
         return self.get_service("workerservice").stash
 
     def _construct_services(self) -> None:
-        self.service_path_map = {}
+        service_path_map: dict[str, AbstractService] = {}
+        initialized_services: list[AbstractService] = []
 
-        for service_klass in self.services:
-            kwargs = {}
-            if service_klass == ActionService:
-                kwargs["store"] = self.action_store
-            store_services = [
-                UserService,
-                WorkerService,
-                SettingsService,
-                DatasetService,
-                UserCodeService,
-                LogService,
-                RequestService,
-                QueueService,
-                JobService,
-                DataSubjectService,
-                NetworkService,
-                PolicyService,
-                NotifierService,
-                NotificationService,
-                DataSubjectMemberService,
-                ProjectService,
-                EnclaveService,
-                CodeHistoryService,
-                MetadataService,
-                BlobStorageService,
-                MigrateStateService,
-                SyftWorkerImageService,
-                SyftWorkerPoolService,
-                SyftImageRegistryService,
-                SyncService,
-                OutputService,
-                UserCodeStatusService,
-            ]
-
-            if OBLV:
-                # relative
-                from ..external.oblv.oblv_service import OblvService
+        # A dict of service and init kwargs.
+        # - "svc" expects a callable (class or function)
+        #     - The callable must return AbstractService or None
+        # - "store" expects a store type
+        #     - By default all services get the document store
+        #     - Pass a custom "store" to override this
+        default_services: list[dict] = [
+            {"svc": ActionService, "store": self.action_store},
+            {"svc": UserService},
+            {"svc": WorkerService},
+            {"svc": SettingsService},
+            {"svc": DatasetService},
+            {"svc": UserCodeService},
+            {"svc": LogService},
+            {"svc": RequestService},
+            {"svc": QueueService},
+            {"svc": JobService},
+            {"svc": DataSubjectService},
+            {"svc": NetworkService},
+            {"svc": PolicyService},
+            {"svc": NotifierService},
+            {"svc": NotificationService},
+            {"svc": DataSubjectMemberService},
+            {"svc": ProjectService},
+            {"svc": EnclaveService},
+            {"svc": CodeHistoryService},
+            {"svc": MetadataService},
+            {"svc": BlobStorageService},
+            {"svc": MigrateStateService},
+            {"svc": SyftWorkerImageService},
+            {"svc": SyftWorkerPoolService},
+            {"svc": SyftImageRegistryService},
+            {"svc": SyncService},
+            {"svc": OutputService},
+            {"svc": UserCodeStatusService},
+            {"svc": VeilidServiceProvider},  # this is lazy
+            {"svc": OblvServiceProvider},  # this is lazy
+        ]
 
-                store_services += [OblvService]
+        for svc_kwargs in default_services:
+            ServiceCls = svc_kwargs.pop("svc")
+            svc_kwargs.setdefault("store", self.document_store)
 
-            if VEILID_ENABLED:
-                # relative
-                from ..service.veilid.veilid_service import VeilidService
+            svc_instance = ServiceCls(**svc_kwargs)
+            if not svc_instance:
+                continue
+            elif not isinstance(svc_instance, AbstractService):
+                raise ValueError(
+                    f"Service {ServiceCls.__name__} must be an instance of AbstractService"
+                )
 
-                store_services += [VeilidService]
+            service_path_map[ServiceCls.__name__.lower()] = svc_instance
+            initialized_services.append(ServiceCls)
 
-            if service_klass in store_services:
-                kwargs["store"] = self.document_store  # type: ignore[assignment]
-            self.service_path_map[service_klass.__name__.lower()] = service_klass(
-                **kwargs
-            )
+        self.services = initialized_services
+        self.service_path_map = service_path_map
 
     def get_service_method(self, path_or_func: str | Callable) -> Callable:
         if callable(path_or_func):
             path_or_func = path_or_func.__qualname__
         return self._get_service_method_from_path(path_or_func)
 
     def get_service(self, path_or_func: str | Callable) -> AbstractService:
@@ -1033,14 +919,32 @@
     def _get_service_method_from_path(self, path: str) -> Callable:
         path_list = path.split(".")
         method_name = path_list.pop()
         service_obj = self._get_service_from_path(path=path)
 
         return getattr(service_obj, method_name)
 
+    def get_temp_dir(self, dir_name: str = "") -> Path:
+        """
+        Get a temporary directory unique to the node.
+        Provide all dbs, blob dirs, and locks using this directory.
+        """
+        root = os.getenv("SYFT_TEMP_ROOT", "syft")
+        p = Path(tempfile.gettempdir(), root, str(self.id), dir_name)
+        p.mkdir(parents=True, exist_ok=True)
+        return p
+
+    def remove_temp_dir(self) -> None:
+        """
+        Remove the temporary directory for this node.
+        """
+        rootdir = self.get_temp_dir()
+        if rootdir.exists():
+            shutil.rmtree(rootdir, ignore_errors=True)
+
     @property
     def settings(self) -> NodeSettingsV2:
         settings_stash = SettingsStash(store=self.document_store)
         if self.signing_key is None:
             raise ValueError(f"{self} has no signing key")
         settings = settings_stash.get_all(self.signing_key.verify_key)
         if settings.is_ok() and len(settings.ok()) > 0:
@@ -1097,15 +1001,14 @@
 
         return True
 
     def await_future(
         self, credentials: SyftVerifyKey, uid: UID
     ) -> QueueItem | None | SyftError:
         # stdlib
-        from time import sleep
 
         # relative
         from ..service.queue.queue import Status
 
         while True:
             result = self.queue_stash.pop_on_complete(credentials, uid)
             if not result.is_ok():
@@ -1130,36 +1033,43 @@
             return queue_obj
         return result.err()
 
     def forward_message(
         self, api_call: SyftAPICall | SignedSyftAPICall
     ) -> Result[QueueItem | SyftObject, Err]:
         node_uid = api_call.message.node_uid
-        if NetworkService not in self.services:
+        if "networkservice" not in self.service_path_map:
             return SyftError(
                 message=(
                     "Node has no network service so we can't "
                     f"forward this message to {node_uid}"
                 )
             )
 
         client = None
-        if node_uid in self.client_cache:
-            client = self.client_cache[node_uid]
-        else:
-            network_service = self.get_service(NetworkService)
-            peer = network_service.stash.get_by_uid(self.verify_key, node_uid)
 
-            if peer.is_ok() and peer.ok():
-                peer = peer.ok()
+        network_service = self.get_service(NetworkService)
+        peer = network_service.stash.get_by_uid(self.verify_key, node_uid)
+
+        if peer.is_ok() and peer.ok():
+            peer = peer.ok()
+
+            # Since we have several routes to a peer
+            # we need to cache the client for a given node_uid along with the route
+            peer_cache_key = hash(node_uid) + hash(peer.pick_highest_priority_route())
+
+            if peer_cache_key in self.peer_client_cache:
+                client = self.peer_client_cache[peer_cache_key]
+            else:
                 context = AuthedServiceContext(
                     node=self, credentials=api_call.credentials
                 )
                 client = peer.client_with_context(context=context)
-                self.client_cache[node_uid] = client
+                self.peer_client_cache[peer_cache_key] = client
+
         if client:
             message: SyftAPICall = api_call.message
             if message.path == "metadata":
                 result = client.metadata
             elif message.path == "login":
                 result = client.connection.login(**message.kwargs)
             elif message.path == "register":
@@ -1592,39 +1502,39 @@
                 raise Exception(f"Could not create user: {result}")
     except Exception as e:
         print("Unable to create new admin", e)
 
     return None
 
 
-def create_oblv_key_pair(
-    worker: Node,
-) -> str | None:
-    try:
-        # relative
-        from ..external.oblv.oblv_keys_stash import OblvKeys
-        from ..external.oblv.oblv_keys_stash import OblvKeysStash
-        from ..external.oblv.oblv_service import generate_oblv_key
-
-        oblv_keys_stash = OblvKeysStash(store=worker.document_store)
-
-        if not len(oblv_keys_stash) and worker.signing_key:
-            public_key, private_key = generate_oblv_key(oblv_key_name=worker.name)
-            oblv_keys = OblvKeys(public_key=public_key, private_key=private_key)
-            res = oblv_keys_stash.set(worker.signing_key.verify_key, oblv_keys)
-            if res.is_ok():
-                print("Successfully generated Oblv Key pair at startup")
-            return res.err()
-        else:
-            print(f"Using Existing Public/Private Key pair: {len(oblv_keys_stash)}")
-    except Exception as e:
-        print("Unable to create Oblv Keys.", e)
-        return None
+# def create_oblv_key_pair(
+#     worker: Node,
+# ) -> str | None:
+#     try:
+#         # relative
+#         from ..external.oblv.oblv_keys_stash import OblvKeys
+#         from ..external.oblv.oblv_keys_stash import OblvKeysStash
+#         from ..external.oblv.oblv_service import generate_oblv_key
+
+#         oblv_keys_stash = OblvKeysStash(store=worker.document_store)
+
+#         if not len(oblv_keys_stash) and worker.signing_key:
+#             public_key, private_key = generate_oblv_key(oblv_key_name=worker.name)
+#             oblv_keys = OblvKeys(public_key=public_key, private_key=private_key)
+#             res = oblv_keys_stash.set(worker.signing_key.verify_key, oblv_keys)
+#             if res.is_ok():
+#                 print("Successfully generated Oblv Key pair at startup")
+#             return res.err()
+#         else:
+#             print(f"Using Existing Public/Private Key pair: {len(oblv_keys_stash)}")
+#     except Exception as e:
+#         print("Unable to create Oblv Keys.", e)
+#         return None
 
-    return None
+#     return None
 
 
 class NodeRegistry:
     __node_registry__: dict[UID, Node] = {}
 
     @classmethod
     def set_node_for(
@@ -1641,14 +1551,19 @@
     def node_for(cls, node_uid: UID) -> Node:
         return cls.__node_registry__.get(node_uid, None)
 
     @classmethod
     def get_all_nodes(cls) -> list[Node]:
         return list(cls.__node_registry__.values())
 
+    @classmethod
+    def remove_node(cls, node_uid: UID) -> None:
+        if node_uid in cls.__node_registry__:
+            del cls.__node_registry__[node_uid]
+
 
 def get_default_worker_tag_by_env(dev_mode: bool = False) -> str | None:
     if in_kubernetes():
         return get_default_worker_image()
     elif dev_mode:
         return "local-dev"
     else:
```

### Comparing `syft-0.8.5b9/src/syft/node/routes.py` & `syft-0.8.6b1/src/syft/node/routes.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/node/run.py` & `syft-0.8.6b1/src/syft/node/run.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/node/server.py` & `syft-0.8.6b1/src/syft/node/server.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/node/worker_settings.py` & `syft-0.8.6b1/src/syft/node/worker_settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/protocol/data_protocol.py` & `syft-0.8.6b1/src/syft/protocol/data_protocol.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/protocol/protocol_version.json` & `syft-0.8.6b1/src/syft/protocol/releases/0.8.5.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('4', OrderedDict([('object_versions', OrderedDict([('ActionObject', "*

 * *            "OrderedDict([('1', OrderedDict([('version', 1), ('hash', "*

 * *            "'632446f1415102490c93fafb56dd9eb29d79623bcc5e9f2e6e37c4f63c2c51c3'), ('action', "*

 * *            "'remove')])), ('2', OrderedDict([('version', 2), ('hash', "*

 * *            "'577aa1f010b90194958a18ec38ee21db3718bd96d9e036501c6ddeefabedf432'), ('action', "*

 * *            "'remove')])), ('3', OrderedDict([('version', 3), ('hash', "*

 * *        […]*

```diff
@@ -1,18 +1,9 @@
 {
-    "1": {
-        "release_name": "0.8.2.json"
-    },
-    "2": {
-        "release_name": "0.8.3.json"
-    },
-    "3": {
-        "release_name": "0.8.4.json"
-    },
-    "dev": {
+    "4": {
         "object_versions": {
             "APIEndpoint": {
                 "1": {
                     "action": "remove",
                     "hash": "c0e83867b107113e6fed06364ba364c24b2f4af35b15a3869b176318d3be7989",
                     "version": 1
                 },
@@ -553,15 +544,15 @@
                     "hash": "f752dfdec6b30e1c849e483ac88ab6f0c71a286199415e4f7bc33c8c2502fc1f",
                     "version": 2
                 }
             },
             "ExecutionOutput": {
                 "1": {
                     "action": "add",
-                    "hash": "abb4ce9172fbba0ea03fcbea7addb06176c8dba6dbcb7143cde350617528a5b7",
+                    "hash": "201c8abcb6595a64140ad0c3b058557229c7790a25fb55ed229ae0efcb63ad07",
                     "version": 1
                 }
             },
             "HTTPConnection": {
                 "1": {
                     "action": "remove",
                     "hash": "5ee19eaf55ecbe7945ea45924c036ec0f500114a2f64176620961a8c2ec94cdb",
```

### Comparing `syft-0.8.5b9/src/syft/protocol/releases/0.8.2.json` & `syft-0.8.6b1/src/syft/protocol/releases/0.8.2.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/protocol/releases/0.8.3.json` & `syft-0.8.6b1/src/syft/protocol/releases/0.8.3.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/protocol/releases/0.8.4.json` & `syft-0.8.6b1/src/syft/protocol/releases/0.8.4.json`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/serde/array.py` & `syft-0.8.6b1/src/syft/serde/array.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/serde/arrow.py` & `syft-0.8.6b1/src/syft/serde/arrow.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/serde/deserialize.py` & `syft-0.8.6b1/src/syft/serde/deserialize.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/serde/lib_permissions.py` & `syft-0.8.6b1/src/syft/serde/lib_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/serde/lib_service_registry.py` & `syft-0.8.6b1/src/syft/serde/lib_service_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/serde/mock.py` & `syft-0.8.6b1/src/syft/serde/mock.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/serde/recursive.py` & `syft-0.8.6b1/src/syft/serde/recursive.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/serde/recursive_primitives.py` & `syft-0.8.6b1/src/syft/serde/recursive_primitives.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/serde/serializable.py` & `syft-0.8.6b1/src/syft/serde/serializable.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/serde/signature.py` & `syft-0.8.6b1/src/syft/serde/signature.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/serde/third_party.py` & `syft-0.8.6b1/src/syft/serde/third_party.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/action/action_data_empty.py` & `syft-0.8.6b1/src/syft/service/action/action_data_empty.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/action/action_graph.py` & `syft-0.8.6b1/src/syft/service/action/action_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -340,16 +340,16 @@
 
 
 @serializable()
 class InMemoryGraphConfig(StoreConfig):
     __canonical_name__ = "InMemoryGraphConfig"
 
     store_type: type[BaseGraphStore] = NetworkXBackingStore
-    client_config: StoreClientConfig = InMemoryStoreClientConfig()
-    locking_config: LockingConfig = ThreadingLockingConfig()
+    client_config: StoreClientConfig = Field(default_factory=InMemoryStoreClientConfig)
+    locking_config: LockingConfig = Field(default_factory=ThreadingLockingConfig)
 
 
 @serializable()
 class ActionGraphStore:
     pass
```

### Comparing `syft-0.8.5b9/src/syft/service/action/action_graph_service.py` & `syft-0.8.6b1/src/syft/service/action/action_graph_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/action/action_object.py` & `syft-0.8.6b1/src/syft/service/action/action_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/action/action_permissions.py` & `syft-0.8.6b1/src/syft/service/action/action_permissions.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/action/action_service.py` & `syft-0.8.6b1/src/syft/service/action/action_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,53 +298,42 @@
         kwargs: dict[str, Any],
         result_id: UID | None = None,
     ) -> Result[ActionObjectPointer, Err]:
         override_execution_permission = (
             context.has_execute_permissions or context.role == ServiceRole.ADMIN
         )
 
+        input_policy = code_item.get_input_policy(context)
+
         if not override_execution_permission:
-            input_policy = code_item.get_input_policy(context)
             if input_policy is None:
                 if not code_item.output_policy_approved:
                     return Err("Execution denied: Your code is waiting for approval")
-                return Err(f"No input poliicy defined for user code: {code_item.id}")
+                return Err(f"No input policy defined for user code: {code_item.id}")
+
+            # Filter input kwargs based on policy
             filtered_kwargs = input_policy.filter_kwargs(
                 kwargs=kwargs, context=context, code_item_id=code_item.id
             )
-            if isinstance(filtered_kwargs, SyftError) or filtered_kwargs.is_err():
+            if filtered_kwargs.is_err():
                 return filtered_kwargs
             filtered_kwargs = filtered_kwargs.ok()
+
+            # validate input policy
+            is_approved = input_policy._is_valid(
+                context=context,
+                usr_input_kwargs=kwargs,
+                code_item_id=code_item.id,
+            )
+            if is_approved.is_err():
+                return is_approved
         else:
             filtered_kwargs = retrieve_from_db(code_item.id, kwargs, context).ok()
         # update input policy to track any input state
 
-        if (
-            not override_execution_permission
-            and code_item.get_input_policy(context) is not None
-        ):
-            expected_input_kwargs = set()
-            for _inp_kwarg in code_item.get_input_policy(context).inputs.values():  # type: ignore
-                keys = _inp_kwarg.keys()
-                for k in keys:
-                    if k not in kwargs:
-                        return Err(
-                            f"{code_item.service_func_name}() missing required keyword argument: '{k}'"
-                        )
-                expected_input_kwargs.update(keys)
-
-            permitted_input_kwargs = list(filtered_kwargs.keys())
-            not_approved_kwargs = set(expected_input_kwargs) - set(
-                permitted_input_kwargs
-            )
-            if len(not_approved_kwargs) > 0:
-                return Err(
-                    f"Input arguments: {not_approved_kwargs} to the function are not approved yet."
-                )
-
         has_twin_inputs = False
 
         real_kwargs = {}
         for key, kwarg_value in filtered_kwargs.items():
             if isinstance(kwarg_value, TwinObject):
                 has_twin_inputs = True
             real_kwargs[key] = kwarg_value
```

### Comparing `syft-0.8.5b9/src/syft/service/action/action_store.py` & `syft-0.8.6b1/src/syft/service/action/action_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/action/action_types.py` & `syft-0.8.6b1/src/syft/service/action/action_types.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/action/numpy.py` & `syft-0.8.6b1/src/syft/service/action/numpy.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/action/pandas.py` & `syft-0.8.6b1/src/syft/service/action/pandas.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/action/plan.py` & `syft-0.8.6b1/src/syft/service/action/plan.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/action/verification.py` & `syft-0.8.6b1/src/syft/service/action/verification.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/blob_storage/remote_profile.py` & `syft-0.8.6b1/src/syft/service/blob_storage/remote_profile.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/blob_storage/service.py` & `syft-0.8.6b1/src/syft/service/blob_storage/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/blob_storage/stash.py` & `syft-0.8.6b1/src/syft/service/blob_storage/stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/code/code_parse.py` & `syft-0.8.6b1/src/syft/service/code/code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/code/status_service.py` & `syft-0.8.6b1/src/syft/service/code/status_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/code/user_code.py` & `syft-0.8.6b1/src/syft/service/code/user_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -536,14 +536,15 @@
         return output_service.get_by_user_code_id(context, self.id)
 
     def apply_output(
         self,
         context: AuthedServiceContext,
         outputs: Any,
         job_id: UID | None = None,
+        input_ids: dict[str, UID] | None = None,
     ) -> ExecutionOutput | SyftError:
         output_policy = self.get_output_policy(context)
         if output_policy is None:
             return SyftError(
                 message="You must wait for the output policy to be approved"
             )
 
@@ -554,14 +555,15 @@
         execution_result = output_service.create(
             context,
             user_code_id=self.id,
             output_ids=output_ids,
             executing_user_verify_key=self.user_verify_key,
             job_id=job_id,
             output_policy_id=output_policy.id,
+            input_ids=input_ids,
         )
         if isinstance(execution_result, SyftError):
             return execution_result
 
         return execution_result
 
     @property
```

### Comparing `syft-0.8.5b9/src/syft/service/code/user_code_parse.py` & `syft-0.8.6b1/src/syft/service/code/user_code_parse.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/code/user_code_service.py` & `syft-0.8.6b1/src/syft/service/code/user_code_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # relative
 from ...abstract_node import AbstractNode
 from ...abstract_node import NodeType
 from ...client.enclave_client import EnclaveClient
 from ...serde.serializable import serializable
 from ...store.document_store import DocumentStore
 from ...store.linked_obj import LinkedObject
+from ...types.cache_object import CachedSyftObject
 from ...types.twin_object import TwinObject
 from ...types.uid import UID
 from ...util.telemetry import instrument
 from ..action.action_object import ActionObject
 from ..action.action_permissions import ActionObjectPermission
 from ..action.action_permissions import ActionPermission
 from ..context import AuthedServiceContext
@@ -61,15 +62,15 @@
     def submit(
         self, context: AuthedServiceContext, code: UserCode | SubmitUserCode
     ) -> UserCode | SyftError:
         """Add User Code"""
         result = self._submit(context=context, code=code)
         if result.is_err():
             return SyftError(message=str(result.err()))
-        return SyftSuccess(message="User Code Submitted")
+        return SyftSuccess(message="User Code Submitted", require_api_update=True)
 
     def _submit(
         self, context: AuthedServiceContext, code: UserCode | SubmitUserCode
     ) -> Result[UserCode, str]:
         if not isinstance(code, UserCode):
             code = code.to(UserCode, context=context)  # type: ignore[unreachable]
 
@@ -365,15 +366,15 @@
         self, kwargs: dict[str, Any], context: AuthedServiceContext
     ) -> bool:
         return len(self.keep_owned_kwargs(kwargs, context)) == len(kwargs)
 
     @service_method(path="code.call", name="call", roles=GUEST_ROLE_LEVEL)
     def call(
         self, context: AuthedServiceContext, uid: UID, **kwargs: Any
-    ) -> SyftSuccess | SyftError:
+    ) -> CachedSyftObject | ActionObject | SyftSuccess | SyftError:
         """Call a User Code Function"""
         kwargs.pop("result_id", None)
         result = self._call(context, uid, **kwargs)
         if result.is_err():
             return SyftError(message=result.err())
         else:
             return result.ok()
@@ -405,14 +406,19 @@
             )
 
             # Override permissions bypasses the cache, since we do not check in/out policies
             skip_fill_cache = override_execution_permission
             # We do not read from output policy cache if there are mock arguments
             skip_read_cache = len(self.keep_owned_kwargs(kwargs, context)) > 0
 
+            # Extract ids from kwargs
+            kwarg2id = map_kwargs_to_id(kwargs)
+
+            input_policy = code.get_input_policy(context)
+
             # Check output policy
             output_policy = code.get_output_policy(context)
             if not override_execution_permission:
                 output_history = code.get_output_history(context=context)
                 if isinstance(output_history, SyftError):
                     return Err(output_history.message)
                 can_execute = self.is_execution_allowed(
@@ -423,33 +429,54 @@
                 if not can_execute:
                     if not code.is_output_policy_approved(context):
                         return Err(
                             "Execution denied: Your code is waiting for approval"
                         )
                     if not (is_valid := output_policy._is_valid(context)):  # type: ignore
                         if len(output_history) > 0 and not skip_read_cache:
+                            last_executed_output = output_history[-1]
+                            # Check if the inputs of the last executed output match
+                            # against the current input
+                            if (
+                                input_policy is not None
+                                and not last_executed_output.check_input_ids(
+                                    kwargs=kwarg2id
+                                )
+                            ):
+                                inp_policy_validation = input_policy._is_valid(
+                                    context,
+                                    usr_input_kwargs=kwarg2id,
+                                    code_item_id=code.id,
+                                )
+                                if inp_policy_validation.is_err():
+                                    return inp_policy_validation
+
                             result: Result[ActionObject, str] = resolve_outputs(
                                 context=context,
-                                output_ids=output_history[-1].output_ids,
+                                output_ids=last_executed_output.output_ids,
                             )
                             if result.is_err():
                                 return result
 
                             res = delist_if_single(result.ok())
-                            return Ok(res)
+                            return Ok(
+                                CachedSyftObject(
+                                    result=res,
+                                    error_msg=is_valid.message,
+                                )
+                            )
                         else:
-                            return is_valid.to_result()
+                            return cast(Err, is_valid.to_result())
                     return can_execute.to_result()  # type: ignore
 
             # Execute the code item
             context.node = cast(AbstractNode, context.node)
 
             action_service = context.node.get_service("actionservice")
 
-            kwarg2id = map_kwargs_to_id(kwargs)
             result_action_object: Result[ActionObject | TwinObject, str] = (
                 action_service._user_code_execute(
                     context, code, kwarg2id, result_id=result_id
                 )
             )
             if result_action_object.is_err():
                 return result_action_object
@@ -466,15 +493,18 @@
 
             # Apply Output Policy to the results and update the OutputPolicyState
 
             # this currently only works for nested syft_functions
             # and admins executing on high side (TODO, decide if we want to increment counter)
             if not skip_fill_cache and output_policy is not None:
                 res = code.apply_output(
-                    context=context, outputs=result, job_id=context.job_id
+                    context=context,
+                    outputs=result,
+                    job_id=context.job_id,
+                    input_ids=kwarg2id,
                 )
                 if isinstance(res, SyftError):
                     return Err(res.message)
             has_result_read_permission = context.extra_kwargs.get(
                 "has_result_read_permission", False
             )
             if isinstance(result, TwinObject):
@@ -514,25 +544,31 @@
         path="code.apply_output", name="apply_output", roles=GUEST_ROLE_LEVEL
     )
     def apply_output(
         self,
         context: AuthedServiceContext,
         user_code_id: UID,
         outputs: Any,
+        input_ids: dict[str, UID] | None = None,
         job_id: UID | None = None,
     ) -> ExecutionOutput | SyftError:
         code_result = self.stash.get_by_uid(context.credentials, user_code_id)
         if code_result.is_err():
             return SyftError(message=code_result.err())
 
         code: UserCode = code_result.ok()
         if not code.get_status(context).approved:
             return SyftError(message="Code is not approved")
 
-        res = code.apply_output(context=context, outputs=outputs, job_id=job_id)
+        res = code.apply_output(
+            context=context,
+            outputs=outputs,
+            job_id=job_id,
+            input_ids=input_ids,
+        )
         return res
 
 
 def resolve_outputs(
     context: AuthedServiceContext,
     output_ids: list[UID],
 ) -> Result[list[ActionObject], str]:
```

### Comparing `syft-0.8.5b9/src/syft/service/code/user_code_stash.py` & `syft-0.8.6b1/src/syft/service/code/user_code_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/code/utils.py` & `syft-0.8.6b1/src/syft/service/code/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/code_history/code_history.py` & `syft-0.8.6b1/src/syft/service/code_history/code_history.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/code_history/code_history_service.py` & `syft-0.8.6b1/src/syft/service/code_history/code_history_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/code_history/code_history_stash.py` & `syft-0.8.6b1/src/syft/service/code_history/code_history_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/context.py` & `syft-0.8.6b1/src/syft/service/context.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/data_subject/data_subject.py` & `syft-0.8.6b1/src/syft/service/data_subject/data_subject.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/data_subject/data_subject_member.py` & `syft-0.8.6b1/src/syft/service/data_subject/data_subject_member.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/data_subject/data_subject_member_service.py` & `syft-0.8.6b1/src/syft/service/data_subject/data_subject_member_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/data_subject/data_subject_service.py` & `syft-0.8.6b1/src/syft/service/data_subject/data_subject_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/dataset/dataset.py` & `syft-0.8.6b1/src/syft/service/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/dataset/dataset_service.py` & `syft-0.8.6b1/src/syft/service/dataset/dataset_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/dataset/dataset_stash.py` & `syft-0.8.6b1/src/syft/service/dataset/dataset_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/enclave/enclave_service.py` & `syft-0.8.6b1/src/syft/service/enclave/enclave_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,17 +92,17 @@
                 )
 
         return SyftSuccess(message="Enclave Code Status Updated Successfully")
 
 
 def get_oblv_service() -> type[AbstractService] | SyftError:
     # relative
-    from ...external import OBLV
+    from ...external import OBLV_ENABLED
 
-    if OBLV:
+    if OBLV_ENABLED:
         # relative
         from ...external.oblv.oblv_service import OblvService
 
         return OblvService
     else:
         return SyftError(
             message="Oblivious is not enabled."
```

### Comparing `syft-0.8.5b9/src/syft/service/job/job_service.py` & `syft-0.8.6b1/src/syft/service/job/job_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/job/job_stash.py` & `syft-0.8.6b1/src/syft/service/job/job_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/log/log.py` & `syft-0.8.6b1/src/syft/service/log/log.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/log/log_service.py` & `syft-0.8.6b1/src/syft/service/log/log_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/log/log_stash.py` & `syft-0.8.6b1/src/syft/service/log/log_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/metadata/metadata_service.py` & `syft-0.8.6b1/src/syft/service/metadata/metadata_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/metadata/migrations.py` & `syft-0.8.6b1/src/syft/service/metadata/migrations.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/metadata/node_metadata.py` & `syft-0.8.6b1/src/syft/service/metadata/node_metadata.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/network/network_service.py` & `syft-0.8.6b1/src/syft/service/network/network_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/network/node_peer.py` & `syft-0.8.6b1/src/syft/service/network/node_peer.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/network/routes.py` & `syft-0.8.6b1/src/syft/service/network/routes.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,17 @@
     priority: int = 1
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, HTTPNodeRoute):
             return hash(self) == hash(other)
         return self == other
 
+    def __hash__(self) -> int:
+        return hash(self.host_or_ip) + hash(self.port) + hash(self.protocol)
+
 
 @serializable()
 class VeilidNodeRoute(SyftObject, NodeRoute):
     __canonical_name__ = "VeilidNodeRoute"
     __version__ = SYFT_OBJECT_VERSION_1
 
     vld_key: str
@@ -102,14 +105,17 @@
     priority: int = 1
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, VeilidNodeRoute):
             return hash(self) == hash(other)
         return self == other
 
+    def __hash__(self) -> int:
+        return hash(self.vld_key)
+
 
 @serializable()
 class PythonNodeRoute(SyftObject, NodeRoute):
     __canonical_name__ = "PythonNodeRoute"
     __version__ = SYFT_OBJECT_VERSION_2
 
     worker_settings: WorkerSettings
@@ -139,14 +145,17 @@
         return cls(id=worker_settings.id, worker_settings=worker_settings)
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, PythonNodeRoute):
             return hash(self) == hash(other)
         return self == other
 
+    def __hash__(self) -> int:
+        return hash(self.worker_settings.id)
+
 
 NodeRouteType = HTTPNodeRoute | PythonNodeRoute | VeilidNodeRoute
 
 
 def route_to_connection(
     route: NodeRoute, context: TransformContext | None = None
 ) -> NodeConnection:
```

### Comparing `syft-0.8.5b9/src/syft/service/notification/email_templates.py` & `syft-0.8.6b1/src/syft/service/notification/email_templates.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/notification/notification_service.py` & `syft-0.8.6b1/src/syft/service/notification/notification_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/notification/notification_stash.py` & `syft-0.8.6b1/src/syft/service/notification/notification_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/notification/notifications.py` & `syft-0.8.6b1/src/syft/service/notification/notifications.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/notifier/notifier.py` & `syft-0.8.6b1/src/syft/service/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/notifier/notifier_service.py` & `syft-0.8.6b1/src/syft/service/notifier/notifier_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/notifier/notifier_stash.py` & `syft-0.8.6b1/src/syft/service/notifier/notifier_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/notifier/smtp_client.py` & `syft-0.8.6b1/src/syft/service/notifier/smtp_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/object_search/migration_state_service.py` & `syft-0.8.6b1/src/syft/service/object_search/migration_state_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/object_search/object_migration_state.py` & `syft-0.8.6b1/src/syft/service/object_search/object_migration_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/output/output_service.py` & `syft-0.8.6b1/src/syft/service/output/output_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     __version__ = SYFT_OBJECT_VERSION_1
 
     executing_user_verify_key: SyftVerifyKey
     user_code_link: LinkedObject
     output_ids: list[UID] | dict[str, UID] | None = None
     job_link: LinkedObject | None = None
     created_at: DateTime = DateTime.now()
+    input_ids: dict[str, UID] | None = None
 
     # Required for __attr_searchable__, set by model_validator
     user_code_id: UID
 
     # Output policy is not a linked object because its saved on the usercode
     output_policy_id: UID | None = None
 
@@ -75,14 +76,15 @@
         cls: type["ExecutionOutput"],
         output_ids: UID | list[UID] | dict[str, UID],
         user_code_id: UID,
         executing_user_verify_key: SyftVerifyKey,
         node_uid: UID,
         job_id: UID | None = None,
         output_policy_id: UID | None = None,
+        input_ids: dict[str, UID] | None = None,
     ) -> "ExecutionOutput":
         # relative
         from ..code.user_code_service import UserCode
         from ..code.user_code_service import UserCodeService
         from ..job.job_service import Job
         from ..job.job_service import JobService
 
@@ -107,14 +109,15 @@
             job_link = None
         return cls(
             output_ids=output_ids,
             user_code_link=user_code_link,
             job_link=job_link,
             executing_user_verify_key=executing_user_verify_key,
             output_policy_id=output_policy_id,
+            input_ids=input_ids,
         )
 
     @property
     def outputs(self) -> list[ActionObject] | dict[str, ActionObject] | None:
         api = APIRegistry.api_for(
             node_uid=self.syft_node_location,
             user_verify_key=self.syft_client_verify_key,
@@ -139,14 +142,38 @@
         if isinstance(ids, dict):
             return list(ids.values())
         elif isinstance(ids, list):
             return ids
         return []
 
     @property
+    def input_id_list(self) -> list[UID]:
+        ids = self.input_ids
+        if isinstance(ids, dict):
+            return list(ids.values())
+        return []
+
+    def check_input_ids(self, kwargs: dict[str, UID]) -> bool:
+        """
+        Checks the input IDs against the stored input IDs.
+
+        Args:
+            kwargs (dict[str, UID]): A dictionary containing the input IDs to be checked.
+
+        Returns:
+            bool: True if the input IDs are valid, False otherwise.
+        """
+        if not self.input_ids:
+            return True
+        for key, value in kwargs.items():  # Iterate over items of kwargs dictionary
+            if key not in self.input_ids or self.input_ids[key] != value:
+                return False
+        return True
+
+    @property
     def job_id(self) -> UID | None:
         return self.job_link.object_uid if self.job_link else None
 
     def get_sync_dependencies(self, api: Any = None) -> list[UID]:
         # Output ids, user code id, job id
         res = []
 
@@ -212,22 +239,24 @@
         self,
         context: AuthedServiceContext,
         user_code_id: UID,
         output_ids: UID | list[UID] | dict[str, UID],
         executing_user_verify_key: SyftVerifyKey,
         job_id: UID | None = None,
         output_policy_id: UID | None = None,
+        input_ids: dict[str, UID] | None = None,
     ) -> ExecutionOutput | SyftError:
         output = ExecutionOutput.from_ids(
             output_ids=output_ids,
             user_code_id=user_code_id,
             executing_user_verify_key=executing_user_verify_key,
             node_uid=context.node.id,  # type: ignore
             job_id=job_id,
             output_policy_id=output_policy_id,
+            input_ids=input_ids,
         )
 
         res = self.stash.set(context.credentials, output)
         return res
 
     @service_method(
         path="output.get_by_user_code_id",
```

### Comparing `syft-0.8.5b9/src/syft/service/policy/policy.py` & `syft-0.8.6b1/src/syft/service/policy/policy.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 import sys
 import types
 from typing import Any
 from typing import cast
 
 # third party
 from RestrictedPython import compile_restricted
+from result import Err
 from result import Ok
+from result import Result
 
 # relative
 from ...abstract_node import AbstractNode
 from ...abstract_node import NodeType
 from ...client.api import APIRegistry
 from ...client.api import NodeIdentity
 from ...node.credentials import SyftVerifyKey
@@ -173,16 +175,27 @@
             init_kwargs = kwargs["init_kwargs"]
             del kwargs["init_kwargs"]
         else:
             # TODO: remove this tech debt, dont remove the id mapping functionality
             init_kwargs = partition_by_node(kwargs)
         super().__init__(*args, init_kwargs=init_kwargs, **kwargs)
 
+    def _is_valid(
+        self,
+        context: AuthedServiceContext,
+        usr_input_kwargs: dict,
+        code_item_id: UID,
+    ) -> Result[bool, str]:
+        raise NotImplementedError
+
     def filter_kwargs(
-        self, kwargs: dict[Any, Any], context: AuthedServiceContext, code_item_id: UID
+        self,
+        kwargs: dict[Any, Any],
+        context: AuthedServiceContext,
+        code_item_id: UID,
     ) -> dict[Any, Any]:
         raise NotImplementedError
 
     @property
     def inputs(self) -> dict[NodeIdentity, Any]:
         return self.init_kwargs
 
@@ -209,15 +222,15 @@
                 action_object_value.syft_action_data  # noqa: B018
             inputs[var_name] = action_object_value
         return inputs
 
 
 def retrieve_from_db(
     code_item_id: UID, allowed_inputs: dict[str, UID], context: AuthedServiceContext
-) -> dict:
+) -> Result[dict[str, Any], str]:
     # relative
     from ...service.action.action_object import TwinMode
 
     context.node = cast(AbstractNode, context.node)
 
     action_service = context.node.get_service("actionservice")
     code_inputs = {}
@@ -235,21 +248,21 @@
             kwarg_value = action_service._get(
                 context=root_context,
                 uid=arg_id,
                 twin_mode=TwinMode.NONE,
                 has_permission=True,
             )
             if kwarg_value.is_err():
-                return SyftError(message=kwarg_value.err())
+                return Err(kwarg_value.err())
             code_inputs[var_name] = kwarg_value.ok()
 
     elif context.node.node_type == NodeType.ENCLAVE:
         dict_object = action_service.get(context=root_context, uid=code_item_id)
         if dict_object.is_err():
-            return SyftError(message=dict_object.err())
+            return Err(dict_object.err())
         for value in dict_object.ok().syft_action_data.values():
             code_inputs.update(value)
 
     else:
         raise Exception(
             f"Invalid Node Type for Code Submission:{context.node.node_type}"
         )
@@ -284,37 +297,78 @@
             value = kwargs[key]
             uid = value
             if not isinstance(uid, UID):
                 uid = getattr(value, "id", None)
 
             if uid != allowed_inputs[key]:
                 raise Exception(
-                    f"Input {type(value)} for {key} not in allowed {allowed_inputs}"
+                    f"Input with uid: {uid} for `{key}` not in allowed inputs: {allowed_inputs}"
                 )
             filtered_kwargs[key] = value
     return filtered_kwargs
 
 
 @serializable()
 class ExactMatch(InputPolicy):
     # version
     __canonical_name__ = "ExactMatch"
     __version__ = SYFT_OBJECT_VERSION_2
 
     def filter_kwargs(
-        self, kwargs: dict[Any, Any], context: AuthedServiceContext, code_item_id: UID
-    ) -> dict[Any, Any]:
-        allowed_inputs = allowed_ids_only(
-            allowed_inputs=self.inputs, kwargs=kwargs, context=context
-        )
-        results = retrieve_from_db(
-            code_item_id=code_item_id, allowed_inputs=allowed_inputs, context=context
-        )
+        self,
+        kwargs: dict[Any, Any],
+        context: AuthedServiceContext,
+        code_item_id: UID,
+    ) -> Result[dict[Any, Any], str]:
+        try:
+            allowed_inputs = allowed_ids_only(
+                allowed_inputs=self.inputs, kwargs=kwargs, context=context
+            )
+
+            results = retrieve_from_db(
+                code_item_id=code_item_id,
+                allowed_inputs=allowed_inputs,
+                context=context,
+            )
+        except Exception as e:
+            return Err(str(e))
         return results
 
+    def _is_valid(
+        self,
+        context: AuthedServiceContext,
+        usr_input_kwargs: dict,
+        code_item_id: UID,
+    ) -> Result[bool, str]:
+        filtered_input_kwargs = self.filter_kwargs(
+            kwargs=usr_input_kwargs,
+            context=context,
+            code_item_id=code_item_id,
+        )
+
+        if filtered_input_kwargs.is_err():
+            return filtered_input_kwargs
+
+        filtered_input_kwargs = filtered_input_kwargs.ok()
+
+        expected_input_kwargs = set()
+        for _inp_kwargs in self.inputs.values():
+            for k in _inp_kwargs.keys():
+                if k not in usr_input_kwargs:
+                    return Err(f"Function missing required keyword argument: '{k}'")
+            expected_input_kwargs.update(_inp_kwargs.keys())
+
+        permitted_input_kwargs = list(filtered_input_kwargs.keys())
+        not_approved_kwargs = set(expected_input_kwargs) - set(permitted_input_kwargs)
+        if len(not_approved_kwargs) > 0:
+            return Err(
+                f"Input arguments: {not_approved_kwargs} to the function are not approved yet."
+            )
+        return Ok(True)
+
 
 @serializable()
 class OutputHistory(SyftObject):
     # version
     __canonical_name__ = "OutputHistory"
     __version__ = SYFT_OBJECT_VERSION_2
```

### Comparing `syft-0.8.5b9/src/syft/service/policy/policy_service.py` & `syft-0.8.6b1/src/syft/service/policy/policy_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/policy/user_policy_stash.py` & `syft-0.8.6b1/src/syft/service/policy/user_policy_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/project/project.py` & `syft-0.8.6b1/src/syft/service/project/project.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/project/project_service.py` & `syft-0.8.6b1/src/syft/service/project/project_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/project/project_stash.py` & `syft-0.8.6b1/src/syft/service/project/project_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/queue/base_queue.py` & `syft-0.8.6b1/src/syft/service/queue/base_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/queue/queue.py` & `syft-0.8.6b1/src/syft/service/queue/queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/queue/queue_service.py` & `syft-0.8.6b1/src/syft/service/queue/queue_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/queue/queue_stash.py` & `syft-0.8.6b1/src/syft/service/queue/queue_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/queue/zmq_queue.py` & `syft-0.8.6b1/src/syft/service/queue/zmq_queue.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/request/request.py` & `syft-0.8.6b1/src/syft/service/request/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -833,16 +833,24 @@
                 return result_request
             self = result_request
 
             approved = self.approve(disable_warnings=True, approve_nested=True)
             if isinstance(approved, SyftError):
                 return approved
 
+            input_ids = {}
+            if code.input_policy is not None:
+                for inps in code.input_policy.inputs.values():
+                    input_ids.update(inps)
+
             res = api.services.code.apply_output(
-                user_code_id=code.id, outputs=result, job_id=job.id
+                user_code_id=code.id,
+                outputs=result,
+                job_id=job.id,
+                input_ids=input_ids,
             )
             if isinstance(res, SyftError):
                 return res
 
         job_info.result = action_object
 
         existing_result = job.result.id if job.result is not None else None
```

### Comparing `syft-0.8.5b9/src/syft/service/request/request_service.py` & `syft-0.8.6b1/src/syft/service/request/request_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from ..response import SyftError
 from ..response import SyftSuccess
 from ..service import AbstractService
 from ..service import SERVICE_TO_TYPES
 from ..service import TYPE_TO_SERVICE
 from ..service import service_method
 from ..user.user import UserView
+from ..user.user_roles import DATA_SCIENTIST_ROLE_LEVEL
 from ..user.user_roles import GUEST_ROLE_LEVEL
 from ..user.user_service import UserService
 from .request import Change
 from .request import Request
 from .request import RequestInfo
 from .request import RequestInfoFilter
 from .request import RequestStatus
@@ -101,15 +102,17 @@
             if result.is_err():
                 return SyftError(message=str(result.err()))
             return result.ok()
         except Exception as e:
             print("Failed to submit Request", e)
             raise e
 
-    @service_method(path="request.get_all", name="get_all")
+    @service_method(
+        path="request.get_all", name="get_all", roles=DATA_SCIENTIST_ROLE_LEVEL
+    )
     def get_all(self, context: AuthedServiceContext) -> list[Request] | SyftError:
         result = self.stash.get_all(context.credentials)
         if result.is_err():
             return SyftError(message=str(result.err()))
         requests = result.ok()
         # return [self.resolve_nested_requests(context, request) for request in requests]
         return requests
```

### Comparing `syft-0.8.5b9/src/syft/service/request/request_stash.py` & `syft-0.8.6b1/src/syft/service/request/request_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/response.py` & `syft-0.8.6b1/src/syft/service/response.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,21 +10,26 @@
 from ..serde.serializable import serializable
 from ..types.base import SyftBaseModel
 
 
 class SyftResponseMessage(SyftBaseModel):
     message: str
     _bool: bool = True
+    require_api_update: bool = False
 
     def __bool__(self) -> bool:
         return self._bool
 
     def __eq__(self, other: Any) -> bool:
         if isinstance(other, SyftResponseMessage):
-            return self.message == other.message and self._bool == other._bool
+            return (
+                self.message == other.message
+                and self._bool == other._bool
+                and self.require_api_update == other.require_api_update
+            )
         return self._bool == other
 
     def __repr__(self) -> str:
         _class_name_ = type(self).__name__
         return f"{_class_name_}: {self.message}"
 
     def __str__(self) -> str:
```

### Comparing `syft-0.8.5b9/src/syft/service/service.py` & `syft-0.8.6b1/src/syft/service/service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/settings/settings.py` & `syft-0.8.6b1/src/syft/service/settings/settings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/settings/settings_service.py` & `syft-0.8.6b1/src/syft/service/settings/settings_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/settings/settings_stash.py` & `syft-0.8.6b1/src/syft/service/settings/settings_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/sync/diff_state.py` & `syft-0.8.6b1/src/syft/service/sync/diff_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/sync/sync_service.py` & `syft-0.8.6b1/src/syft/service/sync/sync_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/sync/sync_stash.py` & `syft-0.8.6b1/src/syft/service/sync/sync_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/sync/sync_state.py` & `syft-0.8.6b1/src/syft/service/sync/sync_state.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/user/user.py` & `syft-0.8.6b1/src/syft/service/user/user.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/user/user_roles.py` & `syft-0.8.6b1/src/syft/service/user/user_roles.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/user/user_service.py` & `syft-0.8.6b1/src/syft/service/user/user_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/user/user_stash.py` & `syft-0.8.6b1/src/syft/service/user/user_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/veilid/veilid_service.py` & `syft-0.8.6b1/src/syft/service/veilid/veilid_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/warnings.py` & `syft-0.8.6b1/src/syft/service/warnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/image_identifier.py` & `syft-0.8.6b1/src/syft/service/worker/image_identifier.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/image_registry.py` & `syft-0.8.6b1/src/syft/service/worker/image_registry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/image_registry_service.py` & `syft-0.8.6b1/src/syft/service/worker/image_registry_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/image_registry_stash.py` & `syft-0.8.6b1/src/syft/service/worker/image_registry_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/utils.py` & `syft-0.8.6b1/src/syft/service/worker/utils.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/worker.py` & `syft-0.8.6b1/src/syft/service/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/worker_image.py` & `syft-0.8.6b1/src/syft/service/worker/worker_image.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/worker_image_service.py` & `syft-0.8.6b1/src/syft/service/worker/worker_image_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/worker_image_stash.py` & `syft-0.8.6b1/src/syft/service/worker/worker_image_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/worker_pool.py` & `syft-0.8.6b1/src/syft/service/worker/worker_pool.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/worker_pool_service.py` & `syft-0.8.6b1/src/syft/service/worker/worker_pool_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/worker_pool_stash.py` & `syft-0.8.6b1/src/syft/service/worker/worker_pool_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/worker_service.py` & `syft-0.8.6b1/src/syft/service/worker/worker_service.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/service/worker/worker_stash.py` & `syft-0.8.6b1/src/syft/service/worker/worker_stash.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/store/blob_storage/__init__.py` & `syft-0.8.6b1/src/syft/store/blob_storage/__init__.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/store/blob_storage/on_disk.py` & `syft-0.8.6b1/src/syft/store/blob_storage/on_disk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # stdlib
 from io import BytesIO
 from pathlib import Path
-from tempfile import gettempdir
 from typing import Any
 
 # third party
 from typing_extensions import Self
 
 # relative
 from . import BlobDeposit
@@ -84,15 +83,15 @@
             return SyftSuccess(message="Successfully deleted file.")
         except FileNotFoundError as e:
             return SyftError(message=f"Failed to delete file: {e}")
 
 
 @serializable()
 class OnDiskBlobStorageClientConfig(BlobStorageClientConfig):
-    base_directory: Path = Path(gettempdir())
+    base_directory: Path
 
 
 @serializable()
 class OnDiskBlobStorageClient(BlobStorageClient):
     config: OnDiskBlobStorageClientConfig
 
     def __init__(self, **data: Any):
@@ -102,8 +101,8 @@
     def connect(self) -> BlobStorageConnection:
         return OnDiskBlobStorageConnection(self.config.base_directory)
 
 
 @serializable()
 class OnDiskBlobStorageConfig(BlobStorageConfig):
     client_type: type[BlobStorageClient] = OnDiskBlobStorageClient
-    client_config: OnDiskBlobStorageClientConfig = OnDiskBlobStorageClientConfig()
+    client_config: OnDiskBlobStorageClientConfig
```

### Comparing `syft-0.8.5b9/src/syft/store/blob_storage/seaweedfs.py` & `syft-0.8.6b1/src/syft/store/blob_storage/seaweedfs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/store/dict_document_store.py` & `syft-0.8.6b1/src/syft/store/dict_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # future
 from __future__ import annotations
 
 # stdlib
 from typing import Any
 
+# third party
+from pydantic import Field
+
 # relative
 from ..node.credentials import SyftVerifyKey
 from ..serde.serializable import serializable
 from ..types import uid
 from .document_store import DocumentStore
 from .document_store import StoreConfig
 from .kv_document_store import KeyValueBackingStore
@@ -97,8 +100,8 @@
                 * ThreadingLockingConfig: threading-based locking, ideal for same-process in-memory stores.
                 * FileLockingConfig: file based locking, ideal for same-device different-processes/threads stores.
             Defaults to ThreadingLockingConfig.
     """
 
     store_type: type[DocumentStore] = DictDocumentStore
     backing_store: type[KeyValueBackingStore] = DictBackingStore
-    locking_config: LockingConfig = ThreadingLockingConfig()
+    locking_config: LockingConfig = Field(default_factory=ThreadingLockingConfig)
```

### Comparing `syft-0.8.5b9/src/syft/store/document_store.py` & `syft-0.8.6b1/src/syft/store/document_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from collections.abc import Callable
 import types
 import typing
 from typing import Any
 
 # third party
 from pydantic import BaseModel
+from pydantic import Field
 from result import Err
 from result import Ok
 from result import Result
 from typeguard import check_type
 
 # relative
 from ..node.credentials import SyftSigningKey
@@ -312,15 +313,15 @@
             root_verify_key = SyftSigningKey.generate().verify_key
         self.node_uid = node_uid
         self.root_verify_key = root_verify_key
         self.settings = settings
         self.store_config = store_config
         self.init_store()
 
-        store_config.locking_config.lock_name = settings.name
+        store_config.locking_config.lock_name = f"StorePartition-{settings.name}"
         self.lock = SyftLock(store_config.locking_config)
 
     def init_store(self) -> Result[Ok, Err]:
         try:
             self.unique_cks = self.settings.unique_keys.all
             self.searchable_cks = self.settings.searchable_keys.all
         except BaseException as e:
@@ -779,8 +780,8 @@
     """
 
     __canonical_name__ = "StoreConfig"
     __version__ = SYFT_OBJECT_VERSION_2
 
     store_type: type[DocumentStore]
     client_config: StoreClientConfig | None = None
-    locking_config: LockingConfig = NoLockingConfig()
+    locking_config: LockingConfig = Field(default_factory=NoLockingConfig)
```

### Comparing `syft-0.8.5b9/src/syft/store/kv_document_store.py` & `syft-0.8.6b1/src/syft/store/kv_document_store.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/store/linked_obj.py` & `syft-0.8.6b1/src/syft/store/linked_obj.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/store/locks.py` & `syft-0.8.6b1/src/syft/store/locks.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/store/mongo_client.py` & `syft-0.8.6b1/src/syft/store/mongo_client.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/store/mongo_codecs.py` & `syft-0.8.6b1/src/syft/store/mongo_codecs.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/store/mongo_document_store.py` & `syft-0.8.6b1/src/syft/store/mongo_document_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # stdlib
 from collections.abc import Callable
 from typing import Any
 
 # third party
+from pydantic import Field
 from pymongo import ASCENDING
 from pymongo.collection import Collection as MongoCollection
 from result import Err
 from result import Ok
 from result import Result
 from typing_extensions import Self
 
@@ -868,8 +869,8 @@
     """
 
     client_config: MongoStoreClientConfig
     store_type: type[DocumentStore] = MongoDocumentStore
     db_name: str = "app"
     backing_store: type[KeyValueBackingStore] = MongoBackingStore
     # TODO: should use a distributed lock, with RedisLockingConfig
-    locking_config: LockingConfig = NoLockingConfig()
+    locking_config: LockingConfig = Field(default_factory=NoLockingConfig)
```

### Comparing `syft-0.8.5b9/src/syft/store/sqlite_document_store.py` & `syft-0.8.6b1/src/syft/store/sqlite_document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 from ..util.util import thread_ident
 from .document_store import DocumentStore
 from .document_store import PartitionSettings
 from .document_store import StoreClientConfig
 from .document_store import StoreConfig
 from .kv_document_store import KeyValueBackingStore
 from .kv_document_store import KeyValueStorePartition
-from .locks import FileLockingConfig
 from .locks import LockingConfig
+from .locks import NoLockingConfig
 from .locks import SyftLock
 
 # here we can create a single connection per cache_key
 # since pytest is concurrent processes, we need to isolate each connection
 # by its filename and optionally the thread that its running in
 # we keep track of each SQLiteBackingStore init in REF_COUNTS
 # when it hits 0 we can close the connection and release the file descriptor
@@ -97,19 +97,15 @@
         self.store_config = store_config
         self._ddtype = ddtype
         if self.store_config.client_config:
             self.file_path = self.store_config.client_config.file_path
         if store_config.client_config:
             self.db_filename = store_config.client_config.filename
 
-        # if tempfile.TemporaryDirectory() varies from process to process
-        # could this cause different locks on the same file
-        temp_dir = tempfile.TemporaryDirectory().name
-        lock_path = Path(temp_dir) / "sqlite_locks" / self.db_filename
-        self.lock_config = FileLockingConfig(client_path=lock_path)
+        self.lock = SyftLock(NoLockingConfig())
         self.create_table()
         REF_COUNTS[cache_key(self.db_filename)] += 1
 
     @property
     def table_name(self) -> str:
         return f"{self.settings.name}_{self.index_name}"
 
@@ -127,22 +123,24 @@
         if self.store_config.client_config:
             connection = sqlite3.connect(
                 self.file_path,
                 timeout=self.store_config.client_config.timeout,
                 check_same_thread=False,  # do we need this if we use the lock?
                 # check_same_thread=self.store_config.client_config.check_same_thread,
             )
-            # TODO: Review OSX compatibility.
             # Set journal mode to WAL.
-            # connection.execute("pragma journal_mode=wal")
+            connection.execute("PRAGMA journal_mode = WAL")
+            connection.execute("PRAGMA busy_timeout = 5000")
+            connection.execute("PRAGMA temp_store = 2")
+            connection.execute("PRAGMA synchronous = 1")
             SQLITE_CONNECTION_POOL_DB[cache_key(self.db_filename)] = connection
 
     def create_table(self) -> None:
         try:
-            with SyftLock(self.lock_config):
+            with self.lock:
                 self.cur.execute(
                     f"create table {self.table_name} (uid VARCHAR(32) NOT NULL PRIMARY KEY, "  # nosec
                     + "repr TEXT NOT NULL, value BLOB NOT NULL, "  # nosec
                     + "sqltime TIMESTAMP DEFAULT CURRENT_TIMESTAMP NOT NULL)"  # nosec
                 )
                 self.db.commit()
         except Exception as e:
@@ -175,15 +173,15 @@
 
     def _commit(self) -> None:
         self.db.commit()
 
     def _execute(
         self, sql: str, *args: list[Any] | None
     ) -> Result[Ok[sqlite3.Cursor], Err[str]]:
-        with SyftLock(self.lock_config):
+        with self.lock:
             cursor: sqlite3.Cursor | None = None
             # err = None
             try:
                 cursor = self.cur.execute(sql, *args)
             except Exception as e:
                 raise_exception(self.table_name, e)
 
@@ -421,15 +419,15 @@
             data corruption.
         `timeout`: int
             How many seconds the connection should wait before raising an exception, if the database
             is locked by another connection. If another connection opens a transaction to modify the
             database, it will be locked until that transaction is committed. Default five seconds.
     """
 
-    filename: str | None = None
+    filename: str = "syftdb.sqlite"
     path: str | Path = Field(default_factory=tempfile.gettempdir)
     check_same_thread: bool = True
     timeout: int = 5
 
     # We need this in addition to Field(default_factory=...)
     # so users can still do SQLiteStoreClientConfig(path=None)
     @field_validator("path", mode="before")
@@ -437,15 +435,15 @@
     def __default_path(cls, path: str | Path | None) -> str | Path:
         if path is None:
             return tempfile.gettempdir()
         return path
 
     @property
     def file_path(self) -> Path | None:
-        return Path(self.path) / self.filename if self.filename is not None else None
+        return Path(self.path) / self.filename
 
 
 @serializable()
 class SQLiteStoreConfig(StoreConfig):
     __canonical_name__ = "SQLiteStoreConfig"
     """SQLite Store config, used by SQLiteStorePartition
 
@@ -463,8 +461,8 @@
                 * FileLockingConfig: file based locking, ideal for same-device different-processes/threads stores.
             Defaults to FileLockingConfig.
     """
 
     client_config: SQLiteStoreClientConfig
     store_type: type[DocumentStore] = SQLiteDocumentStore
     backing_store: type[KeyValueBackingStore] = SQLiteBackingStore
-    locking_config: LockingConfig = FileLockingConfig()
+    locking_config: LockingConfig = Field(default_factory=NoLockingConfig)
```

### Comparing `syft-0.8.5b9/src/syft/types/blob_storage.py` & `syft-0.8.6b1/src/syft/types/blob_storage.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/types/datetime.py` & `syft-0.8.6b1/src/syft/types/datetime.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/types/dicttuple.py` & `syft-0.8.6b1/src/syft/types/dicttuple.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/types/grid_url.py` & `syft-0.8.6b1/src/syft/types/grid_url.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/types/identity.py` & `syft-0.8.6b1/src/syft/types/identity.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/types/syft_metaclass.py` & `syft-0.8.6b1/src/syft/types/syft_metaclass.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/types/syft_migration.py` & `syft-0.8.6b1/src/syft/types/syft_migration.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/types/syft_object.py` & `syft-0.8.6b1/src/syft/types/syft_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/types/syncable_object.py` & `syft-0.8.6b1/src/syft/types/syncable_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/types/transforms.py` & `syft-0.8.6b1/src/syft/types/transforms.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/types/twin_object.py` & `syft-0.8.6b1/src/syft/types/twin_object.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/types/uid.py` & `syft-0.8.6b1/src/syft/types/uid.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/_std_stream_capture.py` & `syft-0.8.6b1/src/syft/util/_std_stream_capture.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/autoreload.py` & `syft-0.8.6b1/src/syft/util/autoreload.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/decorators.py` & `syft-0.8.6b1/src/syft/util/decorators.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/experimental_flags.py` & `syft-0.8.6b1/src/syft/util/experimental_flags.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/filterwarnings.py` & `syft-0.8.6b1/src/syft/util/filterwarnings.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/fonts.py` & `syft-0.8.6b1/src/syft/util/fonts.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/logger.py` & `syft-0.8.6b1/src/syft/util/logger.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/markdown.py` & `syft-0.8.6b1/src/syft/util/markdown.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/notebook_ui/notebook_addons.py` & `syft-0.8.6b1/src/syft/util/notebook_ui/notebook_addons.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/schema.py` & `syft-0.8.6b1/src/syft/util/schema.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/telemetry.py` & `syft-0.8.6b1/src/syft/util/telemetry.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/trace_decorator.py` & `syft-0.8.6b1/src/syft/util/trace_decorator.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/util.py` & `syft-0.8.6b1/src/syft/util/util.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft/util/version_compare.py` & `syft-0.8.6b1/src/syft/util/version_compare.py`

 * *Files identical despite different names*

### Comparing `syft-0.8.5b9/src/syft.egg-info/PKG-INFO` & `syft-0.8.6b1/src/syft.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syft
-Version: 0.8.5b9
+Version: 0.8.6b1
 Summary: Perform numpy-like analysis on data that remains in someone elses server
 Home-page: https://openmined.github.io/PySyft/
 Author: OpenMined
 Author-email: info@openmined.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/OpenMined/PySyft
 Project-URL: Tracker, https://github.com/OpenMined/PySyft/issues
@@ -101,15 +101,15 @@
 Requires-Dist: coverage; extra == "test-plugins"
 Requires-Dist: faker; extra == "test-plugins"
 Requires-Dist: distro; extra == "test-plugins"
 
 <div align="left"> <a href="https://pypi.org/project/syft/"><img src="https://static.pepy.tech/badge/pysyft" /></a> <a href="https://pypi.org/project/syft/"><img src="https://badge.fury.io/py/syft.svg" /></a> <a href="https://hub.docker.com/u/openmined"><img src="https://img.shields.io/badge/docker-images-blue?logo=docker" /></a> <a href="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml"><img src="https://github.com/OpenMined/PySyft/actions/workflows/nightlies.yml/badge.svg?branch=dev" /></a> <a href="https://slack.openmined.org/"><img src="https://img.shields.io/badge/chat-on%20slack-purple?logo=slack" /></a> <a href="https://openmined.github.io/PySyft/"><img src="https://img.shields.io/badge/read-docs-yellow?logo=mdbook" /></a>
 <br /><br /></div>
 
-<img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/title_syft_light.png" width="200px" />
+<img alt="Syft Logo" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/title_syft_light.png" width="200px" />
 
 Perform data science on `data` that remains in `someone else's` server
 
 # Quickstart
 
 ✅ `Linux` ✅ `macOS` ✅ `Windows` ✅ `Docker` ✅ `Podman` ✅ `Kubernetes`
 
@@ -120,49 +120,49 @@
 ```
 
 ## Launch Server
 
 ```python
 # from Jupyter / Python
 import syft as sy
-sy.requires(">=0.8.4,<0.8.5")
+sy.requires(">=0.8.5,<0.8.6")
 node = sy.orchestra.launch(name="my-domain", port=8080, dev_mode=True, reset=True)
 ```
 
 ```bash
 # or from the command line
 $ syft launch --name=my-domain --port=8080 --reset=True
 
 Starting syft-node server on 0.0.0.0:8080
 ```
 
 ## Launch Client
 
 ```python
 import syft as sy
-sy.requires(">=0.8.4,<0.8.5")
+sy.requires(">=0.8.5,<0.8.6")
 domain_client = sy.login(port=8080, email="info@openmined.org", password="changethis")
 ```
 
 ## PySyft in 10 minutes
 
-📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api">API Example Notebooks</a>
+📝 <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api">API Example Notebooks</a>
 
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/00-load-data.ipynb">00-load-data.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/01-submit-code.ipynb">01-submit-code.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/02-review-code-and-approve.ipynb">02-review-code-and-approve.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/03-data-scientist-download-result.ipynb">03-data-scientist-download-result.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/04-jax-example.ipynb">04-jax-example.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/05-custom-policy.ipynb">05-custom-policy.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/06-multiple-code-requests.ipynb">06-multiple-code-requests.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/07-domain-register-control-flow.ipynb">07-domain-register-control-flow.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/08-code-version.ipynb">08-code-version.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/09-blob-storage.ipynb">09-blob-storage.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/10-container-images.ipynb">10-container-images.ipynb</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/api/0.8/11-container-images-k8s.ipynb">11-container-images-k8s.ipynb</a>
 
 ## Deploy Kubernetes Helm Chart
 
 **Note**: Assuming we have a Kubernetes cluster already setup.
 
 #### 1. Add and update Helm repo for Syft
 
@@ -233,19 +233,20 @@
 - Interactive Install 🧙🏽‍♂️ Wizard<sup>BETA</sup> Requires 🛵 `hagrid`: - Run: `hagrid quickstart`
 - PySyft 0.8.1 Requires: 🐍 `python 3.10 - 3.12` - Run: `pip install -U syft`
 - PyGrid Requires: 🐳 `docker`, 🦦 `podman` or ☸️ `kubernetes` - Run: `hagrid launch ...`
 
 # Versions
 
 `0.9.0` - Coming soon...  
-`0.8.5` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
-`0.8.4` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
+`0.8.6` (Beta) - `dev` branch 👈🏽 <a href="https://github.com/OpenMined/PySyft/tree/dev/notebooks/api/0.8">API</a> - Coming soon...  
+`0.8.5` (Stable) - <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/api/0.8">API</a>
 
 Deprecated:
 
+- `0.8.4` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.4/notebooks/api/0.8">API</a>
 - `0.8.3` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.3/notebooks/api/0.8">API</a>
 - `0.8.2` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.2/notebooks/api/0.8">API</a>
 - `0.8.1` - <a href="https://github.com/OpenMined/PySyft/tree/0.8.1/notebooks/api/0.8">API</a>
 - `0.8.0` - <a href="https://github.com/OpenMined/PySyft/tree/0.8/notebooks/api/0.8">API</a>
 - `0.7.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science-dev">Course 3 Updated</a>
 - `0.6.0` - <a href="https://github.com/OpenMined/courses/tree/introduction-to-remote-data-science">Course 3</a>
 - `0.5.1` - <a href="https://github.com/OpenMined/courses/tree/foundations-of-private-computation">Course 2</a> + M1 Hotfix
@@ -259,15 +260,15 @@
 PySyft (Beta): `pip install -U syft --pre`  
 PyGrid (Beta): `hagrid launch ... tag=beta`
 
 HAGrid is a cli / deployment tool so the latest version of `hagrid` is usually the best.
 
 # What is Syft?
 
-<img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
+<img align="right" src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_big.png" alt="Syft" height="250" style="padding-left:30px;">
 
 `Syft` is OpenMined's `open source` stack that provides `secure` and `private` Data Science in Python. Syft decouples `private data` from model training, using techniques like [Federated Learning](https://ai.googleblog.com/2017/04/federated-learning-collaborative.html), [Differential Privacy](https://en.wikipedia.org/wiki/Differential_privacy), and [Encrypted Computation](https://en.wikipedia.org/wiki/Homomorphic_encryption). This is done with a `numpy`-like interface and integration with `Deep Learning` frameworks, so that you as a `Data Scientist` can maintain your current workflow while using these new `privacy-enhancing techniques`.
 
 ### Why should I use Syft?
 
 `Syft` allows a `Data Scientist` to ask `questions` about a `dataset` and, within `privacy limits` set by the `data owner`, get `answers` to those `questions`, all without obtaining a `copy` of the data itself. We call this process `Remote Data Science`. It means in a wide variety of `domains` across society, the current `risks` of sharing information (`copying` data) with someone such as, privacy invasion, IP theft and blackmail will no longer prevent the vast `benefits` such as innovation, insights and scientific discovery which secure access will provide.
 
@@ -277,39 +278,39 @@
 # Tutorials
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/dataowner.png" alt="" width="100" height="100" align="center">
 <p>Data Owner</p></div>
 </th>
 <th align="center">
 <img width="441" height="1">
-<div align="center"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
+<div align="center"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/datascientist.png" alt="" width="100" height="100" align="center">
 <p>Data Scientist</p></div>
 
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/personas_image/dataengineer.png" alt="" width="100" height="100" align="center">
 <p>Data Engineer</p>
 </div>
 </th>
 </tr>
 <tr>
 <td valign="top">
 
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/quickstart/data-owner/02-create-account-configure-pb.ipynb">Create Accounts</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/00-deploy-domain.ipynb">Deploy a Domain Server</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/01-upload-data.ipynb">Upload Private Data</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/02-create-account-configure-pb.ipynb">Create Accounts</a>
 - Manage Privacy Budget</a>
-- <a href="https://github.com/OpenMined/PySyft/tree/0.8.5/notebooks/quickstart/data-owner/03-join-network.ipynb">Join a Network</a>
+- <a href="https://github.com/OpenMined/PySyft/tree/0.8.6/notebooks/quickstart/data-owner/03-join-network.ipynb">Join a Network</a>
 - Learn how PETs streamline Data Policies
 
 </td>
 <td valign="top">
 
 - Install Syft</a>
 - Connect to a Domain</a>
@@ -389,25 +390,25 @@
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_slack_title_light.png" alt="" width="100%" align="center" />
 
-<a href="https://slack.openmined.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
+<a href="https://slack.openmined.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_slack.png" alt="" width="100%" align="center" /></a>
 
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_title_videos_papers_light.png" alt="" width="100%" align="center" />
 
 <p align="left"><sub><sup>
 🎥 <a href="https://www.youtube.com/watch?v=qVf0tPBzr2k">PETs: Remote Data Science Unleashed - R gov 2021</a><br />
 🎥 <a href="https://youtu.be/sCoDWKTbh3s?list=PL_lsbAsL_o2BQKXG7mkGFA8LSApCnhljL">Introduction to Remote Data Science - PyTorch 2021</a><br />
 🎥 <a href="https://youtu.be/kzLeTz_vIeQ?list=PL_lsbAsL_o2BtOz6KUfUI_Zla6Rg5dmyc">The Future of AI Tools - PyTorch 2020</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=4zrU54VIK6k&t=1s">Privacy Preserving AI - MIT Deep Learning Series</a><br />
 🎥 <a href="https://www.youtube.com/watch?v=Pr4erdusiW0">Privacy-Preserving Data Science - TWiML Talk #241</a><br />
@@ -418,106 +419,106 @@
 </sup></sup></p>
 </div>
 </th>
 <th align="center" valign="top">
 <img width="441" height="1">
 <div align="center">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_padawan_title_light.png" alt="" width="100%" align="center" />
 
-<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
+<a href="https://blog.openmined.org/work-on-ais-most-exciting-frontier-no-phd-required/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/panel_padawan.png" alt="" width="100%" align="center"></a>
 
 </div>
 </th>
 </tr>
 </table>
 
 # Courses
 
 <table border="5" bordercolor="grey">
 <tr>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
+<a href="https://courses.openmined.org/courses/our-privacy-opportunity"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_privacy.png" alt="" width="100%" align="center" /></a>
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
+<a href="https://courses.openmined.org/courses/foundations-of-private-computation"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_foundations.png" alt="" width="100%" align="center" /></a>
 </div>
 </th>
 <th align="center">
 <img width="441" height="1">
 <div align="center">
-<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
+<a href="https://courses.openmined.org/courses/introduction-to-remote-data-science"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/course_introduction.png" alt="" width="100%" align="center"></a>
 </div>
 </th>
 </tr>
 </table>
 
 # Contributors
 
 OpenMined and Syft appreciates all contributors, if you would like to fix a bug or suggest a new feature, please see our [guidelines](https://openmined.github.io/PySyft/developer_guide/index.html).<br />
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/contributors_light.jpg" alt="Contributors" width="100%" />
 
 # Supporters
 
 <table border="0">
 <tr>
 <th align="center">
-<a href="https://sloan.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_sloan.png" /></a>
+<a href="https://sloan.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_sloan.png" /></a>
 </th>
 <th align="center">
-<a href="https://opensource.fb.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_meta.png" /></a>
+<a href="https://opensource.fb.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_meta.png" /></a>
 </th>
 <th align="center">
-<a href="https://pytorch.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_torch.png" /></a>
+<a href="https://pytorch.org/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_torch.png" /></a>
 </th>
 <th align="center">
 <a href="https://www.dpmc.govt.nz/">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_nz_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_nz_light.png" />
 </a>
 </th>
 <th align="center">
-<a href="https://twitter.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_twitter.png" /></a>
+<a href="https://twitter.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_twitter.png" /></a>
 </th>
 <th align="center">
-<a href="https://google.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_google.png" /></a>
+<a href="https://google.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_google.png" /></a>
 </th>
 <th align="center">
-<a href="https://microsoft.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_microsoft.png" /></a>
+<a href="https://microsoft.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_microsoft.png" /></a>
 </th>
 <th align="center">
-<a href="https://omidyar.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_on.png" /></a>
+<a href="https://omidyar.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_on.png" /></a>
 </th>
 <th align="center">
-<a href="https://www.udacity.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_udacity.png" /></a>
+<a href="https://www.udacity.com/"><img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_udacity.png" /></a>
 </th>
 <th align="center">
 <a href="https://www.centerfordigitalhealthinnovation.org/">
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_cdhi_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_cdhi_light.png" />
 
 </a>
 </th>
 <th align="center">
 <a href="https://arkhn.org/">
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/logo_arkhn_light.png" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/logo_arkhn_light.png" />
 </a>
 </th>
 </tr>
 </table>
 
 # Open Collective
 
 `OpenMined` is a fiscally sponsored `501(c)(3)` in the USA. We are funded by our generous supporters on <a href="https://opencollective.com/openmined">Open Collective</a>. <br /><br />
 
-<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.5/docs/img/opencollective_light.png" alt="Contributors" width="100%" />
+<img src="https://raw.githubusercontent.com/OpenMined/PySyft/0.8.6/docs/img/opencollective_light.png" alt="Contributors" width="100%" />
 
 # Disclaimer
 
 Syft is under active development and is not yet ready for pilots on private data without our assistance. As early access participants, please contact us via [Slack](https://slack.openmined.org/) or email if you would like to ask a question or have a use case that you would like to discuss.
 
 # License
```

### Comparing `syft-0.8.5b9/src/syft.egg-info/SOURCES.txt` & `syft-0.8.6b1/src/syft.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -73,14 +73,15 @@
 src/syft/node/worker.py
 src/syft/node/worker_settings.py
 src/syft/protocol/data_protocol.py
 src/syft/protocol/protocol_version.json
 src/syft/protocol/releases/0.8.2.json
 src/syft/protocol/releases/0.8.3.json
 src/syft/protocol/releases/0.8.4.json
+src/syft/protocol/releases/0.8.5.json
 src/syft/serde/__init__.py
 src/syft/serde/array.py
 src/syft/serde/arrow.py
 src/syft/serde/capnp.py
 src/syft/serde/deserialize.py
 src/syft/serde/lib_permissions.py
 src/syft/serde/lib_service_registry.py
@@ -226,14 +227,15 @@
 src/syft/store/sqlite_document_store.py
 src/syft/store/blob_storage/__init__.py
 src/syft/store/blob_storage/on_disk.py
 src/syft/store/blob_storage/seaweedfs.py
 src/syft/types/__init__.py
 src/syft/types/base.py
 src/syft/types/blob_storage.py
+src/syft/types/cache_object.py
 src/syft/types/datetime.py
 src/syft/types/dicttuple.py
 src/syft/types/grid_url.py
 src/syft/types/identity.py
 src/syft/types/syft_metaclass.py
 src/syft/types/syft_migration.py
 src/syft/types/syft_object.py
```

### Comparing `syft-0.8.5b9/src/syft.egg-info/requires.txt` & `syft-0.8.6b1/src/syft.egg-info/requires.txt`

 * *Files identical despite different names*

