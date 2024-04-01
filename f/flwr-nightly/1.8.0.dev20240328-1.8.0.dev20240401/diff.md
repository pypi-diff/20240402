# Comparing `tmp/flwr_nightly-1.8.0.dev20240328.tar.gz` & `tmp/flwr_nightly-1.8.0.dev20240401.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flwr_nightly-1.8.0.dev20240328.tar", max compression
+gzip compressed data, was "flwr_nightly-1.8.0.dev20240401.tar", max compression
```

## Comparing `flwr_nightly-1.8.0.dev20240328.tar` & `flwr_nightly-1.8.0.dev20240401.tar`

### file list

```diff
@@ -1,210 +1,211 @@
--rw-r--r--   0        0        0    11358 2024-03-28 23:05:13.653898 flwr_nightly-1.8.0.dev20240328/LICENSE
--rw-r--r--   0        0        0    12916 2024-03-28 23:05:13.653898 flwr_nightly-1.8.0.dev20240328/README.md
--rw-r--r--   0        0        0     5863 2024-03-28 23:05:29.853907 flwr_nightly-1.8.0.dev20240328/pyproject.toml
--rw-r--r--   0        0        0      937 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/__init__.py
--rw-r--r--   0        0        0      720 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/__init__.py
--rw-r--r--   0        0        0     1095 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/app.py
--rw-r--r--   0        0        0     2184 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/example.py
--rw-r--r--   0        0        0     4675 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/flower_toml.py
--rw-r--r--   0        0        0      789 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/__init__.py
--rw-r--r--   0        0        0     5016 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/new.py
--rw-r--r--   0        0        0      725 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/__init__.py
--rw-r--r--   0        0        0      714 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/README.md.tpl
--rw-r--r--   0        0        0      729 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/__init__.py
--rw-r--r--   0        0        0      736 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/__init__.py
--rw-r--r--   0        0        0       21 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
--rw-r--r--   0        0        0      521 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
--rw-r--r--   0        0        0     1173 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
--rw-r--r--   0        0        0       48 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
--rw-r--r--   0        0        0      248 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
--rw-r--r--   0        0        0      594 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
--rw-r--r--   0        0        0       48 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
--rw-r--r--   0        0        0     3675 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
--rw-r--r--   0        0        0      269 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/flower.toml.tpl
--rw-r--r--   0        0        0      408 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
--rw-r--r--   0        0        0      507 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
--rw-r--r--   0        0        0      697 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
--rw-r--r--   0        0        0       30 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/requirements.numpy.txt.tpl
--rw-r--r--   0        0        0      106 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/requirements.pytorch.txt.tpl
--rw-r--r--   0        0        0      209 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/requirements.tensorflow.txt.tpl
--rw-r--r--   0        0        0      789 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/run/__init__.py
--rw-r--r--   0        0        0     2329 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/run/run.py
--rw-r--r--   0        0        0     2300 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/utils.py
--rw-r--r--   0        0        0     1187 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/__init__.py
--rw-r--r--   0        0        0    25536 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/app.py
--rw-r--r--   0        0        0     8183 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/client.py
--rw-r--r--   0        0        0     8047 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/client_app.py
--rw-r--r--   0        0        0     7435 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      735 2024-03-28 23:05:14.069898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/grpc_client/__init__.py
--rw-r--r--   0        0        0     8717 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/grpc_client/connection.py
--rw-r--r--   0        0        0      752 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/grpc_rere_client/__init__.py
--rw-r--r--   0        0        0     7421 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/grpc_rere_client/connection.py
--rw-r--r--   0        0        0      719 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/message_handler/__init__.py
--rw-r--r--   0        0        0     6553 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/message_handler/message_handler.py
--rw-r--r--   0        0        0     1824 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/message_handler/task_handler.py
--rw-r--r--   0        0        0     1143 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/__init__.py
--rw-r--r--   0        0        0     5397 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/centraldp_mods.py
--rw-r--r--   0        0        0     2623 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/comms_mods.py
--rw-r--r--   0        0        0     4918 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/localdp_mod.py
--rw-r--r--   0        0        0      849 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     1095 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
--rw-r--r--   0        0        0    19699 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
--rw-r--r--   0        0        0     1226 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/utils.py
--rw-r--r--   0        0        0     1778 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/node_state.py
--rw-r--r--   0        0        0     2195 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/node_state_tests.py
--rw-r--r--   0        0        0    10283 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/numpy_client.py
--rw-r--r--   0        0        0      735 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/rest_client/__init__.py
--rw-r--r--   0        0        0    12422 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/rest_client/connection.py
--rw-r--r--   0        0        0     1006 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/typing.py
--rw-r--r--   0        0        0     3721 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/__init__.py
--rw-r--r--   0        0        0     1882 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/address.py
--rw-r--r--   0        0        0     1954 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/constant.py
--rw-r--r--   0        0        0     1313 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/context.py
--rw-r--r--   0        0        0      891 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/date.py
--rw-r--r--   0        0        0     6113 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/differential_privacy.py
--rw-r--r--   0        0        0     1074 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/differential_privacy_constants.py
--rw-r--r--   0        0        0     2004 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/dp.py
--rw-r--r--   0        0        0     2812 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/exit_handlers.py
--rw-r--r--   0        0        0     2273 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/grpc.py
--rw-r--r--   0        0        0     6118 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/logger.py
--rw-r--r--   0        0        0    11773 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/message.py
--rw-r--r--   0        0        0     4961 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/object_ref.py
--rw-r--r--   0        0        0     2095 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/parameter.py
--rw-r--r--   0        0        0     1385 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/pyproject.py
--rw-r--r--   0        0        0     1054 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/__init__.py
--rw-r--r--   0        0        0     4652 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/configsrecord.py
--rw-r--r--   0        0        0     1393 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/conversion_utils.py
--rw-r--r--   0        0        0     3923 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/metricsrecord.py
--rw-r--r--   0        0        0     4849 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/parametersrecord.py
--rw-r--r--   0        0        0     3016 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/recordset.py
--rw-r--r--   0        0        0     3879 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/typeddict.py
--rw-r--r--   0        0        0    13798 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/recordset_compat.py
--rw-r--r--   0        0        0    10856 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/retry_invoker.py
--rw-r--r--   0        0        0      731 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/__init__.py
--rw-r--r--   0        0        0      738 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/crypto/__init__.py
--rw-r--r--   0        0        0     2792 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/crypto/shamir.py
--rw-r--r--   0        0        0     3546 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
--rw-r--r--   0        0        0     3026 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
--rw-r--r--   0        0        0     2310 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/quantization.py
--rw-r--r--   0        0        0     2183 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
--rw-r--r--   0        0        0     3221 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
--rw-r--r--   0        0        0    22250 2024-03-28 23:05:14.073898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/serde.py
--rw-r--r--   0        0        0     7782 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/telemetry.py
--rw-r--r--   0        0        0     4382 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/typing.py
--rw-r--r--   0        0        0      666 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/version.py
--rw-r--r--   0        0        0      683 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/__init__.py
--rw-r--r--   0        0        0     3115 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/driver_pb2.py
--rw-r--r--   0        0        0     4670 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/driver_pb2.pyi
--rw-r--r--   0        0        0     7304 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/driver_pb2_grpc.py
--rw-r--r--   0        0        0     2022 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/driver_pb2_grpc.pyi
--rw-r--r--   0        0        0     1084 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/error_pb2.py
--rw-r--r--   0        0        0      734 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/error_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/error_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/error_pb2_grpc.pyi
--rw-r--r--   0        0        0     4316 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/fleet_pb2.py
--rw-r--r--   0        0        0     7325 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/fleet_pb2.pyi
--rw-r--r--   0        0        0     9042 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/fleet_pb2_grpc.py
--rw-r--r--   0        0        0     2491 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/fleet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1081 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/node_pb2.py
--rw-r--r--   0        0        0      751 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/node_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/node_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/node_pb2_grpc.pyi
--rw-r--r--   0        0        0     6009 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/recordset_pb2.py
--rw-r--r--   0        0        0    14161 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/recordset_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/recordset_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/recordset_pb2_grpc.pyi
--rw-r--r--   0        0        0     2472 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/task_pb2.py
--rw-r--r--   0        0        0     4320 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/task_pb2.pyi
--rw-r--r--   0        0        0      159 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/task_pb2_grpc.py
--rw-r--r--   0        0        0       76 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/task_pb2_grpc.pyi
--rw-r--r--   0        0        0     9781 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/transport_pb2.py
--rw-r--r--   0        0        0    21497 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2598 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      766 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0        0 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/py.typed
--rw-r--r--   0        0        0     1785 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/__init__.py
--rw-r--r--   0        0        0    24302 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/app.py
--rw-r--r--   0        0        0     6127 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/client_manager.py
--rw-r--r--   0        0        0     2399 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/client_proxy.py
--rw-r--r--   0        0        0      892 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/compat/__init__.py
--rw-r--r--   0        0        0     5271 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/compat/app.py
--rw-r--r--   0        0        0     3450 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/compat/app_utils.py
--rw-r--r--   0        0        0     7344 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/compat/driver_client_proxy.py
--rw-r--r--   0        0        0     1766 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/compat/legacy_context.py
--rw-r--r--   0        0        0     1061 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/criterion.py
--rw-r--r--   0        0        0      820 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/driver/__init__.py
--rw-r--r--   0        0        0     9660 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/driver/driver.py
--rw-r--r--   0        0        0     4586 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/driver/grpc_driver.py
--rw-r--r--   0        0        0     5121 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/history.py
--rw-r--r--   0        0        0     5592 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/run_serverapp.py
--rw-r--r--   0        0        0    17664 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/server.py
--rw-r--r--   0        0        0     4280 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/server_app.py
--rw-r--r--   0        0        0     1349 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/server_config.py
--rw-r--r--   0        0        0     2836 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/__init__.py
--rw-r--r--   0        0        0    13468 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/aggregate.py
--rw-r--r--   0        0        0     6532 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/bulyan.py
--rw-r--r--   0        0        0    17458 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/dp_adaptive_clipping.py
--rw-r--r--   0        0        0    12904 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/dp_fixed_clipping.py
--rw-r--r--   0        0        0     4877 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     7219 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     5900 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6505 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedadagrad.py
--rw-r--r--   0        0        0     6763 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedadam.py
--rw-r--r--   0        0        0    11799 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedavg.py
--rw-r--r--   0        0        0     9784 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedavg_android.py
--rw-r--r--   0        0        0     8132 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedavgm.py
--rw-r--r--   0        0        0     2704 2024-03-28 23:05:14.077898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedmedian.py
--rw-r--r--   0        0        0     5242 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedopt.py
--rw-r--r--   0        0        0     6862 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedprox.py
--rw-r--r--   0        0        0     5890 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedtrimmedavg.py
--rw-r--r--   0        0        0     6080 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedxgb_bagging.py
--rw-r--r--   0        0        0     5607 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedxgb_cyclic.py
--rw-r--r--   0        0        0     4047 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedxgb_nn_avg.py
--rw-r--r--   0        0        0     6801 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedyogi.py
--rw-r--r--   0        0        0     6285 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/krum.py
--rw-r--r--   0        0        0    10150 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/qfedavg.py
--rw-r--r--   0        0        0     7543 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/strategy.py
--rw-r--r--   0        0        0      707 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/__init__.py
--rw-r--r--   0        0        0      712 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/driver/__init__.py
--rw-r--r--   0        0        0     1932 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/driver/driver_grpc.py
--rw-r--r--   0        0        0     4761 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/driver/driver_servicer.py
--rw-r--r--   0        0        0      711 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/__init__.py
--rw-r--r--   0        0        0      735 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
--rw-r--r--   0        0        0     5993 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
--rw-r--r--   0        0        0     6458 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
--rw-r--r--   0        0        0     4887 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
--rw-r--r--   0        0        0    11818 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
--rw-r--r--   0        0        0      758 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
--rw-r--r--   0        0        0     3036 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
--rw-r--r--   0        0        0      731 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
--rw-r--r--   0        0        0     3161 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
--rw-r--r--   0        0        0      735 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
--rw-r--r--   0        0        0     5906 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
--rw-r--r--   0        0        0      783 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/vce/__init__.py
--rw-r--r--   0        0        0     1466 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
--rw-r--r--   0        0        0     2260 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
--rw-r--r--   0        0        0     6375 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
--rw-r--r--   0        0        0    11789 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/vce/vce_api.py
--rw-r--r--   0        0        0     1003 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/state/__init__.py
--rw-r--r--   0        0        0     8707 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/state/in_memory_state.py
--rw-r--r--   0        0        0    22005 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/state/sqlite_state.py
--rw-r--r--   0        0        0     6036 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/state/state.py
--rw-r--r--   0        0        0     1654 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/state/state_factory.py
--rw-r--r--   0        0        0      913 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/typing.py
--rw-r--r--   0        0        0      908 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/utils/__init__.py
--rw-r--r--   0        0        0     5485 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/utils/tensorboard.py
--rw-r--r--   0        0        0     5301 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/utils/validator.py
--rw-r--r--   0        0        0      902 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/workflow/__init__.py
--rw-r--r--   0        0        0     1082 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/workflow/constant.py
--rw-r--r--   0        0        0    12655 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/workflow/default_workflows.py
--rw-r--r--   0        0        0      880 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/workflow/secure_aggregation/__init__.py
--rw-r--r--   0        0        0     5838 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
--rw-r--r--   0        0        0    29187 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
--rw-r--r--   0        0        0     1400 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/__init__.py
--rw-r--r--   0        0        0    13904 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/app.py
--rw-r--r--   0        0        0      734 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0    20054 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/ray_transport/ray_actor.py
--rw-r--r--   0        0        0     6738 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0     2392 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/ray_transport/utils.py
--rw-r--r--   0        0        0    15685 2024-03-28 23:05:14.081898 flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/run_simulation.py
--rw-r--r--   0        0        0    15257 1970-01-01 00:00:00.000000 flwr_nightly-1.8.0.dev20240328/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-04-01 23:05:40.679554 flwr_nightly-1.8.0.dev20240401/LICENSE
+-rw-r--r--   0        0        0    12916 2024-04-01 23:05:40.679554 flwr_nightly-1.8.0.dev20240401/README.md
+-rw-r--r--   0        0        0     5863 2024-04-01 23:05:54.083566 flwr_nightly-1.8.0.dev20240401/pyproject.toml
+-rw-r--r--   0        0        0      937 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/__init__.py
+-rw-r--r--   0        0        0      720 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/app.py
+-rw-r--r--   0        0        0     2184 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/example.py
+-rw-r--r--   0        0        0     4675 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/flower_toml.py
+-rw-r--r--   0        0        0      789 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/__init__.py
+-rw-r--r--   0        0        0     5016 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/new.py
+-rw-r--r--   0        0        0      725 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/__init__.py
+-rw-r--r--   0        0        0      714 2024-04-01 23:05:41.091554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/README.md.tpl
+-rw-r--r--   0        0        0      729 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/__init__.py
+-rw-r--r--   0        0        0      736 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/__init__.py
+-rw-r--r--   0        0        0       21 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/__init__.py.tpl
+-rw-r--r--   0        0        0      521 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl
+-rw-r--r--   0        0        0     1173 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl
+-rw-r--r--   0        0        0       48 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/client.tensorflow.py.tpl
+-rw-r--r--   0        0        0      248 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/server.numpy.py.tpl
+-rw-r--r--   0        0        0      594 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl
+-rw-r--r--   0        0        0       48 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/server.tensorflow.py.tpl
+-rw-r--r--   0        0        0     3675 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl
+-rw-r--r--   0        0        0      269 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/flower.toml.tpl
+-rw-r--r--   0        0        0      408 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/pyproject.numpy.toml.tpl
+-rw-r--r--   0        0        0      507 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/pyproject.pytorch.toml.tpl
+-rw-r--r--   0        0        0      697 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl
+-rw-r--r--   0        0        0       30 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/requirements.numpy.txt.tpl
+-rw-r--r--   0        0        0      106 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/requirements.pytorch.txt.tpl
+-rw-r--r--   0        0        0      209 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/requirements.tensorflow.txt.tpl
+-rw-r--r--   0        0        0      789 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/run/__init__.py
+-rw-r--r--   0        0        0     2329 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/run/run.py
+-rw-r--r--   0        0        0     2300 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/utils.py
+-rw-r--r--   0        0        0     1187 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/__init__.py
+-rw-r--r--   0        0        0    25445 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/app.py
+-rw-r--r--   0        0        0     8183 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/client.py
+-rw-r--r--   0        0        0     8315 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/client_app.py
+-rw-r--r--   0        0        0     7435 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0     8717 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_client/connection.py
+-rw-r--r--   0        0        0      752 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_rere_client/__init__.py
+-rw-r--r--   0        0        0     8525 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_rere_client/connection.py
+-rw-r--r--   0        0        0     2377 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/heartbeat.py
+-rw-r--r--   0        0        0      719 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/message_handler/__init__.py
+-rw-r--r--   0        0        0     6553 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/message_handler/message_handler.py
+-rw-r--r--   0        0        0     1824 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/message_handler/task_handler.py
+-rw-r--r--   0        0        0     1143 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/__init__.py
+-rw-r--r--   0        0        0     5397 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/centraldp_mods.py
+-rw-r--r--   0        0        0     2623 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/comms_mods.py
+-rw-r--r--   0        0        0     4918 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/localdp_mod.py
+-rw-r--r--   0        0        0      849 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     1095 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py
+-rw-r--r--   0        0        0    19699 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py
+-rw-r--r--   0        0        0     1226 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/utils.py
+-rw-r--r--   0        0        0     1778 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/node_state.py
+-rw-r--r--   0        0        0     2195 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/node_state_tests.py
+-rw-r--r--   0        0        0    10283 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/numpy_client.py
+-rw-r--r--   0        0        0      735 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/rest_client/__init__.py
+-rw-r--r--   0        0        0    14447 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/rest_client/connection.py
+-rw-r--r--   0        0        0     1006 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/typing.py
+-rw-r--r--   0        0        0     3721 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/__init__.py
+-rw-r--r--   0        0        0     1882 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/address.py
+-rw-r--r--   0        0        0     2084 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/constant.py
+-rw-r--r--   0        0        0     1313 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/context.py
+-rw-r--r--   0        0        0      891 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/date.py
+-rw-r--r--   0        0        0     6113 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/differential_privacy.py
+-rw-r--r--   0        0        0     1074 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/differential_privacy_constants.py
+-rw-r--r--   0        0        0     2004 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/dp.py
+-rw-r--r--   0        0        0     2812 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/exit_handlers.py
+-rw-r--r--   0        0        0     2273 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/grpc.py
+-rw-r--r--   0        0        0     6096 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/logger.py
+-rw-r--r--   0        0        0    11773 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/message.py
+-rw-r--r--   0        0        0     4961 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/object_ref.py
+-rw-r--r--   0        0        0     2095 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/parameter.py
+-rw-r--r--   0        0        0     1385 2024-04-01 23:05:41.095554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/pyproject.py
+-rw-r--r--   0        0        0     1054 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/__init__.py
+-rw-r--r--   0        0        0     4652 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/configsrecord.py
+-rw-r--r--   0        0        0     1393 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/conversion_utils.py
+-rw-r--r--   0        0        0     3923 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/metricsrecord.py
+-rw-r--r--   0        0        0     4849 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/parametersrecord.py
+-rw-r--r--   0        0        0     3016 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/recordset.py
+-rw-r--r--   0        0        0     3879 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/typeddict.py
+-rw-r--r--   0        0        0    13798 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/recordset_compat.py
+-rw-r--r--   0        0        0    11669 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/retry_invoker.py
+-rw-r--r--   0        0        0      731 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0      738 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/crypto/__init__.py
+-rw-r--r--   0        0        0     2792 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/crypto/shamir.py
+-rw-r--r--   0        0        0     3546 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py
+-rw-r--r--   0        0        0     3026 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py
+-rw-r--r--   0        0        0     2310 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/quantization.py
+-rw-r--r--   0        0        0     2183 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/secaggplus_constants.py
+-rw-r--r--   0        0        0     3221 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/secaggplus_utils.py
+-rw-r--r--   0        0        0    22250 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/serde.py
+-rw-r--r--   0        0        0     7782 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/telemetry.py
+-rw-r--r--   0        0        0     4382 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/typing.py
+-rw-r--r--   0        0        0      666 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/version.py
+-rw-r--r--   0        0        0      683 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/__init__.py
+-rw-r--r--   0        0        0     3115 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2.py
+-rw-r--r--   0        0        0     4670 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2.pyi
+-rw-r--r--   0        0        0     7304 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2_grpc.py
+-rw-r--r--   0        0        0     2022 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1084 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/error_pb2.py
+-rw-r--r--   0        0        0      734 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/error_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/error_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/error_pb2_grpc.pyi
+-rw-r--r--   0        0        0     4316 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2.py
+-rw-r--r--   0        0        0     7325 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2.pyi
+-rw-r--r--   0        0        0     9042 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2_grpc.py
+-rw-r--r--   0        0        0     2491 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1081 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/node_pb2.py
+-rw-r--r--   0        0        0      751 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/node_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/node_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/node_pb2_grpc.pyi
+-rw-r--r--   0        0        0     6009 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/recordset_pb2.py
+-rw-r--r--   0        0        0    14161 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/recordset_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/recordset_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/recordset_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2472 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/task_pb2.py
+-rw-r--r--   0        0        0     4320 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/task_pb2.pyi
+-rw-r--r--   0        0        0      159 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/task_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/task_pb2_grpc.pyi
+-rw-r--r--   0        0        0     9781 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2.py
+-rw-r--r--   0        0        0    21497 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2598 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      766 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0        0 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/py.typed
+-rw-r--r--   0        0        0     1785 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/__init__.py
+-rw-r--r--   0        0        0    24302 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/app.py
+-rw-r--r--   0        0        0     6127 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/client_manager.py
+-rw-r--r--   0        0        0     2399 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/client_proxy.py
+-rw-r--r--   0        0        0      892 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/__init__.py
+-rw-r--r--   0        0        0     5271 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/app.py
+-rw-r--r--   0        0        0     3450 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/app_utils.py
+-rw-r--r--   0        0        0     7344 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/driver_client_proxy.py
+-rw-r--r--   0        0        0     1766 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/legacy_context.py
+-rw-r--r--   0        0        0     1061 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/criterion.py
+-rw-r--r--   0        0        0      820 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/driver/__init__.py
+-rw-r--r--   0        0        0     9660 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/driver/driver.py
+-rw-r--r--   0        0        0     4586 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/driver/grpc_driver.py
+-rw-r--r--   0        0        0     5121 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/history.py
+-rw-r--r--   0        0        0     5592 2024-04-01 23:05:41.099554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/run_serverapp.py
+-rw-r--r--   0        0        0    17664 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/server.py
+-rw-r--r--   0        0        0     4402 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/server_app.py
+-rw-r--r--   0        0        0     1349 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/server_config.py
+-rw-r--r--   0        0        0     2836 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/__init__.py
+-rw-r--r--   0        0        0    13468 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/aggregate.py
+-rw-r--r--   0        0        0     6532 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/bulyan.py
+-rw-r--r--   0        0        0    17458 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dp_adaptive_clipping.py
+-rw-r--r--   0        0        0    12904 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dp_fixed_clipping.py
+-rw-r--r--   0        0        0     4877 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     7219 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     5900 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6505 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     6763 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedadam.py
+-rw-r--r--   0        0        0    11799 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedavg.py
+-rw-r--r--   0        0        0     9784 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     8132 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedavgm.py
+-rw-r--r--   0        0        0     2704 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedmedian.py
+-rw-r--r--   0        0        0     5242 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedopt.py
+-rw-r--r--   0        0        0     6862 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedprox.py
+-rw-r--r--   0        0        0     5890 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedtrimmedavg.py
+-rw-r--r--   0        0        0     6080 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedxgb_bagging.py
+-rw-r--r--   0        0        0     5607 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedxgb_cyclic.py
+-rw-r--r--   0        0        0     4047 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedxgb_nn_avg.py
+-rw-r--r--   0        0        0     6801 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedyogi.py
+-rw-r--r--   0        0        0     6285 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/krum.py
+-rw-r--r--   0        0        0    10150 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7543 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/strategy.py
+-rw-r--r--   0        0        0      707 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/__init__.py
+-rw-r--r--   0        0        0      712 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/driver/__init__.py
+-rw-r--r--   0        0        0     1932 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/driver/driver_grpc.py
+-rw-r--r--   0        0        0     4761 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/driver/driver_servicer.py
+-rw-r--r--   0        0        0      711 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/__init__.py
+-rw-r--r--   0        0        0      735 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py
+-rw-r--r--   0        0        0     5993 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py
+-rw-r--r--   0        0        0     6458 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py
+-rw-r--r--   0        0        0     4887 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11818 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py
+-rw-r--r--   0        0        0      758 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py
+-rw-r--r--   0        0        0     3036 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py
+-rw-r--r--   0        0        0      731 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/message_handler/__init__.py
+-rw-r--r--   0        0        0     3238 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py
+-rw-r--r--   0        0        0      735 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py
+-rw-r--r--   0        0        0     6734 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py
+-rw-r--r--   0        0        0      783 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/__init__.py
+-rw-r--r--   0        0        0     1466 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py
+-rw-r--r--   0        0        0     2260 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/backend/backend.py
+-rw-r--r--   0        0        0     6375 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py
+-rw-r--r--   0        0        0    12041 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/vce_api.py
+-rw-r--r--   0        0        0     1003 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/__init__.py
+-rw-r--r--   0        0        0     8707 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/in_memory_state.py
+-rw-r--r--   0        0        0    22005 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/sqlite_state.py
+-rw-r--r--   0        0        0     6036 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/state.py
+-rw-r--r--   0        0        0     1654 2024-04-01 23:05:41.103554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/state_factory.py
+-rw-r--r--   0        0        0      913 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/typing.py
+-rw-r--r--   0        0        0      908 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/utils/__init__.py
+-rw-r--r--   0        0        0     5485 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/utils/tensorboard.py
+-rw-r--r--   0        0        0     5301 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/utils/validator.py
+-rw-r--r--   0        0        0      902 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/__init__.py
+-rw-r--r--   0        0        0     1082 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/constant.py
+-rw-r--r--   0        0        0    12655 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/default_workflows.py
+-rw-r--r--   0        0        0      880 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/secure_aggregation/__init__.py
+-rw-r--r--   0        0        0     5838 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py
+-rw-r--r--   0        0        0    29187 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py
+-rw-r--r--   0        0        0     1400 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/__init__.py
+-rw-r--r--   0        0        0    13904 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/app.py
+-rw-r--r--   0        0        0      734 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0    20054 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/ray_actor.py
+-rw-r--r--   0        0        0     6738 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0     2392 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/utils.py
+-rw-r--r--   0        0        0    15685 2024-04-01 23:05:41.107554 flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/run_simulation.py
+-rw-r--r--   0        0        0    15257 1970-01-01 00:00:00.000000 flwr_nightly-1.8.0.dev20240401/PKG-INFO
```

### Comparing `flwr_nightly-1.8.0.dev20240328/LICENSE` & `flwr_nightly-1.8.0.dev20240401/LICENSE`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/README.md` & `flwr_nightly-1.8.0.dev20240401/README.md`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/pyproject.toml` & `flwr_nightly-1.8.0.dev20240401/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.4.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "flwr-nightly"
-version = "1.8.0-dev20240328"
+version = "1.8.0-dev20240401"
 description = "Flower: A Friendly Federated Learning Framework"
 license = "Apache-2.0"
 authors = ["The Flower Authors <hello@flower.ai>"]
 readme = "README.md"
 homepage = "https://flower.ai"
 repository = "https://github.com/adap/flower"
 documentation = "https://flower.ai"
