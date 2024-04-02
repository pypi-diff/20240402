# Comparing `tmp/prodvana-0.3.8.tar.gz` & `tmp/prodvana-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prodvana-0.3.8.tar", max compression
+gzip compressed data, was "prodvana-0.3.9.tar", max compression
```

## Comparing `prodvana-0.3.8.tar` & `prodvana-0.3.9.tar`

### file list

```diff
@@ -1,380 +1,380 @@
--rw-r--r--   0        0        0       81 2023-11-29 19:16:46.167324 prodvana-0.3.8/README.md
--rw-r--r--   0        0        0        0 2023-11-29 19:16:46.167324 prodvana-0.3.8/prodvana/__init__.py
--rw-r--r--   0        0        0     3529 2023-11-29 19:16:46.167324 prodvana-0.3.8/prodvana/client.py
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.003013 prodvana-0.3.8/prodvana/proto/__init__.py
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.003013 prodvana-0.3.8/prodvana/proto/prodvana/__init__.py
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.031013 prodvana-0.3.8/prodvana/proto/prodvana/agent/__init__.py
--rw-r--r--   0        0        0    10322 2023-12-01 02:12:09.547013 prodvana-0.3.8/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
--rw-r--r--   0        0        0    20472 2023-12-01 02:12:09.887013 prodvana-0.3.8/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
--rw-r--r--   0        0        0    24439 2023-12-01 02:12:09.547013 prodvana-0.3.8/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
--rw-r--r--   0        0        0     7291 2023-12-01 02:12:09.887013 prodvana-0.3.8/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.039013 prodvana-0.3.8/prodvana/proto/prodvana/application/__init__.py
--rw-r--r--   0        0        0     3899 2023-12-01 02:12:09.591013 prodvana-0.3.8/prodvana/proto/prodvana/application/application_config_pb2.py
--rw-r--r--   0        0        0     3656 2023-12-01 02:12:09.935013 prodvana-0.3.8/prodvana/proto/prodvana/application/application_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.587013 prodvana-0.3.8/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.931013 prodvana-0.3.8/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    15907 2023-12-01 02:12:09.587013 prodvana-0.3.8/prodvana/proto/prodvana/application/application_manager_pb2.py
--rw-r--r--   0        0        0    16830 2023-12-01 02:12:09.943013 prodvana-0.3.8/prodvana/proto/prodvana/application/application_manager_pb2.pyi
--rw-r--r--   0        0        0    22241 2023-12-01 02:12:09.595013 prodvana-0.3.8/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6755 2023-12-01 02:12:09.947013 prodvana-0.3.8/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2235 2023-12-01 02:12:09.599013 prodvana-0.3.8/prodvana/proto/prodvana/application/object_pb2.py
--rw-r--r--   0        0        0     2184 2023-12-01 02:12:09.939013 prodvana-0.3.8/prodvana/proto/prodvana/application/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.599013 prodvana-0.3.8/prodvana/proto/prodvana/application/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.931013 prodvana-0.3.8/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     2011 2023-12-01 02:12:09.591013 prodvana-0.3.8/prodvana/proto/prodvana/application/user_metadata_pb2.py
--rw-r--r--   0        0        0     1670 2023-12-01 02:12:09.943013 prodvana-0.3.8/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.595013 prodvana-0.3.8/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.939013 prodvana-0.3.8/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.047013 prodvana-0.3.8/prodvana/proto/prodvana/async_task/__init__.py
--rw-r--r--   0        0        0     1540 2023-12-01 02:12:09.635013 prodvana-0.3.8/prodvana/proto/prodvana/async_task/task_metadata_pb2.py
--rw-r--r--   0        0        0     1657 2023-12-01 02:12:09.983013 prodvana-0.3.8/prodvana/proto/prodvana/async_task/task_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.635013 prodvana-0.3.8/prodvana/proto/prodvana/async_task/task_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.979013 prodvana-0.3.8/prodvana/proto/prodvana/async_task/task_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.043013 prodvana-0.3.8/prodvana/proto/prodvana/auth/__init__.py
--rw-r--r--   0        0        0     8480 2023-12-01 02:12:09.615013 prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_manager_pb2.py
--rw-r--r--   0        0        0    10206 2023-12-01 02:12:09.955013 prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
--rw-r--r--   0        0        0    18631 2023-12-01 02:12:09.607013 prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
--rw-r--r--   0        0        0     6767 2023-12-01 02:12:09.963013 prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3181 2023-12-01 02:12:09.615013 prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_pb2.py
--rw-r--r--   0        0        0     5515 2023-12-01 02:12:09.959013 prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.611013 prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.959013 prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.043013 prodvana-0.3.8/prodvana/proto/prodvana/blobs/__init__.py
--rw-r--r--   0        0        0     2733 2023-12-01 02:12:09.607013 prodvana-0.3.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
--rw-r--r--   0        0        0     1947 2023-12-01 02:12:09.951013 prodvana-0.3.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
--rw-r--r--   0        0        0     4464 2023-12-01 02:12:09.603013 prodvana-0.3.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
--rw-r--r--   0        0        0     1398 2023-12-01 02:12:09.955013 prodvana-0.3.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.015013 prodvana-0.3.8/prodvana/proto/prodvana/capability/__init__.py
--rw-r--r--   0        0        0     4830 2023-12-01 02:12:09.423013 prodvana-0.3.8/prodvana/proto/prodvana/capability/capability_pb2.py
--rw-r--r--   0        0        0     5455 2023-12-01 02:12:09.759013 prodvana-0.3.8/prodvana/proto/prodvana/capability/capability_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.423013 prodvana-0.3.8/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.755013 prodvana-0.3.8/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.015013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/__init__.py
--rw-r--r--   0        0        0     1988 2023-12-01 02:12:09.383013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/constants_pb2.py
--rw-r--r--   0        0        0     1667 2023-12-01 02:12:09.739013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/constants_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.407013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/constants_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.703013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/constants_pb2_grpc.pyi
--rw-r--r--   0        0        0     1366 2023-12-01 02:12:09.415013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
--rw-r--r--   0        0        0      869 2023-12-01 02:12:09.751013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.367013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.735013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
--rw-r--r--   0        0        0     3398 2023-12-01 02:12:09.419013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/env_pb2.py
--rw-r--r--   0        0        0     4125 2023-12-01 02:12:09.751013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/env_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.379013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.699013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
--rw-r--r--   0        0        0     2102 2023-12-01 02:12:09.379013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/external_link_pb2.py
--rw-r--r--   0        0        0     1796 2023-12-01 02:12:09.711013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/external_link_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.391013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/external_link_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.707013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/external_link_pb2_grpc.pyi
--rw-r--r--   0        0        0     4409 2023-12-01 02:12:09.411013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/helm_pb2.py
--rw-r--r--   0        0        0     5957 2023-12-01 02:12:09.731013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/helm_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.419013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.715013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
--rw-r--r--   0        0        0     3479 2023-12-01 02:12:09.395013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
--rw-r--r--   0        0        0     7059 2023-12-01 02:12:09.743013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.395013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.743013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     1738 2023-12-01 02:12:09.371013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/links_pb2.py
--rw-r--r--   0        0        0      846 2023-12-01 02:12:09.719013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/links_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.399013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.727013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
--rw-r--r--   0        0        0     1338 2023-12-01 02:12:09.367013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/maturity_pb2.py
--rw-r--r--   0        0        0     1103 2023-12-01 02:12:09.755013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.411013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.719013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
--rw-r--r--   0        0        0     1838 2023-12-01 02:12:09.399013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/meta_pb2.py
--rw-r--r--   0        0        0     2531 2023-12-01 02:12:09.715013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.383013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.731013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0     1866 2023-12-01 02:12:09.415013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/notification_pb2.py
--rw-r--r--   0        0        0     1337 2023-12-01 02:12:09.735013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/notification_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.391013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.747013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
--rw-r--r--   0        0        0     8463 2023-12-01 02:12:09.407013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/parameters_pb2.py
--rw-r--r--   0        0        0    11778 2023-12-01 02:12:09.711013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.371013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.739013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0     9143 2023-12-01 02:12:09.403013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/program_pb2.py
--rw-r--r--   0        0        0    15928 2023-12-01 02:12:09.747013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/program_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.387013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.723013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
--rw-r--r--   0        0        0     2686 2023-12-01 02:12:09.363013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/retry_pb2.py
--rw-r--r--   0        0        0     2757 2023-12-01 02:12:09.703013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/retry_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.375013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.727013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
--rw-r--r--   0        0        0     2989 2023-12-01 02:12:09.387013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/task_pb2.py
--rw-r--r--   0        0        0     4249 2023-12-01 02:12:09.707013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/task_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.375013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.723013 prodvana-0.3.8/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.007013 prodvana-0.3.8/prodvana/proto/prodvana/config_file/__init__.py
--rw-r--r--   0        0        0     3685 2023-12-01 02:12:09.331013 prodvana-0.3.8/prodvana/proto/prodvana/config_file/config_pb2.py
--rw-r--r--   0        0        0     4656 2023-12-01 02:12:09.667013 prodvana-0.3.8/prodvana/proto/prodvana/config_file/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.327013 prodvana-0.3.8/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.663013 prodvana-0.3.8/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.023013 prodvana-0.3.8/prodvana/proto/prodvana/config_writeback/__init__.py
--rw-r--r--   0        0        0     1388 2023-12-01 02:12:09.463013 prodvana-0.3.8/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
--rw-r--r--   0        0        0     1131 2023-12-01 02:12:09.795013 prodvana-0.3.8/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.459013 prodvana-0.3.8/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.795013 prodvana-0.3.8/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.051013 prodvana-0.3.8/prodvana/proto/prodvana/convergence/__init__.py
--rw-r--r--   0        0        0     1371 2023-12-01 02:12:09.647013 prodvana-0.3.8/prodvana/proto/prodvana/convergence/convergence_mode_pb2.py
--rw-r--r--   0        0        0     1159 2023-12-01 02:12:09.995013 prodvana-0.3.8/prodvana/proto/prodvana/convergence/convergence_mode_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.647013 prodvana-0.3.8/prodvana/proto/prodvana/convergence/convergence_mode_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.991013 prodvana-0.3.8/prodvana/proto/prodvana/convergence/convergence_mode_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.039013 prodvana-0.3.8/prodvana/proto/prodvana/delivery/__init__.py
--rw-r--r--   0        0        0     2079 2023-12-01 02:12:09.603013 prodvana-0.3.8/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
--rw-r--r--   0        0        0     2294 2023-12-01 02:12:09.947013 prodvana-0.3.8/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.599013 prodvana-0.3.8/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.951013 prodvana-0.3.8/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.023013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/__init__.py
--rw-r--r--   0        0        0     6161 2023-12-01 02:12:09.467013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/config_pb2.py
--rw-r--r--   0        0        0     8052 2023-12-01 02:12:09.807013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.467013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.799013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
--rw-r--r--   0        0        0     9624 2023-12-01 02:12:09.463013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
--rw-r--r--   0        0        0    10317 2023-12-01 02:12:09.811013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
--rw-r--r--   0        0        0    13097 2023-12-01 02:12:09.471013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3909 2023-12-01 02:12:09.799013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2015 2023-12-01 02:12:09.471013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/object_pb2.py
--rw-r--r--   0        0        0     1862 2023-12-01 02:12:09.807013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.475013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.803013 prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.023013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/__init__.py
--rw-r--r--   0        0        0    31161 2023-12-01 02:12:09.479013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/manager_pb2.py
--rw-r--r--   0        0        0    48560 2023-12-01 02:12:09.823013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
--rw-r--r--   0        0        0    28235 2023-12-01 02:12:09.479013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
--rw-r--r--   0        0        0     9184 2023-12-01 02:12:09.811013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.023013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/__init__.py
--rw-r--r--   0        0        0    38726 2023-12-01 02:12:09.487013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
--rw-r--r--   0        0        0   115827 2023-12-01 02:12:09.819013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.483013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.815013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
--rw-r--r--   0        0        0     3694 2023-12-01 02:12:09.487013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
--rw-r--r--   0        0        0     8878 2023-12-01 02:12:09.815013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.483013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.819013 prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.007013 prodvana-0.3.8/prodvana/proto/prodvana/environment/__init__.py
--rw-r--r--   0        0        0    26543 2023-12-01 02:12:09.323013 prodvana-0.3.8/prodvana/proto/prodvana/environment/clusters_pb2.py
--rw-r--r--   0        0        0    54612 2023-12-01 02:12:09.659013 prodvana-0.3.8/prodvana/proto/prodvana/environment/clusters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.319013 prodvana-0.3.8/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.659013 prodvana-0.3.8/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
--rw-r--r--   0        0        0    14209 2023-12-01 02:12:09.319013 prodvana-0.3.8/prodvana/proto/prodvana/environment/environment_manager_pb2.py
--rw-r--r--   0        0        0    19436 2023-12-01 02:12:09.655013 prodvana-0.3.8/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
--rw-r--r--   0        0        0    25138 2023-12-01 02:12:09.327013 prodvana-0.3.8/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
--rw-r--r--   0        0        0     7335 2023-12-01 02:12:09.663013 prodvana-0.3.8/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.027013 prodvana-0.3.8/prodvana/proto/prodvana/events/__init__.py
--rw-r--r--   0        0        0     5103 2023-12-01 02:12:09.491013 prodvana-0.3.8/prodvana/proto/prodvana/events/events_manager_pb2.py
--rw-r--r--   0        0        0     6267 2023-12-01 02:12:09.827013 prodvana-0.3.8/prodvana/proto/prodvana/events/events_manager_pb2.pyi
--rw-r--r--   0        0        0     2714 2023-12-01 02:12:09.503013 prodvana-0.3.8/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
--rw-r--r--   0        0        0      853 2023-12-01 02:12:09.835013 prodvana-0.3.8/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2727 2023-12-01 02:12:09.495013 prodvana-0.3.8/prodvana/proto/prodvana/events/events_pb2.py
--rw-r--r--   0        0        0     4246 2023-12-01 02:12:09.839013 prodvana-0.3.8/prodvana/proto/prodvana/events/events_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.499013 prodvana-0.3.8/prodvana/proto/prodvana/events/events_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.831013 prodvana-0.3.8/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
--rw-r--r--   0        0        0    17212 2023-12-01 02:12:09.499013 prodvana-0.3.8/prodvana/proto/prodvana/events/types_pb2.py
--rw-r--r--   0        0        0    50754 2023-12-01 02:12:09.831013 prodvana-0.3.8/prodvana/proto/prodvana/events/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.491013 prodvana-0.3.8/prodvana/proto/prodvana/events/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.827013 prodvana-0.3.8/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.007013 prodvana-0.3.8/prodvana/proto/prodvana/impact_analysis/__init__.py
--rw-r--r--   0        0        0     2389 2023-12-01 02:12:09.331013 prodvana-0.3.8/prodvana/proto/prodvana/impact_analysis/impact_analysis_pb2.py
--rw-r--r--   0        0        0     4064 2023-12-01 02:12:09.667013 prodvana-0.3.8/prodvana/proto/prodvana/impact_analysis/impact_analysis_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.335013 prodvana-0.3.8/prodvana/proto/prodvana/impact_analysis/impact_analysis_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.671013 prodvana-0.3.8/prodvana/proto/prodvana/impact_analysis/impact_analysis_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.047013 prodvana-0.3.8/prodvana/proto/prodvana/insights/__init__.py
--rw-r--r--   0        0        0     2205 2023-12-01 02:12:09.631013 prodvana-0.3.8/prodvana/proto/prodvana/insights/insights_pb2.py
--rw-r--r--   0        0        0     3508 2023-12-01 02:12:09.975013 prodvana-0.3.8/prodvana/proto/prodvana/insights/insights_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.631013 prodvana-0.3.8/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.979013 prodvana-0.3.8/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.011013 prodvana-0.3.8/prodvana/proto/prodvana/labels/__init__.py
--rw-r--r--   0        0        0     1845 2023-12-01 02:12:09.347013 prodvana-0.3.8/prodvana/proto/prodvana/labels/labels_pb2.py
--rw-r--r--   0        0        0      854 2023-12-01 02:12:09.687013 prodvana-0.3.8/prodvana/proto/prodvana/labels/labels_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.351013 prodvana-0.3.8/prodvana/proto/prodvana/labels/labels_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.683013 prodvana-0.3.8/prodvana/proto/prodvana/labels/labels_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.051013 prodvana-0.3.8/prodvana/proto/prodvana/managed_resource/__init__.py
--rw-r--r--   0        0        0     8344 2023-12-01 02:12:09.643013 prodvana-0.3.8/prodvana/proto/prodvana/managed_resource/manager_pb2.py
--rw-r--r--   0        0        0    13338 2023-12-01 02:12:09.991013 prodvana-0.3.8/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
--rw-r--r--   0        0        0    12065 2023-12-01 02:12:09.643013 prodvana-0.3.8/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
--rw-r--r--   0        0        0     3657 2023-12-01 02:12:09.987013 prodvana-0.3.8/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.011013 prodvana-0.3.8/prodvana/proto/prodvana/metrics/__init__.py
--rw-r--r--   0        0        0     3762 2023-12-01 02:12:09.343013 prodvana-0.3.8/prodvana/proto/prodvana/metrics/metrics_pb2.py
--rw-r--r--   0        0        0     8746 2023-12-01 02:12:09.675013 prodvana-0.3.8/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.339013 prodvana-0.3.8/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.679013 prodvana-0.3.8/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.015013 prodvana-0.3.8/prodvana/proto/prodvana/object/__init__.py
--rw-r--r--   0        0        0     3353 2023-12-01 02:12:09.355013 prodvana-0.3.8/prodvana/proto/prodvana/object/manager_pb2.py
--rw-r--r--   0        0        0     2751 2023-12-01 02:12:09.699013 prodvana-0.3.8/prodvana/proto/prodvana/object/manager_pb2.pyi
--rw-r--r--   0        0        0     4330 2023-12-01 02:12:09.359013 prodvana-0.3.8/prodvana/proto/prodvana/object/manager_pb2_grpc.py
--rw-r--r--   0        0        0     1255 2023-12-01 02:12:09.691013 prodvana-0.3.8/prodvana/proto/prodvana/object/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2057 2023-12-01 02:12:09.363013 prodvana-0.3.8/prodvana/proto/prodvana/object/meta_pb2.py
--rw-r--r--   0        0        0     3160 2023-12-01 02:12:09.695013 prodvana-0.3.8/prodvana/proto/prodvana/object/meta_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.359013 prodvana-0.3.8/prodvana/proto/prodvana/object/meta_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.695013 prodvana-0.3.8/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.031013 prodvana-0.3.8/prodvana/proto/prodvana/organization/__init__.py
--rw-r--r--   0        0        0    10890 2023-12-01 02:12:09.535013 prodvana-0.3.8/prodvana/proto/prodvana/organization/organization_manager_pb2.py
--rw-r--r--   0        0        0    11248 2023-12-01 02:12:09.867013 prodvana-0.3.8/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
--rw-r--r--   0        0        0    16770 2023-12-01 02:12:09.535013 prodvana-0.3.8/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
--rw-r--r--   0        0        0     5422 2023-12-01 02:12:09.871013 prodvana-0.3.8/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2568 2023-12-01 02:12:09.531013 prodvana-0.3.8/prodvana/proto/prodvana/organization/user_metadata_pb2.py
--rw-r--r--   0        0        0     1972 2023-12-01 02:12:09.875013 prodvana-0.3.8/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.531013 prodvana-0.3.8/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.871013 prodvana-0.3.8/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.031013 prodvana-0.3.8/prodvana/proto/prodvana/pipelines/__init__.py
--rw-r--r--   0        0        0     2038 2023-12-01 02:12:09.543013 prodvana-0.3.8/prodvana/proto/prodvana/pipelines/object_pb2.py
--rw-r--r--   0        0        0     2595 2023-12-01 02:12:09.883013 prodvana-0.3.8/prodvana/proto/prodvana/pipelines/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.543013 prodvana-0.3.8/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.879013 prodvana-0.3.8/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     6748 2023-12-01 02:12:09.539013 prodvana-0.3.8/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
--rw-r--r--   0        0        0    11698 2023-12-01 02:12:09.875013 prodvana-0.3.8/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.539013 prodvana-0.3.8/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.883013 prodvana-0.3.8/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.019013 prodvana-0.3.8/prodvana/proto/prodvana/protection/__init__.py
--rw-r--r--   0        0        0     2777 2023-12-01 02:12:09.431013 prodvana-0.3.8/prodvana/proto/prodvana/protection/attachments_pb2.py
--rw-r--r--   0        0        0     2860 2023-12-01 02:12:09.779013 prodvana-0.3.8/prodvana/proto/prodvana/protection/attachments_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.443013 prodvana-0.3.8/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.763013 prodvana-0.3.8/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
--rw-r--r--   0        0        0     1716 2023-12-01 02:12:09.435013 prodvana-0.3.8/prodvana/proto/prodvana/protection/object_pb2.py
--rw-r--r--   0        0        0     1545 2023-12-01 02:12:09.775013 prodvana-0.3.8/prodvana/proto/prodvana/protection/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.439013 prodvana-0.3.8/prodvana/proto/prodvana/protection/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.763013 prodvana-0.3.8/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     6916 2023-12-01 02:12:09.427013 prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_config_pb2.py
--rw-r--r--   0        0        0    10730 2023-12-01 02:12:09.771013 prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.439013 prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.767013 prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
--rw-r--r--   0        0        0     8444 2023-12-01 02:12:09.443013 prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_manager_pb2.py
--rw-r--r--   0        0        0     9632 2023-12-01 02:12:09.767013 prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
--rw-r--r--   0        0        0    12468 2023-12-01 02:12:09.435013 prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
--rw-r--r--   0        0        0     3716 2023-12-01 02:12:09.771013 prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     3938 2023-12-01 02:12:09.431013 prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_reference_pb2.py
--rw-r--r--   0        0        0     4997 2023-12-01 02:12:09.775013 prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.427013 prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.759013 prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.015013 prodvana-0.3.8/prodvana/proto/prodvana/pvn_wrapper/__init__.py
--rw-r--r--   0        0        0     1789 2023-12-01 02:12:09.355013 prodvana-0.3.8/prodvana/proto/prodvana/pvn_wrapper/output_pb2.py
--rw-r--r--   0        0        0     2809 2023-12-01 02:12:09.691013 prodvana-0.3.8/prodvana/proto/prodvana/pvn_wrapper/output_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.351013 prodvana-0.3.8/prodvana/proto/prodvana/pvn_wrapper/output_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.687013 prodvana-0.3.8/prodvana/proto/prodvana/pvn_wrapper/output_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.043013 prodvana-0.3.8/prodvana/proto/prodvana/release/__init__.py
--rw-r--r--   0        0        0    12085 2023-12-01 02:12:09.619013 prodvana-0.3.8/prodvana/proto/prodvana/release/manager_pb2.py
--rw-r--r--   0        0        0    17840 2023-12-01 02:12:09.971013 prodvana-0.3.8/prodvana/proto/prodvana/release/manager_pb2.pyi
--rw-r--r--   0        0        0    14970 2023-12-01 02:12:09.619013 prodvana-0.3.8/prodvana/proto/prodvana/release/manager_pb2_grpc.py
--rw-r--r--   0        0        0     4458 2023-12-01 02:12:09.963013 prodvana-0.3.8/prodvana/proto/prodvana/release/manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     4702 2023-12-01 02:12:09.623013 prodvana-0.3.8/prodvana/proto/prodvana/release/object_pb2.py
--rw-r--r--   0        0        0    10698 2023-12-01 02:12:09.967013 prodvana-0.3.8/prodvana/proto/prodvana/release/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.623013 prodvana-0.3.8/prodvana/proto/prodvana/release/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.967013 prodvana-0.3.8/prodvana/proto/prodvana/release/object_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.035013 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/__init__.py
--rw-r--r--   0        0        0     2453 2023-12-01 02:12:09.559013 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/object_pb2.py
--rw-r--r--   0        0        0     3325 2023-12-01 02:12:09.899013 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.563013 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.895013 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     9419 2023-12-01 02:37:09.570941 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
--rw-r--r--   0        0        0    17020 2023-12-01 02:37:09.570941 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.563013 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.907013 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    10119 2023-12-01 02:12:09.555013 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
--rw-r--r--   0        0        0    11055 2023-12-01 02:12:09.903013 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
--rw-r--r--   0        0        0    15129 2023-12-01 02:12:09.555013 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
--rw-r--r--   0        0        0     4757 2023-12-01 02:12:09.903013 prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.011013 prodvana-0.3.8/prodvana/proto/prodvana/repo/__init__.py
--rw-r--r--   0        0        0     1987 2023-12-01 02:12:09.343013 prodvana-0.3.8/prodvana/proto/prodvana/repo/repo_pb2.py
--rw-r--r--   0        0        0     2760 2023-12-01 02:12:09.679013 prodvana-0.3.8/prodvana/proto/prodvana/repo/repo_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.347013 prodvana-0.3.8/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.683013 prodvana-0.3.8/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.039013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/__init__.py
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.039013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/__init__.py
--rw-r--r--   0        0        0     2886 2023-12-01 02:12:09.575013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/fetch_pb2.py
--rw-r--r--   0        0        0     5695 2023-12-01 02:12:09.915013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/fetch_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.579013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/fetch_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.923013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/fetch_pb2_grpc.pyi
--rw-r--r--   0        0        0     1562 2023-12-01 02:12:09.579013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/get_info_pb2.py
--rw-r--r--   0        0        0     1537 2023-12-01 02:12:09.919013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/get_info_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.575013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/get_info_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.919013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/get_info_pb2_grpc.pyi
--rw-r--r--   0        0        0     1434 2023-12-01 02:12:09.583013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/features_pb2.py
--rw-r--r--   0        0        0     1320 2023-12-01 02:12:09.923013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/features_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.571013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.927013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
--rw-r--r--   0        0        0     4579 2023-12-01 02:12:09.583013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
--rw-r--r--   0        0        0     6995 2023-12-01 02:12:09.927013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.571013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.911013 prodvana-0.3.8/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.007013 prodvana-0.3.8/prodvana/proto/prodvana/scm/__init__.py
--rw-r--r--   0        0        0     1229 2023-12-01 02:12:09.339013 prodvana-0.3.8/prodvana/proto/prodvana/scm/types_pb2.py
--rw-r--r--   0        0        0      914 2023-12-01 02:12:09.675013 prodvana-0.3.8/prodvana/proto/prodvana/scm/types_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.335013 prodvana-0.3.8/prodvana/proto/prodvana/scm/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.671013 prodvana-0.3.8/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.019013 prodvana-0.3.8/prodvana/proto/prodvana/secrets/__init__.py
--rw-r--r--   0        0        0     6361 2023-12-01 02:12:09.459013 prodvana-0.3.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
--rw-r--r--   0        0        0     4586 2023-12-01 02:12:09.791013 prodvana-0.3.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
--rw-r--r--   0        0        0     9936 2023-12-01 02:12:09.455013 prodvana-0.3.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
--rw-r--r--   0        0        0     2847 2023-12-01 02:12:09.791013 prodvana-0.3.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.027013 prodvana-0.3.8/prodvana/proto/prodvana/service/__init__.py
--rw-r--r--   0        0        0     4620 2023-12-01 02:12:09.523013 prodvana-0.3.8/prodvana/proto/prodvana/service/object_pb2.py
--rw-r--r--   0        0        0     7579 2023-12-01 02:12:09.851013 prodvana-0.3.8/prodvana/proto/prodvana/service/object_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.523013 prodvana-0.3.8/prodvana/proto/prodvana/service/object_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.847013 prodvana-0.3.8/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
--rw-r--r--   0        0        0     1908 2023-12-01 02:12:09.515013 prodvana-0.3.8/prodvana/proto/prodvana/service/parameters_pb2.py
--rw-r--r--   0        0        0     2424 2023-12-01 02:12:09.843013 prodvana-0.3.8/prodvana/proto/prodvana/service/parameters_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.507013 prodvana-0.3.8/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.859013 prodvana-0.3.8/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
--rw-r--r--   0        0        0    30163 2023-12-01 02:12:09.507013 prodvana-0.3.8/prodvana/proto/prodvana/service/service_config_pb2.py
--rw-r--r--   0        0        0    61937 2023-12-01 02:12:09.839013 prodvana-0.3.8/prodvana/proto/prodvana/service/service_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.503013 prodvana-0.3.8/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.843013 prodvana-0.3.8/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    37226 2023-12-01 02:12:09.511013 prodvana-0.3.8/prodvana/proto/prodvana/service/service_manager_pb2.py
--rw-r--r--   0        0        0    45083 2023-12-01 02:12:09.851013 prodvana-0.3.8/prodvana/proto/prodvana/service/service_manager_pb2.pyi
--rw-r--r--   0        0        0    39467 2023-12-01 02:12:09.519013 prodvana-0.3.8/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
--rw-r--r--   0        0        0    11281 2023-12-01 02:12:09.859013 prodvana-0.3.8/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0     2198 2023-12-01 02:12:09.511013 prodvana-0.3.8/prodvana/proto/prodvana/service/user_metadata_pb2.py
--rw-r--r--   0        0        0     2106 2023-12-01 02:12:09.855013 prodvana-0.3.8/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.515013 prodvana-0.3.8/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.855013 prodvana-0.3.8/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.031013 prodvana-0.3.8/prodvana/proto/prodvana/settings/__init__.py
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.035013 prodvana-0.3.8/prodvana/proto/prodvana/settings/organization/__init__.py
--rw-r--r--   0        0        0     7553 2023-12-01 02:12:09.551013 prodvana-0.3.8/prodvana/proto/prodvana/settings/organization/users_pb2.py
--rw-r--r--   0        0        0     8463 2023-12-01 02:12:09.891013 prodvana-0.3.8/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
--rw-r--r--   0        0        0    13863 2023-12-01 02:12:09.551013 prodvana-0.3.8/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
--rw-r--r--   0        0        0     3869 2023-12-01 02:12:09.891013 prodvana-0.3.8/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.027013 prodvana-0.3.8/prodvana/proto/prodvana/stat/__init__.py
--rw-r--r--   0        0        0     1317 2023-12-01 02:12:09.527013 prodvana-0.3.8/prodvana/proto/prodvana/stat/efficiency_pb2.py
--rw-r--r--   0        0        0     1156 2023-12-01 02:12:09.867013 prodvana-0.3.8/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.523013 prodvana-0.3.8/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.863013 prodvana-0.3.8/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.047013 prodvana-0.3.8/prodvana/proto/prodvana/users/__init__.py
--rw-r--r--   0        0        0     1403 2023-12-01 02:12:09.639013 prodvana-0.3.8/prodvana/proto/prodvana/users/users_pb2.py
--rw-r--r--   0        0        0     1640 2023-12-01 02:12:09.983013 prodvana-0.3.8/prodvana/proto/prodvana/users/users_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.639013 prodvana-0.3.8/prodvana/proto/prodvana/users/users_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.987013 prodvana-0.3.8/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.035013 prodvana-0.3.8/prodvana/proto/prodvana/version/__init__.py
--rw-r--r--   0        0        0     1723 2023-12-01 02:12:09.567013 prodvana-0.3.8/prodvana/proto/prodvana/version/source_metadata_pb2.py
--rw-r--r--   0        0        0     2817 2023-12-01 02:12:09.907013 prodvana-0.3.8/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.567013 prodvana-0.3.8/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.911013 prodvana-0.3.8/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.047013 prodvana-0.3.8/prodvana/proto/prodvana/volumes/__init__.py
--rw-r--r--   0        0        0     3089 2023-12-01 02:12:09.627013 prodvana-0.3.8/prodvana/proto/prodvana/volumes/volumes_pb2.py
--rw-r--r--   0        0        0     4793 2023-12-01 02:12:09.975013 prodvana-0.3.8/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.627013 prodvana-0.3.8/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.971013 prodvana-0.3.8/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.019013 prodvana-0.3.8/prodvana/proto/prodvana/workflow/__init__.py
--rw-r--r--   0        0        0     3274 2023-12-01 02:12:09.451013 prodvana-0.3.8/prodvana/proto/prodvana/workflow/integration_config_pb2.py
--rw-r--r--   0        0        0     4328 2023-12-01 02:12:09.779013 prodvana-0.3.8/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.447013 prodvana-0.3.8/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.783013 prodvana-0.3.8/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
--rw-r--r--   0        0        0    37544 2023-12-01 02:12:09.455013 prodvana-0.3.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
--rw-r--r--   0        0        0    53697 2023-12-01 02:12:09.787013 prodvana-0.3.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
--rw-r--r--   0        0        0    59506 2023-12-01 02:12:09.447013 prodvana-0.3.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
--rw-r--r--   0        0        0    17179 2023-12-01 02:12:09.783013 prodvana-0.3.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-12-01 02:12:10.051013 prodvana-0.3.8/prodvana/proto/validate/__init__.py
--rw-r--r--   0        0        0    13684 2023-12-01 02:12:09.651013 prodvana-0.3.8/prodvana/proto/validate/validate_pb2.py
--rw-r--r--   0        0        0    64630 2023-12-01 02:12:09.999013 prodvana-0.3.8/prodvana/proto/validate/validate_pb2.pyi
--rw-r--r--   0        0        0      159 2023-12-01 02:12:09.651013 prodvana-0.3.8/prodvana/proto/validate/validate_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-12-01 02:12:09.995013 prodvana-0.3.8/prodvana/proto/validate/validate_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2023-11-29 19:16:46.207324 prodvana-0.3.8/prodvana/py.typed
--rw-r--r--   0        0        0        0 2023-11-29 19:16:46.207324 prodvana-0.3.8/prodvana/utils/__init__.py
--rw-r--r--   0        0        0      538 2023-11-29 19:16:46.207324 prodvana-0.3.8/prodvana/utils/desired_states.py
--rw-r--r--   0        0        0     1434 2023-11-29 19:16:46.207324 prodvana-0.3.8/prodvana/utils/parameters.py
--rw-r--r--   0        0        0     1731 2023-11-29 19:16:46.207324 prodvana-0.3.8/prodvana/utils/protections.py
--rw-r--r--   0        0        0     2437 2023-11-30 02:22:53.763588 prodvana-0.3.8/prodvana/utils/service_config.py
--rw-r--r--   0        0        0     3916 2023-11-30 02:22:53.763588 prodvana-0.3.8/prodvana/utils/tests/test_service_config.py
--rw-r--r--   0        0        0      746 2023-12-01 02:43:47.902922 prodvana-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0       81 2023-11-27 18:43:36.700858 prodvana-0.3.9/README.md
+-rw-r--r--   0        0        0        0 2023-11-27 18:43:36.700858 prodvana-0.3.9/prodvana/__init__.py
+-rw-r--r--   0        0        0     3529 2023-11-27 18:43:36.700858 prodvana-0.3.9/prodvana/client.py
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.906993 prodvana-0.3.9/prodvana/proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.910993 prodvana-0.3.9/prodvana/proto/prodvana/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.950993 prodvana-0.3.9/prodvana/proto/prodvana/agent/__init__.py
+-rw-r--r--   0        0        0    10322 2023-12-01 08:10:52.450993 prodvana-0.3.9/prodvana/proto/prodvana/agent/agent_interaction_pb2.py
+-rw-r--r--   0        0        0    20472 2023-12-01 08:10:52.802993 prodvana-0.3.9/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi
+-rw-r--r--   0        0        0    24439 2023-12-01 08:10:52.450993 prodvana-0.3.9/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py
+-rw-r--r--   0        0        0     7291 2023-12-01 08:10:52.802993 prodvana-0.3.9/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.946993 prodvana-0.3.9/prodvana/proto/prodvana/application/__init__.py
+-rw-r--r--   0        0        0     3899 2023-12-01 08:10:52.434993 prodvana-0.3.9/prodvana/proto/prodvana/application/application_config_pb2.py
+-rw-r--r--   0        0        0     3656 2023-12-01 08:10:52.786993 prodvana-0.3.9/prodvana/proto/prodvana/application/application_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.426993 prodvana-0.3.9/prodvana/proto/prodvana/application/application_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.790993 prodvana-0.3.9/prodvana/proto/prodvana/application/application_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    15907 2023-12-01 08:10:52.430993 prodvana-0.3.9/prodvana/proto/prodvana/application/application_manager_pb2.py
+-rw-r--r--   0        0        0    16830 2023-12-01 08:10:52.782993 prodvana-0.3.9/prodvana/proto/prodvana/application/application_manager_pb2.pyi
+-rw-r--r--   0        0        0    22241 2023-12-01 08:10:52.430993 prodvana-0.3.9/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6755 2023-12-01 08:10:52.786993 prodvana-0.3.9/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2235 2023-12-01 08:10:52.434993 prodvana-0.3.9/prodvana/proto/prodvana/application/object_pb2.py
+-rw-r--r--   0        0        0     2184 2023-12-01 08:10:52.778993 prodvana-0.3.9/prodvana/proto/prodvana/application/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.442993 prodvana-0.3.9/prodvana/proto/prodvana/application/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.794993 prodvana-0.3.9/prodvana/proto/prodvana/application/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2011 2023-12-01 08:10:52.438993 prodvana-0.3.9/prodvana/proto/prodvana/application/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1670 2023-12-01 08:10:52.782993 prodvana-0.3.9/prodvana/proto/prodvana/application/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.438993 prodvana-0.3.9/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.790993 prodvana-0.3.9/prodvana/proto/prodvana/application/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.954993 prodvana-0.3.9/prodvana/proto/prodvana/async_task/__init__.py
+-rw-r--r--   0        0        0     1540 2023-12-01 08:10:52.478993 prodvana-0.3.9/prodvana/proto/prodvana/async_task/task_metadata_pb2.py
+-rw-r--r--   0        0        0     1657 2023-12-01 08:10:52.826993 prodvana-0.3.9/prodvana/proto/prodvana/async_task/task_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.474993 prodvana-0.3.9/prodvana/proto/prodvana/async_task/task_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.830993 prodvana-0.3.9/prodvana/proto/prodvana/async_task/task_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.954993 prodvana-0.3.9/prodvana/proto/prodvana/auth/__init__.py
+-rw-r--r--   0        0        0     8480 2023-12-01 08:10:52.486993 prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_manager_pb2.py
+-rw-r--r--   0        0        0    10206 2023-12-01 08:10:52.834993 prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi
+-rw-r--r--   0        0        0    18631 2023-12-01 08:10:52.482993 prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     6767 2023-12-01 08:10:52.838993 prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3181 2023-12-01 08:10:52.478993 prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_pb2.py
+-rw-r--r--   0        0        0     5515 2023-12-01 08:10:52.830993 prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.482993 prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.834993 prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.930993 prodvana-0.3.9/prodvana/proto/prodvana/blobs/__init__.py
+-rw-r--r--   0        0        0     2733 2023-12-01 08:10:52.318993 prodvana-0.3.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py
+-rw-r--r--   0        0        0     1947 2023-12-01 08:10:52.678993 prodvana-0.3.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi
+-rw-r--r--   0        0        0     4464 2023-12-01 08:10:52.318993 prodvana-0.3.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     1398 2023-12-01 08:10:52.678993 prodvana-0.3.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.918993 prodvana-0.3.9/prodvana/proto/prodvana/capability/__init__.py
+-rw-r--r--   0        0        0     4830 2023-12-01 08:10:52.242993 prodvana-0.3.9/prodvana/proto/prodvana/capability/capability_pb2.py
+-rw-r--r--   0        0        0     5455 2023-12-01 08:10:52.602993 prodvana-0.3.9/prodvana/proto/prodvana/capability/capability_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.246993 prodvana-0.3.9/prodvana/proto/prodvana/capability/capability_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.606993 prodvana-0.3.9/prodvana/proto/prodvana/capability/capability_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.934993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/__init__.py
+-rw-r--r--   0        0        0     1988 2023-12-01 08:10:52.390993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/constants_pb2.py
+-rw-r--r--   0        0        0     1667 2023-12-01 08:10:52.694993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/constants_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.386993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/constants_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.722993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/constants_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1366 2023-12-01 08:10:52.370993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py
+-rw-r--r--   0        0        0      869 2023-12-01 08:10:52.698993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.382993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.710993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/dangerous_action_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3398 2023-12-01 08:10:52.374993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/env_pb2.py
+-rw-r--r--   0        0        0     4125 2023-12-01 08:10:52.690993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/env_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.366993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/env_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.718993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/env_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2102 2023-12-01 08:10:52.350993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/external_link_pb2.py
+-rw-r--r--   0        0        0     1796 2023-12-01 08:10:52.730993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/external_link_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.334993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/external_link_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.714993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/external_link_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4409 2023-12-01 08:10:52.382993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/helm_pb2.py
+-rw-r--r--   0        0        0     5957 2023-12-01 08:10:52.710993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/helm_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.374993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/helm_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.746993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/helm_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3479 2023-12-01 08:10:52.362993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py
+-rw-r--r--   0        0        0     7059 2023-12-01 08:10:52.726993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.354993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.718993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/kubernetes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1738 2023-12-01 08:10:52.346993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/links_pb2.py
+-rw-r--r--   0        0        0      846 2023-12-01 08:10:52.738993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/links_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.390993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/links_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.742993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/links_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1338 2023-12-01 08:10:52.394993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/maturity_pb2.py
+-rw-r--r--   0        0        0     1103 2023-12-01 08:10:52.746993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/maturity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.338993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.738993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/maturity_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1838 2023-12-01 08:10:52.342993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/meta_pb2.py
+-rw-r--r--   0        0        0     2531 2023-12-01 08:10:52.702993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.342993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.730993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1866 2023-12-01 08:10:52.378993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/notification_pb2.py
+-rw-r--r--   0        0        0     1337 2023-12-01 08:10:52.734993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/notification_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.386993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/notification_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.702993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/notification_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8463 2023-12-01 08:10:52.378993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/parameters_pb2.py
+-rw-r--r--   0        0        0    11778 2023-12-01 08:10:52.742993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.354993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.714993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9143 2023-12-01 08:10:52.334993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/program_pb2.py
+-rw-r--r--   0        0        0    15928 2023-12-01 08:10:52.706993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/program_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.370993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/program_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.690993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/program_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2686 2023-12-01 08:10:52.358993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/retry_pb2.py
+-rw-r--r--   0        0        0     2757 2023-12-01 08:10:52.722993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/retry_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.330993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/retry_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.706993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/retry_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2989 2023-12-01 08:10:52.366993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/task_pb2.py
+-rw-r--r--   0        0        0     4249 2023-12-01 08:10:52.698993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.358993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.734993 prodvana-0.3.9/prodvana/proto/prodvana/common_config/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.938993 prodvana-0.3.9/prodvana/proto/prodvana/config_file/__init__.py
+-rw-r--r--   0        0        0     3685 2023-12-01 08:10:52.402993 prodvana-0.3.9/prodvana/proto/prodvana/config_file/config_pb2.py
+-rw-r--r--   0        0        0     4656 2023-12-01 08:10:52.758993 prodvana-0.3.9/prodvana/proto/prodvana/config_file/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.402993 prodvana-0.3.9/prodvana/proto/prodvana/config_file/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.754993 prodvana-0.3.9/prodvana/proto/prodvana/config_file/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.930993 prodvana-0.3.9/prodvana/proto/prodvana/config_writeback/__init__.py
+-rw-r--r--   0        0        0     1388 2023-12-01 08:10:52.314993 prodvana-0.3.9/prodvana/proto/prodvana/config_writeback/writeback_pb2.py
+-rw-r--r--   0        0        0     1131 2023-12-01 08:10:52.674993 prodvana-0.3.9/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.314993 prodvana-0.3.9/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.674993 prodvana-0.3.9/prodvana/proto/prodvana/config_writeback/writeback_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.962993 prodvana-0.3.9/prodvana/proto/prodvana/convergence/__init__.py
+-rw-r--r--   0        0        0     1371 2023-12-01 08:10:52.522993 prodvana-0.3.9/prodvana/proto/prodvana/convergence/convergence_mode_pb2.py
+-rw-r--r--   0        0        0     1159 2023-12-01 08:10:52.878993 prodvana-0.3.9/prodvana/proto/prodvana/convergence/convergence_mode_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.522993 prodvana-0.3.9/prodvana/proto/prodvana/convergence/convergence_mode_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.874993 prodvana-0.3.9/prodvana/proto/prodvana/convergence/convergence_mode_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.914993 prodvana-0.3.9/prodvana/proto/prodvana/delivery/__init__.py
+-rw-r--r--   0        0        0     2079 2023-12-01 08:10:52.226993 prodvana-0.3.9/prodvana/proto/prodvana/delivery/delivery_config_pb2.py
+-rw-r--r--   0        0        0     2294 2023-12-01 08:10:52.586993 prodvana-0.3.9/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.222993 prodvana-0.3.9/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.586993 prodvana-0.3.9/prodvana/proto/prodvana/delivery/delivery_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.926993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/__init__.py
+-rw-r--r--   0        0        0     6161 2023-12-01 08:10:52.298993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/config_pb2.py
+-rw-r--r--   0        0        0     8052 2023-12-01 08:10:52.662993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.290993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.658993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9624 2023-12-01 08:10:52.294993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/manager_pb2.py
+-rw-r--r--   0        0        0    10317 2023-12-01 08:10:52.658993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi
+-rw-r--r--   0        0        0    13097 2023-12-01 08:10:52.294993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3909 2023-12-01 08:10:52.654993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2015 2023-12-01 08:10:52.298993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/object_pb2.py
+-rw-r--r--   0        0        0     1862 2023-12-01 08:10:52.654993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.302993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.662993 prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.914993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/__init__.py
+-rw-r--r--   0        0        0    31161 2023-12-01 08:10:52.226993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/manager_pb2.py
+-rw-r--r--   0        0        0    48560 2023-12-01 08:10:52.602993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/manager_pb2.pyi
+-rw-r--r--   0        0        0    28235 2023-12-01 08:10:52.230993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     9184 2023-12-01 08:10:52.590993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.918993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/__init__.py
+-rw-r--r--   0        0        0    38726 2023-12-01 08:10:52.238993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py
+-rw-r--r--   0        0        0   115827 2023-12-01 08:10:52.598993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.238993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.594993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/desired_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3694 2023-12-01 08:10:52.242993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/entity_pb2.py
+-rw-r--r--   0        0        0     8878 2023-12-01 08:10:52.594993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.234993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.590993 prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/entity_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.922993 prodvana-0.3.9/prodvana/proto/prodvana/environment/__init__.py
+-rw-r--r--   0        0        0    26543 2023-12-01 08:10:52.270993 prodvana-0.3.9/prodvana/proto/prodvana/environment/clusters_pb2.py
+-rw-r--r--   0        0        0    54612 2023-12-01 08:10:52.630993 prodvana-0.3.9/prodvana/proto/prodvana/environment/clusters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.274993 prodvana-0.3.9/prodvana/proto/prodvana/environment/clusters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.638993 prodvana-0.3.9/prodvana/proto/prodvana/environment/clusters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    14209 2023-12-01 08:10:52.274993 prodvana-0.3.9/prodvana/proto/prodvana/environment/environment_manager_pb2.py
+-rw-r--r--   0        0        0    19436 2023-12-01 08:10:52.634993 prodvana-0.3.9/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi
+-rw-r--r--   0        0        0    25138 2023-12-01 08:10:52.270993 prodvana-0.3.9/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     7335 2023-12-01 08:10:52.634993 prodvana-0.3.9/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.926993 prodvana-0.3.9/prodvana/proto/prodvana/events/__init__.py
+-rw-r--r--   0        0        0     5103 2023-12-01 08:10:52.278993 prodvana-0.3.9/prodvana/proto/prodvana/events/events_manager_pb2.py
+-rw-r--r--   0        0        0     6267 2023-12-01 08:10:52.642993 prodvana-0.3.9/prodvana/proto/prodvana/events/events_manager_pb2.pyi
+-rw-r--r--   0        0        0     2714 2023-12-01 08:10:52.286993 prodvana-0.3.9/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py
+-rw-r--r--   0        0        0      853 2023-12-01 08:10:52.646993 prodvana-0.3.9/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2727 2023-12-01 08:10:52.282993 prodvana-0.3.9/prodvana/proto/prodvana/events/events_pb2.py
+-rw-r--r--   0        0        0     4246 2023-12-01 08:10:52.650993 prodvana-0.3.9/prodvana/proto/prodvana/events/events_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.278993 prodvana-0.3.9/prodvana/proto/prodvana/events/events_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.646993 prodvana-0.3.9/prodvana/proto/prodvana/events/events_pb2_grpc.pyi
+-rw-r--r--   0        0        0    17212 2023-12-01 08:10:52.290993 prodvana-0.3.9/prodvana/proto/prodvana/events/types_pb2.py
+-rw-r--r--   0        0        0    50754 2023-12-01 08:10:52.642993 prodvana-0.3.9/prodvana/proto/prodvana/events/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.282993 prodvana-0.3.9/prodvana/proto/prodvana/events/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.638993 prodvana-0.3.9/prodvana/proto/prodvana/events/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.962993 prodvana-0.3.9/prodvana/proto/prodvana/impact_analysis/__init__.py
+-rw-r--r--   0        0        0     2389 2023-12-01 08:10:52.538993 prodvana-0.3.9/prodvana/proto/prodvana/impact_analysis/impact_analysis_pb2.py
+-rw-r--r--   0        0        0     4064 2023-12-01 08:10:52.890993 prodvana-0.3.9/prodvana/proto/prodvana/impact_analysis/impact_analysis_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.542993 prodvana-0.3.9/prodvana/proto/prodvana/impact_analysis/impact_analysis_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.894993 prodvana-0.3.9/prodvana/proto/prodvana/impact_analysis/impact_analysis_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.930993 prodvana-0.3.9/prodvana/proto/prodvana/insights/__init__.py
+-rw-r--r--   0        0        0     2205 2023-12-01 08:10:52.310993 prodvana-0.3.9/prodvana/proto/prodvana/insights/insights_pb2.py
+-rw-r--r--   0        0        0     3508 2023-12-01 08:10:52.670993 prodvana-0.3.9/prodvana/proto/prodvana/insights/insights_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.310993 prodvana-0.3.9/prodvana/proto/prodvana/insights/insights_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.670993 prodvana-0.3.9/prodvana/proto/prodvana/insights/insights_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.934993 prodvana-0.3.9/prodvana/proto/prodvana/labels/__init__.py
+-rw-r--r--   0        0        0     1845 2023-12-01 08:10:52.326993 prodvana-0.3.9/prodvana/proto/prodvana/labels/labels_pb2.py
+-rw-r--r--   0        0        0      854 2023-12-01 08:10:52.686993 prodvana-0.3.9/prodvana/proto/prodvana/labels/labels_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.330993 prodvana-0.3.9/prodvana/proto/prodvana/labels/labels_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.686993 prodvana-0.3.9/prodvana/proto/prodvana/labels/labels_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.926993 prodvana-0.3.9/prodvana/proto/prodvana/managed_resource/__init__.py
+-rw-r--r--   0        0        0     8344 2023-12-01 08:10:52.306993 prodvana-0.3.9/prodvana/proto/prodvana/managed_resource/manager_pb2.py
+-rw-r--r--   0        0        0    13338 2023-12-01 08:10:52.666993 prodvana-0.3.9/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi
+-rw-r--r--   0        0        0    12065 2023-12-01 08:10:52.306993 prodvana-0.3.9/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3657 2023-12-01 08:10:52.666993 prodvana-0.3.9/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.914993 prodvana-0.3.9/prodvana/proto/prodvana/metrics/__init__.py
+-rw-r--r--   0        0        0     3762 2023-12-01 08:10:52.218993 prodvana-0.3.9/prodvana/proto/prodvana/metrics/metrics_pb2.py
+-rw-r--r--   0        0        0     8746 2023-12-01 08:10:52.582993 prodvana-0.3.9/prodvana/proto/prodvana/metrics/metrics_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.222993 prodvana-0.3.9/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.582993 prodvana-0.3.9/prodvana/proto/prodvana/metrics/metrics_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.942993 prodvana-0.3.9/prodvana/proto/prodvana/object/__init__.py
+-rw-r--r--   0        0        0     3353 2023-12-01 08:10:52.406993 prodvana-0.3.9/prodvana/proto/prodvana/object/manager_pb2.py
+-rw-r--r--   0        0        0     2751 2023-12-01 08:10:52.766993 prodvana-0.3.9/prodvana/proto/prodvana/object/manager_pb2.pyi
+-rw-r--r--   0        0        0     4330 2023-12-01 08:10:52.414993 prodvana-0.3.9/prodvana/proto/prodvana/object/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     1255 2023-12-01 08:10:52.758993 prodvana-0.3.9/prodvana/proto/prodvana/object/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2057 2023-12-01 08:10:52.410993 prodvana-0.3.9/prodvana/proto/prodvana/object/meta_pb2.py
+-rw-r--r--   0        0        0     3160 2023-12-01 08:10:52.762993 prodvana-0.3.9/prodvana/proto/prodvana/object/meta_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.406993 prodvana-0.3.9/prodvana/proto/prodvana/object/meta_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.762993 prodvana-0.3.9/prodvana/proto/prodvana/object/meta_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.918993 prodvana-0.3.9/prodvana/proto/prodvana/organization/__init__.py
+-rw-r--r--   0        0        0    10890 2023-12-01 08:10:52.246993 prodvana-0.3.9/prodvana/proto/prodvana/organization/organization_manager_pb2.py
+-rw-r--r--   0        0        0    11248 2023-12-01 08:10:52.606993 prodvana-0.3.9/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi
+-rw-r--r--   0        0        0    16770 2023-12-01 08:10:52.250993 prodvana-0.3.9/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     5422 2023-12-01 08:10:52.614993 prodvana-0.3.9/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2568 2023-12-01 08:10:52.254993 prodvana-0.3.9/prodvana/proto/prodvana/organization/user_metadata_pb2.py
+-rw-r--r--   0        0        0     1972 2023-12-01 08:10:52.610993 prodvana-0.3.9/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.250993 prodvana-0.3.9/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.610993 prodvana-0.3.9/prodvana/proto/prodvana/organization/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.942993 prodvana-0.3.9/prodvana/proto/prodvana/pipelines/__init__.py
+-rw-r--r--   0        0        0     2038 2023-12-01 08:10:52.414993 prodvana-0.3.9/prodvana/proto/prodvana/pipelines/object_pb2.py
+-rw-r--r--   0        0        0     2595 2023-12-01 08:10:52.766993 prodvana-0.3.9/prodvana/proto/prodvana/pipelines/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.422993 prodvana-0.3.9/prodvana/proto/prodvana/pipelines/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.774993 prodvana-0.3.9/prodvana/proto/prodvana/pipelines/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6748 2023-12-01 08:10:52.418993 prodvana-0.3.9/prodvana/proto/prodvana/pipelines/pipelines_pb2.py
+-rw-r--r--   0        0        0    11698 2023-12-01 08:10:52.770993 prodvana-0.3.9/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.418993 prodvana-0.3.9/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.770993 prodvana-0.3.9/prodvana/proto/prodvana/pipelines/pipelines_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.958993 prodvana-0.3.9/prodvana/proto/prodvana/protection/__init__.py
+-rw-r--r--   0        0        0     2777 2023-12-01 08:10:52.502993 prodvana-0.3.9/prodvana/proto/prodvana/protection/attachments_pb2.py
+-rw-r--r--   0        0        0     2860 2023-12-01 08:10:52.858993 prodvana-0.3.9/prodvana/proto/prodvana/protection/attachments_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.514993 prodvana-0.3.9/prodvana/proto/prodvana/protection/attachments_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.862993 prodvana-0.3.9/prodvana/proto/prodvana/protection/attachments_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1716 2023-12-01 08:10:52.510993 prodvana-0.3.9/prodvana/proto/prodvana/protection/object_pb2.py
+-rw-r--r--   0        0        0     1545 2023-12-01 08:10:52.862993 prodvana-0.3.9/prodvana/proto/prodvana/protection/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.518993 prodvana-0.3.9/prodvana/proto/prodvana/protection/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.874993 prodvana-0.3.9/prodvana/proto/prodvana/protection/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6916 2023-12-01 08:10:52.506993 prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_config_pb2.py
+-rw-r--r--   0        0        0    10730 2023-12-01 08:10:52.854993 prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.518993 prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.870993 prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0     8444 2023-12-01 08:10:52.502993 prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_manager_pb2.py
+-rw-r--r--   0        0        0     9632 2023-12-01 08:10:52.866993 prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi
+-rw-r--r--   0        0        0    12468 2023-12-01 08:10:52.510993 prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     3716 2023-12-01 08:10:52.866993 prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3938 2023-12-01 08:10:52.514993 prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_reference_pb2.py
+-rw-r--r--   0        0        0     4997 2023-12-01 08:10:52.870993 prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.506993 prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.854993 prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_reference_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.942993 prodvana-0.3.9/prodvana/proto/prodvana/pvn_wrapper/__init__.py
+-rw-r--r--   0        0        0     1789 2023-12-01 08:10:52.426993 prodvana-0.3.9/prodvana/proto/prodvana/pvn_wrapper/output_pb2.py
+-rw-r--r--   0        0        0     2809 2023-12-01 08:10:52.778993 prodvana-0.3.9/prodvana/proto/prodvana/pvn_wrapper/output_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.422993 prodvana-0.3.9/prodvana/proto/prodvana/pvn_wrapper/output_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.774993 prodvana-0.3.9/prodvana/proto/prodvana/pvn_wrapper/output_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.922993 prodvana-0.3.9/prodvana/proto/prodvana/release/__init__.py
+-rw-r--r--   0        0        0    12085 2023-12-01 08:10:52.254993 prodvana-0.3.9/prodvana/proto/prodvana/release/manager_pb2.py
+-rw-r--r--   0        0        0    17840 2023-12-01 08:10:52.618993 prodvana-0.3.9/prodvana/proto/prodvana/release/manager_pb2.pyi
+-rw-r--r--   0        0        0    14970 2023-12-01 08:10:52.258993 prodvana-0.3.9/prodvana/proto/prodvana/release/manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4458 2023-12-01 08:10:52.614993 prodvana-0.3.9/prodvana/proto/prodvana/release/manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4702 2023-12-01 08:10:52.262993 prodvana-0.3.9/prodvana/proto/prodvana/release/object_pb2.py
+-rw-r--r--   0        0        0    10698 2023-12-01 08:10:52.618993 prodvana-0.3.9/prodvana/proto/prodvana/release/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.262993 prodvana-0.3.9/prodvana/proto/prodvana/release/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.622993 prodvana-0.3.9/prodvana/proto/prodvana/release/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.962993 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/__init__.py
+-rw-r--r--   0        0        0     2453 2023-12-01 08:10:52.526993 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/object_pb2.py
+-rw-r--r--   0        0        0     3325 2023-12-01 08:10:52.878993 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.534993 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.890993 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9477 2023-12-01 08:13:34.142992 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py
+-rw-r--r--   0        0        0    17509 2023-12-01 08:13:34.142992 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.530993 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.882993 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    10119 2023-12-01 08:10:52.538993 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py
+-rw-r--r--   0        0        0    11055 2023-12-01 08:10:52.886993 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi
+-rw-r--r--   0        0        0    15129 2023-12-01 08:10:52.526993 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     4757 2023-12-01 08:10:52.886993 prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.958993 prodvana-0.3.9/prodvana/proto/prodvana/repo/__init__.py
+-rw-r--r--   0        0        0     1987 2023-12-01 08:10:52.498993 prodvana-0.3.9/prodvana/proto/prodvana/repo/repo_pb2.py
+-rw-r--r--   0        0        0     2760 2023-12-01 08:10:52.850993 prodvana-0.3.9/prodvana/proto/prodvana/repo/repo_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.494993 prodvana-0.3.9/prodvana/proto/prodvana/repo/repo_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.850993 prodvana-0.3.9/prodvana/proto/prodvana/repo/repo_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.950993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.950993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/__init__.py
+-rw-r--r--   0        0        0     2886 2023-12-01 08:10:52.466993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/fetch_pb2.py
+-rw-r--r--   0        0        0     5695 2023-12-01 08:10:52.822993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/fetch_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.462993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/fetch_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.814993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/fetch_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1562 2023-12-01 08:10:52.466993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/get_info_pb2.py
+-rw-r--r--   0        0        0     1537 2023-12-01 08:10:52.818993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/get_info_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.462993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/get_info_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.814993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/get_info_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1434 2023-12-01 08:10:52.454993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/features_pb2.py
+-rw-r--r--   0        0        0     1320 2023-12-01 08:10:52.810993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/features_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.458993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/features_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.806993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/features_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4579 2023-12-01 08:10:52.458993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py
+-rw-r--r--   0        0        0     6995 2023-12-01 08:10:52.810993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.454993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.806993 prodvana-0.3.9/prodvana/proto/prodvana/runtimes/runtimes_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.934993 prodvana-0.3.9/prodvana/proto/prodvana/scm/__init__.py
+-rw-r--r--   0        0        0     1229 2023-12-01 08:10:52.326993 prodvana-0.3.9/prodvana/proto/prodvana/scm/types_pb2.py
+-rw-r--r--   0        0        0      914 2023-12-01 08:10:52.682993 prodvana-0.3.9/prodvana/proto/prodvana/scm/types_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.322993 prodvana-0.3.9/prodvana/proto/prodvana/scm/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.682993 prodvana-0.3.9/prodvana/proto/prodvana/scm/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.922993 prodvana-0.3.9/prodvana/proto/prodvana/secrets/__init__.py
+-rw-r--r--   0        0        0     6361 2023-12-01 08:10:52.266993 prodvana-0.3.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py
+-rw-r--r--   0        0        0     4586 2023-12-01 08:10:52.626993 prodvana-0.3.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi
+-rw-r--r--   0        0        0     9936 2023-12-01 08:10:52.266993 prodvana-0.3.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py
+-rw-r--r--   0        0        0     2847 2023-12-01 08:10:52.626993 prodvana-0.3.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.914993 prodvana-0.3.9/prodvana/proto/prodvana/service/__init__.py
+-rw-r--r--   0        0        0     4620 2023-12-01 08:10:52.202993 prodvana-0.3.9/prodvana/proto/prodvana/service/object_pb2.py
+-rw-r--r--   0        0        0     7579 2023-12-01 08:10:52.558993 prodvana-0.3.9/prodvana/proto/prodvana/service/object_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.210993 prodvana-0.3.9/prodvana/proto/prodvana/service/object_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.578993 prodvana-0.3.9/prodvana/proto/prodvana/service/object_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1908 2023-12-01 08:10:52.206993 prodvana-0.3.9/prodvana/proto/prodvana/service/parameters_pb2.py
+-rw-r--r--   0        0        0     2424 2023-12-01 08:10:52.578993 prodvana-0.3.9/prodvana/proto/prodvana/service/parameters_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.198993 prodvana-0.3.9/prodvana/proto/prodvana/service/parameters_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.570993 prodvana-0.3.9/prodvana/proto/prodvana/service/parameters_pb2_grpc.pyi
+-rw-r--r--   0        0        0    30267 2023-12-01 16:37:08.377773 prodvana-0.3.9/prodvana/proto/prodvana/service/service_config_pb2.py
+-rw-r--r--   0        0        0    62580 2023-12-01 16:37:08.377773 prodvana-0.3.9/prodvana/proto/prodvana/service/service_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.218993 prodvana-0.3.9/prodvana/proto/prodvana/service/service_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.558993 prodvana-0.3.9/prodvana/proto/prodvana/service/service_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    37226 2023-12-01 08:10:52.214993 prodvana-0.3.9/prodvana/proto/prodvana/service/service_manager_pb2.py
+-rw-r--r--   0        0        0    45083 2023-12-01 08:10:52.562993 prodvana-0.3.9/prodvana/proto/prodvana/service/service_manager_pb2.pyi
+-rw-r--r--   0        0        0    39467 2023-12-01 08:10:52.210993 prodvana-0.3.9/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py
+-rw-r--r--   0        0        0    11281 2023-12-01 08:10:52.574993 prodvana-0.3.9/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2198 2023-12-01 08:10:52.206993 prodvana-0.3.9/prodvana/proto/prodvana/service/user_metadata_pb2.py
+-rw-r--r--   0        0        0     2106 2023-12-01 08:10:52.566993 prodvana-0.3.9/prodvana/proto/prodvana/service/user_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.202993 prodvana-0.3.9/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.574993 prodvana-0.3.9/prodvana/proto/prodvana/service/user_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.938993 prodvana-0.3.9/prodvana/proto/prodvana/settings/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.938993 prodvana-0.3.9/prodvana/proto/prodvana/settings/organization/__init__.py
+-rw-r--r--   0        0        0     7553 2023-12-01 08:10:52.398993 prodvana-0.3.9/prodvana/proto/prodvana/settings/organization/users_pb2.py
+-rw-r--r--   0        0        0     8463 2023-12-01 08:10:52.750993 prodvana-0.3.9/prodvana/proto/prodvana/settings/organization/users_pb2.pyi
+-rw-r--r--   0        0        0    13863 2023-12-01 08:10:52.398993 prodvana-0.3.9/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py
+-rw-r--r--   0        0        0     3869 2023-12-01 08:10:52.750993 prodvana-0.3.9/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.966993 prodvana-0.3.9/prodvana/proto/prodvana/stat/__init__.py
+-rw-r--r--   0        0        0     1317 2023-12-01 08:10:52.546993 prodvana-0.3.9/prodvana/proto/prodvana/stat/efficiency_pb2.py
+-rw-r--r--   0        0        0     1156 2023-12-01 08:10:52.898993 prodvana-0.3.9/prodvana/proto/prodvana/stat/efficiency_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.542993 prodvana-0.3.9/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.894993 prodvana-0.3.9/prodvana/proto/prodvana/stat/efficiency_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.910993 prodvana-0.3.9/prodvana/proto/prodvana/users/__init__.py
+-rw-r--r--   0        0        0     1403 2023-12-01 08:10:52.194993 prodvana-0.3.9/prodvana/proto/prodvana/users/users_pb2.py
+-rw-r--r--   0        0        0     1640 2023-12-01 08:10:52.554993 prodvana-0.3.9/prodvana/proto/prodvana/users/users_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.194993 prodvana-0.3.9/prodvana/proto/prodvana/users/users_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.554993 prodvana-0.3.9/prodvana/proto/prodvana/users/users_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.954993 prodvana-0.3.9/prodvana/proto/prodvana/version/__init__.py
+-rw-r--r--   0        0        0     1723 2023-12-01 08:10:52.470993 prodvana-0.3.9/prodvana/proto/prodvana/version/source_metadata_pb2.py
+-rw-r--r--   0        0        0     2817 2023-12-01 08:10:52.822993 prodvana-0.3.9/prodvana/proto/prodvana/version/source_metadata_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.470993 prodvana-0.3.9/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.826993 prodvana-0.3.9/prodvana/proto/prodvana/version/source_metadata_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.946993 prodvana-0.3.9/prodvana/proto/prodvana/volumes/__init__.py
+-rw-r--r--   0        0        0     3089 2023-12-01 08:10:52.446993 prodvana-0.3.9/prodvana/proto/prodvana/volumes/volumes_pb2.py
+-rw-r--r--   0        0        0     4793 2023-12-01 08:10:52.794993 prodvana-0.3.9/prodvana/proto/prodvana/volumes/volumes_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.442993 prodvana-0.3.9/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.798993 prodvana-0.3.9/prodvana/proto/prodvana/volumes/volumes_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.958993 prodvana-0.3.9/prodvana/proto/prodvana/workflow/__init__.py
+-rw-r--r--   0        0        0     3274 2023-12-01 08:10:52.486993 prodvana-0.3.9/prodvana/proto/prodvana/workflow/integration_config_pb2.py
+-rw-r--r--   0        0        0     4328 2023-12-01 08:10:52.838993 prodvana-0.3.9/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.490993 prodvana-0.3.9/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.842993 prodvana-0.3.9/prodvana/proto/prodvana/workflow/integration_config_pb2_grpc.pyi
+-rw-r--r--   0        0        0    37544 2023-12-01 08:10:52.494993 prodvana-0.3.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py
+-rw-r--r--   0        0        0    53697 2023-12-01 08:10:52.846993 prodvana-0.3.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi
+-rw-r--r--   0        0        0    59506 2023-12-01 08:10:52.490993 prodvana-0.3.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py
+-rw-r--r--   0        0        0    17179 2023-12-01 08:10:52.842993 prodvana-0.3.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-12-01 08:10:52.966993 prodvana-0.3.9/prodvana/proto/validate/__init__.py
+-rw-r--r--   0        0        0    13684 2023-12-01 08:10:52.550993 prodvana-0.3.9/prodvana/proto/validate/validate_pb2.py
+-rw-r--r--   0        0        0    64630 2023-12-01 08:10:52.902993 prodvana-0.3.9/prodvana/proto/validate/validate_pb2.pyi
+-rw-r--r--   0        0        0      159 2023-12-01 08:10:52.546993 prodvana-0.3.9/prodvana/proto/validate/validate_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-12-01 08:10:52.898993 prodvana-0.3.9/prodvana/proto/validate/validate_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2023-11-27 18:43:36.728858 prodvana-0.3.9/prodvana/py.typed
+-rw-r--r--   0        0        0        0 2023-11-27 18:43:36.728858 prodvana-0.3.9/prodvana/utils/__init__.py
+-rw-r--r--   0        0        0      538 2023-11-30 20:53:21.989233 prodvana-0.3.9/prodvana/utils/desired_states.py
+-rw-r--r--   0        0        0     1434 2023-11-27 18:43:36.732858 prodvana-0.3.9/prodvana/utils/parameters.py
+-rw-r--r--   0        0        0     1731 2023-11-27 18:43:36.732858 prodvana-0.3.9/prodvana/utils/protections.py
+-rw-r--r--   0        0        0     2437 2023-11-30 01:41:48.113783 prodvana-0.3.9/prodvana/utils/service_config.py
+-rw-r--r--   0        0        0     3916 2023-11-30 01:41:48.113783 prodvana-0.3.9/prodvana/utils/tests/test_service_config.py
+-rw-r--r--   0        0        0      746 2023-12-01 21:50:14.506187 prodvana-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      817 1970-01-01 00:00:00.000000 prodvana-0.3.9/PKG-INFO
```

### Comparing `prodvana-0.3.8/prodvana/client.py` & `prodvana-0.3.9/prodvana/client.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/agent/agent_interaction_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/agent/agent_interaction_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/agent/agent_interaction_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/agent/agent_interaction_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/application/application_config_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/application/application_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/application/application_config_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/application/application_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/application/application_manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/application/application_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/application/application_manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/application/application_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/application/application_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/application/application_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/application/object_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/application/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/application/object_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/application/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/application/user_metadata_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/application/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/application/user_metadata_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/application/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/async_task/task_metadata_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/async_task/task_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/async_task/task_metadata_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/async_task/task_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/auth/auth_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/auth/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/blobs/blobs_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/capability/capability_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/capability/capability_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/capability/capability_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/capability/capability_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/constants_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/constants_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/constants_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/constants_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/dangerous_action_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/dangerous_action_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/env_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/env_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/env_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/env_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/external_link_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/external_link_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/external_link_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/external_link_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/helm_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/helm_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/helm_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/helm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/kubernetes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/links_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/links_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/links_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/links_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/maturity_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/maturity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/maturity_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/maturity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/meta_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/meta_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/notification_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/notification_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/notification_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/notification_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/parameters_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/parameters_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/program_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/program_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/program_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/program_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/retry_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/retry_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/retry_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/retry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/task_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/task_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/common_config/task_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/common_config/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/config_file/config_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/config_file/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/config_file/config_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/config_file/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/config_writeback/writeback_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/config_writeback/writeback_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/config_writeback/writeback_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/convergence/convergence_mode_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/convergence/convergence_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/convergence/convergence_mode_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/convergence/convergence_mode_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/delivery/delivery_config_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/delivery/delivery_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/delivery/delivery_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/config_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/object_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/delivery_extension/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/desired_state/manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/desired_state/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/desired_state/manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/desired_state/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/desired_state/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/desired_state_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/entity_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/desired_state/model/entity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/environment/clusters_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/environment/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/environment/clusters_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/environment/clusters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/environment/environment_manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/environment/environment_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/environment/environment_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/environment/environment_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/events/events_manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/events/events_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/events/events_manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/events/events_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/events/events_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/events/events_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/events/events_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/events/events_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/events/events_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/events/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/events/types_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/events/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/events/types_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/events/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/impact_analysis/impact_analysis_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/impact_analysis/impact_analysis_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/impact_analysis/impact_analysis_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/impact_analysis/impact_analysis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/insights/insights_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/insights/insights_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/insights/insights_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/insights/insights_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/labels/labels_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/labels/labels_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/labels/labels_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/labels/labels_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/managed_resource/manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/managed_resource/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/managed_resource/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/managed_resource/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/metrics/metrics_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/metrics/metrics_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/metrics/metrics_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/metrics/metrics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/object/manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/object/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/object/manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/object/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/object/manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/object/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/object/manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/object/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/object/meta_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/object/meta_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/object/meta_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/object/meta_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/organization/organization_manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/organization/organization_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/organization/organization_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/organization/organization_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/organization/user_metadata_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/organization/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/organization/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/pipelines/object_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/pipelines/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/pipelines/object_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/pipelines/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/pipelines/pipelines_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/pipelines/pipelines_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/pipelines/pipelines_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/protection/attachments_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/protection/attachments_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/protection/attachments_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/protection/attachments_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/protection/object_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/protection/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/protection/object_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/protection/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_config_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_config_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_reference_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_reference_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/protection/protection_reference_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/pvn_wrapper/output_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/pvn_wrapper/output_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/pvn_wrapper/output_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/pvn_wrapper/output_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release/manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/release/manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release/manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/release/manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release/manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/release/manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release/manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/release/manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release/object_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/release/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release/object_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/release/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release_channel/object_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/release_channel/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release_channel/object_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/release_channel/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from prodvana.proto.prodvana.pipelines import pipelines_pb2 as prodvana_dot_pipelines_dot_pipelines__pb2
 from prodvana.proto.prodvana.protection import attachments_pb2 as prodvana_dot_protection_dot_attachments__pb2
 from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 from prodvana.proto.prodvana.workflow import integration_config_pb2 as prodvana_dot_workflow_dot_integration__config__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5prodvana/release_channel/release_channel_config.proto\x12\x18prodvana.release_channel\x1a&prodvana/common_config/constants.proto\x1a prodvana/common_config/env.proto\x1a%prodvana/common_config/maturity.proto\x1a\x1cprodvana/labels/labels.proto\x1a\"prodvana/pipelines/pipelines.proto\x1a%prodvana/protection/attachments.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a\x17validate/validate.proto\"\xcd\x01\n\x06Policy\x12n\n\x0b\x64\x65\x66\x61ult_env\x18\x01 \x03(\x0b\x32\x30.prodvana.release_channel.Policy.DefaultEnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aS\n\x0f\x44\x65\x66\x61ultEnvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\"\xf5\x05\n\x14ReleaseChannelConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\r\n\x05group\x18\x0c \x01(\t\x12\r\n\x05order\x18\x02 \x01(\x03\x12\x32\n\x08maturity\x18\x03 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x30\n\x06policy\x18\x04 \x01(\x0b\x32 .prodvana.release_channel.Policy\x12G\n\x08runtimes\x18\x05 \x03(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12@\n\x12\x64\x65ploy_annotations\x18\x06 \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12=\n\rpreconditions\x18\x07 \x03(\x0b\x32&.prodvana.release_channel.Precondition\x12\x44\n\x0bprotections\x18\x08 \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12P\n\x17\x63onvergence_protections\x18\t \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12U\n\x1cservice_instance_protections\x18\x0b \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12\x33\n\tconstants\x18\n \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x30\n\x06labels\x18\r \x03(\x0b\x32 .prodvana.labels.LabelDefinition\"\xdb\x05\n\x0cPrecondition\x12]\n\x16release_channel_stable\x18\x01 \x01(\x0b\x32;.prodvana.release_channel.Precondition.ReleaseChannelStableH\x00\x12P\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x35.prodvana.release_channel.Precondition.ManualApprovalH\x00\x12H\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x31.prodvana.release_channel.Precondition.CustomTaskH\x00\x12]\n\x16shared_manual_approval\x18\x05 \x01(\x0b\x32;.prodvana.release_channel.Precondition.SharedManualApprovalH\x00\x1a\x7f\n\x14ReleaseChannelStable\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x12\x12\n\x08selector\x18\x03 \x01(\tH\x00\x12\x13\n\x0b\x61llow_empty\x18\x04 \x01(\x08\x42\x13\n\x0cstable_oneof\x12\x03\xf8\x42\x01J\x04\x08\x02\x10\x03R\x08\x64uration\x1aI\n\x0eManualApproval\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x14\n\x0c\x65very_action\x18\x03 \x01(\x08\x1aT\n\nCustomTask\x12\x11\n\ttask_name\x18\x01 \x01(\t\x12\x33\n\x0b\x63ustom_task\x18\x02 \x01(\x0b\x32\x1e.prodvana.pipelines.CustomTask\x1a-\n\x14SharedManualApproval\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x42\x0e\n\x0cpreconditionJ\x04\x08\x04\x10\x05R\nprotection\"\xb9\x02\n\x1bReleaseChannelRuntimeConfig\x12<\n\x07runtime\x18\x02 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\x04name\x18\x03 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12S\n\x17\x63ontainer_orchestration\x18\x01 \x01(\x0b\x32\x30.prodvana.runtimes.ContainerOrchestrationRuntimeH\x00\x12=\n\x04type\x18\x04 \x01(\x0e\x32/.prodvana.release_channel.RuntimeConnectionTypeB\x0c\n\ncapability\"\xe3\x01\n\"ReleaseChannelGroupGeneratorConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12!\n\x10runtime_selector\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61llow_empty\x18\x03 \x01(\x08\x12J\n\x08template\x18\x04 \x01(\x0b\x32..prodvana.release_channel.ReleaseChannelConfigB\x08\xfa\x42\x05\x8a\x01\x02\x08\x01*y\n\x15RuntimeConnectionType\x12\x16\n\x12UNKNOWN_CONNECTION\x10\x00\x12\x16\n\x12LONG_LIVED_COMPUTE\x10\x01\x12\r\n\tEXTENSION\x10\x02\x12\x0b\n\x07\x41WS_ECS\x10\x03\x12\x14\n\x10GOOGLE_CLOUD_RUN\x10\x04\x42TZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/release_channelb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n5prodvana/release_channel/release_channel_config.proto\x12\x18prodvana.release_channel\x1a&prodvana/common_config/constants.proto\x1a prodvana/common_config/env.proto\x1a%prodvana/common_config/maturity.proto\x1a\x1cprodvana/labels/labels.proto\x1a\"prodvana/pipelines/pipelines.proto\x1a%prodvana/protection/attachments.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a\x17validate/validate.proto\"\xcd\x01\n\x06Policy\x12n\n\x0b\x64\x65\x66\x61ult_env\x18\x01 \x03(\x0b\x32\x30.prodvana.release_channel.Policy.DefaultEnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x1aS\n\x0f\x44\x65\x66\x61ultEnvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\"\x96\x06\n\x14ReleaseChannelConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\r\n\x05group\x18\x0c \x01(\t\x12\r\n\x05order\x18\x02 \x01(\x03\x12\x32\n\x08maturity\x18\x03 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x30\n\x06policy\x18\x04 \x01(\x0b\x32 .prodvana.release_channel.Policy\x12G\n\x08runtimes\x18\x05 \x03(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12@\n\x12\x64\x65ploy_annotations\x18\x06 \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12=\n\rpreconditions\x18\x07 \x03(\x0b\x32&.prodvana.release_channel.Precondition\x12\x44\n\x0bprotections\x18\x08 \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12P\n\x17\x63onvergence_protections\x18\t \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12U\n\x1cservice_instance_protections\x18\x0b \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12\x33\n\tconstants\x18\n \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x30\n\x06labels\x18\r \x03(\x0b\x32 .prodvana.labels.LabelDefinition\x12\x1f\n\x17\x64isable_all_protections\x18\x0e \x01(\x08\"\xdb\x05\n\x0cPrecondition\x12]\n\x16release_channel_stable\x18\x01 \x01(\x0b\x32;.prodvana.release_channel.Precondition.ReleaseChannelStableH\x00\x12P\n\x0fmanual_approval\x18\x02 \x01(\x0b\x32\x35.prodvana.release_channel.Precondition.ManualApprovalH\x00\x12H\n\x0b\x63ustom_task\x18\x03 \x01(\x0b\x32\x31.prodvana.release_channel.Precondition.CustomTaskH\x00\x12]\n\x16shared_manual_approval\x18\x05 \x01(\x0b\x32;.prodvana.release_channel.Precondition.SharedManualApprovalH\x00\x1a\x7f\n\x14ReleaseChannelStable\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x12\x12\n\x08selector\x18\x03 \x01(\tH\x00\x12\x13\n\x0b\x61llow_empty\x18\x04 \x01(\x08\x42\x13\n\x0cstable_oneof\x12\x03\xf8\x42\x01J\x04\x08\x02\x10\x03R\x08\x64uration\x1aI\n\x0eManualApproval\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x14\n\x0c\x65very_action\x18\x03 \x01(\x08\x1aT\n\nCustomTask\x12\x11\n\ttask_name\x18\x01 \x01(\t\x12\x33\n\x0b\x63ustom_task\x18\x02 \x01(\x0b\x32\x1e.prodvana.pipelines.CustomTask\x1a-\n\x14SharedManualApproval\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x42\x0e\n\x0cpreconditionJ\x04\x08\x04\x10\x05R\nprotection\"\xb9\x02\n\x1bReleaseChannelRuntimeConfig\x12<\n\x07runtime\x18\x02 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12:\n\x04name\x18\x03 \x01(\tB,\xfa\x42)r\'\x10\x00\x18?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$\x12S\n\x17\x63ontainer_orchestration\x18\x01 \x01(\x0b\x32\x30.prodvana.runtimes.ContainerOrchestrationRuntimeH\x00\x12=\n\x04type\x18\x04 \x01(\x0e\x32/.prodvana.release_channel.RuntimeConnectionTypeB\x0c\n\ncapability\"\xe3\x01\n\"ReleaseChannelGroupGeneratorConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12!\n\x10runtime_selector\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x13\n\x0b\x61llow_empty\x18\x03 \x01(\x08\x12J\n\x08template\x18\x04 \x01(\x0b\x32..prodvana.release_channel.ReleaseChannelConfigB\x08\xfa\x42\x05\x8a\x01\x02\x08\x01*y\n\x15RuntimeConnectionType\x12\x16\n\x12UNKNOWN_CONNECTION\x10\x00\x12\x16\n\x12LONG_LIVED_COMPUTE\x10\x01\x12\r\n\tEXTENSION\x10\x02\x12\x0b\n\x07\x41WS_ECS\x10\x03\x12\x14\n\x10GOOGLE_CLOUD_RUN\x10\x04\x42TZRgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/release_channelb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.release_channel.release_channel_config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -47,30 +47,30 @@
   _RELEASECHANNELRUNTIMECONFIG.fields_by_name['name']._serialized_options = b'\372B)r\'\020\000\030?2!^[a-z]?([a-z0-9-]*[a-z0-9]){0,1}$'
   _RELEASECHANNELGROUPGENERATORCONFIG.fields_by_name['name']._options = None
   _RELEASECHANNELGROUPGENERATORCONFIG.fields_by_name['name']._serialized_options = b'\372B(r&\020\001\030?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$'
   _RELEASECHANNELGROUPGENERATORCONFIG.fields_by_name['runtime_selector']._options = None
   _RELEASECHANNELGROUPGENERATORCONFIG.fields_by_name['runtime_selector']._serialized_options = b'\372B\004r\002\020\001'
   _RELEASECHANNELGROUPGENERATORCONFIG.fields_by_name['template']._options = None
   _RELEASECHANNELGROUPGENERATORCONFIG.fields_by_name['template']._serialized_options = b'\372B\005\212\001\002\010\001'
