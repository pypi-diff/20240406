# Comparing `tmp/auth_lib_profcomff-2023.8.6.tar.gz` & `tmp/auth_lib_profcomff-2024.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auth_lib_profcomff-2023.8.6.tar", last modified: Sun Aug  6 04:25:14 2023, max compression
+gzip compressed data, was "auth_lib_profcomff-2024.4.6.tar", last modified: Sat Apr  6 17:59:02 2024, max compression
```

## Comparing `auth_lib_profcomff-2023.8.6.tar` & `auth_lib_profcomff-2024.4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:25:14.664361 auth_lib_profcomff-2023.8.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-08-06 04:25:14.664361 auth_lib_profcomff-2023.8.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:25:14.664361 auth_lib_profcomff-2023.8.6/auth_lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/aiomethods.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:25:14.664361 auth_lib_profcomff-2023.8.6/auth_lib/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/auth_lib/testing/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-06 04:25:14.664361 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-08-06 04:25:14.000000 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-08-06 04:25:14.000000 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-06 04:25:14.000000 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-06 04:25:14.000000 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-06 04:25:14.000000 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-06 04:25:14.000000 auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-06 04:25:14.664361 auth_lib_profcomff-2023.8.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-08-06 04:25:04.000000 auth_lib_profcomff-2023.8.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:59:02.596228 auth_lib_profcomff-2024.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-06 17:58:54.000000 auth_lib_profcomff-2024.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-06 17:59:02.596228 auth_lib_profcomff-2024.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5553 2024-04-06 17:58:54.000000 auth_lib_profcomff-2024.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:59:02.592229 auth_lib_profcomff-2024.4.6/auth_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 17:58:54.000000 auth_lib_profcomff-2024.4.6/auth_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-06 17:58:54.000000 auth_lib_profcomff-2024.4.6/auth_lib/aiomethods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-06 17:58:54.000000 auth_lib_profcomff-2024.4.6/auth_lib/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4072 2024-04-06 17:58:54.000000 auth_lib_profcomff-2024.4.6/auth_lib/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-04-06 17:58:54.000000 auth_lib_profcomff-2024.4.6/auth_lib/methods.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:59:02.592229 auth_lib_profcomff-2024.4.6/auth_lib/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-06 17:58:54.000000 auth_lib_profcomff-2024.4.6/auth_lib/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-06 17:58:54.000000 auth_lib_profcomff-2024.4.6/auth_lib/testing/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 17:59:02.592229 auth_lib_profcomff-2024.4.6/auth_lib_profcomff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-04-06 17:59:02.000000 auth_lib_profcomff-2024.4.6/auth_lib_profcomff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-06 17:59:02.000000 auth_lib_profcomff-2024.4.6/auth_lib_profcomff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 17:59:02.000000 auth_lib_profcomff-2024.4.6/auth_lib_profcomff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-06 17:59:02.000000 auth_lib_profcomff-2024.4.6/auth_lib_profcomff.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-06 17:59:02.000000 auth_lib_profcomff-2024.4.6/auth_lib_profcomff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 17:59:02.000000 auth_lib_profcomff-2024.4.6/auth_lib_profcomff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 17:59:02.596228 auth_lib_profcomff-2024.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-06 17:58:54.000000 auth_lib_profcomff-2024.4.6/setup.py
```

### Comparing `auth_lib_profcomff-2023.8.6/LICENSE` & `auth_lib_profcomff-2024.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.8.6/PKG-INFO` & `auth_lib_profcomff-2024.4.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,17 @@
-Metadata-Version: 2.1
-Name: auth_lib_profcomff
-Version: 2023.8.6
-Home-page: https://github.com/profcomff/auth-lib
-Author: Semyon Grigoriev
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-Provides-Extra: fastapi
-Provides-Extra: testing
-License-File: LICENSE
-
 # auth-lib
 Библиотека функций авторизации для микросервисов Твой ФФ!
 
 [![pypi](https://img.shields.io/pypi/dm/auth-lib-profcomff?label=PIP%20INSTALLS&style=for-the-badge)](https://pypi.org/project/auth-lib-profcomff)
 [![tg](https://img.shields.io/badge/telegram-Viribus%20unitis-brightgreen?style=for-the-badge&logo=telegram)](https://t.me/+eIMtCymYDepmN2Ey)
 
+
+## Функционал
+Хранение общих методов аутентификации и авторизации для бэкендов Твой ФФ
+
 ## Примеры использования
 ### FastAPI
 ```python
 from auth_lib.fastapi import UnionAuth
 from fastapi import APIRouter, Depends
 router = APIRouter(prefix="/...")
 
@@ -102,7 +95,12 @@
 def test3(client):
     """
     В этом тесте скоупов выдано не будет, библиотека будет проверять
     токен через АПИ
     """
     assert 2*2 == 4
 ```
+
+## Contributing 
+ - Основная [информация](https://github.com/profcomff/.github/wiki/%255Bdev%255D-Backend-%25D1%2580%25D0%25B0%25D0%25B7%25D1%2580%25D0%25B0%25D0%25B1%25D0%25BE%25D1%2582%25D0%25BA%25D0%25B0) по разработке наших приложений
+
+ - [Ссылка](https://github.com/profcomff/auth-lib/blob/main/CONTRIBUTING.md) на страницу с информацией по разработке auth-lib
```

### Comparing `auth_lib_profcomff-2023.8.6/README.md` & `auth_lib_profcomff-2024.4.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,35 @@
+Metadata-Version: 2.1
+Name: auth_lib_profcomff
+Version: 2024.4.6
+Home-page: https://github.com/profcomff/auth-lib
+Author: Semyon Grigoriev
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: aiohttp
+Provides-Extra: fastapi
+Requires-Dist: fastapi; extra == "fastapi"
+Requires-Dist: starlette; extra == "fastapi"
+Requires-Dist: pydantic; extra == "fastapi"
+Requires-Dist: pydantic_settings; extra == "fastapi"
+Provides-Extra: testing
+Requires-Dist: pytest; extra == "testing"
+
 # auth-lib
 Библиотека функций авторизации для микросервисов Твой ФФ!
 
 [![pypi](https://img.shields.io/pypi/dm/auth-lib-profcomff?label=PIP%20INSTALLS&style=for-the-badge)](https://pypi.org/project/auth-lib-profcomff)
 [![tg](https://img.shields.io/badge/telegram-Viribus%20unitis-brightgreen?style=for-the-badge&logo=telegram)](https://t.me/+eIMtCymYDepmN2Ey)
 
+
+## Функционал
+Хранение общих методов аутентификации и авторизации для бэкендов Твой ФФ
+
 ## Примеры использования
 ### FastAPI
 ```python
 from auth_lib.fastapi import UnionAuth
 from fastapi import APIRouter, Depends
 router = APIRouter(prefix="/...")
 
@@ -91,7 +113,12 @@
 def test3(client):
     """
     В этом тесте скоупов выдано не будет, библиотека будет проверять
     токен через АПИ
     """
     assert 2*2 == 4
 ```
+
+## Contributing 
+ - Основная [информация](https://github.com/profcomff/.github/wiki/%255Bdev%255D-Backend-%25D1%2580%25D0%25B0%25D0%25B7%25D1%2580%25D0%25B0%25D0%25B1%25D0%25BE%25D1%2582%25D0%25BA%25D0%25B0) по разработке наших приложений
+
+ - [Ссылка](https://github.com/profcomff/auth-lib/blob/main/CONTRIBUTING.md) на страницу с информацией по разработке auth-lib
```

### Comparing `auth_lib_profcomff-2023.8.6/auth_lib/aiomethods.py` & `auth_lib_profcomff-2024.4.6/auth_lib/aiomethods.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 from urllib.parse import urljoin
 
 import aiohttp
 
-from .exceptions import AuthFailed, IncorrectData, NotFound, SessionExpired
+from .exceptions import AuthFailed, SessionExpired
 
 # See docs on https://api.test.profcomff.com/?urls.primaryName=auth
 
 
 class AsyncAuthLib:
     auth_url: str
     userdata_url: str
@@ -30,20 +30,15 @@
 
     async def check_token(self, token: str) -> dict[str, Any] | None:
         headers = {"Authorization": token}
         async with aiohttp.request(
             "GET",
             urljoin(self.auth_url, "me"),
             headers={"Authorization": token},
-            params={
-                "info": [
-                    "indirect_groups",
-                    "session_scopes",
-                ]
-            },
+            params={"info": ["indirect_groups", "session_scopes", "user_scopes"]},
         ) as r:
             user_session = await r.json()
         if r.ok:
             return user_session
         return None
 
     async def logout(self, token: str) -> bool:
```

### Comparing `auth_lib_profcomff-2023.8.6/auth_lib/exceptions.py` & `auth_lib_profcomff-2024.4.6/auth_lib/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 class AuthError(Exception):
-    def __init__(self, *args, **kwargs):
-        super().__init__("Auth failed")
+    """Базовая ошибка библиотеки auth-lib"""
 
 
 class IncorrectData(AuthError):
     def __init__(self, response: dict):
         super().__init__(str(response))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `auth_lib_profcomff-2023.8.6/auth_lib/fastapi.py` & `auth_lib_profcomff-2024.4.6/auth_lib/fastapi.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.8.6/auth_lib/methods.py` & `auth_lib_profcomff-2024.4.6/auth_lib/methods.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any
 from urllib.parse import urljoin
 
 import requests
 
-from .exceptions import AuthFailed, IncorrectData, NotFound, SessionExpired
+from .exceptions import AuthFailed, SessionExpired
 
 # See docs on https://api.test.profcomff.com/?urls.primaryName=auth
 
 
 class AuthLib:
     auth_url: str
     userdata_url: str
```

### Comparing `auth_lib_profcomff-2023.8.6/auth_lib/testing/testutils.py` & `auth_lib_profcomff-2024.4.6/auth_lib/testing/testutils.py`

 * *Files identical despite different names*

### Comparing `auth_lib_profcomff-2023.8.6/auth_lib_profcomff.egg-info/PKG-INFO` & `auth_lib_profcomff-2024.4.6/auth_lib_profcomff.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,35 @@
 Metadata-Version: 2.1
-Name: auth-lib-profcomff
-Version: 2023.8.6
+Name: auth_lib_profcomff
+Version: 2024.4.6
 Home-page: https://github.com/profcomff/auth-lib
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+Requires-Dist: aiohttp
 Provides-Extra: fastapi
+Requires-Dist: fastapi; extra == "fastapi"
+Requires-Dist: starlette; extra == "fastapi"
+Requires-Dist: pydantic; extra == "fastapi"
+Requires-Dist: pydantic_settings; extra == "fastapi"
 Provides-Extra: testing
-License-File: LICENSE
+Requires-Dist: pytest; extra == "testing"
 
 # auth-lib
 Библиотека функций авторизации для микросервисов Твой ФФ!
 
 [![pypi](https://img.shields.io/pypi/dm/auth-lib-profcomff?label=PIP%20INSTALLS&style=for-the-badge)](https://pypi.org/project/auth-lib-profcomff)
 [![tg](https://img.shields.io/badge/telegram-Viribus%20unitis-brightgreen?style=for-the-badge&logo=telegram)](https://t.me/+eIMtCymYDepmN2Ey)
 
+
+## Функционал
+Хранение общих методов аутентификации и авторизации для бэкендов Твой ФФ
+
 ## Примеры использования
 ### FastAPI
 ```python
 from auth_lib.fastapi import UnionAuth
 from fastapi import APIRouter, Depends
 router = APIRouter(prefix="/...")
 
@@ -102,7 +113,12 @@
 def test3(client):
     """
     В этом тесте скоупов выдано не будет, библиотека будет проверять
     токен через АПИ
     """
     assert 2*2 == 4
 ```
+
+## Contributing 
+ - Основная [информация](https://github.com/profcomff/.github/wiki/%255Bdev%255D-Backend-%25D1%2580%25D0%25B0%25D0%25B7%25D1%2580%25D0%25B0%25D0%25B1%25D0%25BE%25D1%2582%25D0%25BA%25D0%25B0) по разработке наших приложений
+
+ - [Ссылка](https://github.com/profcomff/auth-lib/blob/main/CONTRIBUTING.md) на страницу с информацией по разработке auth-lib
```

### Comparing `auth_lib_profcomff-2023.8.6/setup.py` & `auth_lib_profcomff-2024.4.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as readme_file:
     readme = readme_file.read()
 
+
+with open("requirements.txt", "r", encoding="utf-8") as req_file:
+    req = req_file.read().split("\n")
+
+
 setup(
     name="auth_lib_profcomff",
-    version="2023.08.06",
+    version="2024.04.06",
     author="Semyon Grigoriev",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/profcomff/auth-lib",
     packages=find_packages(),
-    install_requires=["requests", "aiohttp", "setuptools"],
+    install_requires=req,
     extras_require={
         "fastapi": ["fastapi", "starlette", "pydantic", "pydantic_settings"],
         "testing": ["pytest"],
     },
     entry_points={"pytest11": ["pytest_auth_lib = auth_lib.testing"]},
     classifiers=[
         "Programming Language :: Python :: 3.11",
```

