# Comparing `tmp/pyapi-server-0.4.1.tar.gz` & `tmp/pyapi_server-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapi-server-0.4.1.tar", last modified: Wed Oct 11 17:21:02 2023, max compression
+gzip compressed data, was "pyapi_server-0.5.0.tar", last modified: Fri Apr  5 22:59:05 2024, max compression
```

## Comparing `pyapi-server-0.4.1.tar` & `pyapi_server-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2023-10-11 17:20:50.124621 pyapi-server-0.4.1/README.md
--rw-r--r--   0        0        0     7535 2023-10-11 17:20:50.124621 pyapi-server-0.4.1/pyapi/server/__init__.py
--rw-r--r--   0        0        0        0 2023-10-11 17:20:50.124621 pyapi-server-0.4.1/pyapi/server/py.typed
--rw-r--r--   0        0        0     2551 2023-10-11 17:20:50.124621 pyapi-server-0.4.1/pyapi/server/spec.py
--rw-r--r--   0        0        0     3005 2023-10-11 17:20:50.124621 pyapi-server-0.4.1/pyapi/server/validation.py
--rw-r--r--   0        0        0     2758 2023-10-11 17:20:50.124621 pyapi-server-0.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-11 17:20:50.128621 pyapi-server-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0      402 2023-10-11 17:20:50.128621 pyapi-server-0.4.1/tests/conftest.py
--rw-r--r--   0        0        0      564 2023-10-11 17:20:50.128621 pyapi-server-0.4.1/tests/endpoints.py
--rw-r--r--   0        0        0     2737 2023-10-11 17:20:50.128621 pyapi-server-0.4.1/tests/openapi.json
--rw-r--r--   0        0        0        0 2023-10-11 17:20:50.128621 pyapi-server-0.4.1/tests/openapi.unknown
--rw-r--r--   0        0        0     1941 2023-10-11 17:20:50.128621 pyapi-server-0.4.1/tests/openapi.yaml
--rw-r--r--   0        0        0     1919 2023-10-11 17:20:50.128621 pyapi-server-0.4.1/tests/test_app.py
--rw-r--r--   0        0        0     3705 2023-10-11 17:20:50.128621 pyapi-server-0.4.1/tests/test_endpoints.py
--rw-r--r--   0        0        0     1765 2023-10-11 17:20:50.128621 pyapi-server-0.4.1/tests/test_service.py
--rw-r--r--   0        0        0      731 2023-10-11 17:20:50.128621 pyapi-server-0.4.1/tests/test_spec.py
--rw-r--r--   0        0        0     1564 1970-01-01 00:00:00.000000 pyapi-server-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-05 22:58:56.640256 pyapi_server-0.5.0/README.md
+-rw-r--r--   0        0        0     7402 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/pyapi/server/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/pyapi/server/py.typed
+-rw-r--r--   0        0        0     2520 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/pyapi/server/spec.py
+-rw-r--r--   0        0        0     3259 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/pyapi/server/validation.py
+-rw-r--r--   0        0        0     2625 2024-04-05 22:59:05.464253 pyapi_server-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      402 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0      560 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/endpoints.py
+-rw-r--r--   0        0        0     2737 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/openapi.json
+-rw-r--r--   0        0        0        0 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/openapi.unknown
+-rw-r--r--   0        0        0     1941 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/openapi.yaml
+-rw-r--r--   0        0        0     1919 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/test_app.py
+-rw-r--r--   0        0        0     3709 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/test_endpoints.py
+-rw-r--r--   0        0        0     1765 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/test_service.py
+-rw-r--r--   0        0        0      752 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/test_spec.py
+-rw-r--r--   0        0        0     1826 1970-01-01 00:00:00.000000 pyapi_server-0.5.0/PKG-INFO
```

### Comparing `pyapi-server-0.4.1/README.md` & `pyapi_server-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyapi-server-0.4.1/pyapi/server/__init__.py` & `pyapi_server-0.5.0/pyapi/server/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """PyAPI Server."""
+
 from __future__ import annotations
 
 from functools import wraps
 from http import HTTPStatus
 from importlib import import_module
 from inspect import iscoroutine
 from logging import getLogger
 from pathlib import Path
 from types import ModuleType
 from typing import Any, Callable, cast, Mapping, Optional, Union
 from urllib.parse import urlsplit
 