-  _globals['_RUNTIMECONNECTIONTYPE']._serialized_start=2659
-  _globals['_RUNTIMECONNECTIONTYPE']._serialized_end=2780
+  _globals['_RUNTIMECONNECTIONTYPE']._serialized_start=2692
+  _globals['_RUNTIMECONNECTIONTYPE']._serialized_end=2813
   _globals['_POLICY']._serialized_start=412
   _globals['_POLICY']._serialized_end=617
   _globals['_POLICY_DEFAULTENVENTRY']._serialized_start=534
   _globals['_POLICY_DEFAULTENVENTRY']._serialized_end=617
   _globals['_RELEASECHANNELCONFIG']._serialized_start=620
-  _globals['_RELEASECHANNELCONFIG']._serialized_end=1377
-  _globals['_PRECONDITION']._serialized_start=1380
-  _globals['_PRECONDITION']._serialized_end=2111
-  _globals['_PRECONDITION_RELEASECHANNELSTABLE']._serialized_start=1742
-  _globals['_PRECONDITION_RELEASECHANNELSTABLE']._serialized_end=1869
-  _globals['_PRECONDITION_MANUALAPPROVAL']._serialized_start=1871
-  _globals['_PRECONDITION_MANUALAPPROVAL']._serialized_end=1944
-  _globals['_PRECONDITION_CUSTOMTASK']._serialized_start=1946
-  _globals['_PRECONDITION_CUSTOMTASK']._serialized_end=2030
-  _globals['_PRECONDITION_SHAREDMANUALAPPROVAL']._serialized_start=2032
-  _globals['_PRECONDITION_SHAREDMANUALAPPROVAL']._serialized_end=2077
-  _globals['_RELEASECHANNELRUNTIMECONFIG']._serialized_start=2114
-  _globals['_RELEASECHANNELRUNTIMECONFIG']._serialized_end=2427
-  _globals['_RELEASECHANNELGROUPGENERATORCONFIG']._serialized_start=2430
-  _globals['_RELEASECHANNELGROUPGENERATORCONFIG']._serialized_end=2657
+  _globals['_RELEASECHANNELCONFIG']._serialized_end=1410
+  _globals['_PRECONDITION']._serialized_start=1413
+  _globals['_PRECONDITION']._serialized_end=2144
+  _globals['_PRECONDITION_RELEASECHANNELSTABLE']._serialized_start=1775
+  _globals['_PRECONDITION_RELEASECHANNELSTABLE']._serialized_end=1902
+  _globals['_PRECONDITION_MANUALAPPROVAL']._serialized_start=1904
+  _globals['_PRECONDITION_MANUALAPPROVAL']._serialized_end=1977
+  _globals['_PRECONDITION_CUSTOMTASK']._serialized_start=1979
+  _globals['_PRECONDITION_CUSTOMTASK']._serialized_end=2063
+  _globals['_PRECONDITION_SHAREDMANUALAPPROVAL']._serialized_start=2065
+  _globals['_PRECONDITION_SHAREDMANUALAPPROVAL']._serialized_end=2110
+  _globals['_RELEASECHANNELRUNTIMECONFIG']._serialized_start=2147
+  _globals['_RELEASECHANNELRUNTIMECONFIG']._serialized_end=2460
+  _globals['_RELEASECHANNELGROUPGENERATORCONFIG']._serialized_start=2463
+  _globals['_RELEASECHANNELGROUPGENERATORCONFIG']._serialized_end=2690
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_config_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     DEPLOY_ANNOTATIONS_FIELD_NUMBER: builtins.int
     PRECONDITIONS_FIELD_NUMBER: builtins.int
     PROTECTIONS_FIELD_NUMBER: builtins.int
     CONVERGENCE_PROTECTIONS_FIELD_NUMBER: builtins.int
     SERVICE_INSTANCE_PROTECTIONS_FIELD_NUMBER: builtins.int
     CONSTANTS_FIELD_NUMBER: builtins.int
     LABELS_FIELD_NUMBER: builtins.int
