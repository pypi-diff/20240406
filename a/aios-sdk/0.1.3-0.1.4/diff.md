# Comparing `tmp/aios_sdk-0.1.3.tar.gz` & `tmp/aios_sdk-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aios_sdk-0.1.3.tar", max compression
+gzip compressed data, was "aios_sdk-0.1.4.tar", max compression
```

## Comparing `aios_sdk-0.1.3.tar` & `aios_sdk-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,31 @@
--rw-r--r--   0        0        0        0 2024-04-05 20:00:00.579828 aios_sdk-0.1.3/README.md
--rw-r--r--   0        0        0      660 2024-04-06 00:32:15.446423 aios_sdk-0.1.3/aios_sdk/__init__.py
--rw-r--r--   0        0        0      115 2024-04-06 00:26:38.875127 aios_sdk-0.1.3/aios_sdk/models.py
--rw-r--r--   0        0        0      481 2024-04-06 00:36:37.514054 aios_sdk-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      323 1970-01-01 00:00:00.000000 aios_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-05 20:00:00.579828 aios_sdk-0.1.4/README.md
+-rw-r--r--   0        0        0      515 2024-04-06 00:42:11.918238 aios_sdk-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2945 2024-04-05 20:05:44.570072 aios_sdk-0.1.4/rpc/app_state_pb2.py
+-rw-r--r--   0        0        0     4770 2024-04-05 20:05:44.570256 aios_sdk-0.1.4/rpc/app_state_pb2.pyi
+-rw-r--r--   0        0        0     5673 2024-04-05 20:26:55.649399 aios_sdk-0.1.4/rpc/app_state_pb2_grpc.py
+-rw-r--r--   0        0        0     2457 2024-04-05 20:05:44.570420 aios_sdk-0.1.4/rpc/app_state_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1384 2024-04-05 20:05:44.570468 aios_sdk-0.1.4/rpc/helloworld_pb2.py
+-rw-r--r--   0        0        0     1034 2024-04-05 20:05:44.570515 aios_sdk-0.1.4/rpc/helloworld_pb2.pyi
+-rw-r--r--   0        0        0     2405 2024-04-05 20:26:55.649634 aios_sdk-0.1.4/rpc/helloworld_pb2_grpc.py
+-rw-r--r--   0        0        0     1238 2024-04-05 20:05:44.570610 aios_sdk-0.1.4/rpc/helloworld_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2902 2024-04-05 20:05:44.570671 aios_sdk-0.1.4/rpc/inference_pb2.py
+-rw-r--r--   0        0        0     4952 2024-04-05 20:05:44.570788 aios_sdk-0.1.4/rpc/inference_pb2.pyi
+-rw-r--r--   0        0        0     4020 2024-04-05 20:26:55.649871 aios_sdk-0.1.4/rpc/inference_pb2_grpc.py
+-rw-r--r--   0        0        0     1842 2024-04-05 20:05:44.570881 aios_sdk-0.1.4/rpc/inference_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1298 2024-04-05 20:05:44.570924 aios_sdk-0.1.4/rpc/kill_pb2.py
+-rw-r--r--   0        0        0      632 2024-04-05 20:05:44.570968 aios_sdk-0.1.4/rpc/kill_pb2.pyi
+-rw-r--r--   0        0        0     2331 2024-04-05 20:26:55.649991 aios_sdk-0.1.4/rpc/kill_pb2_grpc.py
+-rw-r--r--   0        0        0     1178 2024-04-05 20:05:44.571060 aios_sdk-0.1.4/rpc/kill_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3604 2024-04-05 20:05:44.571111 aios_sdk-0.1.4/rpc/models_pb2.py
+-rw-r--r--   0        0        0     6093 2024-04-05 20:05:44.571217 aios_sdk-0.1.4/rpc/models_pb2.pyi
+-rw-r--r--   0        0        0     8333 2024-04-05 20:26:55.649158 aios_sdk-0.1.4/rpc/models_pb2_grpc.py
+-rw-r--r--   0        0        0     3179 2024-04-05 20:05:44.571330 aios_sdk-0.1.4/rpc/models_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1833 2024-04-05 20:05:44.571375 aios_sdk-0.1.4/rpc/system_info_pb2.py
+-rw-r--r--   0        0        0     2498 2024-04-05 20:05:44.571431 aios_sdk-0.1.4/rpc/system_info_pb2.pyi
+-rw-r--r--   0        0        0     2525 2024-04-05 20:26:55.649752 aios_sdk-0.1.4/rpc/system_info_pb2_grpc.py
+-rw-r--r--   0        0        0     1340 2024-04-05 20:05:44.571528 aios_sdk-0.1.4/rpc/system_info_pb2_grpc.pyi
+-rw-r--r--   0        0        0     3459 2024-04-05 20:05:44.571579 aios_sdk-0.1.4/rpc/websocket_pb2.py
+-rw-r--r--   0        0        0     5489 2024-04-05 20:05:44.571696 aios_sdk-0.1.4/rpc/websocket_pb2.pyi
+-rw-r--r--   0        0        0     5581 2024-04-05 20:26:55.650104 aios_sdk-0.1.4/rpc/websocket_pb2_grpc.py
+-rw-r--r--   0        0        0     2369 2024-04-05 20:05:44.571868 aios_sdk-0.1.4/rpc/websocket_pb2_grpc.pyi
+-rw-r--r--   0        0        0      323 1970-01-01 00:00:00.000000 aios_sdk-0.1.4/PKG-INFO
```

