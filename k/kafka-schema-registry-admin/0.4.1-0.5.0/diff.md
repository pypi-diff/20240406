# Comparing `tmp/kafka_schema_registry_admin-0.4.1.tar.gz` & `tmp/kafka_schema_registry_admin-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_schema_registry_admin-0.4.1.tar", max compression
+gzip compressed data, was "kafka_schema_registry_admin-0.5.0.tar", max compression
```

## Comparing `kafka_schema_registry_admin-0.4.1.tar` & `kafka_schema_registry_admin-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0    11358 2024-03-09 18:55:10.060282 kafka_schema_registry_admin-0.4.1/LICENSE
--rw-r--r--   0        0        0      767 2024-03-09 18:55:10.060282 kafka_schema_registry_admin-0.4.1/README.rst
--rw-r--r--   0        0        0      401 2024-03-10 20:22:40.515006 kafka_schema_registry_admin-0.4.1/kafka_schema_registry_admin/__init__.py
--rw-r--r--   0        0        0     2810 2024-03-10 14:02:08.645495 kafka_schema_registry_admin-0.4.1/kafka_schema_registry_admin/client_wrapper/__init__.py
--rw-r--r--   0        0        0     4086 2024-03-10 20:22:33.804138 kafka_schema_registry_admin-0.4.1/kafka_schema_registry_admin/client_wrapper/errors.py
--rw-r--r--   0        0        0    14774 2024-03-10 20:22:33.804138 kafka_schema_registry_admin-0.4.1/kafka_schema_registry_admin/kafka_schema_registry_admin.py
--rw-r--r--   0        0        0     1662 2024-03-10 20:22:40.515006 kafka_schema_registry_admin-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     1481 1970-01-01 00:00:00.000000 kafka_schema_registry_admin-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-09 18:55:10.060282 kafka_schema_registry_admin-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1240 2024-03-10 20:28:07.462628 kafka_schema_registry_admin-0.5.0/README.rst
+-rw-r--r--   0        0        0      831 2024-04-06 17:19:13.657617 kafka_schema_registry_admin-0.5.0/kafka_schema_registry_admin/__init__.py
+-rw-r--r--   0        0        0    17944 2024-04-06 17:18:24.238586 kafka_schema_registry_admin-0.5.0/kafka_schema_registry_admin/async_schema_registry.py
+-rw-r--r--   0        0        0     2868 2024-04-06 17:18:24.239586 kafka_schema_registry_admin-0.5.0/kafka_schema_registry_admin/client_wrapper/__init__.py
+-rw-r--r--   0        0        0     3731 2024-04-06 17:18:24.239586 kafka_schema_registry_admin-0.5.0/kafka_schema_registry_admin/client_wrapper/async_client.py
+-rw-r--r--   0        0        0     4086 2024-04-06 17:18:24.239586 kafka_schema_registry_admin-0.5.0/kafka_schema_registry_admin/client_wrapper/errors.py
+-rw-r--r--   0        0        0    14341 2024-04-06 17:18:24.239586 kafka_schema_registry_admin-0.5.0/kafka_schema_registry_admin/kafka_schema_registry_admin.py
+-rw-r--r--   0        0        0     1707 2024-04-06 17:19:13.658617 kafka_schema_registry_admin-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1994 1970-01-01 00:00:00.000000 kafka_schema_registry_admin-0.5.0/PKG-INFO
```

### Comparing `kafka_schema_registry_admin-0.4.1/LICENSE` & `kafka_schema_registry_admin-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kafka_schema_registry_admin-0.4.1/kafka_schema_registry_admin/client_wrapper/__init__.py` & `kafka_schema_registry_admin-0.5.0/kafka_schema_registry_admin/client_wrapper/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: Apache License 2.0
-# Copyright 2021 John Mille <john@ews-network.net>
+# Copyright 2024 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from requests import Response
@@ -30,55 +30,56 @@
         }
         self.auth = None
         if basic_auth:
             self.auth = (
                 basic_auth["basic_auth.username"],
                 basic_auth["basic_auth.password"],
             )
