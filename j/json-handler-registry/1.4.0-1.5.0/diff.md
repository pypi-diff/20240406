# Comparing `tmp/json-handler-registry-1.4.0.tar.gz` & `tmp/json-handler-registry-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/json-handler-registry-1.4.0.tar", last modified: Thu Apr  4 16:47:40 2024, max compression
+gzip compressed data, was "dist/json-handler-registry-1.5.0.tar", last modified: Sat Apr  6 14:00:49 2024, max compression
```

## Comparing `json-handler-registry-1.4.0.tar` & `json-handler-registry-1.5.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2024-03-25 18:49:27.000000 json-handler-registry-1.4.0/LICENSE.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       81 2024-03-25 19:02:47.000000 json-handler-registry-1.4.0/MANIFEST.in
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4911 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4394 2024-04-04 16:44:46.000000 json-handler-registry-1.4.0/README.md
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-04-04 16:13:08.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     2466 2024-04-04 15:46:19.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/decoder.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1295 2024-04-04 15:46:10.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/encoder.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/py.typed
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4551 2024-04-04 16:37:45.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/registry.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/support/
--rw-r--r--   0 pawel     (1000) pawel     (1000)      977 2024-04-04 15:59:25.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/support/__init__.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/support/impl/
--rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-04-01 18:10:20.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/support/impl/__init__.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)      358 2024-04-04 15:57:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/support/impl/common.py
--rw-r--r--   0 pawel     (1000) pawel     (1000)     1243 2024-04-01 18:13:30.000000 json-handler-registry-1.4.0/pkg/json_handler_registry/support/impl/dataclasses_json.py
-drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/
--rw-r--r--   0 pawel     (1000) pawel     (1000)     4911 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/PKG-INFO
--rw-r--r--   0 pawel     (1000) pawel     (1000)      676 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/SOURCES.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/dependency_links.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-03-25 19:03:21.000000 json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/not-zip-safe
--rw-r--r--   0 pawel     (1000) pawel     (1000)       22 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/top_level.txt
--rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-04-04 16:47:40.000000 json-handler-registry-1.4.0/setup.cfg
--rwxr-xr-x   0 pawel     (1000) pawel     (1000)     2329 2024-03-25 19:37:00.000000 json-handler-registry-1.4.0/setup.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1077 2024-03-25 18:49:27.000000 json-handler-registry-1.5.0/LICENSE.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       81 2024-03-25 19:02:47.000000 json-handler-registry-1.5.0/MANIFEST.in
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5037 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4520 2024-04-06 13:57:30.000000 json-handler-registry-1.5.0/README.md
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      280 2024-04-06 13:55:25.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     2466 2024-04-04 15:46:19.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/decoder.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1295 2024-04-04 15:46:10.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/encoder.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        0 2023-11-17 22:27:43.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/py.typed
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     4703 2024-04-06 13:54:01.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/registry.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       78 2024-04-06 13:53:39.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      358 2024-04-04 15:57:40.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/config.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/impl/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      380 2024-04-06 13:54:11.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/impl/__init__.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     1250 2024-04-06 13:41:51.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/impl/dataclasses_json.py
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      842 2024-04-06 13:53:19.000000 json-handler-registry-1.5.0/pkg/json_handler_registry/support/manager.py
+drwxr-xr-x   0 pawel     (1000) pawel     (1000)        0 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/
+-rw-r--r--   0 pawel     (1000) pawel     (1000)     5037 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/PKG-INFO
+-rw-r--r--   0 pawel     (1000) pawel     (1000)      716 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/SOURCES.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/dependency_links.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)        1 2024-03-25 19:03:21.000000 json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/not-zip-safe
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       22 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/top_level.txt
+-rw-r--r--   0 pawel     (1000) pawel     (1000)       38 2024-04-06 14:00:49.000000 json-handler-registry-1.5.0/setup.cfg
+-rwxr-xr-x   0 pawel     (1000) pawel     (1000)     2329 2024-03-25 19:37:00.000000 json-handler-registry-1.5.0/setup.py
```

### Comparing `json-handler-registry-1.4.0/LICENSE.txt` & `json-handler-registry-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.4.0/PKG-INFO` & `json-handler-registry-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-handler-registry
-Version: 1.4.0
+Version: 1.5.0
 Summary: Standardized way of registering custom JSON serializers/deserializers.
 Home-page: https://bitbucket.org/massultidev/tunit/
 Author: P.J. Grochowski
 Author-email: pawel.grochowski.dev@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -97,16 +97,15 @@
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from enum import Enum, auto
 from uuid import UUID, uuid4
 
 from dataclasses_json import DataClassJsonMixin
-
-from json_handler_registry.support import PackageSupportManager
+from json_handler_registry.registry import JsonHandlerRegistry
 
 
 class TestEnum(Enum):
   Option1 = auto()
   Option2 = auto()
   Option3 = auto()
 