-from openapi_core import Spec, validate_request, validate_response
+from jsonschema_path import SchemaPath
+from openapi_core import validate_request, validate_response
 from openapi_core.exceptions import OpenAPIError
 from openapi_core.security.exceptions import SecurityProviderError
 from starlette.applications import Starlette
 from starlette.exceptions import HTTPException
 from stringcase import snakecase
 
 from .spec import get_spec_from_file, OperationSpec
@@ -25,31 +27,27 @@
 
 
 class Application(Starlette):
     """PyAPI server application."""
 
     def __init__(
         self,
-        spec: Union[Spec, dict],
+        spec: Union[SchemaPath, dict],
         *,
         module: Optional[Union[str, ModuleType]] = None,
-        validate_schema: bool = True,
         validate_responses: bool = True,
         enforce_case: bool = True,
         custom_format_validators: Optional[Mapping[str, Callable]] = None,
         spec_url: str = "",
         **kwargs,
     ):
         super().__init__(**kwargs)
         if isinstance(spec, dict):
-            extra_kwargs: dict[str, Any] = {}
-            if not validate_schema:
-                extra_kwargs["validator"] = None
-            spec = Spec.from_dict(spec, spec_url=spec_url, **extra_kwargs)
-        self.spec: Spec = spec
+            spec = SchemaPath.from_dict(spec, base_uri=spec_url)
+        self.spec: SchemaPath = spec
         self.validate_responses = validate_responses
         self.enforce_case = enforce_case
         self.custom_format_validators = custom_format_validators
 
         self._operations = OperationSpec.get_all(self.spec)
         self._server_paths = {urlsplit(server["url"]).path for server in self.spec["servers"]}
```

### Comparing `pyapi-server-0.4.1/pyapi/server/spec.py` & `pyapi_server-0.5.0/pyapi/server/spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """Utility classes and functions."""
+
 from __future__ import annotations
 
 import json
 from collections import defaultdict
 from enum import Enum
 from itertools import chain
 from pathlib import Path
-from typing import Callable, Dict, Mapping, Sequence, TYPE_CHECKING
+from typing import Callable, Dict, Mapping, Sequence
 
 import yaml
+from jsonschema_path import SchemaPath
 from stringcase import camelcase
 
-if TYPE_CHECKING:  # pragma: no cover
-    from . import Spec
-
 
 class OperationSpec:
     """Utility class for defining API operations."""
 
     def __init__(
         self, path: str, method: str, spec: dict, parameters: Mapping | Sequence | None = None
     ):
@@ -40,15 +39,15 @@
         if name in self.spec:
             return self.spec[name]
         if (camelcase_name := camelcase(name)) in self.spec:
             return self.spec[camelcase_name]
         return super().__getattribute__(name)
 
     @classmethod