+        self.session = requests.Session()
 
     @evaluate_api_return
     def get(self, api_path: str, *args, **kwargs) -> Response:
         """Get the data from the api_path"""
         headers = kwargs.get("headers", {})
         if not headers:
             kwargs["headers"] = headers
         headers.update(self._default_headers)
         url: str = urlparse(self._base_url + api_path).geturl()
 
-        response = requests.get(url, auth=self.auth, *args, **kwargs)
+        response = self.session.get(url, auth=self.auth, *args, **kwargs)
         return response
 
     @evaluate_api_return
     def post(self, api_path: str, *args, **kwargs) -> Response:
         """POST the data from the api_path"""
         headers = kwargs.get("headers", {})
         if not headers:
             kwargs["headers"] = headers
         headers.update(self._default_headers)
         headers.update(self._post_headers)
         url: str = urlparse(self._base_url + api_path).geturl()
-        response = requests.post(url, auth=self.auth, *args, **kwargs)
+        response = self.session.post(url, auth=self.auth, *args, **kwargs)
         return response
 
     @evaluate_api_return
     def put(self, api_path: str, *args, **kwargs) -> Response:
         """PUT the data from the api_path"""
         headers = kwargs.get("headers", {})
         if not headers:
             kwargs["headers"] = headers
         headers.update(self._default_headers)
         url: str = urlparse(self._base_url + api_path).geturl()
 
-        response = requests.put(url, auth=self.auth, *args, **kwargs)
+        response = self.session.put(url, auth=self.auth, *args, **kwargs)
         return response
 
     @evaluate_api_return
     def delete(self, api_path: str, *args, **kwargs) -> Response:
         """DELETE the data from the api_path"""
         headers = kwargs.get("headers", {})
         if not headers:
             kwargs["headers"] = headers
         headers.update(self._default_headers)
 
         url: str = urlparse(self._base_url + api_path).geturl()
-        response = requests.delete(url, auth=self.auth, *args, **kwargs)
+        response = self.session.delete(url, auth=self.auth, *args, **kwargs)
         return response
```

### Comparing `kafka_schema_registry_admin-0.4.1/kafka_schema_registry_admin/client_wrapper/errors.py` & `kafka_schema_registry_admin-0.5.0/kafka_schema_registry_admin/client_wrapper/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # SPDX-License-Identifier: Apache License 2.0
-# Copyright 2021 John Mille <john@ews-network.net>
+# Copyright 2024 John Mille <john@ews-network.net>
 
 from __future__ import annotations
 
 import functools
 from typing import TYPE_CHECKING, Any
 
 from requests import exceptions as req_exceptions
```

### Comparing `kafka_schema_registry_admin-0.4.1/kafka_schema_registry_admin/kafka_schema_registry_admin.py` & `kafka_schema_registry_admin-0.5.0/kafka_schema_registry_admin/kafka_schema_registry_admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,55 +1,34 @@
 # SPDX-License-Identifier: Apache License 2.0
-# Copyright 2021 John Mille <john@ews-network.net>
+# Copyright 2024 John Mille <john@ews-network.net>
 
 """
 Main module for schema_registry_admin
 """
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
+from . import CompatibilityMode, RegistryMode, Type
+
 if TYPE_CHECKING:
     from requests import Response
 
 import json
-from enum import Enum
 from logging import getLogger
 from urllib.parse import urlencode
 
 from .client_wrapper import Client
 from .client_wrapper.errors import NotFoundException
 
 LOG = getLogger()
 LOG.setLevel("WARN")
 
 
