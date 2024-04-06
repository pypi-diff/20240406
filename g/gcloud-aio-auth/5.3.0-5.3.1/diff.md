# Comparing `tmp/gcloud_aio_auth-5.3.0.tar.gz` & `tmp/gcloud_aio_auth-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcloud_aio_auth-5.3.0.tar", max compression
+gzip compressed data, was "gcloud_aio_auth-5.3.1.tar", max compression
```

## Comparing `gcloud_aio_auth-5.3.0.tar` & `gcloud_aio_auth-5.3.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1063 2024-04-04 13:29:52.859529 gcloud_aio_auth-5.3.0/LICENSE
--rw-r--r--   0        0        0     2039 2024-04-04 13:29:52.859529 gcloud_aio_auth-5.3.0/README.rst
--rw-r--r--   0        0        0     5666 2024-04-04 13:29:52.859529 gcloud_aio_auth-5.3.0/gcloud/aio/auth/__init__.py
--rw-r--r--   0        0        0      184 2024-04-04 13:29:52.859529 gcloud_aio_auth-5.3.0/gcloud/aio/auth/build_constants.py
--rw-r--r--   0        0        0     5377 2024-04-04 13:29:52.859529 gcloud_aio_auth-5.3.0/gcloud/aio/auth/iam.py
--rw-r--r--   0        0        0        0 2024-04-04 13:29:52.859529 gcloud_aio_auth-5.3.0/gcloud/aio/auth/py.typed
--rw-r--r--   0        0        0    15582 2024-04-04 13:29:52.859529 gcloud_aio_auth-5.3.0/gcloud/aio/auth/session.py
--rw-r--r--   0        0        0    18788 2024-04-04 13:29:52.859529 gcloud_aio_auth-5.3.0/gcloud/aio/auth/token.py
--rw-r--r--   0        0        0      735 2024-04-04 13:29:52.859529 gcloud_aio_auth-5.3.0/gcloud/aio/auth/utils.py
--rw-r--r--   0        0        0        0 2024-04-04 13:29:52.859529 gcloud_aio_auth-5.3.0/gcloud/aio/py.typed
--rw-r--r--   0        0        0        0 2024-04-04 13:29:52.859529 gcloud_aio_auth-5.3.0/gcloud/py.typed
--rw-r--r--   0        0        0     1147 2024-04-04 13:29:52.863529 gcloud_aio_auth-5.3.0/pyproject.toml
--rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 gcloud_aio_auth-5.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-06 12:34:44.831872 gcloud_aio_auth-5.3.1/LICENSE
+-rw-r--r--   0        0        0     2039 2024-04-06 12:34:44.831872 gcloud_aio_auth-5.3.1/README.rst
+-rw-r--r--   0        0        0     5666 2024-04-06 12:34:44.831872 gcloud_aio_auth-5.3.1/gcloud/aio/auth/__init__.py
+-rw-r--r--   0        0        0      184 2024-04-06 12:34:44.831872 gcloud_aio_auth-5.3.1/gcloud/aio/auth/build_constants.py
+-rw-r--r--   0        0        0     5377 2024-04-06 12:34:44.831872 gcloud_aio_auth-5.3.1/gcloud/aio/auth/iam.py
+-rw-r--r--   0        0        0        0 2024-04-06 12:34:44.831872 gcloud_aio_auth-5.3.1/gcloud/aio/auth/py.typed
+-rw-r--r--   0        0        0    15582 2024-04-06 12:34:44.831872 gcloud_aio_auth-5.3.1/gcloud/aio/auth/session.py
+-rw-r--r--   0        0        0    18788 2024-04-06 12:34:44.831872 gcloud_aio_auth-5.3.1/gcloud/aio/auth/token.py
+-rw-r--r--   0        0        0      735 2024-04-06 12:34:44.831872 gcloud_aio_auth-5.3.1/gcloud/aio/auth/utils.py
+-rw-r--r--   0        0        0        0 2024-04-06 12:34:44.831872 gcloud_aio_auth-5.3.1/gcloud/aio/py.typed
+-rw-r--r--   0        0        0        0 2024-04-06 12:34:44.831872 gcloud_aio_auth-5.3.1/gcloud/py.typed
+-rw-r--r--   0        0        0     1147 2024-04-06 12:34:44.831872 gcloud_aio_auth-5.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3123 1970-01-01 00:00:00.000000 gcloud_aio_auth-5.3.1/PKG-INFO
```

### Comparing `gcloud_aio_auth-5.3.0/LICENSE` & `gcloud_aio_auth-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-5.3.0/README.rst` & `gcloud_aio_auth-5.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-5.3.0/gcloud/aio/auth/__init__.py` & `gcloud_aio_auth-5.3.1/gcloud/aio/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-5.3.0/gcloud/aio/auth/iam.py` & `gcloud_aio_auth-5.3.1/gcloud/aio/auth/iam.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-5.3.0/gcloud/aio/auth/session.py` & `gcloud_aio_auth-5.3.1/gcloud/aio/auth/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -340,15 +340,15 @@
             params: Optional[Mapping[str, Union[int, str]]] = None,
             stream: bool = False,
             auto_decompress: bool = True,
         ) -> Response:
             if not auto_decompress and not stream:
                 warnings.warn(
                     'the requests library always decompresses responses when '
-                    'outside of streaming mode; when audo_decompress is '
+                    'outside of streaming mode; when auto_decompress is '
                     'False, stream = True must also be set',
                     UserWarning,
                 )
                 stream = True
 
             with self.google_api_lock:
                 resp = self.session.get(
```

### Comparing `gcloud_aio_auth-5.3.0/gcloud/aio/auth/token.py` & `gcloud_aio_auth-5.3.1/gcloud/aio/auth/token.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-5.3.0/gcloud/aio/auth/utils.py` & `gcloud_aio_auth-5.3.1/gcloud/aio/auth/utils.py`

 * *Files identical despite different names*

### Comparing `gcloud_aio_auth-5.3.0/pyproject.toml` & `gcloud_aio_auth-5.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gcloud-aio-auth"
-version = "5.3.0"
+version = "5.3.1"
 description = "Python Client for Google Cloud Auth"
 readme = "README.rst"
 
 repository = "https://github.com/talkiq/gcloud-aio"
 authors = ["Vi Engineering <voiceai-eng@dialpad.com>"]
 license = "MIT"
 
@@ -17,15 +17,15 @@
     'Intended Audience :: Developers',
     'Operating System :: OS Independent',
     'Topic :: Internet',
 ]
 
 [tool.poetry.dependencies]
 python = ">= 3.8, < 4.0"
