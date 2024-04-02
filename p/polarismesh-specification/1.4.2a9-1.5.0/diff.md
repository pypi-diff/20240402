# Comparing `tmp/polarismesh_specification-1.4.2a9.tar.gz` & `tmp/polarismesh_specification-1.5.0.tar.gz`

## Comparing `polarismesh_specification-1.4.2a9.tar` & `polarismesh_specification-1.5.0.tar`

### file list

```diff
@@ -1,78 +1,81 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
--rw-r--r--   0        0        0    14432 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
--rw-r--r--   0        0        0    25362 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
--rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
--rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
--rw-r--r--   0        0        0    13989 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
--rw-r--r--   0        0        0    13680 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
--rw-r--r--   0        0        0    22439 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
--rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/__init__.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/__init__.pyi
--rw-r--r--   0        0        0     9708 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/code_pb2.py
--rw-r--r--   0        0        0    12050 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/code_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/model_pb2.py
--rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/model_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
--rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/namespace_pb2.py
--rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/security/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/security/__init__.pyi
--rw-r--r--   0        0        0     9076 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/security/auth_pb2.py
--rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/__init__.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
--rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/contract_pb2.py
--rw-r--r--   0        0        0     3151 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/contract_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/contract_pb2_grpc.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
--rw-r--r--   0        0        0    17961 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
--rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
--rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
--rw-r--r--   0        0        0    13912 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
--rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
--rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
--rw-r--r--   0        0        0    15970 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
--rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
--rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/.gitignore
--rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/LICENSE.txt
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/README.md
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/pyproject.toml
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.2a9/PKG-INFO
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
+-rw-r--r--   0        0        0    14432 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
+-rw-r--r--   0        0        0    25362 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
+-rw-r--r--   0        0        0     5881 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
+-rw-r--r--   0        0        0    13989 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
+-rw-r--r--   0        0        0    13680 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
+-rw-r--r--   0        0        0    22439 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
+-rw-r--r--   0        0        0     3976 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/__init__.pyi
+-rw-r--r--   0        0        0     9708 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/code_pb2.py
+-rw-r--r--   0        0        0    12050 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/code_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/model_pb2.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
+-rw-r--r--   0        0        0     2828 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/namespace_pb2.py
+-rw-r--r--   0        0        0     3589 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/security/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/security/__init__.pyi
+-rw-r--r--   0        0        0     9076 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/security/auth_pb2.py
+-rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/__init__.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
+-rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
+-rw-r--r--   0        0        0     2238 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/contract_pb2.py
+-rw-r--r--   0        0        0     3739 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/contract_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/contract_pb2_grpc.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
+-rw-r--r--   0        0        0    17961 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
+-rw-r--r--   0        0        0     2935 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
+-rw-r--r--   0        0        0     2479 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
+-rw-r--r--   0        0        0     2494 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
+-rw-r--r--   0        0        0     8476 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
+-rw-r--r--   0        0        0    14272 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
+-rw-r--r--   0        0        0     7799 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
+-rw-r--r--   0        0        0    12323 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
+-rw-r--r--   0        0        0     4985 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/lane_pb2.py
+-rw-r--r--   0        0        0     6454 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/lane_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/lane_pb2_grpc.py
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
+-rw-r--r--   0        0        0    15970 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
+-rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/.gitignore
+-rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/LICENSE.txt
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/README.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 polarismesh_specification-1.5.0/PKG-INFO
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: config_file.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: config_file_response.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: grpc_config_api.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: circuitbreaker.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: fault_detector.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/code_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/code_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: code.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/code_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/model_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/model_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: model.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/model_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/namespace_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/namespace_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: namespace.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/security/auth_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/security/auth_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: auth.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/security/auth_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/security/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/client_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/client_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: client.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: configrelease.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/contract_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/contract_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: contract.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x63ontract.proto\x12\x02v1\"\xf0\x01\n\x0fServiceContract\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0f\n\x07service\x18\x04 \x01(\t\x12\x10\n\x08protocol\x18\x05 \x01(\t\x12\x0f\n\x07version\x18\x06 \x01(\t\x12\x10\n\x08revision\x18\x07 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x08 \x01(\t\x12+\n\ninterfaces\x18\t \x03(\x0b\x32\x17.v1.InterfaceDescriptor\x12\r\n\x05\x63time\x18\n \x01(\t\x12\r\n\x05mtime\x18\x0b \x01(\t\x12\x0e\n\x06status\x18\x0c \x01(\t\"\xed\x01\n\x13InterfaceDescriptor\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x04 \x01(\t\x12.\n\x06source\x18\x05 \x01(\x0e\x32\x1e.v1.InterfaceDescriptor.Source\x12\x10\n\x08revision\x18\x06 \x01(\t\x12\r\n\x05\x63time\x18\x07 \x01(\t\x12\r\n\x05mtime\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\"-\n\x06Source\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06Manual\x10\x01\x12\n\n\x06\x43lient\x10\x02\x42\x95\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x14ServiceContractProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0e\x63ontract.proto\x12\x02v1\"\xfe\x01\n\x0fServiceContract\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\x0f\n\x07service\x18\x04 \x01(\t\x12\x10\n\x08protocol\x18\x05 \x01(\t\x12\x0f\n\x07version\x18\x06 \x01(\t\x12\x10\n\x08revision\x18\x07 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x08 \x01(\t\x12+\n\ninterfaces\x18\t \x03(\x0b\x32\x17.v1.InterfaceDescriptor\x12\r\n\x05\x63time\x18\n \x01(\t\x12\r\n\x05mtime\x18\x0b \x01(\t\x12\x0e\n\x06status\x18\x0c \x01(\t\x12\x0c\n\x04type\x18\x0e \x01(\t\"\xc2\x02\n\x13InterfaceDescriptor\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06method\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x04 \x01(\t\x12.\n\x06source\x18\x05 \x01(\x0e\x32\x1e.v1.InterfaceDescriptor.Source\x12\x10\n\x08revision\x18\x06 \x01(\t\x12\r\n\x05\x63time\x18\x07 \x01(\t\x12\r\n\x05mtime\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\x12\x11\n\tnamespace\x18\n \x01(\t\x12\x0f\n\x07service\x18\x0b \x01(\t\x12\x10\n\x08protocol\x18\x0c \x01(\t\x12\x0f\n\x07version\x18\r \x01(\t\x12\x0c\n\x04type\x18\x0e \x01(\t\"-\n\x06Source\x12\x0b\n\x07UNKNOWN\x10\x00\x12\n\n\x06Manual\x10\x01\x12\n\n\x06\x43lient\x10\x02\x42\x95\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x14ServiceContractProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'contract_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageB\024ServiceContractProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
   _globals['_SERVICECONTRACT']._serialized_start=23
-  _globals['_SERVICECONTRACT']._serialized_end=263
-  _globals['_INTERFACEDESCRIPTOR']._serialized_start=266
-  _globals['_INTERFACEDESCRIPTOR']._serialized_end=503
-  _globals['_INTERFACEDESCRIPTOR_SOURCE']._serialized_start=458
-  _globals['_INTERFACEDESCRIPTOR_SOURCE']._serialized_end=503
+  _globals['_SERVICECONTRACT']._serialized_end=277
+  _globals['_INTERFACEDESCRIPTOR']._serialized_start=280
+  _globals['_INTERFACEDESCRIPTOR']._serialized_end=602
+  _globals['_INTERFACEDESCRIPTOR_SOURCE']._serialized_start=557
+  _globals['_INTERFACEDESCRIPTOR_SOURCE']._serialized_end=602
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/contract_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/contract_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -3,43 +3,45 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ServiceContract(_message.Message):
-    __slots__ = ("id", "name", "namespace", "service", "protocol", "version", "revision", "content", "interfaces", "ctime", "mtime", "status")
+    __slots__ = ("id", "name", "namespace", "service", "protocol", "version", "revision", "content", "interfaces", "ctime", "mtime", "status", "type")
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     SERVICE_FIELD_NUMBER: _ClassVar[int]
     PROTOCOL_FIELD_NUMBER: _ClassVar[int]
     VERSION_FIELD_NUMBER: _ClassVar[int]
     REVISION_FIELD_NUMBER: _ClassVar[int]
     CONTENT_FIELD_NUMBER: _ClassVar[int]
     INTERFACES_FIELD_NUMBER: _ClassVar[int]
     CTIME_FIELD_NUMBER: _ClassVar[int]
     MTIME_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
     id: str
     name: str
     namespace: str
     service: str
     protocol: str
     version: str
     revision: str
     content: str
     interfaces: _containers.RepeatedCompositeFieldContainer[InterfaceDescriptor]
     ctime: str
     mtime: str
     status: str
-    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., namespace: _Optional[str] = ..., service: _Optional[str] = ..., protocol: _Optional[str] = ..., version: _Optional[str] = ..., revision: _Optional[str] = ..., content: _Optional[str] = ..., interfaces: _Optional[_Iterable[_Union[InterfaceDescriptor, _Mapping]]] = ..., ctime: _Optional[str] = ..., mtime: _Optional[str] = ..., status: _Optional[str] = ...) -> None: ...
+    type: str
+    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., namespace: _Optional[str] = ..., service: _Optional[str] = ..., protocol: _Optional[str] = ..., version: _Optional[str] = ..., revision: _Optional[str] = ..., content: _Optional[str] = ..., interfaces: _Optional[_Iterable[_Union[InterfaceDescriptor, _Mapping]]] = ..., ctime: _Optional[str] = ..., mtime: _Optional[str] = ..., status: _Optional[str] = ..., type: _Optional[str] = ...) -> None: ...
 
 class InterfaceDescriptor(_message.Message):
-    __slots__ = ("id", "method", "path", "content", "source", "revision", "ctime", "mtime", "name")
+    __slots__ = ("id", "method", "path", "content", "source", "revision", "ctime", "mtime", "name", "namespace", "service", "protocol", "version", "type")
     class Source(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         UNKNOWN: _ClassVar[InterfaceDescriptor.Source]
         Manual: _ClassVar[InterfaceDescriptor.Source]
         Client: _ClassVar[InterfaceDescriptor.Source]
     UNKNOWN: InterfaceDescriptor.Source
     Manual: InterfaceDescriptor.Source
@@ -49,17 +51,27 @@
     PATH_FIELD_NUMBER: _ClassVar[int]
     CONTENT_FIELD_NUMBER: _ClassVar[int]
     SOURCE_FIELD_NUMBER: _ClassVar[int]
     REVISION_FIELD_NUMBER: _ClassVar[int]
     CTIME_FIELD_NUMBER: _ClassVar[int]
     MTIME_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    NAMESPACE_FIELD_NUMBER: _ClassVar[int]
+    SERVICE_FIELD_NUMBER: _ClassVar[int]
+    PROTOCOL_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
     id: str
     method: str
     path: str
     content: str
     source: InterfaceDescriptor.Source
     revision: str
     ctime: str
     mtime: str
     name: str
-    def __init__(self, id: _Optional[str] = ..., method: _Optional[str] = ..., path: _Optional[str] = ..., content: _Optional[str] = ..., source: _Optional[_Union[InterfaceDescriptor.Source, str]] = ..., revision: _Optional[str] = ..., ctime: _Optional[str] = ..., mtime: _Optional[str] = ..., name: _Optional[str] = ...) -> None: ...
+    namespace: str
+    service: str
+    protocol: str
+    version: str
+    type: str
+    def __init__(self, id: _Optional[str] = ..., method: _Optional[str] = ..., path: _Optional[str] = ..., content: _Optional[str] = ..., source: _Optional[_Union[InterfaceDescriptor.Source, str]] = ..., revision: _Optional[str] = ..., ctime: _Optional[str] = ..., mtime: _Optional[str] = ..., name: _Optional[str] = ..., namespace: _Optional[str] = ..., service: _Optional[str] = ..., protocol: _Optional[str] = ..., version: _Optional[str] = ..., type: _Optional[str] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: grpcapi.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: heartbeat.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/request_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/request_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: request.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from ..service_manage import service_pb2 as service__pb2
 from ..service_manage import contract_pb2 as contract__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rrequest.proto\x12\x02v1\x1a\rservice.proto\x1a\x0e\x63ontract.proto\"-\n\x0e\x44iscoverFilter\x12\x1b\n\x13OnlyHealthyInstance\x18\x01 \x01(\x08\"\xba\x02\n\x0f\x44iscoverRequest\x12\x35\n\x04type\x18\x01 \x01(\x0e\x32\'.v1.DiscoverRequest.DiscoverRequestType\x12\x1c\n\x07service\x18\x02 \x01(\x0b\x32\x0b.v1.Service\x12\"\n\x06\x46ilter\x18\x1e \x01(\x0b\x32\x12.v1.DiscoverFilter\"\xa7\x01\n\x13\x44iscoverRequestType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08INSTANCE\x10\x01\x12\x0b\n\x07\x43LUSTER\x10\x02\x12\x0b\n\x07ROUTING\x10\x03\x12\x0e\n\nRATE_LIMIT\x10\x04\x12\x13\n\x0f\x43IRCUIT_BREAKER\x10\x05\x12\x0c\n\x08SERVICES\x10\x06\x12\x0e\n\nNAMESPACES\x10\x0c\x12\x12\n\x0e\x46\x41ULT_DETECTOR\x10\r\"\x04\x08\x07\x10\x0bJ\x04\x08\x03\x10\x05\x42\x8d\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x0cRequestProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\rrequest.proto\x12\x02v1\x1a\rservice.proto\x1a\x0e\x63ontract.proto\"-\n\x0e\x44iscoverFilter\x12\x1b\n\x13OnlyHealthyInstance\x18\x01 \x01(\x08\"\xca\x02\n\x0f\x44iscoverRequest\x12\x35\n\x04type\x18\x01 \x01(\x0e\x32\'.v1.DiscoverRequest.DiscoverRequestType\x12\x1c\n\x07service\x18\x02 \x01(\x0b\x32\x0b.v1.Service\x12\"\n\x06\x46ilter\x18\x1e \x01(\x0b\x32\x12.v1.DiscoverFilter\"\xb7\x01\n\x13\x44iscoverRequestType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08INSTANCE\x10\x01\x12\x0b\n\x07\x43LUSTER\x10\x02\x12\x0b\n\x07ROUTING\x10\x03\x12\x0e\n\nRATE_LIMIT\x10\x04\x12\x13\n\x0f\x43IRCUIT_BREAKER\x10\x05\x12\x0c\n\x08SERVICES\x10\x06\x12\x0e\n\nNAMESPACES\x10\x0c\x12\x12\n\x0e\x46\x41ULT_DETECTOR\x10\r\x12\x08\n\x04LANE\x10\x64\"\x04\x08\x07\x10\x0b\"\x04\x08\x0e\x10\x63J\x04\x08\x03\x10\x05\x42\x8d\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\x0cRequestProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'request_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageB\014RequestProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
   _globals['_DISCOVERFILTER']._serialized_start=52
   _globals['_DISCOVERFILTER']._serialized_end=97
   _globals['_DISCOVERREQUEST']._serialized_start=100
-  _globals['_DISCOVERREQUEST']._serialized_end=414
+  _globals['_DISCOVERREQUEST']._serialized_end=430
   _globals['_DISCOVERREQUEST_DISCOVERREQUESTTYPE']._serialized_start=241
-  _globals['_DISCOVERREQUEST_DISCOVERREQUESTTYPE']._serialized_end=408
+  _globals['_DISCOVERREQUEST_DISCOVERREQUESTTYPE']._serialized_end=424
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -22,23 +22,25 @@
         CLUSTER: _ClassVar[DiscoverRequest.DiscoverRequestType]
         ROUTING: _ClassVar[DiscoverRequest.DiscoverRequestType]
         RATE_LIMIT: _ClassVar[DiscoverRequest.DiscoverRequestType]
         CIRCUIT_BREAKER: _ClassVar[DiscoverRequest.DiscoverRequestType]
         SERVICES: _ClassVar[DiscoverRequest.DiscoverRequestType]
         NAMESPACES: _ClassVar[DiscoverRequest.DiscoverRequestType]
         FAULT_DETECTOR: _ClassVar[DiscoverRequest.DiscoverRequestType]
+        LANE: _ClassVar[DiscoverRequest.DiscoverRequestType]
     UNKNOWN: DiscoverRequest.DiscoverRequestType
     INSTANCE: DiscoverRequest.DiscoverRequestType
     CLUSTER: DiscoverRequest.DiscoverRequestType
     ROUTING: DiscoverRequest.DiscoverRequestType
     RATE_LIMIT: DiscoverRequest.DiscoverRequestType
     CIRCUIT_BREAKER: DiscoverRequest.DiscoverRequestType
     SERVICES: DiscoverRequest.DiscoverRequestType
     NAMESPACES: DiscoverRequest.DiscoverRequestType
     FAULT_DETECTOR: DiscoverRequest.DiscoverRequestType
+    LANE: DiscoverRequest.DiscoverRequestType
     TYPE_FIELD_NUMBER: _ClassVar[int]
     SERVICE_FIELD_NUMBER: _ClassVar[int]
     FILTER_FIELD_NUMBER: _ClassVar[int]
     type: DiscoverRequest.DiscoverRequestType
     service: _service_pb2.Service
     Filter: DiscoverFilter
     def __init__(self, type: _Optional[_Union[DiscoverRequest.DiscoverRequestType, str]] = ..., service: _Optional[_Union[_service_pb2.Service, _Mapping]] = ..., Filter: _Optional[_Union[DiscoverFilter, _Mapping]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/response_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/response_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: response.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
@@ -21,40 +21,41 @@
 from ..fault_tolerance import circuitbreaker_pb2 as circuitbreaker__pb2
 from ..model import model_pb2 as model__pb2
 from ..service_manage import client_pb2 as client__pb2
 from ..service_manage import configrelease_pb2 as configrelease__pb2
 from ..fault_tolerance import fault_detector_pb2 as fault__detector__pb2
 from ..security import auth_pb2 as auth__pb2
 from ..service_manage import contract_pb2 as contract__pb2
+from ..traffic_manage import lane_pb2 as lane__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eresponse.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x19google/protobuf/any.proto\x1a\x0fnamespace.proto\x1a\rservice.proto\x1a\rrouting.proto\x1a\x0fratelimit.proto\x1a\x14\x63ircuitbreaker.proto\x1a\x0bmodel.proto\x1a\x0c\x63lient.proto\x1a\x13\x63onfigrelease.proto\x1a\x14\x66\x61ult_detector.proto\x1a\nauth.proto\x1a\x0e\x63ontract.proto\"\xfd\x06\n\x08Response\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1a\n\x06\x63lient\x18\x03 \x01(\x0b\x32\n.v1.Client\x12 \n\tnamespace\x18\x04 \x01(\x0b\x32\r.v1.Namespace\x12\x1c\n\x07service\x18\x05 \x01(\x0b\x32\x0b.v1.Service\x12\x1e\n\x08instance\x18\x06 \x01(\x0b\x32\x0c.v1.Instance\x12\x1c\n\x07routing\x18\x07 \x01(\x0b\x32\x0b.v1.Routing\x12\x1f\n\x05\x61lias\x18\x08 \x01(\x0b\x32\x10.v1.ServiceAlias\x12\x1b\n\trateLimit\x18\t \x01(\x0b\x32\x08.v1.Rule\x12*\n\x0e\x63ircuitBreaker\x18\n \x01(\x0b\x32\x12.v1.CircuitBreaker\x12(\n\rconfigRelease\x18\x0b \x01(\x0b\x32\x11.v1.ConfigRelease\x12\x16\n\x04user\x18\x13 \x01(\x0b\x32\x08.v1.User\x12 \n\tuserGroup\x18\x14 \x01(\x0b\x32\r.v1.UserGroup\x12&\n\x0c\x61uthStrategy\x18\x15 \x01(\x0b\x32\x10.v1.AuthStrategy\x12\'\n\x08relation\x18\x16 \x01(\x0b\x32\x15.v1.UserGroupRelation\x12(\n\rloginResponse\x18\x17 \x01(\x0b\x32\x11.v1.LoginResponse\x12\x32\n\x12modifyAuthStrategy\x18\x18 \x01(\x0b\x32\x16.v1.ModifyAuthStrategy\x12,\n\x0fmodifyUserGroup\x18\x19 \x01(\x0b\x32\x13.v1.ModifyUserGroup\x12(\n\tresources\x18\x1a \x01(\x0b\x32\x15.v1.StrategyResources\x12&\n\x0coptionSwitch\x18\x1b \x01(\x0b\x32\x10.v1.OptionSwitch\x12*\n\x0einstanceLabels\x18\x1c \x01(\x0b\x32\x12.v1.InstanceLabels\x12\"\n\x04\x64\x61ta\x18\x1d \x01(\x0b\x32\x14.google.protobuf.Any\x12,\n\x0fserviceContract\x18\x1e \x01(\x0b\x32\x13.v1.ServiceContractJ\x04\x08\x0c\x10\x13\"\xb9\x01\n\x12\x42\x61tchWriteResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04size\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x1f\n\tresponses\x18\x04 \x03(\x0b\x32\x0c.v1.Response\"\x87\x05\n\x12\x42\x61tchQueryResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x61mount\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04size\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12!\n\nnamespaces\x18\x05 \x03(\x0b\x32\r.v1.Namespace\x12\x1d\n\x08services\x18\x06 \x03(\x0b\x32\x0b.v1.Service\x12\x1f\n\tinstances\x18\x07 \x03(\x0b\x32\x0c.v1.Instance\x12\x1d\n\x08routings\x18\x08 \x03(\x0b\x32\x0b.v1.Routing\x12!\n\x07\x61liases\x18\t \x03(\x0b\x32\x10.v1.ServiceAlias\x12\x1c\n\nrateLimits\x18\n \x03(\x0b\x32\x08.v1.Rule\x12\x31\n\x12\x63onfigWithServices\x18\x0b \x03(\x0b\x32\x15.v1.ConfigWithService\x12\x17\n\x05users\x18\x12 \x03(\x0b\x32\x08.v1.User\x12!\n\nuserGroups\x18\x13 \x03(\x0b\x32\r.v1.UserGroup\x12(\n\x0e\x61uthStrategies\x18\x14 \x03(\x0b\x32\x10.v1.AuthStrategy\x12\x1b\n\x07\x63lients\x18\x15 \x03(\x0b\x32\n.v1.Client\x12\"\n\x04\x64\x61ta\x18\x16 \x03(\x0b\x32\x14.google.protobuf.Any\x12\x1c\n\x07summary\x18\x17 \x01(\x0b\x32\x0b.v1.SummaryJ\x04\x08\x0c\x10\x12\"\xc4\x05\n\x10\x44iscoverResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x37\n\x04type\x18\x03 \x01(\x0e\x32).v1.DiscoverResponse.DiscoverResponseType\x12\x1c\n\x07service\x18\x04 \x01(\x0b\x32\x0b.v1.Service\x12\x1f\n\tinstances\x18\x05 \x03(\x0b\x32\x0c.v1.Instance\x12\x1c\n\x07routing\x18\x06 \x01(\x0b\x32\x0b.v1.Routing\x12 \n\trateLimit\x18\x07 \x01(\x0b\x32\r.v1.RateLimit\x12*\n\x0e\x63ircuitBreaker\x18\x08 \x01(\x0b\x32\x12.v1.CircuitBreaker\x12\x1d\n\x08services\x18\t \x03(\x0b\x32\x0b.v1.Service\x12!\n\nnamespaces\x18\n \x03(\x0b\x32\r.v1.Namespace\x12(\n\rfaultDetector\x18\x0b \x01(\x0b\x32\x11.v1.FaultDetector\x12\x1d\n\x08\x61liasFor\x18\x15 \x01(\x0b\x32\x0b.v1.Service\"\xe2\x01\n\x14\x44iscoverResponseType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08INSTANCE\x10\x01\x12\x0b\n\x07\x43LUSTER\x10\x02\x12\x0b\n\x07ROUTING\x10\x03\x12\x0e\n\nRATE_LIMIT\x10\x04\x12\x13\n\x0f\x43IRCUIT_BREAKER\x10\x05\x12\x0c\n\x08SERVICES\x10\x06\x12\x0e\n\nNAMESPACES\x10\x0c\x12\x12\n\x0e\x46\x41ULT_DETECTOR\x10\r\"\x04\x08\x07\x10\x0b*\x04MESH*\x0bMESH_CONFIG*\x0e\x46LUX_DBREFRESH*\x08\x46LUX_SDK*\x0b\x46LUX_SERVERJ\x04\x08\x0c\x10\x15\"n\n\x0cOptionSwitch\x12.\n\x07options\x18\x01 \x03(\x0b\x32\x1d.v1.OptionSwitch.OptionsEntry\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\x0eInstanceLabels\x12.\n\x06labels\x18\x01 \x03(\x0b\x32\x1e.v1.InstanceLabels.LabelsEntry\x1a=\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.v1.StringList:\x02\x38\x01\x42\x8e\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\rResponseProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eresponse.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x19google/protobuf/any.proto\x1a\x0fnamespace.proto\x1a\rservice.proto\x1a\rrouting.proto\x1a\x0fratelimit.proto\x1a\x14\x63ircuitbreaker.proto\x1a\x0bmodel.proto\x1a\x0c\x63lient.proto\x1a\x13\x63onfigrelease.proto\x1a\x14\x66\x61ult_detector.proto\x1a\nauth.proto\x1a\x0e\x63ontract.proto\x1a\nlane.proto\"\xfd\x06\n\x08Response\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1a\n\x06\x63lient\x18\x03 \x01(\x0b\x32\n.v1.Client\x12 \n\tnamespace\x18\x04 \x01(\x0b\x32\r.v1.Namespace\x12\x1c\n\x07service\x18\x05 \x01(\x0b\x32\x0b.v1.Service\x12\x1e\n\x08instance\x18\x06 \x01(\x0b\x32\x0c.v1.Instance\x12\x1c\n\x07routing\x18\x07 \x01(\x0b\x32\x0b.v1.Routing\x12\x1f\n\x05\x61lias\x18\x08 \x01(\x0b\x32\x10.v1.ServiceAlias\x12\x1b\n\trateLimit\x18\t \x01(\x0b\x32\x08.v1.Rule\x12*\n\x0e\x63ircuitBreaker\x18\n \x01(\x0b\x32\x12.v1.CircuitBreaker\x12(\n\rconfigRelease\x18\x0b \x01(\x0b\x32\x11.v1.ConfigRelease\x12\x16\n\x04user\x18\x13 \x01(\x0b\x32\x08.v1.User\x12 \n\tuserGroup\x18\x14 \x01(\x0b\x32\r.v1.UserGroup\x12&\n\x0c\x61uthStrategy\x18\x15 \x01(\x0b\x32\x10.v1.AuthStrategy\x12\'\n\x08relation\x18\x16 \x01(\x0b\x32\x15.v1.UserGroupRelation\x12(\n\rloginResponse\x18\x17 \x01(\x0b\x32\x11.v1.LoginResponse\x12\x32\n\x12modifyAuthStrategy\x18\x18 \x01(\x0b\x32\x16.v1.ModifyAuthStrategy\x12,\n\x0fmodifyUserGroup\x18\x19 \x01(\x0b\x32\x13.v1.ModifyUserGroup\x12(\n\tresources\x18\x1a \x01(\x0b\x32\x15.v1.StrategyResources\x12&\n\x0coptionSwitch\x18\x1b \x01(\x0b\x32\x10.v1.OptionSwitch\x12*\n\x0einstanceLabels\x18\x1c \x01(\x0b\x32\x12.v1.InstanceLabels\x12\"\n\x04\x64\x61ta\x18\x1d \x01(\x0b\x32\x14.google.protobuf.Any\x12,\n\x0fserviceContract\x18\x1e \x01(\x0b\x32\x13.v1.ServiceContractJ\x04\x08\x0c\x10\x13\"\xb9\x01\n\x12\x42\x61tchWriteResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04size\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x1f\n\tresponses\x18\x04 \x03(\x0b\x32\x0c.v1.Response\"\x87\x05\n\x12\x42\x61tchQueryResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x61mount\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04size\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12!\n\nnamespaces\x18\x05 \x03(\x0b\x32\r.v1.Namespace\x12\x1d\n\x08services\x18\x06 \x03(\x0b\x32\x0b.v1.Service\x12\x1f\n\tinstances\x18\x07 \x03(\x0b\x32\x0c.v1.Instance\x12\x1d\n\x08routings\x18\x08 \x03(\x0b\x32\x0b.v1.Routing\x12!\n\x07\x61liases\x18\t \x03(\x0b\x32\x10.v1.ServiceAlias\x12\x1c\n\nrateLimits\x18\n \x03(\x0b\x32\x08.v1.Rule\x12\x31\n\x12\x63onfigWithServices\x18\x0b \x03(\x0b\x32\x15.v1.ConfigWithService\x12\x17\n\x05users\x18\x12 \x03(\x0b\x32\x08.v1.User\x12!\n\nuserGroups\x18\x13 \x03(\x0b\x32\r.v1.UserGroup\x12(\n\x0e\x61uthStrategies\x18\x14 \x03(\x0b\x32\x10.v1.AuthStrategy\x12\x1b\n\x07\x63lients\x18\x15 \x03(\x0b\x32\n.v1.Client\x12\"\n\x04\x64\x61ta\x18\x16 \x03(\x0b\x32\x14.google.protobuf.Any\x12\x1c\n\x07summary\x18\x17 \x01(\x0b\x32\x0b.v1.SummaryJ\x04\x08\x0c\x10\x12\"\xf2\x05\n\x10\x44iscoverResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x37\n\x04type\x18\x03 \x01(\x0e\x32).v1.DiscoverResponse.DiscoverResponseType\x12\x1c\n\x07service\x18\x04 \x01(\x0b\x32\x0b.v1.Service\x12\x1f\n\tinstances\x18\x05 \x03(\x0b\x32\x0c.v1.Instance\x12\x1c\n\x07routing\x18\x06 \x01(\x0b\x32\x0b.v1.Routing\x12 \n\trateLimit\x18\x07 \x01(\x0b\x32\r.v1.RateLimit\x12*\n\x0e\x63ircuitBreaker\x18\x08 \x01(\x0b\x32\x12.v1.CircuitBreaker\x12\x1d\n\x08services\x18\t \x03(\x0b\x32\x0b.v1.Service\x12!\n\nnamespaces\x18\n \x03(\x0b\x32\r.v1.Namespace\x12(\n\rfaultDetector\x18\x0b \x01(\x0b\x32\x11.v1.FaultDetector\x12\x1d\n\x08\x61liasFor\x18\x15 \x01(\x0b\x32\x0b.v1.Service\x12\x1c\n\x05lanes\x18\x16 \x03(\x0b\x32\r.v1.LaneGroup\"\xf2\x01\n\x14\x44iscoverResponseType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08INSTANCE\x10\x01\x12\x0b\n\x07\x43LUSTER\x10\x02\x12\x0b\n\x07ROUTING\x10\x03\x12\x0e\n\nRATE_LIMIT\x10\x04\x12\x13\n\x0f\x43IRCUIT_BREAKER\x10\x05\x12\x0c\n\x08SERVICES\x10\x06\x12\x0e\n\nNAMESPACES\x10\x0c\x12\x12\n\x0e\x46\x41ULT_DETECTOR\x10\r\x12\x08\n\x04LANE\x10\x64\"\x04\x08\x07\x10\x0b\"\x04\x08\x0e\x10\x63*\x04MESH*\x0bMESH_CONFIG*\x0e\x46LUX_DBREFRESH*\x08\x46LUX_SDK*\x0b\x46LUX_SERVERJ\x04\x08\x0c\x10\x15\"n\n\x0cOptionSwitch\x12.\n\x07options\x18\x01 \x03(\x0b\x32\x1d.v1.OptionSwitch.OptionsEntry\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\x0eInstanceLabels\x12.\n\x06labels\x18\x01 \x03(\x0b\x32\x1e.v1.InstanceLabels.LabelsEntry\x1a=\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.v1.StringList:\x02\x38\x01\x42\x8e\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\rResponseProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'response_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageB\rResponseProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
   _globals['_OPTIONSWITCH_OPTIONSENTRY']._options = None
   _globals['_OPTIONSWITCH_OPTIONSENTRY']._serialized_options = b'8\001'
   _globals['_INSTANCELABELS_LABELSENTRY']._options = None
   _globals['_INSTANCELABELS_LABELSENTRY']._serialized_options = b'8\001'
-  _globals['_RESPONSE']._serialized_start=266
-  _globals['_RESPONSE']._serialized_end=1159
-  _globals['_BATCHWRITERESPONSE']._serialized_start=1162
-  _globals['_BATCHWRITERESPONSE']._serialized_end=1347
-  _globals['_BATCHQUERYRESPONSE']._serialized_start=1350
-  _globals['_BATCHQUERYRESPONSE']._serialized_end=1997
-  _globals['_DISCOVERRESPONSE']._serialized_start=2000
-  _globals['_DISCOVERRESPONSE']._serialized_end=2708
-  _globals['_DISCOVERRESPONSE_DISCOVERRESPONSETYPE']._serialized_start=2476
-  _globals['_DISCOVERRESPONSE_DISCOVERRESPONSETYPE']._serialized_end=2702
-  _globals['_OPTIONSWITCH']._serialized_start=2710
-  _globals['_OPTIONSWITCH']._serialized_end=2820
-  _globals['_OPTIONSWITCH_OPTIONSENTRY']._serialized_start=2774
-  _globals['_OPTIONSWITCH_OPTIONSENTRY']._serialized_end=2820
-  _globals['_INSTANCELABELS']._serialized_start=2822
-  _globals['_INSTANCELABELS']._serialized_end=2949
-  _globals['_INSTANCELABELS_LABELSENTRY']._serialized_start=2888
-  _globals['_INSTANCELABELS_LABELSENTRY']._serialized_end=2949
+  _globals['_RESPONSE']._serialized_start=278
+  _globals['_RESPONSE']._serialized_end=1171
+  _globals['_BATCHWRITERESPONSE']._serialized_start=1174
+  _globals['_BATCHWRITERESPONSE']._serialized_end=1359
+  _globals['_BATCHQUERYRESPONSE']._serialized_start=1362
+  _globals['_BATCHQUERYRESPONSE']._serialized_end=2009
+  _globals['_DISCOVERRESPONSE']._serialized_start=2012
+  _globals['_DISCOVERRESPONSE']._serialized_end=2766
+  _globals['_DISCOVERRESPONSE_DISCOVERRESPONSETYPE']._serialized_start=2518
+  _globals['_DISCOVERRESPONSE_DISCOVERRESPONSETYPE']._serialized_end=2760
+  _globals['_OPTIONSWITCH']._serialized_start=2768
+  _globals['_OPTIONSWITCH']._serialized_end=2878
+  _globals['_OPTIONSWITCH_OPTIONSENTRY']._serialized_start=2832
+  _globals['_OPTIONSWITCH_OPTIONSENTRY']._serialized_end=2878
+  _globals['_INSTANCELABELS']._serialized_start=2880
+  _globals['_INSTANCELABELS']._serialized_end=3007
+  _globals['_INSTANCELABELS_LABELSENTRY']._serialized_start=2946
+  _globals['_INSTANCELABELS_LABELSENTRY']._serialized_end=3007
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ..fault_tolerance import circuitbreaker_pb2 as _circuitbreaker_pb2
 from ..model import model_pb2 as _model_pb2
 from ..service_manage import client_pb2 as _client_pb2
 from ..service_manage import configrelease_pb2 as _configrelease_pb2
 from ..fault_tolerance import fault_detector_pb2 as _fault_detector_pb2
 from ..security import auth_pb2 as _auth_pb2
 from ..service_manage import contract_pb2 as _contract_pb2
+from ..traffic_manage import lane_pb2 as _lane_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
@@ -116,60 +117,64 @@
     authStrategies: _containers.RepeatedCompositeFieldContainer[_auth_pb2.AuthStrategy]
     clients: _containers.RepeatedCompositeFieldContainer[_client_pb2.Client]
     data: _containers.RepeatedCompositeFieldContainer[_any_pb2.Any]
     summary: _model_pb2.Summary
     def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., amount: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., size: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., namespaces: _Optional[_Iterable[_Union[_namespace_pb2.Namespace, _Mapping]]] = ..., services: _Optional[_Iterable[_Union[_service_pb2.Service, _Mapping]]] = ..., instances: _Optional[_Iterable[_Union[_service_pb2.Instance, _Mapping]]] = ..., routings: _Optional[_Iterable[_Union[_routing_pb2.Routing, _Mapping]]] = ..., aliases: _Optional[_Iterable[_Union[_service_pb2.ServiceAlias, _Mapping]]] = ..., rateLimits: _Optional[_Iterable[_Union[_ratelimit_pb2.Rule, _Mapping]]] = ..., configWithServices: _Optional[_Iterable[_Union[_configrelease_pb2.ConfigWithService, _Mapping]]] = ..., users: _Optional[_Iterable[_Union[_auth_pb2.User, _Mapping]]] = ..., userGroups: _Optional[_Iterable[_Union[_auth_pb2.UserGroup, _Mapping]]] = ..., authStrategies: _Optional[_Iterable[_Union[_auth_pb2.AuthStrategy, _Mapping]]] = ..., clients: _Optional[_Iterable[_Union[_client_pb2.Client, _Mapping]]] = ..., data: _Optional[_Iterable[_Union[_any_pb2.Any, _Mapping]]] = ..., summary: _Optional[_Union[_model_pb2.Summary, _Mapping]] = ...) -> None: ...
 
 class DiscoverResponse(_message.Message):
-    __slots__ = ("code", "info", "type", "service", "instances", "routing", "rateLimit", "circuitBreaker", "services", "namespaces", "faultDetector", "aliasFor")
+    __slots__ = ("code", "info", "type", "service", "instances", "routing", "rateLimit", "circuitBreaker", "services", "namespaces", "faultDetector", "aliasFor", "lanes")
     class DiscoverResponseType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = ()
         UNKNOWN: _ClassVar[DiscoverResponse.DiscoverResponseType]
         INSTANCE: _ClassVar[DiscoverResponse.DiscoverResponseType]
         CLUSTER: _ClassVar[DiscoverResponse.DiscoverResponseType]
         ROUTING: _ClassVar[DiscoverResponse.DiscoverResponseType]
         RATE_LIMIT: _ClassVar[DiscoverResponse.DiscoverResponseType]
         CIRCUIT_BREAKER: _ClassVar[DiscoverResponse.DiscoverResponseType]
         SERVICES: _ClassVar[DiscoverResponse.DiscoverResponseType]
         NAMESPACES: _ClassVar[DiscoverResponse.DiscoverResponseType]
         FAULT_DETECTOR: _ClassVar[DiscoverResponse.DiscoverResponseType]
+        LANE: _ClassVar[DiscoverResponse.DiscoverResponseType]
     UNKNOWN: DiscoverResponse.DiscoverResponseType
     INSTANCE: DiscoverResponse.DiscoverResponseType
     CLUSTER: DiscoverResponse.DiscoverResponseType
     ROUTING: DiscoverResponse.DiscoverResponseType
     RATE_LIMIT: DiscoverResponse.DiscoverResponseType
     CIRCUIT_BREAKER: DiscoverResponse.DiscoverResponseType
     SERVICES: DiscoverResponse.DiscoverResponseType
     NAMESPACES: DiscoverResponse.DiscoverResponseType
     FAULT_DETECTOR: DiscoverResponse.DiscoverResponseType
+    LANE: DiscoverResponse.DiscoverResponseType
     CODE_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
     TYPE_FIELD_NUMBER: _ClassVar[int]
     SERVICE_FIELD_NUMBER: _ClassVar[int]
     INSTANCES_FIELD_NUMBER: _ClassVar[int]
     ROUTING_FIELD_NUMBER: _ClassVar[int]
     RATELIMIT_FIELD_NUMBER: _ClassVar[int]
     CIRCUITBREAKER_FIELD_NUMBER: _ClassVar[int]
     SERVICES_FIELD_NUMBER: _ClassVar[int]
     NAMESPACES_FIELD_NUMBER: _ClassVar[int]
     FAULTDETECTOR_FIELD_NUMBER: _ClassVar[int]
     ALIASFOR_FIELD_NUMBER: _ClassVar[int]
+    LANES_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
     info: _wrappers_pb2.StringValue
     type: DiscoverResponse.DiscoverResponseType
     service: _service_pb2.Service
     instances: _containers.RepeatedCompositeFieldContainer[_service_pb2.Instance]
     routing: _routing_pb2.Routing
     rateLimit: _ratelimit_pb2.RateLimit
     circuitBreaker: _circuitbreaker_pb2.CircuitBreaker
     services: _containers.RepeatedCompositeFieldContainer[_service_pb2.Service]
     namespaces: _containers.RepeatedCompositeFieldContainer[_namespace_pb2.Namespace]
     faultDetector: _fault_detector_pb2.FaultDetector
     aliasFor: _service_pb2.Service
-    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., type: _Optional[_Union[DiscoverResponse.DiscoverResponseType, str]] = ..., service: _Optional[_Union[_service_pb2.Service, _Mapping]] = ..., instances: _Optional[_Iterable[_Union[_service_pb2.Instance, _Mapping]]] = ..., routing: _Optional[_Union[_routing_pb2.Routing, _Mapping]] = ..., rateLimit: _Optional[_Union[_ratelimit_pb2.RateLimit, _Mapping]] = ..., circuitBreaker: _Optional[_Union[_circuitbreaker_pb2.CircuitBreaker, _Mapping]] = ..., services: _Optional[_Iterable[_Union[_service_pb2.Service, _Mapping]]] = ..., namespaces: _Optional[_Iterable[_Union[_namespace_pb2.Namespace, _Mapping]]] = ..., faultDetector: _Optional[_Union[_fault_detector_pb2.FaultDetector, _Mapping]] = ..., aliasFor: _Optional[_Union[_service_pb2.Service, _Mapping]] = ...) -> None: ...
+    lanes: _containers.RepeatedCompositeFieldContainer[_lane_pb2.LaneGroup]
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., type: _Optional[_Union[DiscoverResponse.DiscoverResponseType, str]] = ..., service: _Optional[_Union[_service_pb2.Service, _Mapping]] = ..., instances: _Optional[_Iterable[_Union[_service_pb2.Instance, _Mapping]]] = ..., routing: _Optional[_Union[_routing_pb2.Routing, _Mapping]] = ..., rateLimit: _Optional[_Union[_ratelimit_pb2.RateLimit, _Mapping]] = ..., circuitBreaker: _Optional[_Union[_circuitbreaker_pb2.CircuitBreaker, _Mapping]] = ..., services: _Optional[_Iterable[_Union[_service_pb2.Service, _Mapping]]] = ..., namespaces: _Optional[_Iterable[_Union[_namespace_pb2.Namespace, _Mapping]]] = ..., faultDetector: _Optional[_Union[_fault_detector_pb2.FaultDetector, _Mapping]] = ..., aliasFor: _Optional[_Union[_service_pb2.Service, _Mapping]] = ..., lanes: _Optional[_Iterable[_Union[_lane_pb2.LaneGroup, _Mapping]]] = ...) -> None: ...
 
 class OptionSwitch(_message.Message):
     __slots__ = ("options",)
     class OptionsEntry(_message.Message):
         __slots__ = ("key", "value")
         KEY_FIELD_NUMBER: _ClassVar[int]
         VALUE_FIELD_NUMBER: _ClassVar[int]
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/service_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: service.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: ratelimit.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: routing.proto
-# Protobuf Python Version: 4.25.0
+# Protobuf Python Version: 4.25.1
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
```

### Comparing `polarismesh_specification-1.4.2a9/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi` & `polarismesh_specification-1.5.0/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/LICENSE.txt` & `polarismesh_specification-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/README.md` & `polarismesh_specification-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/pyproject.toml` & `polarismesh_specification-1.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.2a9/PKG-INFO` & `polarismesh_specification-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: polarismesh-specification
-Version: 1.4.2a9
+Version: 1.5.0
 Project-URL: Documentation, https://github.com/polarismesh/specification#readme
 Project-URL: Issues, https://github.com/polarismesh/specification/issues
 Project-URL: Source, https://github.com/polarismesh/specification
 Author-email: "{authemail@qq.com}" <authemail@qq.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