```

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/app.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/example.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/example.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/flower_toml.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/flower_toml.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/new.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/new.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/README.md.tpl` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/README.md.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/client.numpy.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/client.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/server.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/code/task.pytorch.py.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/new/templates/app/pyproject.tensorflow.toml.tpl`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/run/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/run/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/run/run.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/run/run.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/cli/utils.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/cli/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/app.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     MISSING_EXTRA_REST,
     TRANSPORT_TYPE_GRPC_BIDI,
     TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
     TRANSPORT_TYPES,
 )
 from flwr.common.exit_handlers import register_exit_handlers
-from flwr.common.logger import log, warn_deprecated_feature, warn_experimental_feature
+from flwr.common.logger import log, warn_deprecated_feature
 from flwr.common.message import Error
 from flwr.common.object_ref import load_app, validate
 from flwr.common.retry_invoker import RetryInvoker, exponential
 
 from .grpc_client.connection import grpc_connection
 from .grpc_rere_client.connection import grpc_request_response
 from .message_handler.message_handler import handle_control_message
@@ -381,27 +381,25 @@
 
             client_fn = single_client_factory
 
         def _load_client_app() -> ClientApp:
             return ClientApp(client_fn=client_fn)
 
         load_client_app_fn = _load_client_app
-    else:
-        warn_experimental_feature("`load_client_app_fn`")
 
     # At this point, only `load_client_app_fn` should be used
     # Both `client` and `client_fn` must not be used directly
 
     # Initialize connection context manager
     connection, address, connection_error_type = _init_connection(
         transport, server_address
     )
 
     retry_invoker = RetryInvoker(
-        wait_factory=exponential,
+        wait_gen_factory=exponential,
         recoverable_exceptions=connection_error_type,
         max_tries=max_retries,
         max_time=max_wait_time,
         on_giveup=lambda retry_state: (
             log(
                 WARN,
                 "Giving up reconnection after %.2f seconds and %s tries.",
```

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/client.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/client_app.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/client_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from flwr.client.message_handler.message_handler import (
     handle_legacy_message_from_msgtype,
 )
 from flwr.client.mod.utils import make_ffn
 from flwr.client.typing import ClientFn, Mod
 from flwr.common import Context, Message, MessageType
