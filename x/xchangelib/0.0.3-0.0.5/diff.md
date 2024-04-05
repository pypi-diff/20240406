# Comparing `tmp/xchangelib-0.0.3.tar.gz` & `tmp/xchangelib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchangelib-0.0.3.tar", last modified: Fri Mar 29 00:14:11 2024, max compression
+gzip compressed data, was "xchangelib-0.0.5.tar", last modified: Fri Apr  5 22:59:20 2024, max compression
```

## Comparing `xchangelib-0.0.3.tar` & `xchangelib-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-03-29 00:14:11.999243 xchangelib-0.0.3/
--rw-r--r--   0 rohanv     (501) staff       (20)     1070 2024-03-28 21:34:27.000000 xchangelib-0.0.3/LICENSE
--rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-03-29 00:14:11.998646 xchangelib-0.0.3/PKG-INFO
--rw-r--r--   0 rohanv     (501) staff       (20)      140 2024-03-28 21:34:27.000000 xchangelib-0.0.3/README.md
--rw-r--r--   0 rohanv     (501) staff       (20)      650 2024-03-29 00:13:57.000000 xchangelib-0.0.3/pyproject.toml
--rw-r--r--   0 rohanv     (501) staff       (20)       38 2024-03-29 00:14:11.999409 xchangelib-0.0.3/setup.cfg
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-03-29 00:14:11.989875 xchangelib-0.0.3/src/
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-03-29 00:14:11.994161 xchangelib-0.0.3/src/xchangelib/
--rw-r--r--   0 rohanv     (501) staff       (20)        0 2024-03-28 21:34:27.000000 xchangelib-0.0.3/src/xchangelib/__init__.py
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-03-29 00:14:11.990245 xchangelib-0.0.3/src/xchangelib/docs/
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-03-29 00:14:11.996816 xchangelib-0.0.3/src/xchangelib/docs/source/
--rw-r--r--   0 rohanv     (501) staff       (20)     2246 2024-03-28 21:34:27.000000 xchangelib-0.0.3/src/xchangelib/docs/source/conf.py
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-03-29 00:14:11.997430 xchangelib-0.0.3/src/xchangelib/examples/
--rw-r--r--   0 rohanv     (501) staff       (20)     3414 2024-03-28 21:34:27.000000 xchangelib-0.0.3/src/xchangelib/examples/example_bot.py
--rw-r--r--   0 rohanv     (501) staff       (20)    12187 2024-03-28 21:34:27.000000 xchangelib-0.0.3/src/xchangelib/service_pb2.py
--rw-r--r--   0 rohanv     (501) staff       (20)     8437 2024-03-28 21:34:27.000000 xchangelib-0.0.3/src/xchangelib/service_pb2_grpc.py
--rw-r--r--   0 rohanv     (501) staff       (20)      398 2024-03-28 23:03:26.000000 xchangelib-0.0.3/src/xchangelib/setup.py
--rw-r--r--   0 rohanv     (501) staff       (20)    14292 2024-03-28 21:44:53.000000 xchangelib-0.0.3/src/xchangelib/xchange_client.py
-drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-03-29 00:14:11.998063 xchangelib-0.0.3/src/xchangelib.egg-info/
--rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-03-29 00:14:11.000000 xchangelib-0.0.3/src/xchangelib.egg-info/PKG-INFO
--rw-r--r--   0 rohanv     (501) staff       (20)      444 2024-03-29 00:14:11.000000 xchangelib-0.0.3/src/xchangelib.egg-info/SOURCES.txt
--rw-r--r--   0 rohanv     (501) staff       (20)        1 2024-03-29 00:14:11.000000 xchangelib-0.0.3/src/xchangelib.egg-info/dependency_links.txt
--rw-r--r--   0 rohanv     (501) staff       (20)       49 2024-03-29 00:14:11.000000 xchangelib-0.0.3/src/xchangelib.egg-info/requires.txt
--rw-r--r--   0 rohanv     (501) staff       (20)       11 2024-03-29 00:14:11.000000 xchangelib-0.0.3/src/xchangelib.egg-info/top_level.txt
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.759057 xchangelib-0.0.5/
+-rw-r--r--   0 rohanv     (501) staff       (20)     1070 2024-04-05 22:58:16.000000 xchangelib-0.0.5/LICENSE
+-rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-05 22:59:20.758352 xchangelib-0.0.5/PKG-INFO
+-rw-r--r--   0 rohanv     (501) staff       (20)      140 2024-04-05 22:58:16.000000 xchangelib-0.0.5/README.md
+-rw-r--r--   0 rohanv     (501) staff       (20)      650 2024-04-05 22:58:16.000000 xchangelib-0.0.5/pyproject.toml
+-rw-r--r--   0 rohanv     (501) staff       (20)       38 2024-04-05 22:59:20.759279 xchangelib-0.0.5/setup.cfg
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.746240 xchangelib-0.0.5/src/
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.751584 xchangelib-0.0.5/src/xchangelib/
+-rw-r--r--   0 rohanv     (501) staff       (20)        0 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/__init__.py
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.746538 xchangelib-0.0.5/src/xchangelib/docs/
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.755574 xchangelib-0.0.5/src/xchangelib/docs/source/
+-rw-r--r--   0 rohanv     (501) staff       (20)     2246 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/docs/source/conf.py
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.756395 xchangelib-0.0.5/src/xchangelib/examples/
+-rw-r--r--   0 rohanv     (501) staff       (20)     3414 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/examples/example_bot.py
+-rw-r--r--   0 rohanv     (501) staff       (20)    12187 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/service_pb2.py
+-rw-r--r--   0 rohanv     (501) staff       (20)     8437 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/service_pb2_grpc.py
+-rw-r--r--   0 rohanv     (501) staff       (20)      398 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/setup.py
+-rw-r--r--   0 rohanv     (501) staff       (20)    14298 2024-04-05 22:58:16.000000 xchangelib-0.0.5/src/xchangelib/xchange_client.py
+drwxr-xr-x   0 rohanv     (501) staff       (20)        0 2024-04-05 22:59:20.757418 xchangelib-0.0.5/src/xchangelib.egg-info/
+-rw-r--r--   0 rohanv     (501) staff       (20)      716 2024-04-05 22:59:20.000000 xchangelib-0.0.5/src/xchangelib.egg-info/PKG-INFO
+-rw-r--r--   0 rohanv     (501) staff       (20)      444 2024-04-05 22:59:20.000000 xchangelib-0.0.5/src/xchangelib.egg-info/SOURCES.txt
+-rw-r--r--   0 rohanv     (501) staff       (20)        1 2024-04-05 22:59:20.000000 xchangelib-0.0.5/src/xchangelib.egg-info/dependency_links.txt
+-rw-r--r--   0 rohanv     (501) staff       (20)       49 2024-04-05 22:59:20.000000 xchangelib-0.0.5/src/xchangelib.egg-info/requires.txt
+-rw-r--r--   0 rohanv     (501) staff       (20)       11 2024-04-05 22:59:20.000000 xchangelib-0.0.5/src/xchangelib.egg-info/top_level.txt
```

### Comparing `xchangelib-0.0.3/LICENSE` & `xchangelib-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.3/PKG-INFO` & `xchangelib-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchangelib
-Version: 0.0.3
+Version: 0.0.5
 Summary: A client library for interacting with xchange-v3
 Author-email: Rohan Voddhi <rohan.voddhi@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/UChicagoFM/xchangelib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xchangelib-0.0.3/pyproject.toml` & `xchangelib-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xchangelib"
