# Comparing `tmp/pyln_proto-24.2.tar.gz` & `tmp/pyln_proto-24.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyln_proto-24.2.tar", max compression
+gzip compressed data, was "pyln_proto-24.2.1.tar", max compression
```

## Comparing `pyln_proto-24.2.tar` & `pyln_proto-24.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      976 2024-03-08 19:31:39.104200 pyln_proto-24.2/README.md
--rw-r--r--   0        0        0      491 2024-03-08 19:31:49.340129 pyln_proto-24.2/pyln/proto/__init__.py
--rw-r--r--   0        0        0     4698 2024-03-08 19:31:39.104200 pyln_proto-24.2/pyln/proto/bech32.py
--rwxr-xr-x   0        0        0    15493 2024-03-08 19:31:39.104200 pyln_proto-24.2/pyln/proto/invoice.py
--rw-r--r--   0        0        0       68 2024-03-08 19:31:39.104200 pyln_proto-24.2/pyln/proto/message/Makefile
--rw-r--r--   0        0        0      785 2024-03-08 19:31:39.104200 pyln_proto-24.2/pyln/proto/message/__init__.py
--rw-r--r--   0        0        0     8647 2024-03-08 19:31:39.104200 pyln_proto-24.2/pyln/proto/message/array_types.py
--rw-r--r--   0        0        0    11510 2024-03-08 19:31:39.104200 pyln_proto-24.2/pyln/proto/message/fundamental_types.py
--rw-r--r--   0        0        0    27875 2024-03-08 19:31:39.104200 pyln_proto-24.2/pyln/proto/message/message.py
--rw-r--r--   0        0        0    18733 2024-03-08 19:31:39.104200 pyln_proto-24.2/pyln/proto/onion.py
--rw-r--r--   0        0        0     4367 2024-03-08 19:31:39.104200 pyln_proto-24.2/pyln/proto/primitives.py
--rw-r--r--   0        0        0    12025 2024-03-08 19:31:39.104200 pyln_proto-24.2/pyln/proto/wire.py
--rw-r--r--   0        0        0     3899 2024-03-08 19:31:39.104200 pyln_proto-24.2/pyln/proto/zbase32.py
--rw-r--r--   0        0        0      726 2024-03-08 19:31:49.316129 pyln_proto-24.2/pyproject.toml
--rw-r--r--   0        0        0     1964 1970-01-01 00:00:00.000000 pyln_proto-24.2/PKG-INFO
+-rw-r--r--   0        0        0      976 2024-04-06 07:09:32.412947 pyln_proto-24.2.1/README.md
+-rw-r--r--   0        0        0      493 2024-04-06 07:09:42.192868 pyln_proto-24.2.1/pyln/proto/__init__.py
+-rw-r--r--   0        0        0     4698 2024-04-06 07:09:32.412947 pyln_proto-24.2.1/pyln/proto/bech32.py
+-rwxr-xr-x   0        0        0    15493 2024-04-06 07:09:32.412947 pyln_proto-24.2.1/pyln/proto/invoice.py
+-rw-r--r--   0        0        0       68 2024-04-06 07:09:32.412947 pyln_proto-24.2.1/pyln/proto/message/Makefile
+-rw-r--r--   0        0        0      785 2024-04-06 07:09:32.412947 pyln_proto-24.2.1/pyln/proto/message/__init__.py
+-rw-r--r--   0        0        0     8647 2024-04-06 07:09:32.412947 pyln_proto-24.2.1/pyln/proto/message/array_types.py
+-rw-r--r--   0        0        0    11510 2024-04-06 07:09:32.412947 pyln_proto-24.2.1/pyln/proto/message/fundamental_types.py
+-rw-r--r--   0        0        0    27875 2024-04-06 07:09:32.412947 pyln_proto-24.2.1/pyln/proto/message/message.py
+-rw-r--r--   0        0        0    18733 2024-04-06 07:09:32.412947 pyln_proto-24.2.1/pyln/proto/onion.py
+-rw-r--r--   0        0        0     4367 2024-04-06 07:09:32.412947 pyln_proto-24.2.1/pyln/proto/primitives.py
+-rw-r--r--   0        0        0    12025 2024-04-06 07:09:32.412947 pyln_proto-24.2.1/pyln/proto/wire.py
+-rw-r--r--   0        0        0     3899 2024-04-06 07:09:32.412947 pyln_proto-24.2.1/pyln/proto/zbase32.py
+-rw-r--r--   0        0        0      728 2024-04-06 07:09:42.164868 pyln_proto-24.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1966 1970-01-01 00:00:00.000000 pyln_proto-24.2.1/PKG-INFO
```

### Comparing `pyln_proto-24.2/README.md` & `pyln_proto-24.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyln_proto-24.2/pyln/proto/bech32.py` & `pyln_proto-24.2.1/pyln/proto/bech32.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-24.2/pyln/proto/invoice.py` & `pyln_proto-24.2.1/pyln/proto/invoice.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-24.2/pyln/proto/message/__init__.py` & `pyln_proto-24.2.1/pyln/proto/message/__init__.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-24.2/pyln/proto/message/array_types.py` & `pyln_proto-24.2.1/pyln/proto/message/array_types.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-24.2/pyln/proto/message/fundamental_types.py` & `pyln_proto-24.2.1/pyln/proto/message/fundamental_types.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-24.2/pyln/proto/message/message.py` & `pyln_proto-24.2.1/pyln/proto/message/message.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-24.2/pyln/proto/onion.py` & `pyln_proto-24.2.1/pyln/proto/onion.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-24.2/pyln/proto/primitives.py` & `pyln_proto-24.2.1/pyln/proto/primitives.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-24.2/pyln/proto/wire.py` & `pyln_proto-24.2.1/pyln/proto/wire.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-24.2/pyln/proto/zbase32.py` & `pyln_proto-24.2.1/pyln/proto/zbase32.py`

 * *Files identical despite different names*

### Comparing `pyln_proto-24.2/pyproject.toml` & `pyln_proto-24.2.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyln-proto"
-version = "v24.02"
+version = "v24.02.1"
 description = "This package implements some of the Lightning Network protocol in pure python. It is intended for protocol testing and some minor tooling only. It is not deemed secure enough to handle any amount of real funds (you have been warned!)."
 authors = ["Christian Decker <decker.christian@gmail.com>"]
 license = "BSD-MIT"
 readme = "README.md"
 
 packages = [
   { include = "pyln/proto" },
```

### Comparing `pyln_proto-24.2/PKG-INFO` & `pyln_proto-24.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyln-proto
-Version: 24.2
+Version: 24.2.1
 Summary: This package implements some of the Lightning Network protocol in pure python. It is intended for protocol testing and some minor tooling only. It is not deemed secure enough to handle any amount of real funds (you have been warned!).
 License: BSD-MIT
 Author: Christian Decker
 Author-email: decker.christian@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

