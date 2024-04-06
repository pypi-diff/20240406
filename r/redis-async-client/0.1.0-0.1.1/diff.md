# Comparing `tmp/redis_async_client-0.1.0.tar.gz` & `tmp/redis_async_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_async_client-0.1.0.tar", max compression
+gzip compressed data, was "redis_async_client-0.1.1.tar", max compression
```

## Comparing `redis_async_client-0.1.0.tar` & `redis_async_client-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0      708 2024-04-06 07:13:32.873711 redis_async_client-0.1.0/README.md
--rw-r--r--   0        0        0     2104 2024-04-06 06:03:29.845240 redis_async_client-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      572 2024-04-06 07:12:05.938369 redis_async_client-0.1.0/src/redis_async_client/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 06:39:15.440450 redis_async_client-0.1.0/src/redis_async_client/core/__init__.py
--rw-r--r--   0        0        0       54 2024-04-06 06:50:20.561420 redis_async_client-0.1.0/src/redis_async_client/core/_constants.py
--rw-r--r--   0        0        0       87 2024-04-06 06:50:39.109227 redis_async_client-0.1.0/src/redis_async_client/core/_types.py
--rw-r--r--   0        0        0     3288 2024-04-06 07:23:31.183455 redis_async_client-0.1.0/src/redis_async_client/core/async_client.py
--rw-r--r--   0        0        0     3976 2024-04-06 07:18:11.059140 redis_async_client-0.1.0/src/redis_async_client/core/base.py
--rw-r--r--   0        0        0       53 2024-04-06 06:50:20.561420 redis_async_client-0.1.0/src/redis_async_client/core/exc.py
--rw-r--r--   0        0        0       66 2024-04-06 06:50:39.113227 redis_async_client-0.1.0/src/redis_async_client/core/logger.py
--rw-r--r--   0        0        0        1 2024-04-06 07:12:09.178345 redis_async_client-0.1.0/src/redis_async_client/core/maker.py
--rw-r--r--   0        0        0      765 2024-04-06 06:52:11.324299 redis_async_client-0.1.0/src/redis_async_client/core/settings.py
--rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 redis_async_client-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      708 2024-04-06 07:13:32.873711 redis_async_client-0.1.1/README.md
+-rw-r--r--   0        0        0     2104 2024-04-06 07:38:14.515145 redis_async_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      572 2024-04-06 07:12:05.938369 redis_async_client-0.1.1/src/redis_async_client/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 06:39:15.440450 redis_async_client-0.1.1/src/redis_async_client/core/__init__.py
+-rw-r--r--   0        0        0       54 2024-04-06 06:50:20.561420 redis_async_client-0.1.1/src/redis_async_client/core/_constants.py
+-rw-r--r--   0        0        0       87 2024-04-06 06:50:39.109227 redis_async_client-0.1.1/src/redis_async_client/core/_types.py
+-rw-r--r--   0        0        0     3288 2024-04-06 07:23:31.183455 redis_async_client-0.1.1/src/redis_async_client/core/async_client.py
+-rw-r--r--   0        0        0     3868 2024-04-06 07:35:53.716381 redis_async_client-0.1.1/src/redis_async_client/core/base.py
+-rw-r--r--   0        0        0       53 2024-04-06 06:50:20.561420 redis_async_client-0.1.1/src/redis_async_client/core/exc.py
+-rw-r--r--   0        0        0       66 2024-04-06 06:50:39.113227 redis_async_client-0.1.1/src/redis_async_client/core/logger.py
+-rw-r--r--   0        0        0      756 2024-04-06 07:37:40.647441 redis_async_client-0.1.1/src/redis_async_client/core/settings.py
+-rw-r--r--   0        0        0     1174 1970-01-01 00:00:00.000000 redis_async_client-0.1.1/PKG-INFO
```

### Comparing `redis_async_client-0.1.0/README.md` & `redis_async_client-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `redis_async_client-0.1.0/pyproject.toml` & `redis_async_client-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-async-client"
-version = "0.1.0"
+version = "0.1.1"
 description = "Redis async client."
 authors = ["deskent <battenetciz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `redis_async_client-0.1.0/src/redis_async_client/__init__.py` & `redis_async_client-0.1.1/src/redis_async_client/__init__.py`

 * *Files identical despite different names*

### Comparing `redis_async_client-0.1.0/src/redis_async_client/core/async_client.py` & `redis_async_client-0.1.1/src/redis_async_client/core/async_client.py`

 * *Files identical despite different names*

### Comparing `redis_async_client-0.1.0/src/redis_async_client/core/base.py` & `redis_async_client-0.1.1/src/redis_async_client/core/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from abc import abstractmethod
 
 from redis.asyncio import Redis
 
-from src.redis_async_client.core._constants import STORE_TIME_SEC
-from src.redis_async_client.core._types import JSON
-from src.redis_async_client.core.exc import RedisAsyncClientException
-from src.redis_async_client.core.logger import logger
+from ._constants import STORE_TIME_SEC
+from ._types import JSON
+from .exc import RedisAsyncClientException
+from .logger import logger
 
 
 class RedisBase:
     """Store data in redis.
 
     Attributes:
```

### Comparing `redis_async_client-0.1.0/src/redis_async_client/core/settings.py` & `redis_async_client-0.1.1/src/redis_async_client/core/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 
-import redis.asyncio as redis
+import redis
 
 
 @dataclasses.dataclass
 class RedisSettings:
     """Redis settings class.
 
     Attributes:
@@ -12,15 +12,15 @@
         REDIS_HOST: str = '127.0.0.1'
 
         REDIS_PORT: int = 6379
 
         REDIS_DB: int = 0
 
     Methods
-        get_url_by_name
+        get_url
 
         make_pool
 
     """
 
     REDIS_HOST: str = '127.0.0.1'
     REDIS_PORT: int = 6379
@@ -31,11 +31,11 @@
 
         redis_url: str = (
             f'redis://{self.REDIS_HOST}:{self.REDIS_PORT}/{self.REDIS_DB}'
         )
 
         return redis_url
 
-    def make_pool(self, url: str = '') -> redis.ConnectionPool:
+    def make_pool(self, url: str = '') -> redis.asyncio.ConnectionPool:
         if not url:
             url = self.get_url()
-        return redis.ConnectionPool.from_url(url)
+        return redis.asyncio.ConnectionPool.from_url(url)
```

### Comparing `redis_async_client-0.1.0/PKG-INFO` & `redis_async_client-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-async-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Redis async client.
 License: MIT
 Author: deskent
 Author-email: battenetciz@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

