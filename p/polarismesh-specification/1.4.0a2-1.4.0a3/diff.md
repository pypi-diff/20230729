# Comparing `tmp/polarismesh_specification-1.4.0a2.tar.gz` & `tmp/polarismesh_specification-1.4.0a3.tar.gz`

## Comparing `polarismesh_specification-1.4.0a2.tar` & `polarismesh_specification-1.4.0a3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
--rw-r--r--   0        0        0     9979 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
--rw-r--r--   0        0        0    17621 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
--rw-r--r--   0        0        0     8920 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
--rw-r--r--   0        0        0    10718 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
--rw-r--r--   0        0        0    13575 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
--rw-r--r--   0        0        0    22438 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
--rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
--rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/__init__.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/__init__.pyi
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/code_pb2.py
--rw-r--r--   0        0        0    11989 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/code_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/model_pb2.py
--rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/model_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/namespace_pb2.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/security/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/security/__init__.pyi
--rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/security/auth_pb2.py
--rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
--rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
--rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
--rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
--rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
--rw-r--r--   0        0        0    13649 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
--rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
--rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
--rw-r--r--   0        0        0    10090 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
--rw-r--r--   0        0        0    15969 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
--rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
--rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/.gitignore
--rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/LICENSE.txt
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/README.md
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/pyproject.toml
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a2/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
+-rw-r--r--   0        0        0    10282 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
+-rw-r--r--   0        0        0    18071 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
+-rw-r--r--   0        0        0     5824 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
+-rw-r--r--   0        0        0     9086 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
+-rw-r--r--   0        0        0    10748 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
+-rw-r--r--   0        0        0    13575 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
+-rw-r--r--   0        0        0    22438 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
+-rw-r--r--   0        0        0     3919 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
+-rw-r--r--   0        0        0     5251 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/__init__.pyi
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/code_pb2.py
+-rw-r--r--   0        0        0    11989 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/code_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/model_pb2.py
+-rw-r--r--   0        0        0     3395 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
+-rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/namespace_pb2.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/security/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/security/__init__.pyi
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/security/auth_pb2.py
+-rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
+-rw-r--r--   0        0        0     2605 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
+-rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
+-rw-r--r--   0        0        0    14006 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
+-rw-r--r--   0        0        0     3127 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
+-rw-r--r--   0        0        0     8045 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
+-rw-r--r--   0        0        0    13649 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
+-rw-r--r--   0        0        0     7608 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
+-rw-r--r--   0        0        0    12096 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
+-rw-r--r--   0        0        0    10090 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
+-rw-r--r--   0        0        0    15969 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
+-rw-r--r--   0        0        0     9793 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
+-rw-r--r--   0        0        0    14067 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/.gitignore
+-rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/LICENSE.txt
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/README.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/pyproject.toml
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.4.0a3/PKG-INFO
```

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x63onfig_file.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xeb\x07\n\x0f\x43onfigFileGroup\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfileCount\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x08user_ids\x18\n \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x08user_ids\x12:\n\tgroup_ids\x18\x0b \x03(\x0b\x32\x1c.google.protobuf.StringValueR\tgroup_ids\x12\x46\n\x0fremove_user_ids\x18\r \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x0fremove_user_ids\x12H\n\x10remove_group_ids\x18\x0e \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x10remove_group_ids\x12,\n\x08\x65\x64itable\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x05owner\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08\x62usiness\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\ndepartment\x18\x12 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x33\n\x08metadata\x18\x13 \x03(\x0b\x32!.v1.ConfigFileGroup.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xac\x06\n\nConfigFile\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\t \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0crelease_time\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nrelease_by\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\tencrypted\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0c\x65ncrypt_algo\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"g\n\rConfigFileTag\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xc5\x05\n\x11\x43onfigFileRelease\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\x0e \x03(\x0b\x32\x11.v1.ConfigFileTag\x12*\n\x06\x61\x63tive\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xa7\x06\n\x18\x43onfigFileReleaseHistory\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04type\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\x0c \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06reason\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xbe\x03\n\x12\x43onfigFileTemplate\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\x9e\x04\n\x14\x43lientConfigFileInfo\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12)\n\x03md5\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\x07 \x03(\x0b\x32\x11.v1.ConfigFileTag\x12-\n\tencrypted\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x30\n\npublic_key\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04name\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12@\n\x0crelease_time\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0crelease_time\"\xb2\x01\n\x1c\x43lientWatchConfigFileRequest\x12/\n\tclient_ip\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0cservice_name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x0bwatch_files\x18\x03 \x03(\x0b\x32\x18.v1.ClientConfigFileInfo\"\xa5\x01\n\x17\x43onfigFileExportRequest\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06groups\x18\x02 \x03(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05names\x18\x03 \x03(\x0b\x32\x1c.google.protobuf.StringValueB\x8e\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x0f\x43onfigFileProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11\x63onfig_file.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\"\xeb\x07\n\x0f\x43onfigFileGroup\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfileCount\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x38\n\x08user_ids\x18\n \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x08user_ids\x12:\n\tgroup_ids\x18\x0b \x03(\x0b\x32\x1c.google.protobuf.StringValueR\tgroup_ids\x12\x46\n\x0fremove_user_ids\x18\r \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x0fremove_user_ids\x12H\n\x10remove_group_ids\x18\x0e \x03(\x0b\x32\x1c.google.protobuf.StringValueR\x10remove_group_ids\x12,\n\x08\x65\x64itable\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12+\n\x05owner\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08\x62usiness\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\ndepartment\x18\x12 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x33\n\x08metadata\x18\x13 \x03(\x0b\x32!.v1.ConfigFileGroup.MetadataEntry\x1a/\n\rMetadataEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xac\x06\n\nConfigFile\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\t \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0crelease_time\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nrelease_by\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\tencrypted\x18\x10 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x32\n\x0c\x65ncrypt_algo\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"g\n\rConfigFileTag\x12)\n\x03key\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05value\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xc5\x05\n\x11\x43onfigFileRelease\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\t \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12\x31\n\x0b\x63reate_time\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0c \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\x0e \x03(\x0b\x32\x11.v1.ConfigFileTag\x12*\n\x06\x61\x63tive\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.BoolValue\"\xa7\x06\n\x18\x43onfigFileReleaseHistory\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tnamespace\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x03md5\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04type\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06status\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\x0c \x03(\x0b\x32\x11.v1.ConfigFileTag\x12\x31\n\x0b\x63reate_time\x18\r \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x0e \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x0f \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\x10 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06reason\x18\x11 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xbe\x03\n\x12\x43onfigFileTemplate\x12(\n\x02id\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12*\n\x04name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x66ormat\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63omment\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0b\x63reate_time\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tcreate_by\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x31\n\x0bmodify_time\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tmodify_by\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\x9e\x04\n\x14\x43lientConfigFileInfo\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05group\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12/\n\tfile_name\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07\x63ontent\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x07version\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.UInt64Value\x12)\n\x03md5\x18\x06 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1f\n\x04tags\x18\x07 \x03(\x0b\x32\x11.v1.ConfigFileTag\x12-\n\tencrypted\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.BoolValue\x12\x30\n\npublic_key\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04name\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12@\n\x0crelease_time\x18\x0b \x01(\x0b\x32\x1c.google.protobuf.StringValueR\x0crelease_time\"\xb2\x01\n\x1c\x43lientWatchConfigFileRequest\x12/\n\tclient_ip\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x32\n\x0cservice_name\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12-\n\x0bwatch_files\x18\x03 \x03(\x0b\x32\x18.v1.ClientConfigFileInfo\"\xa5\x01\n\x17\x43onfigFileExportRequest\x12/\n\tnamespace\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06groups\x18\x02 \x03(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05names\x18\x03 \x03(\x0b\x32\x1c.google.protobuf.StringValue\"x\n\x16\x43onfigFileGroupRequest\x12.\n\x08revision\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x11\x63onfig_file_group\x18\x02 \x01(\x0b\x32\x13.v1.ConfigFileGroupB\x8e\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x0f\x43onfigFileProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'config_file_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -41,8 +41,10 @@
   _globals['_CONFIGFILETEMPLATE']._serialized_end=3952
   _globals['_CLIENTCONFIGFILEINFO']._serialized_start=3955
   _globals['_CLIENTCONFIGFILEINFO']._serialized_end=4497
   _globals['_CLIENTWATCHCONFIGFILEREQUEST']._serialized_start=4500
   _globals['_CLIENTWATCHCONFIGFILEREQUEST']._serialized_end=4678
   _globals['_CONFIGFILEEXPORTREQUEST']._serialized_start=4681
   _globals['_CONFIGFILEEXPORTREQUEST']._serialized_end=4846
+  _globals['_CONFIGFILEGROUPREQUEST']._serialized_start=4848
+  _globals['_CONFIGFILEGROUPREQUEST']._serialized_end=4968
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -234,7 +234,15 @@
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     GROUPS_FIELD_NUMBER: _ClassVar[int]
     NAMES_FIELD_NUMBER: _ClassVar[int]
     namespace: _wrappers_pb2.StringValue
     groups: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
     names: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
     def __init__(self, namespace: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., groups: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ..., names: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ...) -> None: ...
+
+class ConfigFileGroupRequest(_message.Message):
+    __slots__ = ["revision", "config_file_group"]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
+    CONFIG_FILE_GROUP_FIELD_NUMBER: _ClassVar[int]
+    revision: _wrappers_pb2.StringValue
+    config_file_group: ConfigFileGroup
+    def __init__(self, revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., config_file_group: _Optional[_Union[ConfigFileGroup, _Mapping]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 from ..config_manage import config_file_pb2 as config__file__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x63onfig_file_response.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x11\x63onfig_file.proto\"n\n\x14\x43onfigSimpleResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xe0\x02\n\x0e\x43onfigResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x0f\x63onfigFileGroup\x18\x03 \x01(\x0b\x32\x13.v1.ConfigFileGroup\x12\"\n\nconfigFile\x18\x04 \x01(\x0b\x32\x0e.v1.ConfigFile\x12\x30\n\x11\x63onfigFileRelease\x18\x05 \x01(\x0b\x32\x15.v1.ConfigFileRelease\x12>\n\x18\x63onfigFileReleaseHistory\x18\x06 \x01(\x0b\x32\x1c.v1.ConfigFileReleaseHistory\x12\x32\n\x12\x63onfigFileTemplate\x18\x07 \x01(\x0b\x32\x16.v1.ConfigFileTemplate\"\xc6\x01\n\x18\x43onfigBatchWriteResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05total\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12%\n\tresponses\x18\x04 \x03(\x0b\x32\x12.v1.ConfigResponse\"\x9d\x03\n\x18\x43onfigBatchQueryResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05total\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12-\n\x10\x63onfigFileGroups\x18\x04 \x03(\x0b\x32\x13.v1.ConfigFileGroup\x12#\n\x0b\x63onfigFiles\x18\x05 \x03(\x0b\x32\x0e.v1.ConfigFile\x12\x31\n\x12\x63onfigFileReleases\x18\x06 \x03(\x0b\x32\x15.v1.ConfigFileRelease\x12@\n\x1a\x63onfigFileReleaseHistories\x18\x07 \x03(\x0b\x32\x1c.v1.ConfigFileReleaseHistory\x12\x33\n\x13\x63onfigFileTemplates\x18\x08 \x03(\x0b\x32\x16.v1.ConfigFileTemplate\"\x9c\x01\n\x14\x43onfigClientResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\nconfigFile\x18\x03 \x01(\x0b\x32\x18.v1.ClientConfigFileInfo\"\xf0\x01\n\x14\x43onfigImportResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x11\x63reateConfigFiles\x18\x03 \x03(\x0b\x32\x0e.v1.ConfigFile\x12\'\n\x0fskipConfigFiles\x18\x04 \x03(\x0b\x32\x0e.v1.ConfigFile\x12,\n\x14overwriteConfigFiles\x18\x05 \x03(\x0b\x32\x0e.v1.ConfigFile\"\x99\x01\n\x14\x43onfigExportResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.BytesValue\"\xaa\x01\n\x1e\x43onfigEncryptAlgorithmResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nalgorithms\x18\x03 \x03(\x0b\x32\x1c.google.protobuf.StringValue\"\xdc\x01\n\x18\x43onfigClientListResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x11\n\tnamespace\x18\x03 \x01(\t\x12\r\n\x05group\x18\x04 \x01(\t\x12\x46\n\x11\x63onfig_file_names\x18\x05 \x03(\x0b\x32\x18.v1.ClientConfigFileInfoR\x11\x63onfig_file_namesB\x96\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x17\x43onfigFileResponseProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x63onfig_file_response.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x11\x63onfig_file.proto\"n\n\x14\x43onfigSimpleResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xe0\x02\n\x0e\x43onfigResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x0f\x63onfigFileGroup\x18\x03 \x01(\x0b\x32\x13.v1.ConfigFileGroup\x12\"\n\nconfigFile\x18\x04 \x01(\x0b\x32\x0e.v1.ConfigFile\x12\x30\n\x11\x63onfigFileRelease\x18\x05 \x01(\x0b\x32\x15.v1.ConfigFileRelease\x12>\n\x18\x63onfigFileReleaseHistory\x18\x06 \x01(\x0b\x32\x1c.v1.ConfigFileReleaseHistory\x12\x32\n\x12\x63onfigFileTemplate\x18\x07 \x01(\x0b\x32\x16.v1.ConfigFileTemplate\"\xc6\x01\n\x18\x43onfigBatchWriteResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05total\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12%\n\tresponses\x18\x04 \x03(\x0b\x32\x12.v1.ConfigResponse\"\x9d\x03\n\x18\x43onfigBatchQueryResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12+\n\x05total\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12-\n\x10\x63onfigFileGroups\x18\x04 \x03(\x0b\x32\x13.v1.ConfigFileGroup\x12#\n\x0b\x63onfigFiles\x18\x05 \x03(\x0b\x32\x0e.v1.ConfigFile\x12\x31\n\x12\x63onfigFileReleases\x18\x06 \x03(\x0b\x32\x15.v1.ConfigFileRelease\x12@\n\x1a\x63onfigFileReleaseHistories\x18\x07 \x03(\x0b\x32\x1c.v1.ConfigFileReleaseHistory\x12\x33\n\x13\x63onfigFileTemplates\x18\x08 \x03(\x0b\x32\x16.v1.ConfigFileTemplate\"\x9c\x01\n\x14\x43onfigClientResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\nconfigFile\x18\x03 \x01(\x0b\x32\x18.v1.ClientConfigFileInfo\"\xf0\x01\n\x14\x43onfigImportResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x11\x63reateConfigFiles\x18\x03 \x03(\x0b\x32\x0e.v1.ConfigFile\x12\'\n\x0fskipConfigFiles\x18\x04 \x03(\x0b\x32\x0e.v1.ConfigFile\x12,\n\x14overwriteConfigFiles\x18\x05 \x03(\x0b\x32\x0e.v1.ConfigFile\"\x99\x01\n\x14\x43onfigExportResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12)\n\x04\x64\x61ta\x18\x03 \x01(\x0b\x32\x1b.google.protobuf.BytesValue\"\xaa\x01\n\x1e\x43onfigEncryptAlgorithmResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x30\n\nalgorithms\x18\x03 \x03(\x0b\x32\x1c.google.protobuf.StringValue\"\x8c\x02\n\x18\x43onfigClientListResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12.\n\x08revision\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x11\n\tnamespace\x18\x04 \x01(\t\x12\r\n\x05group\x18\x05 \x01(\t\x12\x46\n\x11\x63onfig_file_infos\x18\x06 \x03(\x0b\x32\x18.v1.ClientConfigFileInfoR\x11\x63onfig_file_infosB\x96\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x17\x43onfigFileResponseProtoZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'config_file_response_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
@@ -37,9 +37,9 @@
   _globals['_CONFIGIMPORTRESPONSE']._serialized_start=1329
   _globals['_CONFIGIMPORTRESPONSE']._serialized_end=1569
   _globals['_CONFIGEXPORTRESPONSE']._serialized_start=1572
   _globals['_CONFIGEXPORTRESPONSE']._serialized_end=1725
   _globals['_CONFIGENCRYPTALGORITHMRESPONSE']._serialized_start=1728
   _globals['_CONFIGENCRYPTALGORITHMRESPONSE']._serialized_end=1898
   _globals['_CONFIGCLIENTLISTRESPONSE']._serialized_start=1901
-  _globals['_CONFIGCLIENTLISTRESPONSE']._serialized_end=2121
+  _globals['_CONFIGCLIENTLISTRESPONSE']._serialized_end=2169
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -106,19 +106,21 @@
     ALGORITHMS_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
     info: _wrappers_pb2.StringValue
     algorithms: _containers.RepeatedCompositeFieldContainer[_wrappers_pb2.StringValue]
     def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., algorithms: _Optional[_Iterable[_Union[_wrappers_pb2.StringValue, _Mapping]]] = ...) -> None: ...
 
 class ConfigClientListResponse(_message.Message):
-    __slots__ = ["code", "info", "namespace", "group", "config_file_names"]
+    __slots__ = ["code", "info", "revision", "namespace", "group", "config_file_infos"]
     CODE_FIELD_NUMBER: _ClassVar[int]
     INFO_FIELD_NUMBER: _ClassVar[int]
+    REVISION_FIELD_NUMBER: _ClassVar[int]
     NAMESPACE_FIELD_NUMBER: _ClassVar[int]
     GROUP_FIELD_NUMBER: _ClassVar[int]
-    CONFIG_FILE_NAMES_FIELD_NUMBER: _ClassVar[int]
+    CONFIG_FILE_INFOS_FIELD_NUMBER: _ClassVar[int]
     code: _wrappers_pb2.UInt32Value
     info: _wrappers_pb2.StringValue
+    revision: _wrappers_pb2.StringValue
     namespace: str
     group: str
-    config_file_names: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ClientConfigFileInfo]
-    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[str] = ..., group: _Optional[str] = ..., config_file_names: _Optional[_Iterable[_Union[_config_file_pb2.ClientConfigFileInfo, _Mapping]]] = ...) -> None: ...
+    config_file_infos: _containers.RepeatedCompositeFieldContainer[_config_file_pb2.ClientConfigFileInfo]
+    def __init__(self, code: _Optional[_Union[_wrappers_pb2.UInt32Value, _Mapping]] = ..., info: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., revision: _Optional[_Union[_wrappers_pb2.StringValue, _Mapping]] = ..., namespace: _Optional[str] = ..., group: _Optional[str] = ..., config_file_infos: _Optional[_Iterable[_Union[_config_file_pb2.ClientConfigFileInfo, _Mapping]]] = ...) -> None: ...
```

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 _sym_db = _symbol_database.Default()
 
 
 from ..config_manage import config_file_pb2 as config__file__pb2
 from ..config_manage import config_file_response_pb2 as config__file__response__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15grpc_config_api.proto\x12\x02v1\x1a\x11\x63onfig_file.proto\x1a\x1a\x63onfig_file_response.proto2\xcb\x03\n\x11PolarisConfigGRPC\x12\x45\n\rGetConfigFile\x12\x18.v1.ClientConfigFileInfo\x1a\x18.v1.ConfigClientResponse\"\x00\x12>\n\x10\x43reateConfigFile\x12\x0e.v1.ConfigFile\x1a\x18.v1.ConfigClientResponse\"\x00\x12>\n\x10UpdateConfigFile\x12\x0e.v1.ConfigFile\x1a\x18.v1.ConfigClientResponse\"\x00\x12\x46\n\x11PublishConfigFile\x12\x15.v1.ConfigFileRelease\x1a\x18.v1.ConfigClientResponse\"\x00\x12P\n\x10WatchConfigFiles\x12 .v1.ClientWatchConfigFileRequest\x1a\x18.v1.ConfigClientResponse\"\x00\x12U\n\x19GetConfigFileMetadataList\x12\x18.v1.ClientConfigFileInfo\x1a\x1c.v1.ConfigClientListResponse\"\x00\x42\x97\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x18PolarisConfigGRPCServiceZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15grpc_config_api.proto\x12\x02v1\x1a\x11\x63onfig_file.proto\x1a\x1a\x63onfig_file_response.proto2\xcd\x03\n\x11PolarisConfigGRPC\x12\x45\n\rGetConfigFile\x12\x18.v1.ClientConfigFileInfo\x1a\x18.v1.ConfigClientResponse\"\x00\x12>\n\x10\x43reateConfigFile\x12\x0e.v1.ConfigFile\x1a\x18.v1.ConfigClientResponse\"\x00\x12>\n\x10UpdateConfigFile\x12\x0e.v1.ConfigFile\x1a\x18.v1.ConfigClientResponse\"\x00\x12\x46\n\x11PublishConfigFile\x12\x15.v1.ConfigFileRelease\x1a\x18.v1.ConfigClientResponse\"\x00\x12P\n\x10WatchConfigFiles\x12 .v1.ClientWatchConfigFileRequest\x1a\x18.v1.ConfigClientResponse\"\x00\x12W\n\x19GetConfigFileMetadataList\x12\x1a.v1.ConfigFileGroupRequest\x1a\x1c.v1.ConfigClientListResponse\"\x00\x42\x97\x01\n6com.tencent.polaris.specification.api.v1.config.manageB\x18PolarisConfigGRPCServiceZCgithub.com/polarismesh/specification/source/go/api/v1/config_manageb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'grpc_config_api_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n6com.tencent.polaris.specification.api.v1.config.manageB\030PolarisConfigGRPCServiceZCgithub.com/polarismesh/specification/source/go/api/v1/config_manage'
   _globals['_POLARISCONFIGGRPC']._serialized_start=77
