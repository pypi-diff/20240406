# Comparing `tmp/jupyrest-0.1.0.tar.gz` & `tmp/jupyrest-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyrest-0.1.0.tar", max compression
+gzip compressed data, was "jupyrest-0.2.0.tar", max compression
```

## Comparing `jupyrest-0.1.0.tar` & `jupyrest-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,37 @@
--rwxr-xr-x   0        0        0      214 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/__init__.py
--rwxr-xr-x   0        0        0       75 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/__main__.py
--rwxr-xr-x   0        0        0     3019 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/cli.py
--rwxr-xr-x   0        0        0     3985 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/domain.py
--rwxr-xr-x   0        0        0      416 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/errors.py
--rwxr-xr-x   0        0        0     2362 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/executors.py
--rwxr-xr-x   0        0        0     4280 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/model.py
--rwxr-xr-x   0        0        0     8365 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/nbschema.py
--rwxr-xr-x   0        0        0     4740 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/plugin.py
--rwxr-xr-x   0        0        0     5491 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/resolvers.py
--rwxr-xr-x   0        0        0        0 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/workers/__init__.py
--rwxr-xr-x   0        0        0     5050 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/workers/base.py
--rwxr-xr-x   0        0        0        0 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/workers/generated/__init__.py
--rwxr-xr-x   0        0        0    13552 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/workers/generated/jupyrest_pb2.py
--rwxr-xr-x   0        0        0     3798 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/workers/generated/jupyrest_pb2.pyi
--rwxr-xr-x   0        0        0     2581 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/workers/generated/jupyrest_pb2_grpc.py
--rwxr-xr-x   0        0        0    10172 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/workers/grpc.py
--rwxr-xr-x   0        0        0     5454 2021-12-29 21:23:28.716875 jupyrest-0.1.0/jupyrest/workers/http.py
--rwxr-xr-x   0        0        0     1072 2021-12-29 21:23:28.716875 jupyrest-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1467 2021-12-29 21:31:06.685586 jupyrest-0.1.0/setup.py
--rw-r--r--   0        0        0     1432 2021-12-29 21:31:06.686245 jupyrest-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      287 2024-04-06 05:51:39.265478 jupyrest-0.2.0/jupyrest/__init__.py
+-rw-r--r--   0        0        0     4352 2024-04-06 05:51:39.265478 jupyrest-0.2.0/jupyrest/client.py
+-rw-r--r--   0        0        0     3761 2024-04-06 05:51:39.266023 jupyrest-0.2.0/jupyrest/contracts.py
+-rw-r--r--   0        0        0        0 2024-04-06 05:51:39.266575 jupyrest-0.2.0/jupyrest/default_impl/__init__.py
+-rw-r--r--   0        0        0     3326 2024-04-06 05:51:39.267104 jupyrest-0.2.0/jupyrest/default_impl/builder.py
+-rw-r--r--   0        0        0      357 2024-04-06 05:51:39.267646 jupyrest-0.2.0/jupyrest/default_impl/execution_task_handler.py
+-rw-r--r--   0        0        0     1547 2024-04-06 05:51:39.268188 jupyrest-0.2.0/jupyrest/default_impl/executor.py
+-rw-r--r--   0        0        0      808 2024-04-06 05:51:39.268778 jupyrest-0.2.0/jupyrest/default_impl/file_namer.py
+-rw-r--r--   0        0        0      884 2024-04-06 05:51:39.268867 jupyrest-0.2.0/jupyrest/default_impl/input_output_validator.py
+-rw-r--r--   0        0        0      798 2024-04-06 05:51:39.269377 jupyrest-0.2.0/jupyrest/default_impl/notebook_converter.py
+-rw-r--r--   0        0        0     2738 2024-04-06 05:51:39.269986 jupyrest-0.2.0/jupyrest/default_impl/notebook_repository.py
+-rw-r--r--   0        0        0      446 2024-04-06 05:51:39.270498 jupyrest-0.2.0/jupyrest/default_impl/output_reader.py
+-rw-r--r--   0        0        0     1610 2024-04-06 05:51:39.271059 jupyrest-0.2.0/jupyrest/default_impl/parameterizer.py
+-rw-r--r--   0        0        0     2731 2024-04-06 05:51:39.271059 jupyrest-0.2.0/jupyrest/error.py
+-rw-r--r--   0        0        0      630 2024-04-06 05:51:39.271609 jupyrest-0.2.0/jupyrest/file_object.py
+-rw-r--r--   0        0        0        0 2024-04-06 05:51:39.272156 jupyrest-0.2.0/jupyrest/http/__init__.py
+-rw-r--r--   0        0        0     6841 2024-04-06 05:51:39.272749 jupyrest-0.2.0/jupyrest/http/asgi.py
+-rw-r--r--   0        0        0     1223 2024-04-06 05:51:39.273303 jupyrest-0.2.0/jupyrest/http/models.py
+-rw-r--r--   0        0        0        0 2024-04-06 05:51:39.273303 jupyrest-0.2.0/jupyrest/infra/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-06 05:51:39.273859 jupyrest-0.2.0/jupyrest/infra/azure/__init__.py
+-rw-r--r--   0        0        0     1253 2024-04-06 05:51:39.274399 jupyrest-0.2.0/jupyrest/infra/azure/builder.py
+-rw-r--r--   0        0        0     1588 2024-04-06 05:51:39.274940 jupyrest-0.2.0/jupyrest/infra/azure/execution_repository.py
+-rw-r--r--   0        0        0      707 2024-04-06 05:51:39.275586 jupyrest-0.2.0/jupyrest/infra/azure/execution_task_handler.py
+-rw-r--r--   0        0        0     1068 2024-04-06 05:51:39.275586 jupyrest-0.2.0/jupyrest/infra/azure/file_object_client.py
+-rw-r--r--   0        0        0        0 2024-04-06 05:51:39.276098 jupyrest-0.2.0/jupyrest/infra/in_memory/__init__.py
+-rw-r--r--   0        0        0      803 2024-04-06 05:51:39.276646 jupyrest-0.2.0/jupyrest/infra/in_memory/builder.py
+-rw-r--r--   0        0        0      856 2024-04-06 05:51:39.277191 jupyrest-0.2.0/jupyrest/infra/in_memory/execution_repository.py
+-rw-r--r--   0        0        0      674 2024-04-06 05:51:39.277735 jupyrest-0.2.0/jupyrest/infra/in_memory/file_object_client.py
+-rw-r--r--   0        0        0     4728 2024-04-06 05:51:39.278289 jupyrest-0.2.0/jupyrest/model.py
+-rw-r--r--   0        0        0    11475 2024-04-06 05:51:39.278831 jupyrest-0.2.0/jupyrest/nbschema.py
+-rw-r--r--   0        0        0      602 2024-04-06 05:51:39.279389 jupyrest-0.2.0/jupyrest/notebook_config.py
+-rw-r--r--   0        0        0     5440 2024-04-06 05:51:39.279925 jupyrest-0.2.0/jupyrest/notebook_execution/commands.py
+-rw-r--r--   0        0        0      494 2024-04-06 05:51:39.280465 jupyrest-0.2.0/jupyrest/notebook_execution/common.py
+-rw-r--r--   0        0        0     1189 2024-04-06 05:51:39.281008 jupyrest-0.2.0/jupyrest/notebook_execution/entity.py
+-rw-r--r--   0        0        0     1876 2024-04-06 05:51:39.281561 jupyrest-0.2.0/jupyrest/notebook_execution/queries.py
+-rw-r--r--   0        0        0      941 2024-04-06 05:51:39.288349 jupyrest-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1300 1970-01-01 00:00:00.000000 jupyrest-0.2.0/PKG-INFO
```

### Comparing `jupyrest-0.1.0/jupyrest/executors.py` & `jupyrest-0.2.0/jupyrest/default_impl/executor.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,61 +2,37 @@
 from datetime import datetime
 from dataclasses import dataclass
 from nbformat.notebooknode import NotebookNode
 from typing import Optional
 from nbclient.client import NotebookClient
 from nbclient.exceptions import CellExecutionError, CellTimeoutError
 import logging