+    DISABLE_ALL_PROTECTIONS_FIELD_NUMBER: builtins.int
     name: builtins.str
     """intentionally does not reference cluster - this allows us to copy release channels across clusters via the same config"""
     group: builtins.str
     """if specified, this release channel is part of a group. This can affect how release channels are rendered on the Prodvana web interface."""
     order: builtins.int
     """deprecated"""
     maturity: prodvana.proto.prodvana.common_config.maturity_pb2.Maturity.ValueType
@@ -119,14 +120,18 @@
     def service_instance_protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig]:
         """protections that all service instances in this release channel should get"""
     @property
     def constants(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.constants_pb2.Constant]:
         """constants made available in template substitutions"""
     @property
     def labels(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.labels.labels_pb2.LabelDefinition]: ...
+    disable_all_protections: builtins.bool
+    """Disable all protections for this release channel - protections will not be created for any service instances in this release channel.
+    This is useful for release channels that are used for testing or are not yet in production (e.g., fast creation of new tenants).
+    """
     def __init__(
         self,
         *,
         name: builtins.str = ...,
         group: builtins.str = ...,
         order: builtins.int = ...,
         maturity: prodvana.proto.prodvana.common_config.maturity_pb2.Maturity.ValueType = ...,
@@ -135,17 +140,18 @@
         deploy_annotations: prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig | None = ...,
         preconditions: collections.abc.Iterable[global___Precondition] | None = ...,
         protections: collections.abc.Iterable[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig] | None = ...,
         convergence_protections: collections.abc.Iterable[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig] | None = ...,
         service_instance_protections: collections.abc.Iterable[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig] | None = ...,
         constants: collections.abc.Iterable[prodvana.proto.prodvana.common_config.constants_pb2.Constant] | None = ...,
         labels: collections.abc.Iterable[prodvana.proto.prodvana.labels.labels_pb2.LabelDefinition] | None = ...,
+        disable_all_protections: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["deploy_annotations", b"deploy_annotations", "policy", b"policy"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["constants", b"constants", "convergence_protections", b"convergence_protections", "deploy_annotations", b"deploy_annotations", "group", b"group", "labels", b"labels", "maturity", b"maturity", "name", b"name", "order", b"order", "policy", b"policy", "preconditions", b"preconditions", "protections", b"protections", "runtimes", b"runtimes", "service_instance_protections", b"service_instance_protections"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["constants", b"constants", "convergence_protections", b"convergence_protections", "deploy_annotations", b"deploy_annotations", "disable_all_protections", b"disable_all_protections", "group", b"group", "labels", b"labels", "maturity", b"maturity", "name", b"name", "order", b"order", "policy", b"policy", "preconditions", b"preconditions", "protections", b"protections", "runtimes", b"runtimes", "service_instance_protections", b"service_instance_protections"]) -> None: ...
 
 global___ReleaseChannelConfig = ReleaseChannelConfig
 
 class Precondition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     class ReleaseChannelStable(google.protobuf.message.Message):
```

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/release_channel/release_channel_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/repo/repo_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/repo/repo_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/repo/repo_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/repo/repo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/fetch_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/fetch_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/fetch_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/fetch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/get_info_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/get_info_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/runtimes/extensions/get_info_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/runtimes/extensions/get_info_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/runtimes/features_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/runtimes/features_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/runtimes/features_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/runtimes/features_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/runtimes/runtimes_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/scm/types_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/scm/types_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/scm/types_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/scm/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/secrets/secrets_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/service/object_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/service/object_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/service/object_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/service/object_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/service/parameters_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/service/parameters_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/service/parameters_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/service/parameters_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/service/service_config_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/service/service_config_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from prodvana.proto.prodvana.runtimes import runtimes_config_pb2 as prodvana_dot_runtimes_dot_runtimes__config__pb2
 from prodvana.proto.prodvana.workflow import integration_config_pb2 as prodvana_dot_workflow_dot_integration__config__pb2
 from prodvana.proto.prodvana.service import parameters_pb2 as prodvana_dot_service_dot_parameters__pb2
 from prodvana.proto.prodvana.volumes import volumes_pb2 as prodvana_dot_volumes_dot_volumes__pb2
 from prodvana.proto.validate import validate_pb2 as validate_dot_validate__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/service/service_config.proto\x12\x10prodvana.service\x1a\x1egoogle/protobuf/duration.proto\x1a$prodvana/capability/capability.proto\x1a&prodvana/common_config/constants.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a!prodvana/common_config/helm.proto\x1a%prodvana/common_config/maturity.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a!prodvana/common_config/task.proto\x1a\'prodvana/delivery/delivery_config.proto\x1a(prodvana/delivery_extension/config.proto\x1a%prodvana/protection/attachments.proto\x1a.prodvana/protection/protection_reference.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a!prodvana/service/parameters.proto\x1a\x1eprodvana/volumes/volumes.proto\x1a\x17validate/validate.proto\"1\n\x0eReplicasConfig\x12\x0f\n\x05\x66ixed\x18\x01 \x01(\x05H\x00\x42\x0e\n\x0c\x63onfig_oneof\"\xaa\x02\n\x0eMetricAnalysis\x12J\n\x0csuccess_rate\x18\x02 \x01(\x0b\x32\x32.prodvana.service.MetricAnalysis.SuccessRateConfigH\x00\x12\x45\n\x0blatency_p95\x18\x03 \x01(\x0b\x32..prodvana.service.MetricAnalysis.LatencyConfigH\x00\x1a\x32\n\x11SuccessRateConfig\x12\x1d\n\x15min_threshold_percent\x18\x01 \x01(\x01\x1a?\n\rLatencyConfig\x12.\n\x0bmax_latency\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x10\n\x0e\x61nalysis_oneof\"\xb7\x02\n\x15ReleaseStrategyConfig\x12<\n\x19individual_stage_deadline\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1a\x61utomated_testing_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12:\n\x10metrics_analysis\x18\x03 \x03(\x0b\x32 .prodvana.service.MetricAnalysis\x12\x17\n\x0fmanual_approval\x18\x04 \x01(\x08\x12\x31\n\x0e\x63heck_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x66\x61ilure_threshold\x18\x06 \x01(\x05\"f\n\tTLSSecret\x12\x14\n\nraw_secret\x18\x03 \x01(\tH\x00\x12\x30\n\x06secret\x18\x04 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x11\n\ntls_secret\x12\x03\xf8\x42\x01\"\x81\x01\n\x0eTLSCertificate\x12\x37\n\x08tls_cert\x18\x01 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x36\n\x07tls_key\x18\x02 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"j\n\x0b\x43\x65rtificate\x12/\n\x03tls\x18\x01 \x01(\x0b\x32 .prodvana.service.TLSCertificateH\x00\x12\x16\n\x0c\x61ws_acm_cert\x18\x02 \x01(\tH\x00\x42\x12\n\x0b\x63\x65rtificate\x12\x03\xf8\x42\x01\"\xb3\x0b\n\x17PerReleaseChannelConfig\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12&\n\x10\x63ustom_hostnames\x18\x02 \x03(\tB\x0c\xfa\x42\t\x92\x01\x06\"\x04r\x02h\x01\x12W\n\x08programs\x18\x05 \x03(\x0b\x32\x36.prodvana.common_config.PerReleaseChannelProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12+\n\x04\x63\x65rt\x18\x06 \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12:\n\x0f\x64\x65livery_config\x18\x07 \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x08 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\t \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x43\n\x0epre_push_tasks\x18\n \x03(\x0b\x32\x1c.prodvana.service.TaskConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12U\n\x13\x64\x65livery_extensions\x18\x12 \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x41\n\x10runtime_specific\x18\x0b \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x11 \x01(\t\x12\x45\n\x11runtime_extension\x18\r \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x0e \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x10 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x0f \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12\x31\n\x07\x61ws_ecs\x18\x16 \x01(\x0b\x32\x1e.prodvana.service.AwsEcsConfigH\x00\x12\x42\n\x10google_cloud_run\x18\x18 \x01(\x0b\x32&.prodvana.service.GoogleCloudRunConfigH\x00\x12h\n\x03\x65nv\x18\x13 \x03(\x0b\x32\x32.prodvana.service.PerReleaseChannelConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12\x33\n\tconstants\x18\x14 \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x44\n\x0bprotections\x18\x15 \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12P\n\x17\x63onvergence_protections\x18\x17 \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x0c\x10\r\",\n\x13\x43\x61pabilityReference\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x18\x43ompiledCapabilityConfig\x12\x39\n\ncapability\x18\x01 \x01(\x0b\x32%.prodvana.capability.CapabilityConfig\".\n\x10ProgramReference\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"6\n\rTaskReference\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"\xf1\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x0c\x62\x61se_program\x18\x02 \x01(\x0b\x32\".prodvana.service.ProgramReference\x12\x39\n\x0cretry_config\x18\x03 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12,\n\x03ref\x18\x04 \x01(\x0b\x32\x1f.prodvana.service.TaskReference\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xa2\x02\n\x17\x44\x65liveryExtensionConfig\x12G\n\x07inlined\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12\x1b\n\x08instance\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12H\n\x03ref\x18\x04 \x01(\x0b\x32\x39.prodvana.delivery_extension.DeliveryExtensionInstanceRefH\x00\x12\x44\n\tlifecycle\x18\x02 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycleB\n\xfa\x42\x07\x82\x01\x04 \x00 \x01\x42\x11\n\ndefinition\x12\x03\xf8\x42\x01\"\x9e\x02\n\x19\x44\x65liveryExtensionInstance\x12G\n\x07inlined\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12H\n\x03ref\x18\x03 \x01(\x0b\x32\x39.prodvana.delivery_extension.DeliveryExtensionInstanceRefH\x00\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x44\n\tlifecycle\x18\x04 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycleB\n\xfa\x42\x07\x82\x01\x04 \x00 \x01\x42\x11\n\ndefinition\x12\x03\xf8\x42\x01\"\x9c\x02\n\x15RuntimeSpecificConfig\x12@\n\x03k8s\x18\x01 \x01(\x0b\x32\x31.prodvana.service.RuntimeSpecificConfig.K8SConfigH\x00\x1a\xae\x01\n\tK8SConfig\x12\x66\n\x13service_annotations\x18\x01 \x03(\x0b\x32I.prodvana.service.RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry\x1a\x39\n\x17ServiceAnnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0eruntime_config\"\x86\x01\n\x16RuntimeExtensionConfig\x12@\n\x10parameter_values\x18\x01 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12*\n\"clear_on_per_release_channel_merge\x18\x02 \x01(\x08\"&\n\x12\x41utoRollbackConfig\x12\x10\n\x08\x64isabled\x18\x01 \x01(\x08\"\xca\x03\n\x0c\x41wsEcsConfig\x12!\n\x19\x65\x63s_service_name_override\x18\x01 \x01(\t\x12P\n\x0ftask_definition\x18\x02 \x01(\x0b\x32-.prodvana.service.AwsEcsConfig.TaskDefinitionB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\\\n\x15network_configuration\x18\x03 \x01(\x0b\x32\x33.prodvana.service.AwsEcsConfig.NetworkConfigurationB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x1a\x8a\x01\n\x0eTaskDefinition\x12\x1a\n\x07inlined\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12>\n\x05local\x18\x02 \x01(\x0b\x32#.prodvana.common_config.LocalConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01H\x00\x42\x1c\n\x15task_definition_oneof\x12\x03\xf8\x42\x01\x1aZ\n\x14NetworkConfiguration\x12\x0f\n\x07subnets\x18\x01 \x03(\t\x12\x17\n\x0fsecurity_groups\x18\x02 \x03(\t\x12\x18\n\x10\x61ssign_public_ip\x18\x03 \x01(\x08\"\x85\x01\n\x14GoogleCloudRunConfig\x12\x1a\n\x07inlined\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12>\n\x05local\x18\x02 \x01(\x0b\x32#.prodvana.common_config.LocalConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01H\x00\x42\x11\n\nspec_oneof\x12\x03\xf8\x42\x01\"\xeb\x10\n\rServiceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x13\n\x0b\x61pplication\x18\x14 \x01(\t\x12\x46\n\x08programs\x18\x02 \x03(\x0b\x32%.prodvana.common_config.ProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x41\n\x10release_strategy\x18\x05 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12U\n\x13per_release_channel\x18\t \x03(\x0b\x32).prodvana.service.PerReleaseChannelConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\x0c\x63\x61pabilities\x18\n \x03(\x0b\x32%.prodvana.service.CapabilityReferenceB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12:\n\x0f\x64\x65livery_config\x18\x0b \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0c \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\r \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x34\n\x0epre_push_tasks\x18\x0f \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1d \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12Q\n\x1c\x64\x65livery_extension_instances\x18\x1e \x03(\x0b\x32+.prodvana.service.DeliveryExtensionInstance\x12\x41\n\x10runtime_specific\x18\x10 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x1c \x01(\t\x12N\n\nparameters\x18\x15 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x42\n\x10parameter_values\x18\x16 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12\x33\n\tconstants\x18! \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x34\n\x11progress_deadline\x18\x18 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x12 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x13 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x1b \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1a \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12\x31\n\x07\x61ws_ecs\x18# \x01(\x0b\x32\x1e.prodvana.service.AwsEcsConfigH\x00\x12\x42\n\x10google_cloud_run\x18$ \x01(\x0b\x32&.prodvana.service.GoogleCloudRunConfigH\x00\x12M\n\x12parameters_autogen\x18\x17 \x01(\x0e\x32\x31.prodvana.service.ServiceConfig.ParametersAutogen\x12;\n\rauto_rollback\x18\x19 \x01(\x0b\x32$.prodvana.service.AutoRollbackConfig\x12\x1c\n\x14no_cleanup_on_delete\x18\x1f \x01(\x08\x12^\n\x03\x65nv\x18  \x03(\x0b\x32(.prodvana.service.ServiceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12\x1f\n\x17\x61sync_set_desired_state\x18\" \x01(\x08\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\"M\n\x11ParametersAutogen\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05IMAGE\x10\x02\x12\x16\n\x12IMAGE_AND_REPLICAS\x10\x03\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\x0e\x10\x0fJ\x04\x08\x11\x10\x12R\x08\x65xternalR\x10image_repositoryR\rbase_templateR\x15\x63ontainer_registry_idR\x0bprotections\"\x97\x10\n\x1d\x43ompiledServiceInstanceConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x12 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x32\n\x08maturity\x18\x05 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x41\n\x10release_strategy\x18\x06 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12\x18\n\x10\x63ustom_hostnames\x18\x07 \x03(\t\x12+\n\x04\x63\x65rt\x18\n \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12\x46\n\x07runtime\x18\x0b \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x1b \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12@\n\x0c\x63\x61pabilities\x18\x0c \x03(\x0b\x32*.prodvana.service.CompiledCapabilityConfig\x12:\n\x0f\x64\x65livery_config\x18\r \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0e \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\x0f \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x34\n\x0epre_push_tasks\x18\x11 \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1e \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12Q\n\x1c\x64\x65livery_extension_instances\x18\x1f \x03(\x0b\x32+.prodvana.service.DeliveryExtensionInstance\x12\x41\n\x10runtime_specific\x18\x13 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12?\n\nparameters\x18\x18 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x19 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x33\n\tconstants\x18! \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x34\n\x11progress_deadline\x18\x1a \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x16 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x17 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1d \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12\x31\n\x07\x61ws_ecs\x18% \x01(\x0b\x32\x1e.prodvana.service.AwsEcsConfigH\x00\x12\x42\n\x10google_cloud_run\x18\' \x01(\x0b\x32&.prodvana.service.GoogleCloudRunConfigH\x00\x12n\n\x03\x65nv\x18\x1c \x03(\x0b\x32\x38.prodvana.service.CompiledServiceInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12\x1c\n\x14no_cleanup_on_delete\x18  \x01(\x08\x12\x44\n\x0bprotections\x18\" \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12P\n\x17\x63onvergence_protections\x18& \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\x10\x10\x11J\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16J\x04\x08#\x10$J\x04\x08$\x10%R\rbase_templateR\x0cruntime_type\"\x88\x02\n\x11\x43ompiledJobConfig\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x46\n\x07runtime\x18\x04 \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x05 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%prodvana/service/service_config.proto\x12\x10prodvana.service\x1a\x1egoogle/protobuf/duration.proto\x1a$prodvana/capability/capability.proto\x1a&prodvana/common_config/constants.proto\x1a prodvana/common_config/env.proto\x1a.prodvana/common_config/kubernetes_config.proto\x1a!prodvana/common_config/helm.proto\x1a%prodvana/common_config/maturity.proto\x1a\'prodvana/common_config/parameters.proto\x1a$prodvana/common_config/program.proto\x1a\"prodvana/common_config/retry.proto\x1a!prodvana/common_config/task.proto\x1a\'prodvana/delivery/delivery_config.proto\x1a(prodvana/delivery_extension/config.proto\x1a%prodvana/protection/attachments.proto\x1a.prodvana/protection/protection_reference.proto\x1a\x35prodvana/release_channel/release_channel_config.proto\x1a\'prodvana/runtimes/runtimes_config.proto\x1a*prodvana/workflow/integration_config.proto\x1a!prodvana/service/parameters.proto\x1a\x1eprodvana/volumes/volumes.proto\x1a\x17validate/validate.proto\"1\n\x0eReplicasConfig\x12\x0f\n\x05\x66ixed\x18\x01 \x01(\x05H\x00\x42\x0e\n\x0c\x63onfig_oneof\"\xaa\x02\n\x0eMetricAnalysis\x12J\n\x0csuccess_rate\x18\x02 \x01(\x0b\x32\x32.prodvana.service.MetricAnalysis.SuccessRateConfigH\x00\x12\x45\n\x0blatency_p95\x18\x03 \x01(\x0b\x32..prodvana.service.MetricAnalysis.LatencyConfigH\x00\x1a\x32\n\x11SuccessRateConfig\x12\x1d\n\x15min_threshold_percent\x18\x01 \x01(\x01\x1a?\n\rLatencyConfig\x12.\n\x0bmax_latency\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationB\x10\n\x0e\x61nalysis_oneof\"\xb7\x02\n\x15ReleaseStrategyConfig\x12<\n\x19individual_stage_deadline\x18\x01 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1a\x61utomated_testing_duration\x18\x02 \x01(\x0b\x32\x19.google.protobuf.Duration\x12:\n\x10metrics_analysis\x18\x03 \x03(\x0b\x32 .prodvana.service.MetricAnalysis\x12\x17\n\x0fmanual_approval\x18\x04 \x01(\x08\x12\x31\n\x0e\x63heck_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x19\n\x11\x66\x61ilure_threshold\x18\x06 \x01(\x05\"f\n\tTLSSecret\x12\x14\n\nraw_secret\x18\x03 \x01(\tH\x00\x12\x30\n\x06secret\x18\x04 \x01(\x0b\x32\x1e.prodvana.common_config.SecretH\x00\x42\x11\n\ntls_secret\x12\x03\xf8\x42\x01\"\x81\x01\n\x0eTLSCertificate\x12\x37\n\x08tls_cert\x18\x01 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x36\n\x07tls_key\x18\x02 \x01(\x0b\x32\x1b.prodvana.service.TLSSecretB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\"j\n\x0b\x43\x65rtificate\x12/\n\x03tls\x18\x01 \x01(\x0b\x32 .prodvana.service.TLSCertificateH\x00\x12\x16\n\x0c\x61ws_acm_cert\x18\x02 \x01(\tH\x00\x42\x12\n\x0b\x63\x65rtificate\x12\x03\xf8\x42\x01\"\xb3\x0b\n\x17PerReleaseChannelConfig\x12 \n\x0frelease_channel\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12&\n\x10\x63ustom_hostnames\x18\x02 \x03(\tB\x0c\xfa\x42\t\x92\x01\x06\"\x04r\x02h\x01\x12W\n\x08programs\x18\x05 \x03(\x0b\x32\x36.prodvana.common_config.PerReleaseChannelProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12+\n\x04\x63\x65rt\x18\x06 \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12:\n\x0f\x64\x65livery_config\x18\x07 \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x08 \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\t \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x43\n\x0epre_push_tasks\x18\n \x03(\x0b\x32\x1c.prodvana.service.TaskConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12U\n\x13\x64\x65livery_extensions\x18\x12 \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x41\n\x10runtime_specific\x18\x0b \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x11 \x01(\t\x12\x45\n\x11runtime_extension\x18\r \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x0e \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x10 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x0f \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12\x31\n\x07\x61ws_ecs\x18\x16 \x01(\x0b\x32\x1e.prodvana.service.AwsEcsConfigH\x00\x12\x42\n\x10google_cloud_run\x18\x18 \x01(\x0b\x32&.prodvana.service.GoogleCloudRunConfigH\x00\x12h\n\x03\x65nv\x18\x13 \x03(\x0b\x32\x32.prodvana.service.PerReleaseChannelConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12\x33\n\tconstants\x18\x14 \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x44\n\x0bprotections\x18\x15 \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12P\n\x17\x63onvergence_protections\x18\x17 \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x03\x10\x04J\x04\x08\x04\x10\x05J\x04\x08\x0c\x10\r\",\n\x13\x43\x61pabilityReference\x12\x15\n\x04name\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\"U\n\x18\x43ompiledCapabilityConfig\x12\x39\n\ncapability\x18\x01 \x01(\x0b\x32%.prodvana.capability.CapabilityConfig\".\n\x10ProgramReference\x12\x0e\n\x04name\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"6\n\rTaskReference\x12\x19\n\x0frelease_channel\x18\x01 \x01(\tH\x00\x42\n\n\x03ref\x12\x03\xf8\x42\x01\"\xf1\x01\n\nTaskConfig\x12@\n\x07program\x18\x01 \x01(\x0b\x32%.prodvana.common_config.ProgramConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\x38\n\x0c\x62\x61se_program\x18\x02 \x01(\x0b\x32\".prodvana.service.ProgramReference\x12\x39\n\x0cretry_config\x18\x03 \x01(\x0b\x32#.prodvana.common_config.RetryConfig\x12,\n\x03ref\x18\x04 \x01(\x0b\x32\x1f.prodvana.service.TaskReference\"p\n\x0eProtectionLink\x12;\n\tlifecycle\x18\x03 \x01(\x0b\x32(.prodvana.protection.ProtectionLifecycle\x12\x15\n\rattachment_id\x18\x04 \x01(\tJ\x04\x08\x01\x10\x02J\x04\x08\x02\x10\x03\"\xa2\x02\n\x17\x44\x65liveryExtensionConfig\x12G\n\x07inlined\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12\x1b\n\x08instance\x18\x03 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12H\n\x03ref\x18\x04 \x01(\x0b\x32\x39.prodvana.delivery_extension.DeliveryExtensionInstanceRefH\x00\x12\x44\n\tlifecycle\x18\x02 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycleB\n\xfa\x42\x07\x82\x01\x04 \x00 \x01\x42\x11\n\ndefinition\x12\x03\xf8\x42\x01\"\x9e\x02\n\x19\x44\x65liveryExtensionInstance\x12G\n\x07inlined\x18\x01 \x01(\x0b\x32\x34.prodvana.delivery_extension.DeliveryExtensionConfigH\x00\x12H\n\x03ref\x18\x03 \x01(\x0b\x32\x39.prodvana.delivery_extension.DeliveryExtensionInstanceRefH\x00\x12\x15\n\x04name\x18\x02 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01\x12\x44\n\tlifecycle\x18\x04 \x01(\x0e\x32%.prodvana.common_config.TaskLifecycleB\n\xfa\x42\x07\x82\x01\x04 \x00 \x01\x42\x11\n\ndefinition\x12\x03\xf8\x42\x01\"\x9c\x02\n\x15RuntimeSpecificConfig\x12@\n\x03k8s\x18\x01 \x01(\x0b\x32\x31.prodvana.service.RuntimeSpecificConfig.K8SConfigH\x00\x1a\xae\x01\n\tK8SConfig\x12\x66\n\x13service_annotations\x18\x01 \x03(\x0b\x32I.prodvana.service.RuntimeSpecificConfig.K8SConfig.ServiceAnnotationsEntry\x1a\x39\n\x17ServiceAnnotationsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\x42\x10\n\x0eruntime_config\"\x86\x01\n\x16RuntimeExtensionConfig\x12@\n\x10parameter_values\x18\x01 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12*\n\"clear_on_per_release_channel_merge\x18\x02 \x01(\x08\"&\n\x12\x41utoRollbackConfig\x12\x10\n\x08\x64isabled\x18\x01 \x01(\x08\"\xca\x03\n\x0c\x41wsEcsConfig\x12!\n\x19\x65\x63s_service_name_override\x18\x01 \x01(\t\x12P\n\x0ftask_definition\x18\x02 \x01(\x0b\x32-.prodvana.service.AwsEcsConfig.TaskDefinitionB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x12\\\n\x15network_configuration\x18\x03 \x01(\x0b\x32\x33.prodvana.service.AwsEcsConfig.NetworkConfigurationB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01\x1a\x8a\x01\n\x0eTaskDefinition\x12\x1a\n\x07inlined\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12>\n\x05local\x18\x02 \x01(\x0b\x32#.prodvana.common_config.LocalConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01H\x00\x42\x1c\n\x15task_definition_oneof\x12\x03\xf8\x42\x01\x1aZ\n\x14NetworkConfiguration\x12\x0f\n\x07subnets\x18\x01 \x03(\t\x12\x17\n\x0fsecurity_groups\x18\x02 \x03(\t\x12\x18\n\x10\x61ssign_public_ip\x18\x03 \x01(\x08\"\x85\x01\n\x14GoogleCloudRunConfig\x12\x1a\n\x07inlined\x18\x01 \x01(\tB\x07\xfa\x42\x04r\x02\x10\x01H\x00\x12>\n\x05local\x18\x02 \x01(\x0b\x32#.prodvana.common_config.LocalConfigB\x08\xfa\x42\x05\x8a\x01\x02\x10\x01H\x00\x42\x11\n\nspec_oneof\x12\x03\xf8\x42\x01\"\xbd\x11\n\rServiceConfig\x12\x39\n\x04name\x18\x01 \x01(\tB+\xfa\x42(r&\x10\x01\x18?2 ^[a-z]([a-z0-9-]*[a-z0-9]){0,1}$\x12\x13\n\x0b\x61pplication\x18\x14 \x01(\t\x12\x46\n\x08programs\x18\x02 \x03(\x0b\x32%.prodvana.common_config.ProgramConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x41\n\x10release_strategy\x18\x05 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12U\n\x13per_release_channel\x18\t \x03(\x0b\x32).prodvana.service.PerReleaseChannelConfigB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12J\n\x0c\x63\x61pabilities\x18\n \x03(\x0b\x32%.prodvana.service.CapabilityReferenceB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12:\n\x0f\x64\x65livery_config\x18\x0b \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0c \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\r \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x34\n\x0epre_push_tasks\x18\x0f \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1d \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12Q\n\x1c\x64\x65livery_extension_instances\x18\x1e \x03(\x0b\x32+.prodvana.service.DeliveryExtensionInstance\x12P\n\x17\x63onvergence_protections\x18% \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12\x41\n\x10runtime_specific\x18\x10 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12\x1a\n\x12runtime_connection\x18\x1c \x01(\t\x12N\n\nparameters\x18\x15 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinitionB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12\x42\n\x10parameter_values\x18\x16 \x01(\x0b\x32(.prodvana.service.ServiceParameterValues\x12\x33\n\tconstants\x18! \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x34\n\x11progress_deadline\x18\x18 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x12 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x13 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x43\n\x0f\x65xternal_config\x18\x1b \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1a \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12\x31\n\x07\x61ws_ecs\x18# \x01(\x0b\x32\x1e.prodvana.service.AwsEcsConfigH\x00\x12\x42\n\x10google_cloud_run\x18$ \x01(\x0b\x32&.prodvana.service.GoogleCloudRunConfigH\x00\x12M\n\x12parameters_autogen\x18\x17 \x01(\x0e\x32\x31.prodvana.service.ServiceConfig.ParametersAutogen\x12;\n\rauto_rollback\x18\x19 \x01(\x0b\x32$.prodvana.service.AutoRollbackConfig\x12\x1c\n\x14no_cleanup_on_delete\x18\x1f \x01(\x08\x12^\n\x03\x65nv\x18  \x03(\x0b\x32(.prodvana.service.ServiceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12\x1f\n\x17\x61sync_set_desired_state\x18\" \x01(\x08\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\"M\n\x11ParametersAutogen\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x08\n\x04NONE\x10\x01\x12\t\n\x05IMAGE\x10\x02\x12\x16\n\x12IMAGE_AND_REPLICAS\x10\x03\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x06\x10\x07J\x04\x08\x07\x10\x08J\x04\x08\x08\x10\tJ\x04\x08\x0e\x10\x0fJ\x04\x08\x11\x10\x12R\x08\x65xternalR\x10image_repositoryR\rbase_templateR\x15\x63ontainer_registry_idR\x0bprotections\"\x97\x10\n\x1d\x43ompiledServiceInstanceConfig\x12\x0f\n\x07service\x18\x01 \x01(\t\x12\x13\n\x0b\x61pplication\x18\x12 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x32\n\x08replicas\x18\x04 \x01(\x0b\x32 .prodvana.service.ReplicasConfig\x12\x32\n\x08maturity\x18\x05 \x01(\x0e\x32 .prodvana.common_config.Maturity\x12\x41\n\x10release_strategy\x18\x06 \x01(\x0b\x32\'.prodvana.service.ReleaseStrategyConfig\x12\x18\n\x10\x63ustom_hostnames\x18\x07 \x03(\t\x12+\n\x04\x63\x65rt\x18\n \x01(\x0b\x32\x1d.prodvana.service.Certificate\x12\x46\n\x07runtime\x18\x0b \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x1b \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfig\x12@\n\x0c\x63\x61pabilities\x18\x0c \x03(\x0b\x32*.prodvana.service.CompiledCapabilityConfig\x12:\n\x0f\x64\x65livery_config\x18\r \x01(\x0b\x32!.prodvana.delivery.DeliveryConfig\x12\x38\n\x07volumes\x18\x0e \x03(\x0b\x32\x18.prodvana.volumes.VolumeB\r\xfa\x42\n\x92\x01\x07\"\x05\x8a\x01\x02\x10\x01\x12@\n\x12\x64\x65ploy_annotations\x18\x0f \x01(\x0b\x32$.prodvana.workflow.AnnotationsConfig\x12\x34\n\x0epre_push_tasks\x18\x11 \x03(\x0b\x32\x1c.prodvana.service.TaskConfig\x12\x46\n\x13\x64\x65livery_extensions\x18\x1e \x03(\x0b\x32).prodvana.service.DeliveryExtensionConfig\x12Q\n\x1c\x64\x65livery_extension_instances\x18\x1f \x03(\x0b\x32+.prodvana.service.DeliveryExtensionInstance\x12\x41\n\x10runtime_specific\x18\x13 \x01(\x0b\x32\'.prodvana.service.RuntimeSpecificConfig\x12?\n\nparameters\x18\x18 \x03(\x0b\x32+.prodvana.common_config.ParameterDefinition\x12@\n\x10parameter_values\x18\x19 \x03(\x0b\x32&.prodvana.common_config.ParameterValue\x12\x33\n\tconstants\x18! \x03(\x0b\x32 .prodvana.common_config.Constant\x12\x34\n\x11progress_deadline\x18\x1a \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x45\n\x11runtime_extension\x18\x16 \x01(\x0b\x32(.prodvana.service.RuntimeExtensionConfigH\x00\x12\x45\n\x11kubernetes_config\x18\x17 \x01(\x0b\x32(.prodvana.common_config.KubernetesConfigH\x00\x12\x32\n\x04helm\x18\x1d \x01(\x0b\x32\".prodvana.common_config.HelmConfigH\x00\x12\x31\n\x07\x61ws_ecs\x18% \x01(\x0b\x32\x1e.prodvana.service.AwsEcsConfigH\x00\x12\x42\n\x10google_cloud_run\x18\' \x01(\x0b\x32&.prodvana.service.GoogleCloudRunConfigH\x00\x12n\n\x03\x65nv\x18\x1c \x03(\x0b\x32\x38.prodvana.service.CompiledServiceInstanceConfig.EnvEntryB\'\xfa\x42$\x9a\x01!\x18\x01\"\x1dr\x1b\x32\x19^[a-zA-Z_]+[a-zA-Z0-9_]*$\x12\x1c\n\x14no_cleanup_on_delete\x18  \x01(\x08\x12\x44\n\x0bprotections\x18\" \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x12P\n\x17\x63onvergence_protections\x18& \x03(\x0b\x32/.prodvana.protection.ProtectionAttachmentConfig\x1aL\n\x08\x45nvEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12/\n\x05value\x18\x02 \x01(\x0b\x32 .prodvana.common_config.EnvValue:\x02\x38\x01\x42\x0e\n\x0c\x63onfig_oneofJ\x04\x08\x08\x10\tJ\x04\x08\t\x10\nJ\x04\x08\x10\x10\x11J\x04\x08\x14\x10\x15J\x04\x08\x15\x10\x16J\x04\x08#\x10$J\x04\x08$\x10%R\rbase_templateR\x0cruntime_type\"\x88\x02\n\x11\x43ompiledJobConfig\x12\x13\n\x0bname_prefix\x18\x01 \x01(\t\x12\x17\n\x0frelease_channel\x18\x02 \x01(\t\x12\x37\n\x08programs\x18\x03 \x03(\x0b\x32%.prodvana.common_config.ProgramConfig\x12\x46\n\x07runtime\x18\x04 \x01(\x0b\x32\x35.prodvana.release_channel.ReleaseChannelRuntimeConfig\x12\x44\n\x11runtime_execution\x18\x05 \x01(\x0b\x32).prodvana.runtimes.RuntimeExecutionConfigBLZJgithub.com/prodvana/prodvana-public/go/prodvana-sdk/proto/prodvana/serviceb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'prodvana.service.service_config_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -178,19 +178,19 @@
   _globals['_AWSECSCONFIG_TASKDEFINITION']._serialized_start=5219
   _globals['_AWSECSCONFIG_TASKDEFINITION']._serialized_end=5357
   _globals['_AWSECSCONFIG_NETWORKCONFIGURATION']._serialized_start=5359
   _globals['_AWSECSCONFIG_NETWORKCONFIGURATION']._serialized_end=5449
   _globals['_GOOGLECLOUDRUNCONFIG']._serialized_start=5452
   _globals['_GOOGLECLOUDRUNCONFIG']._serialized_end=5585
   _globals['_SERVICECONFIG']._serialized_start=5588
-  _globals['_SERVICECONFIG']._serialized_end=7743
+  _globals['_SERVICECONFIG']._serialized_end=7825
   _globals['_SERVICECONFIG_ENVENTRY']._serialized_start=3237
   _globals['_SERVICECONFIG_ENVENTRY']._serialized_end=3313
-  _globals['_SERVICECONFIG_PARAMETERSAUTOGEN']._serialized_start=7541
-  _globals['_SERVICECONFIG_PARAMETERSAUTOGEN']._serialized_end=7618
-  _globals['_COMPILEDSERVICEINSTANCECONFIG']._serialized_start=7746
-  _globals['_COMPILEDSERVICEINSTANCECONFIG']._serialized_end=9817
+  _globals['_SERVICECONFIG_PARAMETERSAUTOGEN']._serialized_start=7623
+  _globals['_SERVICECONFIG_PARAMETERSAUTOGEN']._serialized_end=7700
+  _globals['_COMPILEDSERVICEINSTANCECONFIG']._serialized_start=7828
+  _globals['_COMPILEDSERVICEINSTANCECONFIG']._serialized_end=9899
   _globals['_COMPILEDSERVICEINSTANCECONFIG_ENVENTRY']._serialized_start=3237
   _globals['_COMPILEDSERVICEINSTANCECONFIG_ENVENTRY']._serialized_end=3313
-  _globals['_COMPILEDJOBCONFIG']._serialized_start=9820
-  _globals['_COMPILEDJOBCONFIG']._serialized_end=10084
+  _globals['_COMPILEDJOBCONFIG']._serialized_start=9902
+  _globals['_COMPILEDJOBCONFIG']._serialized_end=10166
 # @@protoc_insertion_point(module_scope)
```

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/service/service_config_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/service/service_config_pb2.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,16 @@
         """
     @property
     def constants(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.constants_pb2.Constant]:
         """constants made available in template substitutions"""
     @property
     def protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig]: ...
     @property
-    def convergence_protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig]: ...
+    def convergence_protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig]:
+        """TODO: unused today, but will be used for per-service per-RC convergence protections in the future"""
     def __init__(
         self,
         *,
         release_channel: builtins.str = ...,
         custom_hostnames: collections.abc.Iterable[builtins.str] | None = ...,
         programs: collections.abc.Iterable[prodvana.proto.prodvana.common_config.program_pb2.PerReleaseChannelProgramConfig] | None = ...,
         cert: global___Certificate | None = ...,
@@ -722,14 +723,15 @@
     CAPABILITIES_FIELD_NUMBER: builtins.int
     DELIVERY_CONFIG_FIELD_NUMBER: builtins.int
     VOLUMES_FIELD_NUMBER: builtins.int
     DEPLOY_ANNOTATIONS_FIELD_NUMBER: builtins.int
     PRE_PUSH_TASKS_FIELD_NUMBER: builtins.int
     DELIVERY_EXTENSIONS_FIELD_NUMBER: builtins.int
     DELIVERY_EXTENSION_INSTANCES_FIELD_NUMBER: builtins.int
+    CONVERGENCE_PROTECTIONS_FIELD_NUMBER: builtins.int
     RUNTIME_SPECIFIC_FIELD_NUMBER: builtins.int
     RUNTIME_CONNECTION_FIELD_NUMBER: builtins.int
     PARAMETERS_FIELD_NUMBER: builtins.int
     PARAMETER_VALUES_FIELD_NUMBER: builtins.int
     CONSTANTS_FIELD_NUMBER: builtins.int
     PROGRESS_DEADLINE_FIELD_NUMBER: builtins.int
     RUNTIME_EXTENSION_FIELD_NUMBER: builtins.int
@@ -766,14 +768,17 @@
     def pre_push_tasks(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___TaskConfig]:
         """DEPRECATED: Replace with delivery_extensions"""
     @property
     def delivery_extensions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtensionConfig]: ...
     @property
     def delivery_extension_instances(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___DeliveryExtensionInstance]: ...
     @property
+    def convergence_protections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig]:
+        """Convergence protections applied to all release channels."""
+    @property
     def runtime_specific(self) -> global___RuntimeSpecificConfig: ...
     runtime_connection: builtins.str
     """which runtime connection to use in each release channel.
     optional if only one runtime makes sense for the service config.
     """
     @property
     def parameters(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition]: ...
@@ -826,14 +831,15 @@
         capabilities: collections.abc.Iterable[global___CapabilityReference] | None = ...,
         delivery_config: prodvana.proto.prodvana.delivery.delivery_config_pb2.DeliveryConfig | None = ...,
         volumes: collections.abc.Iterable[prodvana.proto.prodvana.volumes.volumes_pb2.Volume] | None = ...,
         deploy_annotations: prodvana.proto.prodvana.workflow.integration_config_pb2.AnnotationsConfig | None = ...,
         pre_push_tasks: collections.abc.Iterable[global___TaskConfig] | None = ...,
         delivery_extensions: collections.abc.Iterable[global___DeliveryExtensionConfig] | None = ...,
         delivery_extension_instances: collections.abc.Iterable[global___DeliveryExtensionInstance] | None = ...,
+        convergence_protections: collections.abc.Iterable[prodvana.proto.prodvana.protection.attachments_pb2.ProtectionAttachmentConfig] | None = ...,
         runtime_specific: global___RuntimeSpecificConfig | None = ...,
         runtime_connection: builtins.str = ...,
         parameters: collections.abc.Iterable[prodvana.proto.prodvana.common_config.parameters_pb2.ParameterDefinition] | None = ...,
         parameter_values: prodvana.proto.prodvana.service.parameters_pb2.ServiceParameterValues | None = ...,
         constants: collections.abc.Iterable[prodvana.proto.prodvana.common_config.constants_pb2.Constant] | None = ...,
         progress_deadline: google.protobuf.duration_pb2.Duration | None = ...,
         runtime_extension: global___RuntimeExtensionConfig | None = ...,
@@ -845,15 +851,15 @@
         parameters_autogen: global___ServiceConfig.ParametersAutogen.ValueType = ...,
         auto_rollback: global___AutoRollbackConfig | None = ...,
         no_cleanup_on_delete: builtins.bool = ...,
         env: collections.abc.Mapping[builtins.str, prodvana.proto.prodvana.common_config.env_pb2.EnvValue] | None = ...,
         async_set_desired_state: builtins.bool = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["auto_rollback", b"auto_rollback", "aws_ecs", b"aws_ecs", "config_oneof", b"config_oneof", "delivery_config", b"delivery_config", "deploy_annotations", b"deploy_annotations", "external_config", b"external_config", "google_cloud_run", b"google_cloud_run", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "parameter_values", b"parameter_values", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "async_set_desired_state", b"async_set_desired_state", "auto_rollback", b"auto_rollback", "aws_ecs", b"aws_ecs", "capabilities", b"capabilities", "config_oneof", b"config_oneof", "constants", b"constants", "delivery_config", b"delivery_config", "delivery_extension_instances", b"delivery_extension_instances", "delivery_extensions", b"delivery_extensions", "deploy_annotations", b"deploy_annotations", "env", b"env", "external_config", b"external_config", "google_cloud_run", b"google_cloud_run", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "name", b"name", "no_cleanup_on_delete", b"no_cleanup_on_delete", "parameter_values", b"parameter_values", "parameters", b"parameters", "parameters_autogen", b"parameters_autogen", "per_release_channel", b"per_release_channel", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["application", b"application", "async_set_desired_state", b"async_set_desired_state", "auto_rollback", b"auto_rollback", "aws_ecs", b"aws_ecs", "capabilities", b"capabilities", "config_oneof", b"config_oneof", "constants", b"constants", "convergence_protections", b"convergence_protections", "delivery_config", b"delivery_config", "delivery_extension_instances", b"delivery_extension_instances", "delivery_extensions", b"delivery_extensions", "deploy_annotations", b"deploy_annotations", "env", b"env", "external_config", b"external_config", "google_cloud_run", b"google_cloud_run", "helm", b"helm", "kubernetes_config", b"kubernetes_config", "name", b"name", "no_cleanup_on_delete", b"no_cleanup_on_delete", "parameter_values", b"parameter_values", "parameters", b"parameters", "parameters_autogen", b"parameters_autogen", "per_release_channel", b"per_release_channel", "pre_push_tasks", b"pre_push_tasks", "programs", b"programs", "progress_deadline", b"progress_deadline", "release_strategy", b"release_strategy", "replicas", b"replicas", "runtime_connection", b"runtime_connection", "runtime_extension", b"runtime_extension", "runtime_specific", b"runtime_specific", "volumes", b"volumes"]) -> None: ...
     def WhichOneof(self, oneof_group: typing_extensions.Literal["config_oneof", b"config_oneof"]) -> typing_extensions.Literal["runtime_extension", "kubernetes_config", "external_config", "helm", "aws_ecs", "google_cloud_run"] | None: ...
 
 global___ServiceConfig = ServiceConfig
 
 class CompiledServiceInstanceConfig(google.protobuf.message.Message):
     """a compiled version of ServiceConfig specific to a service instance, with release-channel configs applied"""
```

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/service/service_manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/service/service_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/service/service_manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/service/service_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/service/service_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/service/service_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/service/user_metadata_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/service/user_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/service/user_metadata_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/service/user_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/settings/organization/users_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/settings/organization/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/settings/organization/users_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/settings/organization/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/settings/organization/users_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/stat/efficiency_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/stat/efficiency_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/stat/efficiency_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/stat/efficiency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/users/users_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/users/users_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/users/users_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/users/users_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/version/source_metadata_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/version/source_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/version/source_metadata_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/version/source_metadata_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/volumes/volumes_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/volumes/volumes_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/volumes/volumes_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/volumes/volumes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/workflow/integration_config_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/workflow/integration_config_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/workflow/integration_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py` & `prodvana-0.3.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py` & `prodvana-0.3.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi` & `prodvana-0.3.9/prodvana/proto/prodvana/workflow/workflow_manager_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/validate/validate_pb2.py` & `prodvana-0.3.9/prodvana/proto/validate/validate_pb2.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/proto/validate/validate_pb2.pyi` & `prodvana-0.3.9/prodvana/proto/validate/validate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/utils/desired_states.py` & `prodvana-0.3.9/prodvana/utils/desired_states.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/utils/parameters.py` & `prodvana-0.3.9/prodvana/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/utils/protections.py` & `prodvana-0.3.9/prodvana/utils/protections.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/utils/service_config.py` & `prodvana-0.3.9/prodvana/utils/service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/prodvana/utils/tests/test_service_config.py` & `prodvana-0.3.9/prodvana/utils/tests/test_service_config.py`

 * *Files identical despite different names*

### Comparing `prodvana-0.3.8/pyproject.toml` & `prodvana-0.3.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prodvana"
-version = "0.3.8"
+version = "0.3.9"
 description = "Prodvana's client libraries"
 readme = "README.md"
 authors = []
 homepage = "https://prodvana.io"
 documentation = "https://docs.prodvana.io"
 repository = "https://github.com/prodvana/prodvana-public"
 exclude = ["examples"]
```

### Comparing `prodvana-0.3.8/PKG-INFO` & `prodvana-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prodvana
-Version: 0.3.8
+Version: 0.3.9
 Summary: Prodvana's client libraries
 Home-page: https://prodvana.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-api-python-client (>=2.58.0,<3.0)
```

