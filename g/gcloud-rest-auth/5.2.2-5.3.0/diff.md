# Comparing `tmp/gcloud_rest_auth-5.2.2.tar.gz` & `tmp/gcloud_rest_auth-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud_rest_auth-5.2.2.tar", max compression
+gzip compressed data, was "gcloud_rest_auth-5.3.0.tar", max compression
```

## Comparing `gcloud_rest_auth-5.2.2.tar` & `gcloud_rest_auth-5.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2024-03-14 13:48:37.000000 gcloud_rest_auth-5.2.2/LICENSE
--rw-r--r--   0        0        0     2048 2024-03-14 13:48:37.000000 gcloud_rest_auth-5.2.2/README.rst
--rw-r--r--   0        0        0        0 2024-03-14 13:48:37.000000 gcloud_rest_auth-5.2.2/gcloud/py.typed
--rw-r--r--   0        0        0     5643 2024-03-14 13:48:38.000000 gcloud_rest_auth-5.2.2/gcloud/rest/auth/__init__.py
--rw-r--r--   0        0        0      184 2024-03-14 13:48:38.000000 gcloud_rest_auth-5.2.2/gcloud/rest/auth/build_constants.py
--rw-r--r--   0        0        0     5254 2024-03-14 13:48:38.000000 gcloud_rest_auth-5.2.2/gcloud/rest/auth/iam.py
--rw-r--r--   0        0        0        0 2024-03-14 13:48:37.000000 gcloud_rest_auth-5.2.2/gcloud/rest/auth/py.typed
--rw-r--r--   0        0        0    14778 2024-03-14 13:48:38.000000 gcloud_rest_auth-5.2.2/gcloud/rest/auth/session.py
--rw-r--r--   0        0        0    18455 2024-03-14 13:48:38.000000 gcloud_rest_auth-5.2.2/gcloud/rest/auth/token.py
--rw-r--r--   0        0        0      735 2024-03-14 13:48:38.000000 gcloud_rest_auth-5.2.2/gcloud/rest/auth/utils.py
--rw-r--r--   0        0        0        0 2024-03-14 13:48:37.000000 gcloud_rest_auth-5.2.2/gcloud/rest/py.typed
--rw-r--r--   0        0        0     1152 2024-03-14 13:48:37.000000 gcloud_rest_auth-5.2.2/pyproject.toml
--rw-r--r--   0        0        0     3134 1970-01-01 00:00:00.000000 gcloud_rest_auth-5.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-04 13:26:06.000000 gcloud_rest_auth-5.3.0/LICENSE
+-rw-r--r--   0        0        0     2048 2024-04-04 13:26:06.000000 gcloud_rest_auth-5.3.0/README.rst
+-rw-r--r--   0        0        0        0 2024-04-04 13:26:06.000000 gcloud_rest_auth-5.3.0/gcloud/py.typed
+-rw-r--r--   0        0        0     5643 2024-04-04 13:26:07.000000 gcloud_rest_auth-5.3.0/gcloud/rest/auth/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-04 13:26:07.000000 gcloud_rest_auth-5.3.0/gcloud/rest/auth/build_constants.py
+-rw-r--r--   0        0        0     5254 2024-04-04 13:26:07.000000 gcloud_rest_auth-5.3.0/gcloud/rest/auth/iam.py
+-rw-r--r--   0        0        0        0 2024-04-04 13:26:06.000000 gcloud_rest_auth-5.3.0/gcloud/rest/auth/py.typed
+-rw-r--r--   0        0        0    15336 2024-04-04 13:26:07.000000 gcloud_rest_auth-5.3.0/gcloud/rest/auth/session.py
+-rw-r--r--   0        0        0    18455 2024-04-04 13:26:07.000000 gcloud_rest_auth-5.3.0/gcloud/rest/auth/token.py
+-rw-r--r--   0        0        0      735 2024-04-04 13:26:07.000000 gcloud_rest_auth-5.3.0/gcloud/rest/auth/utils.py
+-rw-r--r--   0        0        0        0 2024-04-04 13:26:06.000000 gcloud_rest_auth-5.3.0/gcloud/rest/py.typed
+-rw-r--r--   0        0        0     1152 2024-04-04 13:26:06.000000 gcloud_rest_auth-5.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3134 1970-01-01 00:00:00.000000 gcloud_rest_auth-5.3.0/PKG-INFO
```

### Comparing `gcloud_rest_auth-5.2.2/LICENSE` & `gcloud_rest_auth-5.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-5.2.2/README.rst` & `gcloud_rest_auth-5.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-5.2.2/gcloud/rest/auth/__init__.py` & `gcloud_rest_auth-5.3.0/gcloud/rest/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-5.2.2/gcloud/rest/auth/iam.py` & `gcloud_rest_auth-5.3.0/gcloud/rest/auth/iam.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-5.2.2/gcloud/rest/auth/session.py` & `gcloud_rest_auth-5.3.0/gcloud/rest/auth/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import importlib.metadata
 import logging
 import threading