-from opentelemetry import trace
+from ..contracts import NotebookExeuctor
 
 logger = logging.getLogger(__name__)
-tracer = trace.get_tracer(__name__)
 
 
-class BaseNotebookExeuctor(ABC):
-    @abstractmethod
-    def get_kernelspec_language(self) -> str:
-        pass
-
-    @abstractmethod
-    async def execute_notebook_async(self, notebook: NotebookNode) -> Optional[str]:
-        """Executes a notebook in place. Returns an exception string if any.
-
-        Args:
-            notebook (NotebookNode): notebook to execute
-
-        Returns:
-            Optional[str]: exception
-        """
-        pass
-
-
-class OtelNotebookClient(NotebookClient):
-    """A NotebookClient that emits OpenTelemetry Spans."""
 
-    async def async_execute(self, reset_kc: bool = False, **kwargs) -> NotebookNode:
-        with tracer.start_as_current_span("nbclient.async_execute"):
-            return await super().async_execute(reset_kc=reset_kc, **kwargs)
 
 
-class IPythonNotebookExecutor(BaseNotebookExeuctor):
+class IPythonNotebookExecutor(NotebookExeuctor):
     def __init__(
         self, kernel_name="python3", timeout_seconds=600, language="python"
     ) -> None:
         self._kernel_name = kernel_name
         self._timeout_seconds = timeout_seconds
         self._language = language
 
     def get_kernelspec_language(self) -> str:
         return self._language
 
     async def execute_notebook_async(self, notebook: NotebookNode) -> Optional[str]:
         exception: Optional[str] = None
         try:
