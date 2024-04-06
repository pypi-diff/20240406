# Comparing `tmp/redis_async_client-0.1.1.tar.gz` & `tmp/redis_async_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_async_client-0.1.1.tar", max compression
+gzip compressed data, was "redis_async_client-0.1.2.tar", max compression
```

## Comparing `redis_async_client-0.1.1.tar` & `redis_async_client-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      708 2024-04-06 07:13:32.873711 redis_async_client-0.1.1/README.md
--rw-r--r--   0        0        0     2104 2024-04-06 07:38:14.515145 redis_async_client-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      572 2024-04-06 07:12:05.938369 redis_async_client-0.1.1/src/redis_async_client/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 06:39:15.440450 redis_async_client-0.1.1/src/redis_async_client/core/__init__.py
--rw-r--r--   0        0        0       54 2024-04-06 06:50:20.561420 redis_async_client-0.1.1/src/redis_async_client/core/_constants.py
--rw-r--r--   0        0        0       87 2024-04-06 06:50:39.109227 redis_async_client-0.1.1/src/redis_async_client/core/_types.py
--rw-r--r--   0        0        0     3288 2024-04-06 07:23:31.183455 redis_async_client-0.1.1/src/redis_async_client/core/async_client.py
--rw-r--r--   0        0        0     3868 2024-04-06 07:35:53.716381 redis_async_client-0.1.1/src/redis_async_client/core/base.py
--rw-r--r--   0        0        0       53 2024-04-06 06:50:20.561420 redis_async_client-0.1.1/src/redis_async_client/core/exc.py
--rw-r--r--   0        0        0       66 2024-04-06 06:50:39.113227 redis_async_client-0.1.1/src/redis_async_client/core/logger.py
--rw-r--r--   0        0        0      756 2024-04-06 07:37:40.647441 redis_async_client-0.1.1/src/redis_async_client/core/settings.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 redis_async_client-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      708 2024-04-06 07:13:32.873711 redis_async_client-0.1.2/README.md
+-rw-r--r--   0        0        0     2223 2024-04-06 07:48:23.101942 redis_async_client-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      572 2024-04-06 07:12:05.938369 redis_async_client-0.1.2/src/redis_async_client/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 06:39:15.440450 redis_async_client-0.1.2/src/redis_async_client/core/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-06 06:50:20.561420 redis_async_client-0.1.2/src/redis_async_client/core/_constants.py
+-rw-r--r--   0        0        0       87 2024-04-06 06:50:39.109227 redis_async_client-0.1.2/src/redis_async_client/core/_types.py
+-rw-r--r--   0        0        0     3288 2024-04-06 07:23:31.183455 redis_async_client-0.1.2/src/redis_async_client/core/async_client.py
+-rw-r--r--   0        0        0     3868 2024-04-06 07:35:53.716381 redis_async_client-0.1.2/src/redis_async_client/core/base.py
+-rw-r--r--   0        0        0       53 2024-04-06 06:50:20.561420 redis_async_client-0.1.2/src/redis_async_client/core/exc.py
+-rw-r--r--   0        0        0       66 2024-04-06 06:50:39.113227 redis_async_client-0.1.2/src/redis_async_client/core/logger.py
+-rw-r--r--   0        0        0      756 2024-04-06 07:37:40.647441 redis_async_client-0.1.2/src/redis_async_client/core/settings.py
+-rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 redis_async_client-0.1.2/PKG-INFO
```

### Comparing `redis_async_client-0.1.1/README.md` & `redis_async_client-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `redis_async_client-0.1.1/pyproject.toml` & `redis_async_client-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [tool.poetry]
 name = "redis-async-client"
-version = "0.1.1"
+version = "0.1.2"
 description = "Redis async client."
 authors = ["deskent <battenetciz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
+repository = "https://github.com/Deskent/redis_async_client"
+homepage = "https://pypi.org/project/redis-async-client/"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 redis = "^5.0.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
```

### Comparing `redis_async_client-0.1.1/src/redis_async_client/__init__.py` & `redis_async_client-0.1.2/src/redis_async_client/__init__.py`

 * *Files identical despite different names*

### Comparing `redis_async_client-0.1.1/src/redis_async_client/core/async_client.py` & `redis_async_client-0.1.2/src/redis_async_client/core/async_client.py`

 * *Files identical despite different names*

### Comparing `redis_async_client-0.1.1/src/redis_async_client/core/base.py` & `redis_async_client-0.1.2/src/redis_async_client/core/base.py`

 * *Files identical despite different names*

### Comparing `redis_async_client-0.1.1/src/redis_async_client/core/settings.py` & `redis_async_client-0.1.2/src/redis_async_client/core/settings.py`

 * *Files identical despite different names*

### Comparing `redis_async_client-0.1.1/PKG-INFO` & `redis_async_client-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: redis-async-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Redis async client.
+Home-page: https://pypi.org/project/redis-async-client/
 License: MIT
 Author: deskent
 Author-email: battenetciz@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: redis (>=5.0.3,<6.0.0)
+Project-URL: Repository, https://github.com/Deskent/redis_async_client
 Description-Content-Type: text/markdown
 
 ### Installation
 
     pip install redis-async-client
 
 ### Usage Async
```