+from flwr.common.logger import warn_preview_feature
 
 from .typing import ClientAppCallable
 
 
 class ClientApp:
     """Flower ClientApp.
 
@@ -119,14 +120,16 @@
         """
 
         def train_decorator(train_fn: ClientAppCallable) -> ClientAppCallable:
             """Register the train fn with the ServerApp object."""
             if self._call:
                 raise _registration_error(MessageType.TRAIN)
 
+            warn_preview_feature("ClientApp-register-train-function")
+
             # Register provided function with the ClientApp object
             # Wrap mods around the wrapped step function
             self._train = make_ffn(train_fn, self._mods)
 
             # Return provided function unmodified
             return train_fn
 
@@ -147,14 +150,16 @@
         """
 
         def evaluate_decorator(evaluate_fn: ClientAppCallable) -> ClientAppCallable:
             """Register the evaluate fn with the ServerApp object."""
             if self._call:
                 raise _registration_error(MessageType.EVALUATE)
 
+            warn_preview_feature("ClientApp-register-evaluate-function")
+
             # Register provided function with the ClientApp object
             # Wrap mods around the wrapped step function
             self._evaluate = make_ffn(evaluate_fn, self._mods)
 
             # Return provided function unmodified
             return evaluate_fn
 
@@ -175,14 +180,16 @@
         """
 
         def query_decorator(query_fn: ClientAppCallable) -> ClientAppCallable:
             """Register the query fn with the ServerApp object."""
             if self._call:
                 raise _registration_error(MessageType.QUERY)
 