-aiohttp = ">= 3.3.0, < 4.0.0"
+aiohttp = ">= 3.9.0, < 4.0.0"
 backoff = ">= 1.0.0, < 3.0.0"
 chardet = ">= 2.0, < 6.0"
 # See https://cryptography.io/en/latest/api-stability/#deprecation
 cryptography = ">= 2.0.0, < 45.0.0"  # pin max to < (major + 3)
 pyjwt = ">= 1.5.3, < 3.0.0"
 # requests = ">= 2.2.1, < 3.0.0"
```

### Comparing `gcloud_aio_auth-5.3.0/PKG-INFO` & `gcloud_aio_auth-5.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcloud-aio-auth
-Version: 5.3.0
+Version: 5.3.1
 Summary: Python Client for Google Cloud Auth
 Home-page: https://github.com/talkiq/gcloud-aio
 License: MIT
 Author: Vi Engineering
 Author-email: voiceai-eng@dialpad.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
-Requires-Dist: aiohttp (>=3.3.0,<4.0.0)
+Requires-Dist: aiohttp (>=3.9.0,<4.0.0)
 Requires-Dist: backoff (>=1.0.0,<3.0.0)
 Requires-Dist: chardet (>=2.0,<6.0)
 Requires-Dist: cryptography (>=2.0.0,<45.0.0)
 Requires-Dist: pyjwt (>=1.5.3,<3.0.0)
 Project-URL: Repository, https://github.com/talkiq/gcloud-aio
 Description-Content-Type: text/x-rst
```