-class Type(Enum):
-    AVRO = "AVRO"
-    JSON = "JSON"
-    PROTOBUFF = "PROTOBUF"
-
-
-class RegistryMode(Enum):
-    IMPORT = "IMPORT"
-    READONLY = "READONLY"
-    READWRITE = "READWRITE"
-
-
-class CompatibilityMode(Enum):
-    BACKWARD = "BACKWARD"
-    BACKWARD_TRANSITIVE = "BACKWARD_TRANSITIVE"
-    FORWARD = "FORWARD"
-    FORWARD_TRANSITIVE = "FORWARD_TRANSITIVE"
-    FULL = "FULL"
-    FULL_TRANSITIVE = "FULL_TRANSITIVE"
-    NONE = "NONE"
-
-
 class SchemaRegistry:
 
     def __init__(self, base_url: str, *args, **kwargs):
         username = kwargs.get("basic_auth.username", None)
         password = kwargs.get("basic_auth.password", None)
         basic_auth: dict = {}
         if username and password:
@@ -80,15 +59,14 @@
             url_path += "?" + urlencode(
                 {"subjectPrefix": subject_prefix, "deleted": "true"}
             )
         elif subject_prefix:
             url_path += f"?subjectPrefix={subject_prefix}"
         elif deleted:
             url_path += f"?deleted=true"
-        print(url_path)
         return self.client.get(url_path)
 
     def get_subject_versions(self, subject_name: str) -> Response:
         """
         Method to get the list of subjects in the schema registry
         https://docs.confluent.io/platform/current/schema-registry/develop/api.html#get--subjects-(string-%20subject)-versions
         """
```

### Comparing `kafka_schema_registry_admin-0.4.1/pyproject.toml` & `kafka_schema_registry_admin-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "kafka-schema-registry-admin"
-version = "0.4.1"
+version = "0.5.0"
 description = "Pure HTTP client to manage schemas in Schema Registry"
 authors = ["John Preston <john@ews-network.net>"]
 license = "Apache License 2.0"
 classifiers = [
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
@@ -16,34 +16,36 @@
         "Programming Language :: Python :: 3.11",
     ]
 readme = "README.rst"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.28.0"
+httpx = "^0.27.0"
 
 [tool.poetry.group.dev.dependencies]
 testcontainers = "^4.0.0"
 black = "^24"
 isort = "^5.10.1"
 coverage = "^7.4"
 Sphinx = "^7.2"
 pre-commit = "^3.6"
 pytest = "^8.1"
 tbump = "^6.9.0"
+pytest-asyncio = "^0.23.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/kafka_schema_registry_admin"
 
 [tool.tbump.version]
-current = "0.4.1"
+current = "0.5.0"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `kafka_schema_registry_admin-0.4.1/PKG-INFO` & `kafka_schema_registry_admin-0.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 Metadata-Version: 2.1
 Name: kafka-schema-registry-admin
-Version: 0.4.1
+Version: 0.5.0
 Summary: Pure HTTP client to manage schemas in Schema Registry
 License: Apache-2.0
 Author: John Preston
 Author-email: john@ews-network.net
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Description-Content-Type: text/x-rst
 
 ===========================
 Kafka schema registry admin
 ===========================
 
 Simple / light HTTP client library (using requests) to manipulate schemas and definitions into Schema Registry.
 
 * Confluent API specification is documented `here <https://docs.confluent.io/platform/current/schema-registry/develop/api.html#overview>`__
 
 * RedPanda API specification is documented `here <https://docs.redpanda.com/current/manage/schema-reg/schema-reg-api/>`__
 
+.. warning::
+
+    RedPanda SR does not have 100% compatibility with Confluent's.
+    Confluent Cloud specific endpoints not implemented (and no plans to be).
+
 
 Usage
 ======
 
 Very simple example to manipulate the schema registry and its resources.
+Every function returns the ``requests.Response`` object to allow you to implement any kind of logic from there,
+instead of trying to implement it for you.
+
+Non 2xx HTTP codes raise exceptions which are in the ``kafka_schema_registry_admin.client_wrapper.errors``
+More specific exceptions will be created in due course to identify exact exceptions.
 
 .. code-block::
 
     from kafka_schema_registry_admin import SchemaRegistry
 
     registry = SchemaRegistry("http://localhost:8081")
-    subjects = registry.get_all_subjects()
-    schemas = registry.get_all_schemas()
+    subjects = registry.get_all_subjects().json()
```

