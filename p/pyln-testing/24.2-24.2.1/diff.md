# Comparing `tmp/pyln_testing-24.2.tar.gz` & `tmp/pyln_testing-24.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyln_testing-24.2.tar", max compression
+gzip compressed data, was "pyln_testing-24.2.1.tar", max compression
```

## Comparing `pyln_testing-24.2.tar` & `pyln_testing-24.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2397 2024-03-08 19:31:41.092401 pyln_testing-24.2/README.md
--rw-r--r--   0        0        0       57 2024-03-08 19:31:52.716317 pyln_testing-24.2/pyln/testing/__init__.py
--rw-r--r--   0        0        0     4005 2024-03-08 19:31:41.092401 pyln_testing-24.2/pyln/testing/btcproxy.py
--rw-r--r--   0        0        0     7999 2024-03-08 19:31:41.092401 pyln_testing-24.2/pyln/testing/db.py
--rw-r--r--   0        0        0    21683 2024-03-08 19:31:41.092401 pyln_testing-24.2/pyln/testing/fixtures.py
--rw-r--r--   0        0        0    13033 2024-03-08 19:31:41.092401 pyln_testing-24.2/pyln/testing/gossip.py
--rw-r--r--   0        0        0    10040 2024-03-08 19:31:41.092401 pyln_testing-24.2/pyln/testing/grpc.py
--rw-r--r--   0        0        0    81266 2024-03-08 19:31:41.092401 pyln_testing-24.2/pyln/testing/grpc2py.py
--rw-r--r--   0        0        0    65485 2024-03-08 19:31:41.092401 pyln_testing-24.2/pyln/testing/utils.py
--rw-r--r--   0        0        0      972 2024-03-08 19:31:52.680317 pyln_testing-24.2/pyproject.toml
--rw-r--r--   0        0        0     3563 1970-01-01 00:00:00.000000 pyln_testing-24.2/PKG-INFO
+-rw-r--r--   0        0        0     2397 2024-04-06 07:09:32.181819 pyln_testing-24.2.1/README.md
+-rw-r--r--   0        0        0       59 2024-04-06 07:09:41.417812 pyln_testing-24.2.1/pyln/testing/__init__.py
+-rw-r--r--   0        0        0     4005 2024-04-06 07:09:32.181819 pyln_testing-24.2.1/pyln/testing/btcproxy.py
+-rw-r--r--   0        0        0     7999 2024-04-06 07:09:32.181819 pyln_testing-24.2.1/pyln/testing/db.py
+-rw-r--r--   0        0        0    21683 2024-04-06 07:09:32.181819 pyln_testing-24.2.1/pyln/testing/fixtures.py
+-rw-r--r--   0        0        0    13033 2024-04-06 07:09:32.181819 pyln_testing-24.2.1/pyln/testing/gossip.py
+-rw-r--r--   0        0        0    10040 2024-04-06 07:09:32.181819 pyln_testing-24.2.1/pyln/testing/grpc.py
+-rw-r--r--   0        0        0    81266 2024-04-06 07:09:32.181819 pyln_testing-24.2.1/pyln/testing/grpc2py.py
+-rw-r--r--   0        0        0    65485 2024-04-06 07:09:32.181819 pyln_testing-24.2.1/pyln/testing/utils.py
+-rw-r--r--   0        0        0      974 2024-04-06 07:09:41.393812 pyln_testing-24.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3565 1970-01-01 00:00:00.000000 pyln_testing-24.2.1/PKG-INFO
```

### Comparing `pyln_testing-24.2/README.md` & `pyln_testing-24.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyln_testing-24.2/pyln/testing/btcproxy.py` & `pyln_testing-24.2.1/pyln/testing/btcproxy.py`

 * *Files identical despite different names*

### Comparing `pyln_testing-24.2/pyln/testing/db.py` & `pyln_testing-24.2.1/pyln/testing/db.py`

 * *Files identical despite different names*

### Comparing `pyln_testing-24.2/pyln/testing/fixtures.py` & `pyln_testing-24.2.1/pyln/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `pyln_testing-24.2/pyln/testing/gossip.py` & `pyln_testing-24.2.1/pyln/testing/gossip.py`

 * *Files identical despite different names*

### Comparing `pyln_testing-24.2/pyln/testing/grpc.py` & `pyln_testing-24.2.1/pyln/testing/grpc.py`

 * *Files identical despite different names*

### Comparing `pyln_testing-24.2/pyln/testing/grpc2py.py` & `pyln_testing-24.2.1/pyln/testing/grpc2py.py`

 * *Files identical despite different names*

### Comparing `pyln_testing-24.2/pyln/testing/utils.py` & `pyln_testing-24.2.1/pyln/testing/utils.py`

 * *Files identical despite different names*

### Comparing `pyln_testing-24.2/pyproject.toml` & `pyln_testing-24.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyln-testing"
-version = "v24.02"
+version = "v24.02.1"
 description = "Test your Core Lightning integration, plugins or whatever you want"
 authors = ["Christian Decker <decker.christian@gmail.com>"]
 license = "BSD-MIT"
 readme = "README.md"
 
 packages = [
   { include = "pyln/testing" },
```

### Comparing `pyln_testing-24.2/PKG-INFO` & `pyln_testing-24.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyln-testing
-Version: 24.2
+Version: 24.2.1
 Summary: Test your Core Lightning integration, plugins or whatever you want
 License: BSD-MIT
 Author: Christian Decker
 Author-email: decker.christian@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