@@ -122,26 +121,28 @@
 testData = TestDataClass(
   timestamp=datetime.now().astimezone(),
   id=uuid4(),
   option=TestEnum.Option2,
   value=Decimal(7)
 )
 
-PackageSupportManager.getPackageSupportConfig('dataclasses-json').enable()
+JsonHandlerRegistry.packageSupportManager.getPackageSupportConfig('dataclasses-json').enable()
 assert TestDataClass.from_json(testData.to_json()) == testData
-PackageSupportManager.getPackageSupportConfig('dataclasses-json').disable()
+JsonHandlerRegistry.packageSupportManager.getPackageSupportConfig('dataclasses-json').disable()
 
 # Instead of using 'PackageSupportManager' you can also manually register encoder:
 from json_handler_registry.registry import JsonHandlerRegistry
 from json_handler_registry.support.impl.dataclasses_json import DataClassJsonEncoder
 JsonHandlerRegistry.registerEncoder(DataClassJsonEncoder)
 ```
 
 ### Changelog:
 ---
+- Version: 1.5.0
+    - Package support manager is now accessible from handler registry.
 - Version: 1.4.0
     - Preserving registration order of encoders/decoders.
     - Configurable auto enable/disable registry feature. (Active by default.)
 - Version: 1.3.0
     - Support for `dataclasses-json` package.
     - Debug methods for listing registered encoders/decoders.
 - Version: 1.2.0
```

