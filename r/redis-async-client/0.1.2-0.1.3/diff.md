# Comparing `tmp/redis_async_client-0.1.2.tar.gz` & `tmp/redis_async_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_async_client-0.1.2.tar", max compression
+gzip compressed data, was "redis_async_client-0.1.3.tar", max compression
```

## Comparing `redis_async_client-0.1.2.tar` & `redis_async_client-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      708 2024-04-06 07:13:32.873711 redis_async_client-0.1.2/README.md
--rw-r--r--   0        0        0     2223 2024-04-06 07:48:23.101942 redis_async_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      572 2024-04-06 07:12:05.938369 redis_async_client-0.1.2/src/redis_async_client/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 06:39:15.440450 redis_async_client-0.1.2/src/redis_async_client/core/__init__.py
--rw-r--r--   0        0        0       54 2024-04-06 06:50:20.561420 redis_async_client-0.1.2/src/redis_async_client/core/_constants.py
--rw-r--r--   0        0        0       87 2024-04-06 06:50:39.109227 redis_async_client-0.1.2/src/redis_async_client/core/_types.py
--rw-r--r--   0        0        0     3288 2024-04-06 07:23:31.183455 redis_async_client-0.1.2/src/redis_async_client/core/async_client.py
--rw-r--r--   0        0        0     3868 2024-04-06 07:35:53.716381 redis_async_client-0.1.2/src/redis_async_client/core/base.py
--rw-r--r--   0        0        0       53 2024-04-06 06:50:20.561420 redis_async_client-0.1.2/src/redis_async_client/core/exc.py
--rw-r--r--   0        0        0       66 2024-04-06 06:50:39.113227 redis_async_client-0.1.2/src/redis_async_client/core/logger.py
--rw-r--r--   0        0        0      756 2024-04-06 07:37:40.647441 redis_async_client-0.1.2/src/redis_async_client/core/settings.py
--rw-r--r--   0        0        0     1301 1970-01-01 00:00:00.000000 redis_async_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      704 2024-04-06 07:54:06.206659 redis_async_client-0.1.3/README.md
+-rw-r--r--   0        0        0     2223 2024-04-06 08:03:28.645307 redis_async_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      653 2024-04-06 08:04:14.972887 redis_async_client-0.1.3/src/redis_async_client/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 06:39:15.440450 redis_async_client-0.1.3/src/redis_async_client/core/__init__.py
+-rw-r--r--   0        0        0     3869 2024-04-06 08:03:13.985441 redis_async_client-0.1.3/src/redis_async_client/core/_base.py
+-rw-r--r--   0        0        0       54 2024-04-06 08:00:40.522853 redis_async_client-0.1.3/src/redis_async_client/core/_constants.py
+-rw-r--r--   0        0        0       66 2024-04-06 06:50:39.113227 redis_async_client-0.1.3/src/redis_async_client/core/_logger.py
+-rw-r--r--   0        0        0       87 2024-04-06 07:58:23.004145 redis_async_client-0.1.3/src/redis_async_client/core/_types.py
+-rw-r--r--   0        0        0     3290 2024-04-06 08:04:13.056904 redis_async_client-0.1.3/src/redis_async_client/core/async_client.py
+-rw-r--r--   0        0        0       53 2024-04-06 06:50:20.561420 redis_async_client-0.1.3/src/redis_async_client/core/exc.py
+-rw-r--r--   0        0        0      760 2024-04-06 08:03:13.477445 redis_async_client-0.1.3/src/redis_async_client/core/settings.py
+-rw-r--r--   0        0        0     1297 1970-01-01 00:00:00.000000 redis_async_client-0.1.3/PKG-INFO
```

### Comparing `redis_async_client-0.1.2/README.md` & `redis_async_client-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,14 +10,14 @@
     pool: redis_async.ConnectionPool = redis_settings.make_pool()
     async with redis_async.Redis(connection_pool=pool) as conn:
         async_client = AsyncRedisClient(conn)
         data = await async_client.health_check()
         assert data == {'test': 'test'}
 
     or
-    
+
     from redis_async_client import RedisSettings, get_redis_connection
 
     redis_settings = RedisSettings()
     async for client in get_redis_connection(redis_settings):
         data = await client.health_check()
         assert data == {'test': 'test'}
```

### Comparing `redis_async_client-0.1.2/pyproject.toml` & `redis_async_client-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redis-async-client"
-version = "0.1.2"
+version = "0.1.3"
 description = "Redis async client."
 authors = ["deskent <battenetciz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Deskent/redis_async_client"
 homepage = "https://pypi.org/project/redis-async-client/"
```

### Comparing `redis_async_client-0.1.2/src/redis_async_client/__init__.py` & `redis_async_client-0.1.3/src/redis_async_client/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import AsyncGenerator
 
 from redis import asyncio as redis_async
 
 from .core.async_client import AsyncRedisClient
+from .core.exc import RedisAsyncClientException
 from .core.settings import RedisSettings
 
 
 __all__ = (
     "AsyncRedisClient",
     "RedisSettings",
+    "RedisAsyncClientException",
     "get_redis_connection",
 )
 
 
 async def get_redis_connection(
     redis_settings: RedisSettings,
 ) -> AsyncGenerator[AsyncRedisClient, None]:
```

### Comparing `redis_async_client-0.1.2/src/redis_async_client/core/async_client.py` & `redis_async_client-0.1.3/src/redis_async_client/core/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Any
 
-from ._constants import STORE_TIME_SEC
-from ._types import JSON
-from .base import (
+from ._base import (
     AppendOperator,
     DeleteOperator,
     LoadOperator,
     RedisBase,
     SaveOperator,
     UpdateOperator,
 )
-from .logger import logger
+from ._constants import STORE_TIME_SEC
+from ._logger import logger
+from ._types import JSON
 
 
 class AsyncRedisClient(RedisBase):
     """
     Class for work with Redis database
 
         Methods:
```

### Comparing `redis_async_client-0.1.2/src/redis_async_client/core/base.py` & `redis_async_client-0.1.3/src/redis_async_client/core/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 from abc import abstractmethod
 
 from redis.asyncio import Redis
 
 from ._constants import STORE_TIME_SEC
+from ._logger import logger
 from ._types import JSON
 from .exc import RedisAsyncClientException
-from .logger import logger
 
 
 class RedisBase:
     """Store data in redis.
 
     Attributes:
```

### Comparing `redis_async_client-0.1.2/src/redis_async_client/core/settings.py` & `redis_async_client-0.1.3/src/redis_async_client/core/settings.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import dataclasses
 
 import redis
 
 
 @dataclasses.dataclass
 class RedisSettings:
-    """Redis settings class.
+    """Redis settings dataclass.
 
     Attributes:
 
         REDIS_HOST: str = '127.0.0.1'
 
         REDIS_PORT: int = 6379
```

### Comparing `redis_async_client-0.1.2/PKG-INFO` & `redis_async_client-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-async-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: Redis async client.
 Home-page: https://pypi.org/project/redis-async-client/
 License: MIT
 Author: deskent
 Author-email: battenetciz@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -27,15 +27,15 @@
     pool: redis_async.ConnectionPool = redis_settings.make_pool()
     async with redis_async.Redis(connection_pool=pool) as conn:
         async_client = AsyncRedisClient(conn)
         data = await async_client.health_check()
         assert data == {'test': 'test'}
 
     or
-    
+
     from redis_async_client import RedisSettings, get_redis_connection
 
     redis_settings = RedisSettings()
     async for client in get_redis_connection(redis_settings):
         data = await client.health_check()
         assert data == {'test': 'test'}
```