+import warnings
 from abc import ABCMeta
 from abc import abstractmethod
 from abc import abstractproperty
 from typing import Any
 from typing import AnyStr
 from typing import IO
 from typing import Mapping
@@ -50,14 +51,15 @@
         pass
 
     @abstractmethod
     def get(
         self, url: str, headers: Optional[Mapping[str, str]],
         timeout: float, params: Optional[Mapping[str, Union[int, str]]],
         stream: bool,
+        auto_decompress: bool,
     ) -> Response:
         pass
 
     @abstractmethod
     def patch(
         self, url: str, headers: Mapping[str, str],
         data: Optional[Union[bytes, str]], timeout: float,
@@ -194,27 +196,29 @@
 
         def get(  # type: ignore[override]
             self, url: str,
             headers: Optional[Mapping[str, str]] = None,
             timeout: Timeout = 10,
             params: Optional[Mapping[str, Union[int, str]]] = None,
             stream: Optional[bool] = None,
+            auto_decompress: bool = True,
         ) -> aiohttp.ClientResponse:
             if not isinstance(timeout, aiohttp.ClientTimeout):
                 timeout = aiohttp.ClientTimeout(total=timeout)
 
             if stream is not None:
                 log.warning(
                     'passed unused argument stream=%s to AioSession: '
                     'this argument is only used by SyncSession',
                     stream,
                 )
             resp = self.session.get(
                 url, headers=headers,
                 timeout=timeout, params=params,
+                auto_decompress=auto_decompress,
             )
             _raise_for_status(resp)
             return resp
 
         def patch(  # type: ignore[override]
             self, url: str, headers: Mapping[str, str],
             data: Optional[Union[bytes, str]] = None,
@@ -331,15 +335,25 @@
             return resp
 
         def get(
             self, url: str, headers: Optional[Mapping[str, str]] = None,
             timeout: float = 10,
             params: Optional[Mapping[str, Union[int, str]]] = None,
             stream: bool = False,
+            auto_decompress: bool = True,
         ) -> Response:
+            if not auto_decompress and not stream:
+                warnings.warn(
+                    'the requests library always decompresses responses when '
+                    'outside of streaming mode; when audo_decompress is '
+                    'False, stream = True must also be set',
+                    UserWarning,
+                )
+                stream = True
+
             with self.google_api_lock:
                 resp = self.session.get(
                     url, headers=headers, timeout=timeout,
                     params=params, stream=stream,
                 )
             resp.raise_for_status()
             return resp
```

### Comparing `gcloud_rest_auth-5.2.2/gcloud/rest/auth/token.py` & `gcloud_rest_auth-5.3.0/gcloud/rest/auth/token.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-5.2.2/gcloud/rest/auth/utils.py` & `gcloud_rest_auth-5.3.0/gcloud/rest/auth/utils.py`

 * *Files identical despite different names*

### Comparing `gcloud_rest_auth-5.2.2/pyproject.toml` & `gcloud_rest_auth-5.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcloud-rest-auth"
-version = "5.2.2"
+version = "5.3.0"
 description = "Python Client for Google Cloud Auth"
 readme = "README.rst"
 
 repository = "https://github.com/talkiq/gcloud-aio"
 authors = ["Vi Engineering <voiceai-eng@dialpad.com>"]
 license = "MIT"
 
@@ -27,16 +27,16 @@
 # See https://cryptography.io/en/latest/api-stability/#deprecation
 cryptography = ">= 2.0.0, < 45.0.0"  # pin max to < (major + 3)
 pyjwt = ">= 1.5.3, < 3.0.0"
 requests = ">= 2.2.1, < 3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "8.1.1"
-# pytest-asyncio = "0.23.5"
-pytest-mock = "3.12.0"
+# pytest-asyncio = "0.23.6"
+pytest-mock = "3.14.0"
 
 [[tool.poetry.source]]
 name = "pypi"
 priority = "primary"
 
 [tool.pytest.ini_options]
 # addopts = "-Werror"  # TODO: fixme
```

### Comparing `gcloud_rest_auth-5.2.2/PKG-INFO` & `gcloud_rest_auth-5.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloud-rest-auth
-Version: 5.2.2
+Version: 5.3.0
 Summary: Python Client for Google Cloud Auth
 Home-page: https://github.com/talkiq/gcloud-aio
 License: MIT
 Author: Vi Engineering
 Author-email: voiceai-eng@dialpad.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