+            warn_preview_feature("ClientApp-register-query-function")
+
             # Register provided function with the ClientApp object
             # Wrap mods around the wrapped step function
             self._query = make_ffn(query_fn, self._mods)
 
             # Return provided function unmodified
             return query_fn
```

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/dpfedavg_numpy_client.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/grpc_client/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/grpc_client/connection.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/grpc_rere_client/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_rere_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/grpc_rere_client/connection.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/grpc_rere_client/connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,49 +11,57 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Contextmanager for a gRPC request-response channel to the Flower server."""
 
 
+import random
+import threading
 from contextlib import contextmanager
 from copy import copy
 from logging import DEBUG, ERROR
 from pathlib import Path
-from typing import Callable, Dict, Iterator, Optional, Tuple, Union, cast
+from typing import Callable, Iterator, Optional, Tuple, Union, cast
 
+from flwr.client.heartbeat import start_ping_loop
 from flwr.client.message_handler.message_handler import validate_out_message
 from flwr.client.message_handler.task_handler import get_task_ins, validate_task_ins
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH
+from flwr.common.constant import (
+    PING_BASE_MULTIPLIER,
+    PING_CALL_TIMEOUT,
+    PING_DEFAULT_INTERVAL,
+    PING_RANDOM_RANGE,
+)
 from flwr.common.grpc import create_channel
-from flwr.common.logger import log, warn_experimental_feature
+from flwr.common.logger import log
 from flwr.common.message import Message, Metadata
 from flwr.common.retry_invoker import RetryInvoker
 from flwr.common.serde import message_from_taskins, message_to_taskres
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     DeleteNodeRequest,
+    PingRequest,
+    PingResponse,
     PullTaskInsRequest,
     PushTaskResRequest,
 )
 from flwr.proto.fleet_pb2_grpc import FleetStub  # pylint: disable=E0611
 from flwr.proto.node_pb2 import Node  # pylint: disable=E0611
 from flwr.proto.task_pb2 import TaskIns  # pylint: disable=E0611
 
-KEY_NODE = "node"
-KEY_METADATA = "in_message_metadata"
-
 
 def on_channel_state_change(channel_connectivity: str) -> None:
     """Log channel connectivity."""
     log(DEBUG, channel_connectivity)
 
 
 @contextmanager
-def grpc_request_response(
+def grpc_request_response(  # pylint: disable=R0914, R0915
     server_address: str,
     insecure: bool,
     retry_invoker: RetryInvoker,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,  # pylint: disable=W0613
     root_certificates: Optional[Union[bytes, str]] = None,
 ) -> Iterator[
     Tuple[
@@ -91,67 +99,99 @@
     Returns
     -------
     receive : Callable
     send : Callable
     create_node : Optional[Callable]
     delete_node : Optional[Callable]
     """
-    warn_experimental_feature("`grpc-rere`")
-
     if isinstance(root_certificates, str):
         root_certificates = Path(root_certificates).read_bytes()
 
     channel = create_channel(
         server_address=server_address,
         insecure=insecure,
         root_certificates=root_certificates,
         max_message_length=max_message_length,
     )
     channel.subscribe(on_channel_state_change)
-    stub = FleetStub(channel)
 
-    # Necessary state to validate messages to be sent
-    state: Dict[str, Optional[Metadata]] = {KEY_METADATA: None}
-
-    # Enable create_node and delete_node to store node
-    node_store: Dict[str, Optional[Node]] = {KEY_NODE: None}
+    # Shared variables for inner functions
+    stub = FleetStub(channel)
+    metadata: Optional[Metadata] = None
+    node: Optional[Node] = None
+    ping_thread: Optional[threading.Thread] = None
+    ping_stop_event = threading.Event()
 
     ###########################################################################
-    # receive/send functions
+    # ping/create_node/delete_node/receive/send functions
     ###########################################################################
 
+    def ping() -> None:
+        # Get Node
+        if node is None:
+            log(ERROR, "Node instance missing")
+            return
+
+        # Construct the ping request
+        req = PingRequest(node=node, ping_interval=PING_DEFAULT_INTERVAL)
+
+        # Call FleetAPI
+        res: PingResponse = stub.Ping(req, timeout=PING_CALL_TIMEOUT)
+
+        # Check if success
+        if not res.success:
+            raise RuntimeError("Ping failed unexpectedly.")
+
+        # Wait
+        rd = random.uniform(*PING_RANDOM_RANGE)
+        next_interval: float = PING_DEFAULT_INTERVAL - PING_CALL_TIMEOUT
+        next_interval *= PING_BASE_MULTIPLIER + rd
+        if not ping_stop_event.is_set():
+            ping_stop_event.wait(next_interval)
+
     def create_node() -> None:
         """Set create_node."""
+        # Call FleetAPI
         create_node_request = CreateNodeRequest()
         create_node_response = retry_invoker.invoke(
             stub.CreateNode,
             request=create_node_request,
         )
-        node_store[KEY_NODE] = create_node_response.node
+
+        # Remember the node and the ping-loop thread
+        nonlocal node, ping_thread
+        node = cast(Node, create_node_response.node)
+        ping_thread = start_ping_loop(ping, ping_stop_event)
 
     def delete_node() -> None:
         """Set delete_node."""
         # Get Node
-        if node_store[KEY_NODE] is None:
+        nonlocal node
+        if node is None:
             log(ERROR, "Node instance missing")
             return
-        node: Node = cast(Node, node_store[KEY_NODE])
 
+        # Stop the ping-loop thread
+        ping_stop_event.set()
+        if ping_thread is not None:
+            ping_thread.join()
+
+        # Call FleetAPI
         delete_node_request = DeleteNodeRequest(node=node)
         retry_invoker.invoke(stub.DeleteNode, request=delete_node_request)
 
-        del node_store[KEY_NODE]
+        # Cleanup
+        node = None
 
     def receive() -> Optional[Message]:
         """Receive next task from server."""
         # Get Node
-        if node_store[KEY_NODE] is None:
+        if node is None:
             log(ERROR, "Node instance missing")
             return None
-        node: Node = cast(Node, node_store[KEY_NODE])
 
         # Request instructions (task) from server
         request = PullTaskInsRequest(node=node)
         response = retry_invoker.invoke(stub.PullTaskIns, request=request)
 
         # Get the current TaskIns
         task_ins: Optional[TaskIns] = get_task_ins(response)
@@ -163,44 +203,46 @@
         ):
             task_ins = None
 
         # Construct the Message
         in_message = message_from_taskins(task_ins) if task_ins else None
 
         # Remember `metadata` of the in message
-        state[KEY_METADATA] = copy(in_message.metadata) if in_message else None
+        nonlocal metadata
+        metadata = copy(in_message.metadata) if in_message else None
 
         # Return the message if available
         return in_message
 
     def send(message: Message) -> None:
         """Send task result back to server."""
         # Get Node
-        if node_store[KEY_NODE] is None:
+        if node is None:
             log(ERROR, "Node instance missing")
             return
 
-        # Get incoming message
-        in_metadata = state[KEY_METADATA]
-        if in_metadata is None:
+        # Get the metadata of the incoming message
+        nonlocal metadata
+        if metadata is None:
             log(ERROR, "No current message")
             return
 
         # Validate out message
-        if not validate_out_message(message, in_metadata):
+        if not validate_out_message(message, metadata):
             log(ERROR, "Invalid out message")
             return
 
         # Construct TaskRes
         task_res = message_to_taskres(message)
 
         # Serialize ProtoBuf to bytes
         request = PushTaskResRequest(task_res_list=[task_res])
         _ = retry_invoker.invoke(stub.PushTaskRes, request)
 
-        state[KEY_METADATA] = None
+        # Cleanup
+        metadata = None
 
     try:
         # Yield methods
         yield (receive, send, create_node, delete_node)
     except Exception as exc:  # pylint: disable=broad-except
         log(ERROR, exc)
```

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/message_handler/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/message_handler/message_handler.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/message_handler/message_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/message_handler/task_handler.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/message_handler/task_handler.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/centraldp_mods.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/centraldp_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/comms_mods.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/comms_mods.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/localdp_mod.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/localdp_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/secure_aggregation/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/secure_aggregation/secagg_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/secure_aggregation/secaggplus_mod.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/mod/utils.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/mod/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/node_state.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/node_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/node_state_tests.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/node_state_tests.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/numpy_client.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/rest_client/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/rest_client/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/rest_client/connection.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/rest_client/connection.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,59 +11,66 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 """Contextmanager for a REST request-response channel to the Flower server."""
 
 
+import random
 import sys
