# Comparing `tmp/diambra-engine-2.2.1.tar.gz` & `tmp/diambra-engine-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diambra-engine-2.2.1.tar", last modified: Sun Feb 18 16:52:49 2024, max compression
+gzip compressed data, was "diambra-engine-2.2.2.tar", last modified: Sat Apr  6 12:13:25 2024, max compression
```

## Comparing `diambra-engine-2.2.1.tar` & `diambra-engine-2.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:52:49.008512 diambra-engine-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-18 16:52:49.008512 diambra-engine-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-02-18 16:52:34.000000 diambra-engine-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:52:49.004512 diambra-engine-2.2.1/diambra/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-18 16:52:34.000000 diambra-engine-2.2.1/diambra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:52:49.004512 diambra-engine-2.2.1/diambra/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-02-18 16:52:34.000000 diambra-engine-2.2.1/diambra/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28509 2024-02-18 16:52:47.000000 diambra-engine-2.2.1/diambra/engine/interface_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-02-18 16:52:47.000000 diambra-engine-2.2.1/diambra/engine/interface_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-18 16:52:49.004512 diambra-engine-2.2.1/diambra_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-02-18 16:52:48.000000 diambra-engine-2.2.1/diambra_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-02-18 16:52:48.000000 diambra-engine-2.2.1/diambra_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-18 16:52:48.000000 diambra-engine-2.2.1/diambra_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-02-18 16:52:48.000000 diambra-engine-2.2.1/diambra_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-18 16:52:48.000000 diambra-engine-2.2.1/diambra_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-18 16:52:49.008512 diambra-engine-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-02-18 16:52:34.000000 diambra-engine-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:13:25.184984 diambra-engine-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-06 12:13:25.184984 diambra-engine-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-06 12:13:10.000000 diambra-engine-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:13:25.180984 diambra-engine-2.2.2/diambra/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 12:13:10.000000 diambra-engine-2.2.2/diambra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:13:25.180984 diambra-engine-2.2.2/diambra/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-06 12:13:10.000000 diambra-engine-2.2.2/diambra/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28509 2024-04-06 12:13:23.000000 diambra-engine-2.2.2/diambra/engine/interface_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10562 2024-04-06 12:13:23.000000 diambra-engine-2.2.2/diambra/engine/interface_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 12:13:25.184984 diambra-engine-2.2.2/diambra_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-06 12:13:25.000000 diambra-engine-2.2.2/diambra_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-06 12:13:25.000000 diambra-engine-2.2.2/diambra_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 12:13:25.000000 diambra-engine-2.2.2/diambra_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-06 12:13:25.000000 diambra-engine-2.2.2/diambra_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-06 12:13:25.000000 diambra-engine-2.2.2/diambra_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 12:13:25.184984 diambra-engine-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-04-06 12:13:10.000000 diambra-engine-2.2.2/setup.py
```

### Comparing `diambra-engine-2.2.1/PKG-INFO` & `diambra-engine-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-engine
-Version: 2.2.1
+Version: 2.2.2
 Summary: DIAMBRA™ Arena Engine API Client
 Home-page: https://diambra.ai
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

### Comparing `diambra-engine-2.2.1/diambra/engine/__init__.py` & `diambra-engine-2.2.2/diambra/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `diambra-engine-2.2.1/diambra/engine/interface_pb2.py` & `diambra-engine-2.2.2/diambra/engine/interface_pb2.py`

 * *Files identical despite different names*

### Comparing `diambra-engine-2.2.1/diambra/engine/interface_pb2_grpc.py` & `diambra-engine-2.2.2/diambra/engine/interface_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `diambra-engine-2.2.1/diambra_engine.egg-info/PKG-INFO` & `diambra-engine-2.2.2/diambra_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diambra-engine
-Version: 2.2.1
+Version: 2.2.2
 Summary: DIAMBRA™ Arena Engine API Client
 Home-page: https://diambra.ai
 Author: DIAMBRA Team
 Author-email: info@diambra.ai
 License: Custom
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: OS Independent
```

### Comparing `diambra-engine-2.2.1/setup.py` & `diambra-engine-2.2.2/setup.py`

 * *Files identical despite different names*

