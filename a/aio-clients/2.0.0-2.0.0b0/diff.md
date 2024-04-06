# Comparing `tmp/aio_clients-2.0.0.tar.gz` & `tmp/aio_clients-2.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_clients-2.0.0.tar", max compression
+gzip compressed data, was "aio_clients-2.0.0b0.tar", max compression
```

## Comparing `aio_clients-2.0.0.tar` & `aio_clients-2.0.0b0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-08-09 19:13:51.372000 aio_clients-2.0.0/LICENSE
--rw-r--r--   0        0        0     2984 2023-08-09 19:13:51.372000 aio_clients-2.0.0/README.md
--rw-r--r--   0        0        0      242 2023-08-09 19:13:51.372000 aio_clients-2.0.0/aio_clients/__init__.py
--rw-r--r--   0        0        0      228 2023-08-09 19:13:51.372000 aio_clients-2.0.0/aio_clients/__version__.py
--rw-r--r--   0        0        0     8218 2023-08-09 19:13:51.372000 aio_clients-2.0.0/aio_clients/client.py
--rw-r--r--   0        0        0        0 2023-08-09 19:13:51.372000 aio_clients-2.0.0/aio_clients/exceptions.py
--rw-r--r--   0        0        0       90 2023-08-09 19:13:51.376000 aio_clients-2.0.0/aio_clients/multipart/__init__.py
--rw-r--r--   0        0        0      521 2023-08-09 19:13:51.376000 aio_clients-2.0.0/aio_clients/multipart/main.py
--rw-r--r--   0        0        0      414 2023-08-09 19:13:51.376000 aio_clients-2.0.0/aio_clients/multipart/struct.py
--rw-r--r--   0        0        0     1121 2023-08-09 19:13:51.376000 aio_clients-2.0.0/aio_clients/struct.py
--rw-r--r--   0        0        0      660 2023-08-09 19:13:51.376000 aio_clients-2.0.0/aio_clients/types.py
--rw-r--r--   0        0        0      739 2023-08-09 19:13:51.376000 aio_clients-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 aio_clients-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-09 19:06:35.438205 aio_clients-2.0.0b0/LICENSE
+-rw-r--r--   0        0        0     2984 2023-08-09 19:06:35.438205 aio_clients-2.0.0b0/README.md
+-rw-r--r--   0        0        0      242 2023-08-09 19:06:35.438205 aio_clients-2.0.0b0/aio_clients/__init__.py
+-rw-r--r--   0        0        0      228 2023-08-09 19:06:35.438205 aio_clients-2.0.0b0/aio_clients/__version__.py
+-rw-r--r--   0        0        0     8218 2023-08-09 19:06:35.438205 aio_clients-2.0.0b0/aio_clients/client.py
+-rw-r--r--   0        0        0        0 2023-08-09 19:06:35.438205 aio_clients-2.0.0b0/aio_clients/exceptions.py
+-rw-r--r--   0        0        0       90 2023-08-09 19:06:35.438205 aio_clients-2.0.0b0/aio_clients/multipart/__init__.py
+-rw-r--r--   0        0        0      521 2023-08-09 19:06:35.438205 aio_clients-2.0.0b0/aio_clients/multipart/main.py
+-rw-r--r--   0        0        0      414 2023-08-09 19:06:35.438205 aio_clients-2.0.0b0/aio_clients/multipart/struct.py
+-rw-r--r--   0        0        0     1121 2023-08-09 19:06:35.438205 aio_clients-2.0.0b0/aio_clients/struct.py
+-rw-r--r--   0        0        0      660 2023-08-09 19:06:35.438205 aio_clients-2.0.0b0/aio_clients/types.py
+-rw-r--r--   0        0        0      744 2023-08-09 19:06:35.438205 aio_clients-2.0.0b0/pyproject.toml
+-rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 aio_clients-2.0.0b0/PKG-INFO
```

### Comparing `aio_clients-2.0.0/LICENSE` & `aio_clients-2.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_clients-2.0.0/README.md` & `aio_clients-2.0.0b0/README.md`

 * *Files identical despite different names*

### Comparing `aio_clients-2.0.0/aio_clients/client.py` & `aio_clients-2.0.0b0/aio_clients/client.py`

 * *Files identical despite different names*

### Comparing `aio_clients-2.0.0/aio_clients/multipart/main.py` & `aio_clients-2.0.0b0/aio_clients/multipart/main.py`

 * *Files identical despite different names*

### Comparing `aio_clients-2.0.0/aio_clients/struct.py` & `aio_clients-2.0.0b0/aio_clients/struct.py`

 * *Files identical despite different names*

### Comparing `aio_clients-2.0.0/aio_clients/types.py` & `aio_clients-2.0.0b0/aio_clients/types.py`

 * *Files identical despite different names*

### Comparing `aio_clients-2.0.0/pyproject.toml` & `aio_clients-2.0.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-clients"
-version = "2.0.0"
+version = "2.0.0-beta"
 description = "Python aiohttp client"
 authors = ["Denis Malin <denis@malina.page>"]
 license = "MIT License"
 
 readme = "README.md"
 
 homepage = "https://github.com/skar404/aio-clients"
```

### Comparing `aio_clients-2.0.0/PKG-INFO` & `aio_clients-2.0.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aio-clients
-Version: 2.0.0
+Version: 2.0.0b0
 Summary: Python aiohttp client
 Home-page: https://github.com/skar404/aio-clients
 License: MIT
 Author: Denis Malin
 Author-email: denis@malina.page
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