-            await OtelNotebookClient(
+            await NotebookClient(
                 nb=notebook,
                 timeout=self._timeout_seconds,
                 kernel_name=self._kernel_name,
                 log=logger,
             ).async_execute()
         except CellExecutionError as cee:
             # handle cases where the notebook calls sys.exit(0),
```

### Comparing `jupyrest-0.1.0/jupyrest/model.py` & `jupyrest-0.2.0/jupyrest/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 from pydantic import BaseModel, parse_obj_as
-from typing import Callable, Type, Dict
+from typing import Callable, Type, Dict, cast
+from typing_extensions import Self
+import json
+
+named_model_registry: Dict[str, Type["NamedModel"]] = {}
 
 
 class NamedModelConflict(Exception):
     pass
 
 
 class NamedModel(BaseModel):
@@ -11,18 +15,19 @@
     stored in a `__ns__` class property. This information
     is a part of the objects JSON schema representation.
 
     Make a NamedModel:
 
     ```
     class MyNamedModel(NamedModel):
-        __ns__ = "models/MyNamedModel"
-
         prop1: str
         prop2: int
+
+        class Config:
+            __ns__ = "models/MyNamedModel"
     ```
 
     The benefit of a NamedModel is that it knows how to
     take a generic object and deserialize it to the correct
     subclass.
 
     ```
@@ -34,92 +39,101 @@
     model_json = json.loads(model.json())
 
     parsed_model = NamedModel.parse_obj(model_json)
     assert isinstance(parsed_model, MyNamedModel)
     ```
     """
 
-    # a mapping from namespaces -> subclasses of NamedModel
-    __nsmap__: Dict[str, Type["NamedModel"]] = {}
-    # the name of this type (the namespace)
-    __ns__: str
+    @classmethod
+    def _get_ns_key(cls) -> str:
+        if hasattr(cls.Config, "NS_KEY"):
+            return cls.Config.NS_KEY
+        else:
+            return NamedModel.Config.NS_KEY
+
+    @classmethod
+    def get_class_namespace(cls):
+        """Get the namespace for this class."""
+        if hasattr(cls.Config, "__ns__"):
+            return str(getattr(cls.Config, "__ns__"))
+        else:
+            raise ValueError(f"Class {cls} does not have a namespace")
 
     @classmethod
     def _iter_subclasses(cls):
         """Iterate over the subclasses for a
         particular type `cls` including `cls` itself.
         """
-        yield cls
+        global named_model_registry
+        if cls is not NamedModel:
+            if cls.get_class_namespace() not in named_model_registry:
+                named_model_registry[cls.get_class_namespace()] = cls
+
+            yield cls
         for sk in cls.__subclasses__():
             yield from sk._iter_subclasses()
 
     def dict(self, *args, **kwargs):
         """When we convert to a dict, we want
         to save the name of the model.
         """
         d = super().dict(*args, **kwargs)
-        d[self.Config.NS_KEY] = getattr(self, self.Config.NS_KEY)
+        NS_KEY = self._get_ns_key()
+        d[NS_KEY] = self.get_class_namespace()
         return d
 
+    def json(self, *args, **kwargs):
+        d = self.__config__.json_loads(super().json(*args, **kwargs))
+        NS_KEY = self._get_ns_key()
+        d[NS_KEY] = self.get_class_namespace()
+        return self.__config__.json_dumps(d)
+
     @classmethod
-    def parse_obj(cls, data, *args, **kwargs):
-        NS_KEY = cls.Config.NS_KEY
+    def parse_obj(cls, data, *args, **kwargs) -> Self:
+        NS_KEY = cls._get_ns_key()
 
         def data_has_ns_info(o):
             """This will tell us whether we should
             try parsing `data` or not
             """
             return isinstance(o, dict) and NS_KEY in data and isinstance(o[NS_KEY], str)
 
         def subclass_has_ns_info(sk):
             return hasattr(sk, NS_KEY) and isinstance(getattr(sk, NS_KEY), str)
 
         def subclass_has_name(name: str) -> Callable[[Type["NamedModel"]], bool]:
             def _check_name(sk: Type["NamedModel"]) -> bool:
-                return getattr(sk, NS_KEY) == name
+                return sk.get_class_namespace() == name
 
             return _check_name
 
         def get_subclass_for_ns(ns: str):
-            if ns not in NamedModel.__nsmap__:
-                # find the correct subclass
-                sks = filter(subclass_has_ns_info, cls._iter_subclasses())
-                sks = filter(subclass_has_name(data[NS_KEY]), sks)
-                sks = set(sks)
-
-                # we should only have at most 1 subclass
-                # for a given name
-                if len(sks) > 1:
-                    raise NamedModelConflict(f"{sks} have conflicting names {ns}")
-                elif len(sks) == 1:
-                    sk = sks.pop()
-                    NamedModel.__nsmap__[ns] = sk
-                else:
-                    return None
-
-            return NamedModel.__nsmap__[ns]
+            if ns not in named_model_registry:
+                list(cls._iter_subclasses())
+            return named_model_registry.get(ns, None)
 
         # if data has the namespace information we are looking for
         if data_has_ns_info(data):
             subclass = get_subclass_for_ns(data[NS_KEY])
             if subclass is not None:
-                return parse_obj_as(subclass, data)
+                return cast(Self, parse_obj_as(subclass, data))
 
         return parse_obj_as(cls, data)
 
     class Config:
-
+        # the name of this type (the namespace)
+        __ns__: str
         NS_KEY: str = "__ns__"
 
         @staticmethod
         def schema_extra(schema, model: Type["NamedModel"]) -> None:
             """Augment the json schema to add the required
             namespace property.
             """
-            NS_KEY = model.Config.NS_KEY
+            NS_KEY = model._get_ns_key()
 
             # by default, the description is the class docstring
             # this is not relevant so we will remove it
             if "description" in schema and schema["description"] is not None:
                 del schema["description"]
 
             if "properties" in schema and schema["properties"] is not None:
```

### Comparing `jupyrest-0.1.0/jupyrest/nbschema.py` & `jupyrest-0.2.0/jupyrest/nbschema.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,29 @@
 import json
 from nbformat.notebooknode import NotebookNode
 import scrapbook as sb
 from jsonschema import Draft7Validator, RefResolver
 from jsonschema.exceptions import best_match
-from typing import Optional, Dict, Type, Union, Any, Set
+from typing import Optional, Dict, Type, Union, Any, Set, List, Iterable
+from pydantic.schema import schema as pydantic_schema
+from unittest.mock import patch
 from urllib.parse import urlparse
 from pydantic import BaseModel
 from datetime import datetime, date
 from papermill.translators import papermill_translators, PythonTranslator
 from enum import Enum
-
-
-class ConfigSections(str, Enum):
-    INPUT = "input"
-    OUTPUT = "output"
-
-
-NotebookConfig = Dict
-
+from copy import deepcopy
+from .model import NamedModel
 
 class SchemaValidationResponse(BaseModel):
     is_valid: bool
     error: Optional[str] = None
 
 
 class NbSchemaBase(BaseModel):
-    """
-    Base class for all NbSchema models.
-    Inherits from Pydantic BaseModel.
-    """
-
     pass
 
 
 class ModelCollection:
     """
     Stores NbSchemaBase implementations along with their aliases.
     """
@@ -56,14 +46,23 @@
         if not self.has_alias(alias=alias):
             raise KeyError(f"Model for alias {alias} not found.")
         return self._map[alias]
 
     def is_empty(self) -> bool:
         return len(self._map.keys()) == 0
 
+    def has_model(self, model_type: Type[NbSchemaBase]) -> bool:
+        return model_type in self._map.values()
+
+    def get_alias(self, model_type: Type[NbSchemaBase]) -> str:
+        for k, v in self._map.items():
+            if v == model_type:
+                return k
+        raise KeyError(f"Alias for model {model_type} not found.")
+
 
 class NbSchemaEncoder(json.JSONEncoder):
     """
     JSONEncoder that can encode NbSchemaBase objects to json().
     This also encodes datetime objects to strings in iso format.
     """
 
@@ -84,55 +83,56 @@
     @classmethod
     def translate(cls, val):
         if isinstance(val, NbSchemaBase):
             return f"{val!r}"
         return super().translate(val)
 
 
-class OutputResult(BaseModel):
+class OutputResult(NamedModel):
     present: bool
     json_str: str
 
+    class Config:
+        __ns__ = "jupyrest.nbschema.OutputResult"
+
 
 class NotebookSchemaProcessor:
 
     OUTPUTS_KEY = "nbschema_outputs"
     SCHEME = "nbschema"
 
-    def __init__(self, models: Optional[ModelCollection] = None) -> None:
-        self._models = models or ModelCollection()
+    def __init__(self, models: Dict[str, Type[NbSchemaBase]]) -> None:
+        self._models = ModelCollection()
+        for model_alias, model_type in models.items():
+            self._models.add_model(alias=model_alias, model_type=model_type)
         self._ref_resolver = RefResolver(
             "", {}, handlers={self.SCHEME: self._resolve_ref}
         )
         papermill_translators.register("python", NbSchemaTranslator)
 
     @classmethod
     def _uri_to_alias(cls, uri: str):
         scheme = urlparse(uri).scheme
         if scheme != cls.SCHEME:
             raise ValueError(f"Invalid uri scheme {scheme}")
         return uri.replace(f"{cls.SCHEME}://", "")
 
-    def _get_validator(self, schema: Optional[Dict] = None):
+    def _get_validator(self, schema: Dict):
         Draft7Validator.check_schema(schema)
-        if not self._models.is_empty():
-            return Draft7Validator(schema=schema, resolver=self._ref_resolver)
-        else:
-            return Draft7Validator(schema=schema)
+        return Draft7Validator(schema=schema)
+
 
-    def _validate_instance(
-        self, instance: Optional[Dict], schema: Optional[Dict] = None
+    def validate_instance(
+        self, instance: Dict, schema: Dict
     ) -> SchemaValidationResponse:
-        # if we have a schema to validate against
-        if schema is not None:
-            # Check that this is a valid JSONSchema. Raise an exception if it is not.
-            validator = self._get_validator(schema=schema)
-            error = best_match(validator.iter_errors(instance=instance))
-            if error is not None:
-                return SchemaValidationResponse(is_valid=False, error=str(error))
+        # Check that this is a valid JSONSchema. Raise an exception if it is not.
+        validator = self._get_validator(schema=schema)
+        error = best_match(validator.iter_errors(instance=instance))
+        if error is not None:
+            return SchemaValidationResponse(is_valid=False, error=str(error))
         return SchemaValidationResponse(is_valid=True)
 
     def _resolve_ref(self, ref: str):
         alias = self._uri_to_alias(uri=ref)
         return self._models.get_model(alias=alias).schema()
 
     @property
@@ -187,32 +187,14 @@
                     objs = []
                     for item in payload:
                         obj = self.inject_model_refs(item_schema, item)
                         objs.append(obj)
                     return objs
         return payload
 
-    def validate_input(
-        self, input: Dict, notebook_config: Optional[NotebookConfig]
-    ) -> SchemaValidationResponse:
-        input_schema = (
-            notebook_config.get(ConfigSections.INPUT, None) if notebook_config else None
-        )
-        return self._validate_instance(instance=input, schema=input_schema,)
-
-    def validate_output(
-        self, output, notebook_config: Optional[NotebookConfig]
-    ) -> SchemaValidationResponse:
-        output_schema = (
-            notebook_config.get(ConfigSections.OUTPUT, None)
-            if notebook_config
-            else None
-        )
-        return self._validate_instance(instance=output, schema=output_schema)
-
     @classmethod
     def save_output(cls, data: Union[str, NbSchemaBase], **kwargs):
         """
         Simple wrapper around scrapbook's glue() function.
         The only difference is that the `name` parameter
         is set to OUTPUTS_KEY. The data to save should
         be a string compatible with the "application/json"
@@ -240,7 +222,100 @@
         """
         nb = sb.read_notebook(notebook)
         if self.OUTPUTS_KEY in nb.scraps.data_dict:
             json_str = nb.scraps.data_dict[self.OUTPUTS_KEY]
             return OutputResult(present=True, json_str=json_str)
         else:
             return OutputResult(present=False, json_str="")
+
+    def fix_schemas(self, schema: Dict, add_model_definitions: bool) -> Dict:
+        obj = deepcopy(schema)
+        mc = self._models
+
+        def get_ref_paths(obj: Dict) -> Dict[str, List[List[Union[str, int]]]]:
+
+            ref_locs: Dict[str, List[List[Union[str, int]]]] = {}
+
+            def add_ref(ref: str, path: List[Union[str, int]]):
+                nonlocal ref_locs
+                if ref in ref_locs:
+                    ref_locs[ref].append(path)
+                else:
+                    ref_locs[ref] = [path]
+
+            def get_ref_paths_inner(
+                obj: Union[Dict, List], path: List[Union[str, int]]
+            ):
+                if isinstance(obj, dict):
+                    for key, value in obj.items():
+                        curr_path = path + [key]
+                        if (
+                            key == "$ref"
+                            and isinstance(value, str)
+                            and value.startswith("nbschema://")
+                        ):
+                            add_ref(ref=value, path=path)
+                        elif isinstance(value, (list, dict)):
+                            get_ref_paths_inner(obj=value, path=curr_path)
+                elif isinstance(obj, list):
+                    for index, value in enumerate(obj):
+                        curr_path = path + [index]
+                        if isinstance(value, (list, dict)):
+                            get_ref_paths_inner(obj=value, path=curr_path)
+
+            get_ref_paths_inner(obj=obj, path=[])
+
+            return ref_locs
+
+        def get_value(obj: Dict, path: List[Union[str, int]]):
+            curr = obj
+            for part in path:
+                curr = curr[part]
+            return curr
+
+        def set_value(obj: Dict, ref_path: List[Union[str, int]], ref_value: str):
+            curr = obj
+            for part in ref_path:
+                curr = curr[part]
+            curr["$ref"] = ref_value
+
+        def resolve_definitions(model_refs: Iterable[str]):
+            model_name_map = {}
+            models = []
+            for model_ref in model_refs:
+                alias = NotebookSchemaProcessor._uri_to_alias(uri=model_ref)
+                model_type = mc.get_model(alias)
+                model_name_map[model_type] = alias
+                models.append(model_type)
+
+            def new_get_model_name_map(*args, **kwargs):
+                return model_name_map
+
+            with patch(
+                "pydantic.schema.get_model_name_map", new=new_get_model_name_map
+            ):
+                return pydantic_schema(models)
+
+        def update_nbschema_refs(
+            obj: Dict, ref_locs: Dict[str, List[List[Union[str, int]]]]
+        ):
+            for ref in ref_locs:
+                alias = self._uri_to_alias(ref)
+                for ref_path in ref_locs[ref]:
+                    ref_value = f"#/definitions/{alias}"
+                    set_value(obj=obj, ref_path=ref_path, ref_value=ref_value)
+
+        def add_definitions(
+            obj: Dict, ref_locs: Dict[str, List[List[Union[str, int]]]]
+        ):
+            definitions = resolve_definitions(model_refs=ref_locs.keys())
+            if "definitions" in definitions:
+                if "definitions" not in obj:
+                    obj["definitions"] = {}
+                obj["definitions"].update(definitions["definitions"])
+
+        ref_locs = get_ref_paths(obj=obj)
+        if add_model_definitions:
+            add_definitions(obj=obj, ref_locs=ref_locs)
+        update_nbschema_refs(obj=obj, ref_locs=ref_locs)
+
+        return obj
```

### Comparing `jupyrest-0.1.0/PKG-INFO` & `jupyrest-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 Metadata-Version: 2.1
 Name: jupyrest
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool to expose Jupyter notebooks as a REST API.
 Author: Koushik Krishnan
-Author-email: kokrishn@microsoft.com
-Requires-Python: >=3.7,<3.9
+Author-email: unequal09swims@icloud.com
+Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Dist: azure-storage-blob (>=12.8.1,<13.0.0)
-Requires-Dist: black (==21.7b0)
-Requires-Dist: click (>=7.1.2,<8.0.0)
-Requires-Dist: cryptography (<=3.4.7)
-Requires-Dist: entrypoints (>=0.3,<0.4)
-Requires-Dist: fastapi (>=0.65.2,<0.66.0)
-Requires-Dist: grpcio (>=1.38.0,<2.0.0)
-Requires-Dist: grpcio-tools (>=1.38.0,<2.0.0)
-Requires-Dist: ipykernel (>=6.0.1,<7.0.0)
-Requires-Dist: ipython (>=7.25.0,<8.0.0)
-Requires-Dist: jsonschema (>=3.2.0,<4.0.0)
-Requires-Dist: jupyter-client (<=6.1.12)
-Requires-Dist: nbclient (>=0.5.1,<0.6.0)
-Requires-Dist: nbconvert (==5.6.1)
-Requires-Dist: nbformat (>=5.1.3,<6.0.0)
-Requires-Dist: opentelemetry-api (>=1.5.0,<2.0.0)
-Requires-Dist: papermill (>=2.2,<2.3)
-Requires-Dist: pydantic (>=1.8,<2.0)
-Requires-Dist: pywin32 (==301); sys_platform == "win32"
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
+Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
+Requires-Dist: anyio (>=4.3.0,<5.0.0)
+Requires-Dist: azure-storage-blob (>=12.19.1,<13.0.0)
+Requires-Dist: azure-storage-queue (>=12.9.0,<13.0.0)
+Requires-Dist: entrypoints (>=0.4,<0.5)
+Requires-Dist: fastapi (>=0.110.0,<0.111.0)
+Requires-Dist: ipykernel (>=6.29.3,<7.0.0)
+Requires-Dist: ipython (>=8.18.1,<8.19.0) ; python_version >= "3.9" and python_version < "3.10"
+Requires-Dist: ipython (>=8.19.0) ; python_version >= "3.10"
+Requires-Dist: jsonschema (>=4.21.1,<5.0.0)
+Requires-Dist: nbclient (>=0.10.0,<0.11.0)
+Requires-Dist: nbconvert (>=7.16.3,<8.0.0)
+Requires-Dist: nbformat (>=5.10.3,<6.0.0)
+Requires-Dist: notebook (>=7.1.2,<8.0.0)
+Requires-Dist: papermill (>=2.5.0,<3.0.0)
+Requires-Dist: pydantic (>=1.10.14,<2.0.0)
 Requires-Dist: scrapbook (>=0.5.0,<0.6.0)
-Requires-Dist: setuptools-rust (>=0.12.1,<0.13.0)
-Requires-Dist: textwrap3 (>=0.9.2,<0.10.0)
-Requires-Dist: typer (>=0.3.2,<0.4.0)
-Requires-Dist: typing-extensions (>=3.7.4,<4.0.0); python_version < "3.8"
-Requires-Dist: uvicorn (>=0.14.0,<0.15.0)
+Requires-Dist: uvicorn (>=0.29.0,<0.30.0)
```