+import threading
 from contextlib import contextmanager
 from copy import copy
 from logging import ERROR, INFO, WARN
-from typing import Callable, Dict, Iterator, Optional, Tuple, Union, cast
+from typing import Callable, Iterator, Optional, Tuple, Union
 
+from flwr.client.heartbeat import start_ping_loop
 from flwr.client.message_handler.message_handler import validate_out_message
 from flwr.client.message_handler.task_handler import get_task_ins, validate_task_ins
 from flwr.common import GRPC_MAX_MESSAGE_LENGTH
-from flwr.common.constant import MISSING_EXTRA_REST
+from flwr.common.constant import (
+    MISSING_EXTRA_REST,
+    PING_BASE_MULTIPLIER,
+    PING_CALL_TIMEOUT,
+    PING_DEFAULT_INTERVAL,
+    PING_RANDOM_RANGE,
+)
 from flwr.common.logger import log
 from flwr.common.message import Message, Metadata
 from flwr.common.retry_invoker import RetryInvoker
 from flwr.common.serde import message_from_taskins, message_to_taskres
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     CreateNodeResponse,
     DeleteNodeRequest,
+    PingRequest,
+    PingResponse,
     PullTaskInsRequest,
     PullTaskInsResponse,
     PushTaskResRequest,
     PushTaskResResponse,
 )
 from flwr.proto.node_pb2 import Node  # pylint: disable=E0611
 from flwr.proto.task_pb2 import TaskIns  # pylint: disable=E0611
 
 try:
     import requests
 except ModuleNotFoundError:
     sys.exit(MISSING_EXTRA_REST)
 
 