-  _globals['_POLARISCONFIGGRPC']._serialized_end=536
+  _globals['_POLARISCONFIGGRPC']._serialized_end=538
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         self.WatchConfigFiles = channel.unary_unary(
                 '/v1.PolarisConfigGRPC/WatchConfigFiles',
                 request_serializer=config__file__pb2.ClientWatchConfigFileRequest.SerializeToString,
                 response_deserializer=config__file__response__pb2.ConfigClientResponse.FromString,
                 )
         self.GetConfigFileMetadataList = channel.unary_unary(
                 '/v1.PolarisConfigGRPC/GetConfigFileMetadataList',
-                request_serializer=config__file__pb2.ClientConfigFileInfo.SerializeToString,
+                request_serializer=config__file__pb2.ConfigFileGroupRequest.SerializeToString,
                 response_deserializer=config__file__response__pb2.ConfigClientListResponse.FromString,
                 )
 
 
 class PolarisConfigGRPCServicer(object):
     """Missing associated documentation comment in .proto file."""
 
@@ -82,15 +82,15 @@
         """订阅配置变更
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetConfigFileMetadataList(self, request, context):
-        """拉取配置变更列表
+        """拉取指定配置分组下的配置文件列表
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_PolarisConfigGRPCServicer_to_server(servicer, server):
@@ -118,15 +118,15 @@
             'WatchConfigFiles': grpc.unary_unary_rpc_method_handler(
                     servicer.WatchConfigFiles,
                     request_deserializer=config__file__pb2.ClientWatchConfigFileRequest.FromString,
                     response_serializer=config__file__response__pb2.ConfigClientResponse.SerializeToString,
             ),
             'GetConfigFileMetadataList': grpc.unary_unary_rpc_method_handler(
                     servicer.GetConfigFileMetadataList,
-                    request_deserializer=config__file__pb2.ClientConfigFileInfo.FromString,
+                    request_deserializer=config__file__pb2.ConfigFileGroupRequest.FromString,
                     response_serializer=config__file__response__pb2.ConfigClientListResponse.SerializeToString,
             ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'v1.PolarisConfigGRPC', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
@@ -228,11 +228,11 @@
             call_credentials=None,
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/v1.PolarisConfigGRPC/GetConfigFileMetadataList',
-            config__file__pb2.ClientConfigFileInfo.SerializeToString,
+            config__file__pb2.ConfigFileGroupRequest.SerializeToString,
             config__file__response__pb2.ConfigClientListResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/code_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/code_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/code_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/model_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/model_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/model_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/namespace_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/namespace_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/security/auth_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/security/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/security/auth_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/security/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/client_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/client_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/request_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/request_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/response_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/response_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/service_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/service_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi` & `polarismesh_specification-1.4.0a3/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/LICENSE.txt` & `polarismesh_specification-1.4.0a3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/README.md` & `polarismesh_specification-1.4.0a3/README.md`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/pyproject.toml` & `polarismesh_specification-1.4.0a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.4.0a2/PKG-INFO` & `polarismesh_specification-1.4.0a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarismesh-specification
-Version: 1.4.0a2
+Version: 1.4.0a3
 Project-URL: Documentation, https://github.com/polarismesh/specification#readme
 Project-URL: Issues, https://github.com/polarismesh/specification/issues
 Project-URL: Source, https://github.com/polarismesh/specification
 Author-email: "{authemail@qq.com}" <authemail@qq.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