-    def get_all(cls, spec: Spec) -> Dict[str, OperationSpec]:
+    def get_all(cls, spec: SchemaPath) -> Dict[str, OperationSpec]:
         """Builds a dict of all operations in the spec."""
         return {
             op_spec["operationId"]: cls(
                 path,
                 method,
                 op_spec,
                 path_spec.get("parameters", []) + op_spec.get("parameters", []),
```

### Comparing `pyapi-server-0.4.1/pyapi/server/validation.py` & `pyapi_server-0.5.0/pyapi/server/validation.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """OpenAPI request and response wrappers; adapted from openapi-core."""
+
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
 from typing import Optional, Union
 
 from openapi_core import protocols
 from openapi_core.validation.request.datatypes import RequestParameters
 from starlette.datastructures import Headers
@@ -45,41 +46,46 @@
 
     @property
     def method(self) -> str:
         """Return the request HTTP method."""
         return self.request.method.lower()
 
     @property
-    def body(self) -> Optional[str]:
+    def body(self) -> Optional[bytes]:
         """Return the request body as string, if present."""
-        if isinstance(self._body, bytes):
-            return self._body.decode("utf-8")
+        if isinstance(self._body, str):
+            return self._body.encode("utf-8")
         return self._body
 
     @property
     def mimetype(self) -> str:
         """Return the request content type."""
         content_type = self.request.headers.get("Content-Type")
         if content_type:
             return content_type.partition(";")[0]
 
         return ""
 
+    @property
+    def content_type(self) -> str:
+        """Return the request content type."""
+        return self.mimetype
+
 
 class OpenAPIResponse(protocols.Response):
     """Wrapper for PyAPI Server responses."""
 
     def __init__(self, response: Response):
         self.response = response
 
     @property
-    def data(self) -> str:
+    def data(self) -> bytes:
         """Return the response content as string."""
-        if isinstance(self.response.body, bytes):
-            return self.response.body.decode("utf-8")
+        if isinstance(self.response.body, str):
+            return self.response.body.encode("utf-8")
         return self.response.body
 
     @property
     def status_code(self) -> int:
         """Return the response HTTP status code."""
         return self.response.status_code
 
@@ -88,7 +94,12 @@
         """Return the response content type."""
         return self.response.media_type or ""
 
     @property
     def headers(self) -> Headers:
         """Return the response headers."""
         return self.response.headers
+
+    @property
+    def content_type(self) -> str:
+        """Return the response content type."""
+        return self.mimetype
```

### Comparing `pyapi-server-0.4.1/pyproject.toml` & `pyapi_server-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 [project]
 name = "pyapi-server"
-version = "0.4.1"
+version = "0.5.0"
 description = "Lightweight API framework using an OpenAPI spec for routing and validation."
 readme = "README.md"
 authors = [
     { name = "Berislav Lopac", email = "berislav@lopac.net" },
 ]
 requires-python = ">=3.8,<4.0"
 dependencies = [
     "PyYAML>=5.4",
     "stringcase>=1.2.0",
-    "openapi-core>=0.16.1",
+    "openapi-core>=0.18",
     "starlette>=0.21.0",
+    "jsonschema-path>=0.3.2",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://pyapi-server.readthedocs.io"
@@ -25,32 +26,31 @@
 [project.optional-dependencies]
 uvicorn = [
     "uvicorn>=0.18.3",
 ]
 
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [tool.pdm.build]
 includes = [
     "pyapi/server/",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
     "pytest-asyncio>=0.18.3",
     "pytest-cov>=3.0.0",
     "pytest-flake8>=1.1.1",
     "pytest-mypy>=0.9.1",
     "requests>=2.27.1",
     "pytest>=7.1.1",
-    "black>=22.1.0",
     "pydocstyle>=6.1.1",
     "mypy>=0.942",
     "toml>=0.10.2",
     "pytest-spec>=3.2.0",
     "isort>=5.10.1",
     "tox>=4.4.6",
     "tox-pdm>=0.6.1",
@@ -61,27 +61,26 @@
     "mkdocs-material>=8.5.6",
 ]
 
 [tool.pdm.scripts.tests]
 cmd = "pytest --spec --cov"
 
 [tool.pdm.scripts.check-lint]
-shell = "    ruff pyapi/\n    black --check .\n    isort --check .\n"
+shell = "    ruff check .\n    ruff format --check .\n    isort --check .\n"
 
-[tool.pdm.scripts.check-typing]
-cmd = "mypy --install-types --non-interactive pyapi/"
+[tool.pdm.scripts.reformat]
+shell = "    isort .\n    ruff format .\n"
 
-[tool.pdm.scripts.check-docs]
-cmd = "pydocstyle pyapi/"
+[tool.pdm.scripts.check-typing]
+cmd = "mypy --install-types --non-interactive"
 
 [tool.pdm.scripts.checks]
 composite = [
     "check-lint",
     "check-typing",
-    "check-docs",
 ]
 
 [tool.pdm.scripts.new-commits]
 shell = "git log $(git describe --tags --abbrev=0)..HEAD --oneline --no-decorate"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
@@ -99,56 +98,54 @@
 show_missing = true
 fail_under = 80
 exclude_lines = [
     "pragma: no cover",
     "@abstract",
 ]
 
-[tool.black]
-line-length = 96
-target-version = [
-    "py38",
-    "py39",
-    "py310",
-    "py311",
-    "py312",
-]
-verbose = false
-skip-string-normalization = false
-
 [tool.isort]
 profile = "black"
 line_length = 96
 filter_files = true
 force_alphabetical_sort_within_sections = true
 
 [tool.ruff]
+line-length = 96
+target-version = "py311"
+output-format = "grouped"
+
+[tool.ruff.lint]
 select = [
-    "E",
-    "F",
+    "E4",
+    "E7",
+    "E9",
     "W",
+    "F",
     "D",
-    "PL",
-    "ERA",
-    "N",
 ]
 ignore = [
     "D104",
     "D107",
     "D203",
     "D212",
     "D401",
     "D407",
-    "PLR0913",
+    "D413",
 ]
-line-length = 96
-target-version = "py38"
-output-format = "grouped"
 
-[tool.pydocstyle]
-add-ignore = "D104, D107, D212, D401"
-convention = "google"
-match-dir = "^(?!tests|examples).*"
+[tool.ruff.lint.per-file-ignores]
+"__init__.py" = [
+    "F401",
+]
+"tests/*" = [
+    "D",
+]
+"example/*" = [
+    "D",
+]
 
 [tool.mypy]
 mypy_path = "pyapi/"
+files = [
+    "pyapi/",
+]
 ignore_missing_imports = true
```

### Comparing `pyapi-server-0.4.1/tests/endpoints.py` & `pyapi_server-0.5.0/tests/endpoints.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,9 +18,8 @@
 
 async def dummy_post_endpoint(request):
     body = await request.body()
     assert json.loads(body.decode()) == {"foo": "bar"}
     return Response(status_code=HTTPStatus.NO_CONTENT.value)
 
 
-async def endpoint_returning_nothing(request):
-    ...
+async def endpoint_returning_nothing(request): ...
```

### Comparing `pyapi-server-0.4.1/tests/openapi.json` & `pyapi_server-0.5.0/tests/openapi.json`

 * *Files identical despite different names*

### Comparing `pyapi-server-0.4.1/tests/openapi.yaml` & `pyapi_server-0.5.0/tests/openapi.yaml`

 * *Files identical despite different names*

### Comparing `pyapi-server-0.4.1/tests/test_app.py` & `pyapi_server-0.5.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `pyapi-server-0.4.1/tests/test_endpoints.py` & `pyapi_server-0.5.0/tests/test_endpoints.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 
 from pyapi.server import Application
 
 
 def test_endpoints_are_defined_as_named_module_with_dotted_name(spec_dict):
     spec_dict["paths"]["/test"]["get"]["operationId"] = "endpoints.dummyTestEndpoint"
     spec_dict["paths"]["/test"]["post"]["operationId"] = "endpoints.dummyPostEndpoint"
-    spec_dict["paths"]["/test/{test_arg}"]["get"][
-        "operationId"
-    ] = "endpoints.dummyTestEndpointWithArgument"
+    spec_dict["paths"]["/test/{test_arg}"]["get"]["operationId"] = (
+        "endpoints.dummyTestEndpointWithArgument"
+    )
     spec_dict["paths"]["/test-async"]["get"]["operationId"] = "endpoints.dummyTestEndpointCoro"
     app = Application(spec_dict, module="tests")
     route = app.routes[0]
     assert callable(route.endpoint)
     assert route.endpoint.__name__ == "dummy_test_endpoint"
     assert route.path == "/test"
 
@@ -30,17 +30,17 @@
 
 
 def test_endpoints_are_defined_as_imported_module_with_dotted_names(spec_dict):
     import tests
 
     spec_dict["paths"]["/test"]["get"]["operationId"] = "endpoints.dummyTestEndpoint"
     spec_dict["paths"]["/test"]["post"]["operationId"] = "endpoints.dummyPostEndpoint"
-    spec_dict["paths"]["/test/{test_arg}"]["get"][
-        "operationId"
-    ] = "endpoints.dummyTestEndpointWithArgument"
+    spec_dict["paths"]["/test/{test_arg}"]["get"]["operationId"] = (
+        "endpoints.dummyTestEndpointWithArgument"
+    )
     spec_dict["paths"]["/test-async"]["get"]["operationId"] = "endpoints.dummyTestEndpointCoro"
     app = Application(spec_dict, module=tests)
     route = app.routes[0]
     assert callable(route.endpoint)
     assert route.endpoint.__name__ == "dummy_test_endpoint"
     assert route.path == "/test"
```

### Comparing `pyapi-server-0.4.1/tests/test_service.py` & `pyapi_server-0.5.0/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `pyapi-server-0.4.1/tests/test_spec.py` & `pyapi_server-0.5.0/tests/test_spec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from openapi_core import Spec
+from jsonschema_path import SchemaPath
 
 from pyapi.server.spec import OperationSpec
 
 
 def test_OperationSpec_get_all_creates_dict_of_operations(spec_dict):
-    spec = Spec.from_dict(spec_dict)
+    spec = SchemaPath.from_dict(spec_dict)
     operation_ids = (
         "dummyTestEndpoint",
         "dummyPostEndpoint",
         "dummyTestEndpointWithArgument",
         "dummyTestEndpointCoro",
     )
     operations = OperationSpec.get_all(spec)
     assert sorted(operations) == sorted(operation_ids)
 
 
 def test_OperationSpec_groups_parameters_by_type(spec_dict):
-    operations = OperationSpec.get_all(Spec.from_dict(spec_dict))
+    operations = OperationSpec.get_all(SchemaPath.from_dict(spec_dict))
     operation = operations["dummyTestEndpointWithArgument"]
     assert hasattr(operation, "parameters")
     assert "test_arg" in operation.parameters["path"]
```

### Comparing `pyapi-server-0.4.1/PKG-INFO` & `pyapi_server-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 Metadata-Version: 2.1
 Name: pyapi-server
-Version: 0.4.1
+Version: 0.5.0
 Summary: Lightweight API framework using an OpenAPI spec for routing and validation.
+Home-page: https://pyapi-server.readthedocs.io
+Author-Email: Berislav Lopac <berislav@lopac.net>
 License: MIT
-Author-email: Berislav Lopac <berislav@lopac.net>
-Requires-Python: >=3.8,<4.0
+Project-URL: Homepage, https://pyapi-server.readthedocs.io
+Project-URL: Documentation, https://pyapi-server.readthedocs.io
+Project-URL: Repository, https://github.com/berislavlopac/pyapi-server
+Requires-Python: <4.0,>=3.8
+Requires-Dist: PyYAML>=5.4
+Requires-Dist: stringcase>=1.2.0
+Requires-Dist: openapi-core>=0.18
+Requires-Dist: starlette>=0.21.0
+Requires-Dist: jsonschema-path>=0.3.2
+Requires-Dist: uvicorn>=0.18.3; extra == "uvicorn"
 Provides-Extra: uvicorn
-Project-URL: documentation, https://pyapi-server.readthedocs.io
-Project-URL: homepage, https://pyapi-server.readthedocs.io
-Project-URL: repository, https://github.com/berislavlopac/pyapi-server
 Description-Content-Type: text/markdown
 
 # PyAPI Server
 
 [![Build Status](https://b11c.semaphoreci.com/badges/pyapi-server/branches/main.svg?style=shields&key=e9eeb9d2-6487-4aba-9207-e46c84f9bc6f)](https://b11c.semaphoreci.com/projects/pyapi-server)
 [![Documentation Status](https://readthedocs.org/projects/pyapi-server/badge/?version=latest)](https://pyapi-server.readthedocs.io/en/latest/?badge=latest)
 
@@ -26,8 +33,7 @@
 
 ```python
 from pyapi.server import Application
 from some.path import endpoints
 
 app = Application.from_file("path/to/openapi.yaml", module=endpoints)
 ```
-
```