### Comparing `json-handler-registry-1.4.0/README.md` & `json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: json-handler-registry
+Version: 1.5.0
+Summary: Standardized way of registering custom JSON serializers/deserializers.
+Home-page: https://bitbucket.org/massultidev/tunit/
+Author: P.J. Grochowski
+Author-email: pawel.grochowski.dev@gmail.com
+License: MIT
+Classifier: Programming Language :: Python :: 3.7
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![PyPI license](https://img.shields.io/pypi/l/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![Downloads](https://static.pepy.tech/badge/json-handler-registry)](https://pepy.tech/project/json-handler-registry)
 
 # JSON Handler Registry
 ---
@@ -82,16 +97,15 @@
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from enum import Enum, auto
 from uuid import UUID, uuid4
 
 from dataclasses_json import DataClassJsonMixin
-
-from json_handler_registry.support import PackageSupportManager
+from json_handler_registry.registry import JsonHandlerRegistry
 
 
 class TestEnum(Enum):
   Option1 = auto()
   Option2 = auto()
   Option3 = auto()
 
@@ -107,26 +121,28 @@
 testData = TestDataClass(
   timestamp=datetime.now().astimezone(),
   id=uuid4(),
   option=TestEnum.Option2,
   value=Decimal(7)
 )
 
-PackageSupportManager.getPackageSupportConfig('dataclasses-json').enable()
+JsonHandlerRegistry.packageSupportManager.getPackageSupportConfig('dataclasses-json').enable()
 assert TestDataClass.from_json(testData.to_json()) == testData
-PackageSupportManager.getPackageSupportConfig('dataclasses-json').disable()
+JsonHandlerRegistry.packageSupportManager.getPackageSupportConfig('dataclasses-json').disable()
 
 # Instead of using 'PackageSupportManager' you can also manually register encoder:
 from json_handler_registry.registry import JsonHandlerRegistry
 from json_handler_registry.support.impl.dataclasses_json import DataClassJsonEncoder
 JsonHandlerRegistry.registerEncoder(DataClassJsonEncoder)
 ```
 
 ### Changelog:
 ---
+- Version: 1.5.0
+    - Package support manager is now accessible from handler registry.
 - Version: 1.4.0
     - Preserving registration order of encoders/decoders.
     - Configurable auto enable/disable registry feature. (Active by default.)
 - Version: 1.3.0
     - Support for `dataclasses-json` package.
     - Debug methods for listing registered encoders/decoders.
 - Version: 1.2.0
```

### Comparing `json-handler-registry-1.4.0/pkg/json_handler_registry/decoder.py` & `json-handler-registry-1.5.0/pkg/json_handler_registry/decoder.py`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.4.0/pkg/json_handler_registry/encoder.py` & `json-handler-registry-1.5.0/pkg/json_handler_registry/encoder.py`

 * *Files identical despite different names*

### Comparing `json-handler-registry-1.4.0/pkg/json_handler_registry/registry.py` & `json-handler-registry-1.5.0/pkg/json_handler_registry/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from collections import OrderedDict
 from functools import partial
 from typing import Any, List, Type, Union, cast
 
 from json_handler_registry import __logger as logger
 from json_handler_registry.decoder import DecoderRegistryDict, IJsonDecoder, _JsonDecoderRegistryProxy
 from json_handler_registry.encoder import EncoderRegistryDict, IJsonEncoder, _JsonEncoderRegistryProxy
+from json_handler_registry.support.manager import PackageSupportManager
 
 JsonEncoder = Union[Type[IJsonEncoder], IJsonEncoder]
 JsonDecoder = Union[Type[IJsonDecoder], IJsonDecoder]
 
 
 class _RegistryGuardPartial(partial):
 
@@ -36,14 +37,16 @@
 
     _ENCODER_REGISTRY: EncoderRegistryDict = OrderedDict()
     _DECODER_REGISTRY: DecoderRegistryDict = OrderedDict()
 
     autoEnable: bool = True
     autoDisable: bool = True
 
+    packageSupportManager: Type[PackageSupportManager] = PackageSupportManager
+
     @classmethod
     def isEmpty(cls) -> bool:
         return (
             len(cls._ENCODER_REGISTRY) <= 0 and
             len(cls._DECODER_REGISTRY) <= 0
         )
```

### Comparing `json-handler-registry-1.4.0/pkg/json_handler_registry/support/impl/dataclasses_json.py` & `json-handler-registry-1.5.0/pkg/json_handler_registry/support/impl/dataclasses_json.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from decimal import Decimal
 from enum import Enum
 from typing import Optional, cast
 from uuid import UUID
 
 from json_handler_registry.encoder import EncodingResult, IJsonEncoder
 from json_handler_registry.registry import JsonHandlerRegistry
-from json_handler_registry.support import PackageSupportConfig
+from json_handler_registry.support.config import PackageSupportConfig
 
 
 class DataClassJsonEncoder(IJsonEncoder):
     def encodeObject(self, obj: object) -> Optional[EncodingResult]:
         if isinstance(obj, datetime):
             return obj.timestamp()
         if isinstance(obj, UUID):
```

### Comparing `json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/PKG-INFO` & `json-handler-registry-1.5.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: json-handler-registry
-Version: 1.4.0
-Summary: Standardized way of registering custom JSON serializers/deserializers.
-Home-page: https://bitbucket.org/massultidev/tunit/
-Author: P.J. Grochowski
-Author-email: pawel.grochowski.dev@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3.7
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![PyPI license](https://img.shields.io/pypi/l/json-handler-registry.svg)](https://pypi.python.org/pypi/json-handler-registry)
 [![Downloads](https://static.pepy.tech/badge/json-handler-registry)](https://pepy.tech/project/json-handler-registry)
 
 # JSON Handler Registry
 ---
@@ -97,16 +82,15 @@
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from enum import Enum, auto
 from uuid import UUID, uuid4
 
 from dataclasses_json import DataClassJsonMixin
-
-from json_handler_registry.support import PackageSupportManager
+from json_handler_registry.registry import JsonHandlerRegistry
 
 
 class TestEnum(Enum):
   Option1 = auto()
   Option2 = auto()
   Option3 = auto()
 
@@ -122,26 +106,28 @@
 testData = TestDataClass(
   timestamp=datetime.now().astimezone(),
   id=uuid4(),
   option=TestEnum.Option2,
   value=Decimal(7)
 )
 
-PackageSupportManager.getPackageSupportConfig('dataclasses-json').enable()
+JsonHandlerRegistry.packageSupportManager.getPackageSupportConfig('dataclasses-json').enable()
 assert TestDataClass.from_json(testData.to_json()) == testData
-PackageSupportManager.getPackageSupportConfig('dataclasses-json').disable()
+JsonHandlerRegistry.packageSupportManager.getPackageSupportConfig('dataclasses-json').disable()
 
 # Instead of using 'PackageSupportManager' you can also manually register encoder:
 from json_handler_registry.registry import JsonHandlerRegistry
 from json_handler_registry.support.impl.dataclasses_json import DataClassJsonEncoder
 JsonHandlerRegistry.registerEncoder(DataClassJsonEncoder)
 ```
 
 ### Changelog:
 ---
+- Version: 1.5.0
+    - Package support manager is now accessible from handler registry.
 - Version: 1.4.0
     - Preserving registration order of encoders/decoders.
     - Configurable auto enable/disable registry feature. (Active by default.)
 - Version: 1.3.0
     - Support for `dataclasses-json` package.
     - Debug methods for listing registered encoders/decoders.
 - Version: 1.2.0
```

### Comparing `json-handler-registry-1.4.0/pkg/json_handler_registry.egg-info/SOURCES.txt` & `json-handler-registry-1.5.0/pkg/json_handler_registry.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 pkg/json_handler_registry/registry.py
 pkg/json_handler_registry.egg-info/PKG-INFO
 pkg/json_handler_registry.egg-info/SOURCES.txt
 pkg/json_handler_registry.egg-info/dependency_links.txt
 pkg/json_handler_registry.egg-info/not-zip-safe
 pkg/json_handler_registry.egg-info/top_level.txt
 pkg/json_handler_registry/support/__init__.py
+pkg/json_handler_registry/support/config.py
+pkg/json_handler_registry/support/manager.py
 pkg/json_handler_registry/support/impl/__init__.py
-pkg/json_handler_registry/support/impl/common.py
 pkg/json_handler_registry/support/impl/dataclasses_json.py
```

### Comparing `json-handler-registry-1.4.0/setup.py` & `json-handler-registry-1.5.0/setup.py`

 * *Files identical despite different names*