-KEY_NODE = "node"
-KEY_METADATA = "in_message_metadata"
-
-
 PATH_CREATE_NODE: str = "api/v0/fleet/create-node"
 PATH_DELETE_NODE: str = "api/v0/fleet/delete-node"
 PATH_PULL_TASK_INS: str = "api/v0/fleet/pull-task-ins"
 PATH_PUSH_TASK_RES: str = "api/v0/fleet/push-task-res"
+PATH_PING: str = "api/v0/fleet/ping"
 
 
 @contextmanager
-# pylint: disable-next=too-many-statements
-def http_request_response(
+def http_request_response(  # pylint: disable=R0914, R0915
     server_address: str,
     insecure: bool,  # pylint: disable=unused-argument
     retry_invoker: RetryInvoker,
     max_message_length: int = GRPC_MAX_MESSAGE_LENGTH,  # pylint: disable=W0613
     root_certificates: Optional[
         Union[bytes, str]
     ] = None,  # pylint: disable=unused-argument
@@ -123,24 +130,79 @@
     elif isinstance(root_certificates, bytes):
         log(
             ERROR,
             "For the REST API, the root certificates "
             "must be provided as a string path to the client.",
         )
 
-    # Necessary state to validate messages to be sent
-    state: Dict[str, Optional[Metadata]] = {KEY_METADATA: None}
-
-    # Enable create_node and delete_node to store node
-    node_store: Dict[str, Optional[Node]] = {KEY_NODE: None}
+    # Shared variables for inner functions
+    metadata: Optional[Metadata] = None
+    node: Optional[Node] = None
+    ping_thread: Optional[threading.Thread] = None
+    ping_stop_event = threading.Event()
 
     ###########################################################################
-    # receive/send functions
+    # ping/create_node/delete_node/receive/send functions
     ###########################################################################
 
+    def ping() -> None:
+        # Get Node
+        if node is None:
+            log(ERROR, "Node instance missing")
+            return
+
+        # Construct the ping request
+        req = PingRequest(node=node, ping_interval=PING_DEFAULT_INTERVAL)
+        req_bytes: bytes = req.SerializeToString()
+
+        # Send the request
+        res = requests.post(
+            url=f"{base_url}/{PATH_PING}",
+            headers={
+                "Accept": "application/protobuf",
+                "Content-Type": "application/protobuf",
+            },
+            data=req_bytes,
+            verify=verify,
+            timeout=PING_CALL_TIMEOUT,
+        )
+
+        # Check status code and headers
+        if res.status_code != 200:
+            return
+        if "content-type" not in res.headers:
+            log(
+                WARN,
+                "[Node] POST /%s: missing header `Content-Type`",
+                PATH_PULL_TASK_INS,
+            )
+            return
+        if res.headers["content-type"] != "application/protobuf":
+            log(
+                WARN,
+                "[Node] POST /%s: header `Content-Type` has wrong value",
+                PATH_PULL_TASK_INS,
+            )
+            return
+
+        # Deserialize ProtoBuf from bytes
+        ping_res = PingResponse()
+        ping_res.ParseFromString(res.content)
+
+        # Check if success
+        if not ping_res.success:
+            raise RuntimeError("Ping failed unexpectedly.")
+
+        # Wait
+        rd = random.uniform(*PING_RANDOM_RANGE)
+        next_interval: float = PING_DEFAULT_INTERVAL - PING_CALL_TIMEOUT
+        next_interval *= PING_BASE_MULTIPLIER + rd
+        if not ping_stop_event.is_set():
+            ping_stop_event.wait(next_interval)
+
     def create_node() -> None:
         """Set create_node."""
         create_node_req_proto = CreateNodeRequest()
         create_node_req_bytes: bytes = create_node_req_proto.SerializeToString()
 
         res = retry_invoker.invoke(
             requests.post,
@@ -171,23 +233,33 @@
                 PATH_PULL_TASK_INS,
             )
             return
 
         # Deserialize ProtoBuf from bytes
         create_node_response_proto = CreateNodeResponse()
         create_node_response_proto.ParseFromString(res.content)
-        # pylint: disable-next=no-member
-        node_store[KEY_NODE] = create_node_response_proto.node
+
+        # Remember the node and the ping-loop thread
+        nonlocal node, ping_thread
+        node = create_node_response_proto.node
+        ping_thread = start_ping_loop(ping, ping_stop_event)
 
     def delete_node() -> None:
         """Set delete_node."""
-        if node_store[KEY_NODE] is None:
+        nonlocal node
+        if node is None:
             log(ERROR, "Node instance missing")
             return
-        node: Node = cast(Node, node_store[KEY_NODE])
+
+        # Stop the ping-loop thread
+        ping_stop_event.set()
+        if ping_thread is not None:
+            ping_thread.join()
+
+        # Send DeleteNode request
         delete_node_req_proto = DeleteNodeRequest(node=node)
         delete_node_req_req_bytes: bytes = delete_node_req_proto.SerializeToString()
         res = retry_invoker.invoke(
             requests.post,
             url=f"{base_url}/{PATH_DELETE_NODE}",
             headers={
                 "Accept": "application/protobuf",
@@ -211,21 +283,23 @@
         if res.headers["content-type"] != "application/protobuf":
             log(
                 WARN,
                 "[Node] POST /%s: header `Content-Type` has wrong value",
                 PATH_PULL_TASK_INS,
             )
 
+        # Cleanup
+        node = None
+
     def receive() -> Optional[Message]:
         """Receive next task from server."""
         # Get Node
-        if node_store[KEY_NODE] is None:
+        if node is None:
             log(ERROR, "Node instance missing")
             return None
-        node: Node = cast(Node, node_store[KEY_NODE])
 
         # Request instructions (task) from server
         pull_task_ins_req_proto = PullTaskInsRequest(node=node)
         pull_task_ins_req_bytes: bytes = pull_task_ins_req_proto.SerializeToString()
 
         # Request instructions (task) from server
         res = retry_invoker.invoke(
@@ -269,37 +343,37 @@
         if task_ins is not None and not (
             task_ins.task.consumer.node_id == node.node_id
             and validate_task_ins(task_ins)
         ):
             task_ins = None
 
         # Return the Message if available
+        nonlocal metadata
         message = None
-        state[KEY_METADATA] = None
         if task_ins is not None:
             message = message_from_taskins(task_ins)
-            state[KEY_METADATA] = copy(message.metadata)
+            metadata = copy(message.metadata)
             log(INFO, "[Node] POST /%s: success", PATH_PULL_TASK_INS)
         return message
 
     def send(message: Message) -> None:
         """Send task result back to server."""
         # Get Node
-        if node_store[KEY_NODE] is None:
+        if node is None:
             log(ERROR, "Node instance missing")
             return
 
         # Get incoming message
-        in_metadata = state[KEY_METADATA]
-        if in_metadata is None:
+        nonlocal metadata
+        if metadata is None:
             log(ERROR, "No current message")
             return
 
         # Validate out message
-        if not validate_out_message(message, in_metadata):
+        if not validate_out_message(message, metadata):
             log(ERROR, "Invalid out message")
             return
 
         # Construct TaskRes
         task_res = message_to_taskres(message)
 
         # Serialize ProtoBuf to bytes
@@ -317,15 +391,15 @@
                 "Content-Type": "application/protobuf",
             },
             data=push_task_res_request_bytes,
             verify=verify,
             timeout=None,
         )
 
-        state[KEY_METADATA] = None
+        metadata = None
 
         # Check status code and headers
         if res.status_code != 200:
             return
         if "content-type" not in res.headers:
             log(
                 WARN,
```

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/client/typing.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/client/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/address.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/address.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/constant.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/constant.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,20 @@
 TRANSPORT_TYPES = [
     TRANSPORT_TYPE_GRPC_BIDI,
     TRANSPORT_TYPE_GRPC_RERE,
     TRANSPORT_TYPE_REST,
     TRANSPORT_TYPE_VCE,
 ]
 
+# Constants for ping
+PING_DEFAULT_INTERVAL = 30
+PING_CALL_TIMEOUT = 5
+PING_BASE_MULTIPLIER = 0.8
+PING_RANDOM_RANGE = (-0.1, 0.1)
+
 
 class MessageType:
     """Message type."""
 
     TRAIN = "train"
     EVALUATE = "evaluate"
     QUERY = "query"
```

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/context.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/date.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/date.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/differential_privacy.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/differential_privacy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/differential_privacy_constants.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/differential_privacy_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/dp.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/dp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/exit_handlers.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/exit_handlers.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/grpc.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/logger.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -160,21 +160,21 @@
         FLOWER_LOGGER.addHandler(http_handler)
 
 
 logger = logging.getLogger(LOGGER_NAME)  # pylint: disable=invalid-name
 log = logger.log  # pylint: disable=invalid-name
 
 
-def warn_experimental_feature(name: str) -> None:
-    """Warn the user when they use an experimental feature."""
+def warn_preview_feature(name: str) -> None:
+    """Warn the user when they use a preview feature."""
     log(
         WARN,
-        """EXPERIMENTAL FEATURE: %s
+        """PREVIEW FEATURE: %s
 
-            This is an experimental feature. It could change significantly or be removed
+            This is a preview feature. It could change significantly or be removed
             entirely in future versions of Flower.
         """,
         name,
     )
 
 
 def warn_deprecated_feature(name: str) -> None:
```

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/message.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/message.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/object_ref.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/object_ref.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/parameter.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/parameter.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/pyproject.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/pyproject.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/configsrecord.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/configsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/conversion_utils.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/metricsrecord.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/metricsrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/parametersrecord.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/parametersrecord.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/recordset.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/recordset.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/record/typeddict.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/record/typeddict.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/recordset_compat.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/recordset_compat.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/retry_invoker.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/retry_invoker.py`

 * *Files 8% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 # pylint: disable-next=too-many-instance-attributes
 class RetryInvoker:
     """Wrapper class for retry (with backoff) triggered by exceptions.
 
     Parameters
     ----------
-    wait_factory: Callable[[], Generator[float, None, None]]
+    wait_gen_factory: Callable[[], Generator[float, None, None]]
         A generator yielding successive wait times in seconds. If the generator
         is finite, the giveup event will be triggered when the generator raises
         `StopIteration`.
     recoverable_exceptions: Union[Type[Exception], Tuple[Type[Exception]]]
         An exception type (or tuple of types) that triggers backoff.
     max_tries: Optional[int]
         The maximum number of attempts to make before giving up. Once exhausted,
@@ -125,27 +125,34 @@
         A callable to be executed in the event of success. The parameter is a
         data class object detailing the invocation.
     on_backoff: Optional[Callable[[RetryState], None]] (default: None)
         A callable to be executed in the event of a backoff. The parameter is a
         data class object detailing the invocation.
     on_giveup: Optional[Callable[[RetryState], None]] (default: None)
         A callable to be executed in the event that `max_tries` or `max_time` is
-        exceeded, `should_giveup` returns True, or `wait_factory()` generator raises
+        exceeded, `should_giveup` returns True, or `wait_gen_factory()` generator raises
         `StopInteration`. The parameter is a data class object detailing the
         invocation.
     jitter: Optional[Callable[[float], float]] (default: full_jitter)
-        A function of the value yielded by `wait_factory()` returning the actual time
-        to wait. This function helps distribute wait times stochastically to avoid
+        A function of the value yielded by `wait_gen_factory()` returning the actual
+        time to wait. This function helps distribute wait times stochastically to avoid
         timing collisions across concurrent clients. Wait times are jittered by
         default using the `full_jitter` function. To disable jittering, pass
         `jitter=None`.
     should_giveup: Optional[Callable[[Exception], bool]] (default: None)
         A function accepting an exception instance, returning whether or not
         to give up prematurely before other give-up conditions are evaluated.
         If set to None, the strategy is to never give up prematurely.
+    wait_function: Optional[Callable[[float], None]] (default: None)
+        A function that defines how to wait between retry attempts. It accepts
+        one argument, the wait time in seconds, allowing the use of various waiting
+        mechanisms (e.g., asynchronous waits or event-based synchronization) suitable
+        for different execution environments. If set to `None`, the `wait_function`
+        defaults to `time.sleep`, which is ideal for synchronous operations. Custom
+        functions should manage execution flow to prevent blocking or interference.
 
     Examples
     --------
     Initialize a `RetryInvoker` with exponential backoff and invoke a function:
 
     >>> invoker = RetryInvoker(
     ...     exponential,  # Or use `lambda: exponential(3, 2)` to pass arguments
@@ -155,34 +162,38 @@
     ... )
     >>> invoker.invoke(my_func, arg1, arg2, kw1=kwarg1)
     """
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
-        wait_factory: Callable[[], Generator[float, None, None]],
+        wait_gen_factory: Callable[[], Generator[float, None, None]],
         recoverable_exceptions: Union[Type[Exception], Tuple[Type[Exception], ...]],
         max_tries: Optional[int],
         max_time: Optional[float],
         *,
         on_success: Optional[Callable[[RetryState], None]] = None,
         on_backoff: Optional[Callable[[RetryState], None]] = None,
         on_giveup: Optional[Callable[[RetryState], None]] = None,
         jitter: Optional[Callable[[float], float]] = full_jitter,
         should_giveup: Optional[Callable[[Exception], bool]] = None,
+        wait_function: Optional[Callable[[float], None]] = None,
     ) -> None:
-        self.wait_factory = wait_factory
+        self.wait_gen_factory = wait_gen_factory
         self.recoverable_exceptions = recoverable_exceptions
         self.max_tries = max_tries
         self.max_time = max_time
         self.on_success = on_success
         self.on_backoff = on_backoff
         self.on_giveup = on_giveup
         self.jitter = jitter
         self.should_giveup = should_giveup
+        if wait_function is None:
+            wait_function = time.sleep
+        self.wait_function = wait_function
 
     # pylint: disable-next=too-many-locals
     def invoke(
         self,
         target: Callable[..., Any],
         *args: Any,
         **kwargs: Any,
@@ -208,40 +219,40 @@
         -------
         Any
             The result of the given callable invocation.
 
         Raises
         ------
         Exception
-            If the number of tries exceeds `max_tries`, if the total time
-            exceeds `max_time`, if `wait_factory()` generator raises `StopInteration`,
+            If the number of tries exceeds `max_tries`, if the total time exceeds
+            `max_time`, if `wait_gen_factory()` generator raises `StopInteration`,
             or if the `should_giveup` returns True for a raised exception.
 
         Notes
         -----
-        The time between retries is determined by the provided `wait_factory()`
+        The time between retries is determined by the provided `wait_gen_factory()`
         generator and can optionally be jittered using the `jitter` function.
         The recoverable exceptions that trigger a retry, as well as conditions to
         stop retries, are also determined by the class's initialization parameters.
         """
 
         def try_call_event_handler(
             handler: Optional[Callable[[RetryState], None]]
         ) -> None:
             if handler is not None:
                 handler(cast(RetryState, ref_state[0]))
 
         try_cnt = 0
-        wait_generator = self.wait_factory()
-        start = time.time()
+        wait_generator = self.wait_gen_factory()
+        start = time.monotonic()
         ref_state: List[Optional[RetryState]] = [None]
 
         while True:
             try_cnt += 1
-            elapsed_time = time.time() - start
+            elapsed_time = time.monotonic() - start
             state = RetryState(
                 target=target,
                 args=args,
                 kwargs=kwargs,
                 tries=try_cnt,
                 elapsed_time=elapsed_time,
             )
@@ -278,12 +289,12 @@
                     try_call_event_handler(self.on_giveup)
                     raise err from None
 
                 # Trigger backoff event
                 try_call_event_handler(self.on_backoff)
 
                 # Sleep
-                time.sleep(wait_time)
+                self.wait_function(state.actual_wait)
             else:
                 # Trigger success event
                 try_call_event_handler(self.on_success)
                 return ret
```

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/crypto/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/crypto/shamir.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/crypto/shamir.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/crypto/symmetric_encryption.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/ndarrays_arithmetic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/quantization.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/quantization.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/secaggplus_constants.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/secaggplus_constants.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/secure_aggregation/secaggplus_utils.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/secure_aggregation/secaggplus_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/serde.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/serde.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/telemetry.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/telemetry.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/typing.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/common/version.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/common/version.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/driver_pb2.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/driver_pb2.pyi` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/driver_pb2_grpc.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/driver_pb2_grpc.pyi` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/driver_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/error_pb2.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/error_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/error_pb2.pyi` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/error_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/fleet_pb2.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/fleet_pb2.pyi` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/fleet_pb2_grpc.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/fleet_pb2_grpc.pyi` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/fleet_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/node_pb2.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/node_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/node_pb2.pyi` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/recordset_pb2.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/recordset_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/recordset_pb2.pyi` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/recordset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/task_pb2.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/task_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/task_pb2.pyi` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/transport_pb2.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/transport_pb2.pyi` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/transport_pb2_grpc.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/proto/transport_pb2_grpc.pyi` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/app.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/client_manager.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/client_proxy.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/compat/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/compat/app.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/compat/app_utils.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/app_utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/compat/driver_client_proxy.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/driver_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/compat/legacy_context.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/compat/legacy_context.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/criterion.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/criterion.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/driver/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/driver/driver.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/driver/driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/driver/grpc_driver.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/driver/grpc_driver.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/history.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/history.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/run_serverapp.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/run_serverapp.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/server.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/server_app.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/server_app.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # ==============================================================================
 """Flower ServerApp."""
 
 
 from typing import Callable, Optional
 
 from flwr.common import Context, RecordSet
+from flwr.common.logger import warn_preview_feature
 from flwr.server.strategy import Strategy
 
 from .client_manager import ClientManager
 from .compat import start_driver
 from .driver import Driver
 from .server import Server
 from .server_config import ServerConfig
@@ -116,14 +117,16 @@
                     >>>
                     >>> @app.main()
                     >>> def main(driver: Driver, context: Context) -> None:
                     >>>    print("ServerApp running")
                     """,
                 )
 
+            warn_preview_feature("ServerApp-register-main-function")
+
             # Register provided function with the ServerApp object
             self._main = main_fn
 
             # Return provided function unmodified
             return main_fn
 
         return main_decorator
```

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/server_config.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/server_config.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/aggregate.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/bulyan.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/bulyan.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/dp_adaptive_clipping.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dp_adaptive_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/dp_fixed_clipping.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dp_fixed_clipping.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/dpfedavg_adaptive.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/dpfedavg_fixed.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fault_tolerant_fedavg.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedadagrad.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedadam.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedavg.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedavg_android.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedavgm.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedmedian.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedmedian.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedopt.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedprox.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedprox.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedtrimmedavg.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedtrimmedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedxgb_bagging.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedxgb_bagging.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedxgb_cyclic.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedxgb_cyclic.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedxgb_nn_avg.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedxgb_nn_avg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/fedyogi.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/krum.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/krum.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/qfedavg.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/strategy/strategy.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/driver/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/driver/driver_grpc.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/driver/driver_grpc.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/driver/driver_servicer.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/driver/driver_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_bidi/grpc_server.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/grpc_rere/fleet_servicer.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/message_handler/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/message_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/message_handler/message_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,16 @@
 
 
 def ping(
     request: PingRequest,  # pylint: disable=unused-argument
     state: State,  # pylint: disable=unused-argument
 ) -> PingResponse:
     """."""
-    return PingResponse(success=True)
+    res = state.acknowledge_ping(request.node.node_id, request.ping_interval)
+    return PingResponse(success=res)
 
 
 def pull_task_ins(request: PullTaskInsRequest, state: State) -> PullTaskInsResponse:
     """Pull TaskIns handler."""
     # Get node_id if client node is not anonymous
     node = request.node  # pylint: disable=no-member
     node_id: Optional[int] = None if node.anonymous else node.node_id
```

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/rest_rere/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/rest_rere/rest_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import sys
 
 from flwr.common.constant import MISSING_EXTRA_REST
 from flwr.proto.fleet_pb2 import (  # pylint: disable=E0611
     CreateNodeRequest,
     DeleteNodeRequest,
+    PingRequest,
     PullTaskInsRequest,
     PushTaskResRequest,
 )
 from flwr.server.superlink.fleet.message_handler import message_handler
 from flwr.server.superlink.state import State
 
 try:
@@ -148,19 +149,46 @@
     return Response(
         status_code=200,
         content=push_task_res_response_bytes,
         headers={"Content-Type": "application/protobuf"},
     )
 
 
+async def ping(request: Request) -> Response:
+    """Ping."""
+    _check_headers(request.headers)
+
+    # Get the request body as raw bytes
+    ping_request_bytes: bytes = await request.body()
+
+    # Deserialize ProtoBuf
+    ping_request_proto = PingRequest()
+    ping_request_proto.ParseFromString(ping_request_bytes)
+
+    # Get state from app
+    state: State = app.state.STATE_FACTORY.state()
+
+    # Handle message
+    ping_response_proto = message_handler.ping(request=ping_request_proto, state=state)
+
+    # Return serialized ProtoBuf
+    ping_response_bytes = ping_response_proto.SerializeToString()
+    return Response(
+        status_code=200,
+        content=ping_response_bytes,
+        headers={"Content-Type": "application/protobuf"},
+    )
+
+
 routes = [
     Route("/api/v0/fleet/create-node", create_node, methods=["POST"]),
     Route("/api/v0/fleet/delete-node", delete_node, methods=["POST"]),
     Route("/api/v0/fleet/pull-task-ins", pull_task_ins, methods=["POST"]),
     Route("/api/v0/fleet/push-task-res", push_task_res, methods=["POST"]),
+    Route("/api/v0/fleet/ping", ping, methods=["POST"]),
 ]
 
 app: Starlette = Starlette(
     debug=False,
     routes=routes,
 )
```

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/vce/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/vce/backend/backend.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/backend/backend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/backend/raybackend.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/fleet/vce/vce_api.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/fleet/vce/vce_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -219,14 +219,15 @@
         await asyncio.gather(*[w_t for w_t in worker_tasks if not w_t.done()])
 
         # Terminate backend
         await backend.terminate()
 
 
 # pylint: disable=too-many-arguments,unused-argument,too-many-locals,too-many-branches
+# pylint: disable=too-many-statements
 def start_vce(
     backend_name: str,
     backend_config_json_stream: str,
     app_dir: str,
     f_stop: asyncio.Event,
     client_app: Optional[ClientApp] = None,
     client_app_attr: Optional[str] = None,
@@ -337,11 +338,18 @@
                 nodes_mapping,
                 state_factory,
                 node_states,
                 f_stop,
             )
         )
     except LoadClientAppError as loadapp_ex:
+        f_stop_delay = 10
+        log(
+            ERROR,
+            "LoadClientAppError exception encountered. Terminating simulation in %is",
+            f_stop_delay,
+        )
+        time.sleep(f_stop_delay)
         f_stop.set()  # set termination event
         raise loadapp_ex
     except Exception as ex:
         raise ex
```

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/state/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/state/in_memory_state.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/in_memory_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/state/sqlite_state.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/sqlite_state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/state/state.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/state.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/superlink/state/state_factory.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/superlink/state/state_factory.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/typing.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/typing.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/utils/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/utils/tensorboard.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/utils/tensorboard.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/utils/validator.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/utils/validator.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/workflow/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/workflow/constant.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/constant.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/workflow/default_workflows.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/default_workflows.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/workflow/secure_aggregation/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/secure_aggregation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/secure_aggregation/secagg_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/server/workflow/secure_aggregation/secaggplus_workflow.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/app.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/app.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/ray_transport/__init__.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/ray_transport/ray_actor.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/ray_actor.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/ray_transport/ray_client_proxy.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/ray_transport/utils.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/ray_transport/utils.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/src/py/flwr/simulation/run_simulation.py` & `flwr_nightly-1.8.0.dev20240401/src/py/flwr/simulation/run_simulation.py`

 * *Files identical despite different names*

### Comparing `flwr_nightly-1.8.0.dev20240328/PKG-INFO` & `flwr_nightly-1.8.0.dev20240401/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flwr-nightly
-Version: 1.8.0.dev20240328
+Version: 1.8.0.dev20240401
 Summary: Flower: A Friendly Federated Learning Framework
 Home-page: https://flower.ai
 License: Apache-2.0
 Keywords: flower,fl,federated learning,federated analytics,federated evaluation,machine learning
 Author: The Flower Authors
 Author-email: hello@flower.ai
 Requires-Python: >=3.8,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flwr-nightly Version: 1.8.0.dev20240328 Summary:
+Metadata-Version: 2.1 Name: flwr-nightly Version: 1.8.0.dev20240401 Summary:
 Flower: A Friendly Federated Learning Framework Home-page: https://flower.ai
 License: Apache-2.0 Keywords: flower,fl,federated learning,federated
 analytics,federated evaluation,machine learning Author: The Flower Authors
 Author-email: hello@flower.ai Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Science/Research Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Operating System
```

