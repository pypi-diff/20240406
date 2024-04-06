# Comparing `tmp/pyln_client-24.2.tar.gz` & `tmp/pyln_client-24.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyln_client-24.2.tar", max compression
+gzip compressed data, was "pyln_client-24.2.1.tar", max compression
```

## Comparing `pyln_client-24.2.tar` & `pyln_client-24.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     2940 2024-03-08 19:31:39.140513 pyln_client-24.2/README.md
--rw-r--r--   0        0        0      574 2024-03-08 19:31:55.292644 pyln_client-24.2/pyln/client/__init__.py
--rw-r--r--   0        0        0      889 2024-03-08 19:31:39.140513 pyln_client-24.2/pyln/client/clnutils.py
--rwxr-xr-x   0        0        0    26212 2024-03-08 19:31:39.140513 pyln_client-24.2/pyln/client/gossmap.py
--rw-r--r--   0        0        0    13877 2024-03-08 19:31:39.140513 pyln_client-24.2/pyln/client/gossmapstats.py
--rw-r--r--   0        0        0    52168 2024-03-08 19:31:39.140513 pyln_client-24.2/pyln/client/lightning.py
--rw-r--r--   0        0        0    39872 2024-03-08 19:31:39.140513 pyln_client-24.2/pyln/client/plugin.py
--rw-r--r--   0        0        0      610 2024-03-08 19:31:55.260644 pyln_client-24.2/pyproject.toml
--rw-r--r--   0        0        0     3626 1970-01-01 00:00:00.000000 pyln_client-24.2/PKG-INFO
+-rw-r--r--   0        0        0     2940 2024-04-06 07:09:32.797663 pyln_client-24.2.1/README.md
+-rw-r--r--   0        0        0      576 2024-04-06 07:09:46.009872 pyln_client-24.2.1/pyln/client/__init__.py
+-rw-r--r--   0        0        0      889 2024-04-06 07:09:32.797663 pyln_client-24.2.1/pyln/client/clnutils.py
+-rwxr-xr-x   0        0        0    26212 2024-04-06 07:09:32.797663 pyln_client-24.2.1/pyln/client/gossmap.py
+-rw-r--r--   0        0        0    13877 2024-04-06 07:09:32.797663 pyln_client-24.2.1/pyln/client/gossmapstats.py
+-rw-r--r--   0        0        0    52168 2024-04-06 07:09:32.797663 pyln_client-24.2.1/pyln/client/lightning.py
+-rw-r--r--   0        0        0    39872 2024-04-06 07:09:32.797663 pyln_client-24.2.1/pyln/client/plugin.py
+-rw-r--r--   0        0        0      612 2024-04-06 07:09:45.977872 pyln_client-24.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3628 1970-01-01 00:00:00.000000 pyln_client-24.2.1/PKG-INFO
```

### Comparing `pyln_client-24.2/README.md` & `pyln_client-24.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyln_client-24.2/pyln/client/__init__.py` & `pyln_client-24.2.1/pyln/client/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .lightning import LightningRpc, RpcError, Millisatoshi
 from .plugin import Plugin, monkey_patch, RpcException
 from .gossmap import Gossmap, GossmapNode, GossmapChannel, GossmapHalfchannel, GossmapNodeId, LnFeatureBits
 from .gossmapstats import GossmapStats
 
-__version__ = "v24.02"
+__version__ = "v24.02.1"
 
 __all__ = [
     "LightningRpc",
     "Plugin",
     "RpcError",
     "RpcException",
     "Millisatoshi",
```

### Comparing `pyln_client-24.2/pyln/client/clnutils.py` & `pyln_client-24.2.1/pyln/client/clnutils.py`

 * *Files identical despite different names*

### Comparing `pyln_client-24.2/pyln/client/gossmap.py` & `pyln_client-24.2.1/pyln/client/gossmap.py`

 * *Files identical despite different names*

### Comparing `pyln_client-24.2/pyln/client/gossmapstats.py` & `pyln_client-24.2.1/pyln/client/gossmapstats.py`

 * *Files identical despite different names*

### Comparing `pyln_client-24.2/pyln/client/lightning.py` & `pyln_client-24.2.1/pyln/client/lightning.py`

 * *Files identical despite different names*

### Comparing `pyln_client-24.2/pyln/client/plugin.py` & `pyln_client-24.2.1/pyln/client/plugin.py`

 * *Files identical despite different names*

### Comparing `pyln_client-24.2/pyproject.toml` & `pyln_client-24.2.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyln-client"
-version = "v24.02"
+version = "v24.02.1"
 description = "Client library and plugin library for Core Lightning"
 authors = ["Christian Decker <decker.christian@gmail.com>"]
 license = "BSD-MIT"
 readme = "README.md"
 
 packages = [
   { include = "pyln/client" },
```

### Comparing `pyln_client-24.2/PKG-INFO` & `pyln_client-24.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyln-client
-Version: 24.2
+Version: 24.2.1
 Summary: Client library and plugin library for Core Lightning
 License: BSD-MIT
 Author: Christian Decker
 Author-email: decker.christian@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

