# Comparing `tmp/pyln_grpc_proto-24.2.tar.gz` & `tmp/pyln_grpc_proto-24.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyln_grpc_proto-24.2.tar", max compression
+gzip compressed data, was "pyln_grpc_proto-24.2.1.tar", max compression
```

## Comparing `pyln_grpc_proto-24.2.tar` & `pyln_grpc_proto-24.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      228 2024-03-08 19:31:42.015761 pyln_grpc_proto-24.2/README.md
--rw-r--r--   0        0        0      190 2024-03-08 19:31:51.679682 pyln_grpc_proto-24.2/pyln/grpc/__init__.py
--rw-r--r--   0        0        0   124970 2024-03-08 19:31:42.015761 pyln_grpc_proto-24.2/pyln/grpc/node_pb2.py
--rw-r--r--   0        0        0    95685 2024-03-08 19:31:42.015761 pyln_grpc_proto-24.2/pyln/grpc/node_pb2_grpc.py
--rw-r--r--   0        0        0     5436 2024-03-08 19:31:42.015761 pyln_grpc_proto-24.2/pyln/grpc/primitives_pb2.py
--rw-r--r--   0        0        0        0 2024-03-08 19:31:42.015761 pyln_grpc_proto-24.2/pyln/grpc/py.typed
--rw-r--r--   0        0        0      599 2024-03-08 19:31:51.651682 pyln_grpc_proto-24.2/pyproject.toml
--rw-r--r--   0        0        0      871 1970-01-01 00:00:00.000000 pyln_grpc_proto-24.2/PKG-INFO
+-rw-r--r--   0        0        0      228 2024-04-06 07:09:31.970921 pyln_grpc_proto-24.2.1/README.md
+-rw-r--r--   0        0        0      192 2024-04-06 07:09:42.426971 pyln_grpc_proto-24.2.1/pyln/grpc/__init__.py
+-rw-r--r--   0        0        0   124970 2024-04-06 07:09:31.974921 pyln_grpc_proto-24.2.1/pyln/grpc/node_pb2.py
+-rw-r--r--   0        0        0    95685 2024-04-06 07:09:31.974921 pyln_grpc_proto-24.2.1/pyln/grpc/node_pb2_grpc.py
+-rw-r--r--   0        0        0     5436 2024-04-06 07:09:31.974921 pyln_grpc_proto-24.2.1/pyln/grpc/primitives_pb2.py
+-rw-r--r--   0        0        0        0 2024-04-06 07:09:31.974921 pyln_grpc_proto-24.2.1/pyln/grpc/py.typed
+-rw-r--r--   0        0        0      601 2024-04-06 07:09:42.398970 pyln_grpc_proto-24.2.1/pyproject.toml
+-rw-r--r--   0        0        0      873 1970-01-01 00:00:00.000000 pyln_grpc_proto-24.2.1/PKG-INFO
```

### Comparing `pyln_grpc_proto-24.2/pyln/grpc/node_pb2.py` & `pyln_grpc_proto-24.2.1/pyln/grpc/node_pb2.py`

 * *Files identical despite different names*

### Comparing `pyln_grpc_proto-24.2/pyln/grpc/node_pb2_grpc.py` & `pyln_grpc_proto-24.2.1/pyln/grpc/node_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pyln_grpc_proto-24.2/pyln/grpc/primitives_pb2.py` & `pyln_grpc_proto-24.2.1/pyln/grpc/primitives_pb2.py`

 * *Files identical despite different names*

### Comparing `pyln_grpc_proto-24.2/pyproject.toml` & `pyln_grpc_proto-24.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "pyln-grpc-proto"
-version = "v24.02"
+version = "v24.02.1"
 description = "The compiled GRPC proto for CLN"
 authors = ["Christian Decker <decker@blockstream.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     { include = "pyln/grpc/*.py" },
```

### Comparing `pyln_grpc_proto-24.2/PKG-INFO` & `pyln_grpc_proto-24.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyln-grpc-proto
-Version: 24.2
+Version: 24.2.1
 Summary: The compiled GRPC proto for CLN
 License: MIT
 Author: Christian Decker
 Author-email: decker@blockstream.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