-version = "0.0.3"
+version = "0.0.5"
 authors = [
     { name="Rohan Voddhi", email="rohan.voddhi@gmail.com" },
 ]
 description = "A client library for interacting with xchange-v3"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ['setuptools>=69.0','protobuf==5.26.0', 'grpcio==1.62.1']
```

### Comparing `xchangelib-0.0.3/src/xchangelib/docs/source/conf.py` & `xchangelib-0.0.5/src/xchangelib/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.3/src/xchangelib/examples/example_bot.py` & `xchangelib-0.0.5/src/xchangelib/examples/example_bot.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.3/src/xchangelib/service_pb2.py` & `xchangelib-0.0.5/src/xchangelib/service_pb2.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.3/src/xchangelib/service_pb2_grpc.py` & `xchangelib-0.0.5/src/xchangelib/service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `xchangelib-0.0.3/src/xchangelib/xchange_client.py` & `xchangelib-0.0.5/src/xchangelib/xchange_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         """
         self.host = host
         self.username = username
         self.password = password
         self.positions = defaultdict(int)
         self.open_orders = dict()
         self.order_books = {sym: OrderBook() for sym in SYMBOLS}
-        self.order_id = int(time.time())  # start order id number from time
+        self.order_id = int(time.time() * 1e9)  # start order id number from time
         self.history = []
         self.connected = False
         self.call = None
         if silent:
             _LOGGER.setLevel(logging.WARNING)
```

### Comparing `xchangelib-0.0.3/src/xchangelib.egg-info/PKG-INFO` & `xchangelib-0.0.5/src/xchangelib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchangelib
-Version: 0.0.3
+Version: 0.0.5
 Summary: A client library for interacting with xchange-v3
 Author-email: Rohan Voddhi <rohan.voddhi@gmail.com>
 License: MIT License
 Project-URL: Homepage, https://github.com/UChicagoFM/xchangelib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

