# Comparing `tmp/xknxproject-3.7.0.tar.gz` & `tmp/xknxproject-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xknxproject-3.7.0.tar", last modified: Mon Feb 26 08:26:15 2024, max compression
+gzip compressed data, was "xknxproject-3.7.1.tar", last modified: Sat Apr  6 20:26:50 2024, max compression
```

## Comparing `xknxproject-3.7.0.tar` & `xknxproject-3.7.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:26:15.265692 xknxproject-3.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-02-26 08:26:01.000000 xknxproject-3.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-02-26 08:26:01.000000 xknxproject-3.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    23722 2024-02-26 08:26:15.265692 xknxproject-3.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-02-26 08:26:01.000000 xknxproject-3.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-02-26 08:26:01.000000 xknxproject-3.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-26 08:26:15.265692 xknxproject-3.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:26:15.257692 xknxproject-3.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-02-26 08:26:01.000000 xknxproject-3.7.0/test/test_knxproj.py
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-02-26 08:26:01.000000 xknxproject-3.7.0/test/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:26:15.261692 xknxproject-3.7.0/xknxproject/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:26:15.261692 xknxproject-3.7.0/xknxproject/combination/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/combination/combination.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/const.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:26:15.261692 xknxproject-3.7.0/xknxproject/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:26:15.261692 xknxproject-3.7.0/xknxproject/loader/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/loader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/loader/application_program_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/loader/hardware_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/loader/knx_master_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    18584 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/loader/project_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:26:15.261692 xknxproject-3.7.0/xknxproject/models/
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/models/knxproject.py
--rw-r--r--   0 runner    (1001) docker     (127)    21422 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/models/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/models/static.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/xknxproj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:26:15.261692 xknxproject-3.7.0/xknxproject/xml/
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15709 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/xml/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:26:15.261692 xknxproject-3.7.0/xknxproject/zip/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-02-26 08:26:01.000000 xknxproject-3.7.0/xknxproject/zip/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-26 08:26:15.265692 xknxproject-3.7.0/xknxproject.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    23722 2024-02-26 08:26:15.000000 xknxproject-3.7.0/xknxproject.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-02-26 08:26:15.000000 xknxproject-3.7.0/xknxproject.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-26 08:26:15.000000 xknxproject-3.7.0/xknxproject.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-26 08:26:15.000000 xknxproject-3.7.0/xknxproject.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-26 08:26:15.000000 xknxproject-3.7.0/xknxproject.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:26:50.212486 xknxproject-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-04-06 20:26:41.000000 xknxproject-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-06 20:26:41.000000 xknxproject-3.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    23722 2024-04-06 20:26:50.212486 xknxproject-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-04-06 20:26:41.000000 xknxproject-3.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-06 20:26:41.000000 xknxproject-3.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 20:26:50.212486 xknxproject-3.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:26:50.208486 xknxproject-3.7.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-06 20:26:41.000000 xknxproject-3.7.1/test/test_knxproj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-06 20:26:41.000000 xknxproject-3.7.1/test/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:26:50.208486 xknxproject-3.7.1/xknxproject/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:26:50.212486 xknxproject-3.7.1/xknxproject/combination/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/combination/combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:26:50.212486 xknxproject-3.7.1/xknxproject/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:26:50.212486 xknxproject-3.7.1/xknxproject/loader/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/loader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10338 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/loader/application_program_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4476 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/loader/hardware_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/loader/knx_master_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18585 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/loader/project_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:26:50.212486 xknxproject-3.7.1/xknxproject/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/models/knxproject.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25685 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/models/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/xknxproj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:26:50.212486 xknxproject-3.7.1/xknxproject/xml/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15886 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/xml/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:26:50.212486 xknxproject-3.7.1/xknxproject/zip/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-06 20:26:41.000000 xknxproject-3.7.1/xknxproject/zip/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 20:26:50.212486 xknxproject-3.7.1/xknxproject.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    23722 2024-04-06 20:26:50.000000 xknxproject-3.7.1/xknxproject.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-06 20:26:50.000000 xknxproject-3.7.1/xknxproject.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 20:26:50.000000 xknxproject-3.7.1/xknxproject.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-06 20:26:50.000000 xknxproject-3.7.1/xknxproject.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 20:26:50.000000 xknxproject-3.7.1/xknxproject.egg-info/top_level.txt
```

### Comparing `xknxproject-3.7.0/LICENSE` & `xknxproject-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xknxproject-3.7.0/PKG-INFO` & `xknxproject-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xknxproject
-Version: 3.7.0
+Version: 3.7.1
 Summary: A library to gather information from ETS project files used for KNX
 Author-email: Marvin Wichmann <me@marvin-wichmann.de>, Matthias Alphart <farmio@alphart.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `xknxproject-3.7.0/README.md` & `xknxproject-3.7.1/README.md`

 * *Files identical despite different names*

### Comparing `xknxproject-3.7.0/pyproject.toml` & `xknxproject-3.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xknxproject-3.7.0/test/test_knxproj.py` & `xknxproject-3.7.1/test/test_knxproj.py`

 * *Files identical despite different names*

### Comparing `xknxproject-3.7.0/test/test_util.py` & `xknxproject-3.7.1/test/test_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Test utilities."""
+
 import pytest
 
 from xknxproject.util import get_dpt_type, parse_dpt_types
 
 
 @pytest.mark.parametrize(
     ("dpt_string", "expected"),
```

### Comparing `xknxproject-3.7.0/xknxproject/combination/combination.py` & `xknxproject-3.7.1/xknxproject/combination/combination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Combine the project data for more details inferred from linked objects."""
+
 from __future__ import annotations
 
 from typing import NamedTuple
 
 from xknxproject.models import CommunicationObject, DPTType, KNXProject
```

### Comparing `xknxproject-3.7.0/xknxproject/const.py` & `xknxproject-3.7.1/xknxproject/const.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Constants for the library."""
+
 from typing import Final
 
 ETS_6_SCHEMA_VERSION: Final = 21
 ETS_5_7_SCHEMA_VERSION: Final = 20
 ETS_5_6_SCHEMA_VERSION: Final = 14
 ETS_4_2_SCHEMA_VERSION: Final = 11
```

### Comparing `xknxproject-3.7.0/xknxproject/loader/application_program_loader.py` & `xknxproject-3.7.1/xknxproject/loader/application_program_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Application Program Loader."""
+
 from __future__ import annotations
 
 from collections.abc import Iterator
 import logging
 from typing import Any
 from xml.etree import ElementTree
 from zipfile import Path
@@ -10,14 +11,15 @@
 from xknxproject.models import (
     Allocator,
     ApplicationProgram,
     ComObject,
     ComObjectRef,
     DeviceInstance,
     ModuleDefinitionArgumentInfo,
+    ModuleDefinitionNumericArg,
 )
 from xknxproject.util import parse_dpt_types, parse_xml_flag
 
 _LOGGER = logging.getLogger("xknxproject.log")
 
 
 class ApplicationProgramLoader:
@@ -44,46 +46,59 @@
         com_objects: dict[str, ComObject] = {}  # {Id: ComObject}
 
         used_module_arguments: dict[str, ModuleDefinitionArgumentInfo] = {
             attribute.ref_id: ModuleDefinitionArgumentInfo()
             for device in devices
             for attribute in device.module_instance_arguments()
         }
+        numeric_args: dict[str, ModuleDefinitionNumericArg] = {}
         allocators: dict[str, Allocator] = {}
 
         with application_program_path.open(mode="rb") as application_xml:
             tree_iterator = ElementTree.iterparse(application_xml, events=("start",))
             for _, elem in tree_iterator:
                 if elem.tag.endswith("ComObject"):
                     # we take all since we don't know which are referenced to yet
                     identifier = elem.attrib.get("Id")
                     com_objects[identifier] = ApplicationProgramLoader.parse_com_object(
                         elem, identifier
                     )
                 elif elem.tag.endswith("ComObjectRef"):
                     if (_id := elem.attrib.get("Id")) in used_com_object_ref_ids:
-                        com_object_refs[
-                            _id
-                        ] = ApplicationProgramLoader.parse_com_object_ref(elem, _id)
+                        com_object_refs[_id] = (
+                            ApplicationProgramLoader.parse_com_object_ref(elem, _id)
+                        )
                     elem.clear()
                 elif elem.tag.endswith("Allocator"):  # Allocators/Allocator
                     allocators[elem.attrib.get("Id")] = Allocator(
                         identifier=elem.attrib.get("Id"),
                         name=elem.attrib.get("Name"),
                         start=int(elem.attrib.get("Start")),
                         end=int(elem.attrib.get("maxInclusive")),
                     )
-                elif elem.tag.endswith("Argument"):  # ModuleDefs/ModuleDef/Arguments/
+                elif elem.tag.endswith("Argument"):
+                    # ModuleDefs/ModuleDef/Arguments/
+                    # or ModuleDefs/ModuleDef/SubModuleDefs/ModuleDef/Arguments/
                     if (_id := elem.attrib.get("Id")) in used_module_arguments:
                         allocates = elem.attrib.get("Allocates")
                         used_module_arguments[_id] = ModuleDefinitionArgumentInfo(
                             name=elem.attrib.get("Name"),
                             allocates=int(allocates) if allocates is not None else None,
                         )
                     elem.clear()
+                elif elem.tag.endswith("NumericArg"):
+                    # in dynamic section of Modules
+                    if (_id := elem.attrib.get("RefId")) in used_module_arguments:
+                        value = elem.attrib.get("Value")
+                        numeric_args[_id] = ModuleDefinitionNumericArg(
+                            allocator_ref_id=elem.attrib.get("AllocatorRefId"),
+                            base_value=elem.attrib.get("BaseValue"),
+                            value=int(value) if value is not None else None,
+                        )
+                    elem.clear()
                 elif elem.tag.endswith("Languages"):
                     elem.clear()
                     # hold iterator for optional translation parsing
                     break
                 elem.clear()
 
             if language_code is not None:
@@ -96,14 +111,15 @@
                 )
 
             return ApplicationProgram(
                 com_objects=com_objects,
                 com_object_refs=com_object_refs,
                 allocators=allocators,
                 module_def_arguments=used_module_arguments,
+                numeric_args=numeric_args,
             )
 
     @staticmethod
     def parse_translations(
         tree_iterator: Iterator[tuple[str, Any]],
         com_objects: dict[str, ComObject],
         com_object_refs: dict[str, ComObjectRef],
```

### Comparing `xknxproject-3.7.0/xknxproject/loader/hardware_loader.py` & `xknxproject-3.7.1/xknxproject/loader/hardware_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Hardware Loader."""
+
 from __future__ import annotations
 
 from xml.etree import ElementTree
 from zipfile import Path
 
 from xknxproject.models import HardwareToPrograms, Product
 from xknxproject.zip import KNXProjContents
```

### Comparing `xknxproject-3.7.0/xknxproject/loader/knx_master_loader.py` & `xknxproject-3.7.1/xknxproject/loader/knx_master_loader.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """KNX Master Data Loader."""
+
 from __future__ import annotations
 
 import logging
 from xml.etree import ElementTree
 from zipfile import Path
 
 from xknxproject.const import ETS4_PRODUCT_LANGUAGES
```

### Comparing `xknxproject-3.7.0/xknxproject/loader/project_loader.py` & `xknxproject-3.7.1/xknxproject/loader/project_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Project file loader."""
+
 from __future__ import annotations
 
 import re
 from xml.etree import ElementTree
 
 from xknxproject.models import (
     ChannelNode,
```

### Comparing `xknxproject-3.7.0/xknxproject/models/__init__.py` & `xknxproject-3.7.1/xknxproject/models/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Xknxproj models."""
+
 # flake8: noqa
 from .knxproject import (
     Area,
     Channel,
     CommunicationObject,
     Device,
     DPTType,
@@ -25,14 +26,15 @@
     ComObjectRef,
     DeviceInstance,
     HardwareToPrograms,
     KNXMasterData,
     ModuleInstance,
     ModuleInstanceArgument,
     ModuleDefinitionArgumentInfo,
+    ModuleDefinitionNumericArg,
     Product,
     TranslationsType,
     XMLArea,
     XMLFunction,
     XMLGroupAddress,
     XMLGroupAddressRef,
     XMLGroupRange,
```

### Comparing `xknxproject-3.7.0/xknxproject/models/knxproject.py` & `xknxproject-3.7.1/xknxproject/models/knxproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Define output type for parsed KNX project."""
+
 from __future__ import annotations
 
 from typing import TypedDict
 
 
 class DPTType(TypedDict):
     """DPT type dictionary."""
@@ -40,15 +41,17 @@
     flags: Flags
 
 
 class ModuleInstanceInfos(TypedDict):
     """Information about module association for CommunicationObjects."""
 
     definition: str
-    root_number: int  # `Number` assigned by ComObject - without Module base object number added
+    root_number: (
+        int  # `Number` assigned by ComObject - without Module base object number added
+    )
 
 
 class Device(TypedDict):
     """Devices dictionary."""
 
     name: str
     hardware_name: str
```

### Comparing `xknxproject-3.7.0/xknxproject/models/models.py` & `xknxproject-3.7.1/xknxproject/models/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Define internally used data structures."""
+
 from __future__ import annotations
 
 from collections.abc import Iterator
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 import logging
 import re
 
 from xknxproject.models.knxproject import DPTType, ModuleInstanceInfos
 from xknxproject.models.static import GroupAddressStyle, SpaceType
 from xknxproject.zip import KNXProjContents
 
@@ -179,25 +180,25 @@
     def module_instance_arguments(self) -> Iterator[ModuleInstanceArgument]:
         """Iterate ModuleInstance arguments."""
         for _module_instance in self.module_instances:
             yield from _module_instance.arguments
 
     def merge_application_program_info(self, application: ApplicationProgram) -> None:
         """Merge items with their parent objects from the application program."""
-        for attribute in self.module_instance_arguments():
-            attribute.name = application.module_def_arguments[attribute.ref_id].name
-            attribute.allocates = application.module_def_arguments[
-                attribute.ref_id
+        for argument in self.module_instance_arguments():
+            argument.name = application.module_def_arguments[argument.ref_id].name
+            argument.allocates = application.module_def_arguments[
+                argument.ref_id
             ].allocates
 
         for com_instance in self.com_object_instance_refs:
             com_instance.merge_application_program_info(application)
             com_instance.apply_module_base_number_argument(
                 module_instances=self.module_instances,
-                application_allocators=application.allocators,
+                application=application,
             )
 
         self._complete_channel_placeholders()
 
     def _complete_channel_placeholders(self) -> None:
         """Replace placeholders in channel names with module instance arguments."""
         for channel in self.channels:
@@ -227,32 +228,57 @@
     name: str
 
 
 @dataclass
 class ModuleInstance:
     """Class that represents a ModuleInstance."""
 
-    identifier: str
-    ref_id: str
+    identifier: str  # MD-4_M-15_MI-2 / MD-4_M-15_MI-2_SM-1_M-1_MI-2-1-2
+    ref_id: str  # MD-<int>_M-<int>
     arguments: list[ModuleInstanceArgument]
 
+    module_def_id: str = field(init=False)  # MD-<int>
+    # MD-<int>_M-<int>_MI-<int> if SubModule - reference may contain base values for arguments
+    base_module: str | None = field(init=False)
+    # ModuleDefUniqueNumber with SubModule id if present (used in result json)
+    definition_id: str = field(init=False)  # MD-<int>[_SM-<int>]
+
+    def __post_init__(self) -> None:
+        """Set is_submodule based on the identifier."""
+        self.module_def_id = self.ref_id.split("_")[0]
+        _submodule_match = re.search(r"(_SM-[^_]+)", self.identifier)
+        if _submodule_match is not None:
+            self.base_module = f"{self.identifier.split('_SM-')[0]}"
+            self.definition_id = f"{self.module_def_id}{_submodule_match.group()}"
+        else:
+            self.base_module = None
+            self.definition_id = self.module_def_id
+
+    def complete_arguments_ref_id(self, application_program_ref: str) -> None:
+        """Prepend the ref_id with the application program ref."""
+        for arg in self.arguments:
+            arg.complete_ref_id(application_program_ref, self.module_def_id)
+
 
 @dataclass
 class ModuleInstanceArgument:
     """Class that represents a ModuleInstance Argument."""
 
     ref_id: str
     value: str
     # resolved from application by `ref_id` ModuleDefs/ModuleDef/Arguments/Argument
     name: str = ""  # "Name" type="knx:Identifier50_t" use="required"
     allocates: int | None = None  # "Allocates" type="xs:unsignedLong" use="optional"
 
-    def complete_ref_id(self, application_program_ref: str) -> None:
+    def complete_ref_id(self, application_program_ref: str, module_def_id: str) -> None:
         """Prepend the ref_id with the application program ref."""
-        self.ref_id = f"{application_program_ref}_{self.ref_id}"
+        if self.ref_id.startswith("SM-"):  # SubModule
+            self.ref_id = f"{application_program_ref}_{module_def_id}_{self.ref_id}"
+        else:
+            self.ref_id = f"{application_program_ref}_{self.ref_id}"
 
 
 @dataclass
 class ComObjectInstanceRef:
     """Class that represents a ComObjectInstanceRef instance."""
 
     identifier: str | None  # "Id" - xs:ID
@@ -287,21 +313,37 @@
     # assigned when module arguments are applied
     module: ModuleInstanceInfos | None = None
 
     def resolve_com_object_ref_id(
         self, application_program_ref: str, knx_proj_contents: KNXProjContents
     ) -> None:
         """Prepend the ref_id with the application program ref."""
-        # Remove module and ModuleInstance occurrence as they will not be in the application program directly
-        ref_id = re.sub(r"(M-\d+?_MI-\d+?_)", "", self.ref_id)
-        if knx_proj_contents.is_ets4_project():
-            self.com_object_ref_id = ref_id
+        if knx_proj_contents.is_ets4_project() and self.ref_id.startswith(
+            application_program_ref
+        ):
+            # ETS4 doesn't use shortened ref_id and I think it doesn't support modules at all
+            self.com_object_ref_id = self.ref_id
+            return
+
+        if self.ref_id.startswith("O-"):
+            ref_id = self.ref_id
+        elif self.ref_id.startswith("MD-"):
+            # Remove module and ModuleInstance occurrence as they will not be in the application program directly
+            module_definition = self.ref_id.split("_")[0]
+            object_reference = self.ref_id[self.ref_id.index("_O-") :]
+            _submodule_match = re.search(r"(_SM-[^_]+)", self.ref_id)
+            submodule = _submodule_match.group() if _submodule_match is not None else ""
+            ref_id = f"{module_definition}{submodule}{object_reference}"
         else:
-            self.application_program_id_prefix = f"{application_program_ref}_"
-            self.com_object_ref_id = f"{application_program_ref}_{ref_id}"
+            raise ValueError(
+                f"Unknown ref_id format: {self.ref_id} in application: {application_program_ref}"
+            )
+
+        self.application_program_id_prefix = f"{application_program_ref}_"
+        self.com_object_ref_id = f"{application_program_ref}_{ref_id}"
 
     def merge_application_program_info(self, application: ApplicationProgram) -> None:
         """Fill missing information with information parsed from the application program."""
         if self.com_object_ref_id is None:
             _LOGGER.warning(
                 "ComObjectInstanceRef %s has no ComObjectRefId",
                 self.identifier,
@@ -339,47 +381,80 @@
         if isinstance(com_object, ComObject):
             self.number = com_object.number
             self.base_number_argument_ref = com_object.base_number_argument_ref
 
     def apply_module_base_number_argument(
         self,
         module_instances: list[ModuleInstance],
-        application_allocators: dict[str, Allocator],
+        application: ApplicationProgram,
     ) -> None:
         """Apply module argument of base number."""
         if (
             self.base_number_argument_ref is None
             or not self.ref_id.startswith("MD-")
             or self.number is None  # only for type safety
         ):
             return
-        # there are 2 ways to get the base number
-        # 1. from the module instance arguments value "ObjNumberBase" directly
-        # 2. from the module defs allocator - adding the "Start" value to
-        #   (the modules index - 1) * allocator size
-        #   in this case the module instance argument value is the reference part
-        #   of the allocator id ("L-1") - at least in the application tested (MDT Dali 64)
+
+        def _parse_base_number_argument(
+            module_instance: ModuleInstance,
+            base_number_argument_ref: str,
+        ) -> int:
+            """Parse the argument value."""
+            # there are 2 ways to get the base number
+            # 1. from the module instance arguments value "ObjNumberBase" directly
+            # 2. from the module defs allocator - adding the "Start" value to
+            #   (the modules index - 1) * allocator size
+            #   in this case the module instance argument value is the reference part
+            #   of the allocator id ("L-1") - at least in the application tested (MDT Dali 64)
+            #
+            #   for SubModules the NumericArg item may use a BaseValue reference to an
+            #   Argument of the base ModuleDef containing the base value for all its SubModules
+            result = 0
+            base_number_argument = next(
+                arg
+                for arg in module_instance.arguments
+                if arg.ref_id == base_number_argument_ref
+            )
+
+            try:
+                # path (1) if value is a number, we are done
+                # base module value should already be included
+                return int(base_number_argument.value)
+            except ValueError:
+                # path (2) value is a reference to an Allocator
+                if module_instance.base_module:
+                    # recurse to get the base number from the base module (for SubModule value)
+                    num_arg = application.numeric_args.get(base_number_argument.ref_id)
+                    if (
+                        num_arg is not None
+                        and (base_value_ref := num_arg.base_value) is not None
+                    ):
+                        base_module = next(
+                            mi
+                            for mi in module_instances
+                            if mi.identifier == module_instance.base_module
+                        )
+                        result += _parse_base_number_argument(
+                            module_instance=base_module,
+                            base_number_argument_ref=base_value_ref,
+                        )
+                return result + self._base_number_from_allocator(
+                    base_number_argument, application.allocators
+                )
+
         _module_instance = next(
             mi for mi in module_instances if self.ref_id.startswith(f"{mi.identifier}_")
         )
         com_object_number = self.number
-        base_number_argument = next(
-            arg
-            for arg in _module_instance.arguments
-            if arg.ref_id == self.base_number_argument_ref
+        self.number += _parse_base_number_argument(
+            _module_instance, self.base_number_argument_ref
         )
-        try:
-            self.number += int(base_number_argument.value)
-        except ValueError:
-            self.number += self._base_number_from_allocator(
-                base_number_argument, application_allocators
-            )
-
         self.module = ModuleInstanceInfos(
-            definition=self.ref_id.split("_")[0],
+            definition=_module_instance.definition_id,
             root_number=com_object_number,
         )
 
     def _base_number_from_allocator(
         self,
         base_number_argument: ModuleInstanceArgument,
         application_allocators: dict[str, Allocator],
@@ -408,14 +483,15 @@
 class ApplicationProgram:
     """Class that represents an ApplicationProgram instance."""
 
     com_objects: dict[str, ComObject]  # {Id: ComObject}
     com_object_refs: dict[str, ComObjectRef]  # {Id: ComObjectRef}
     allocators: dict[str, Allocator]  # {Id: Allocator}
     module_def_arguments: dict[str, ModuleDefinitionArgumentInfo]  # {Id: ...}
+    numeric_args: dict[str, ModuleDefinitionNumericArg]  # {RefId: ...}
 
 
 @dataclass
 class Allocator:
     """Allocator."""
 
     identifier: str
@@ -429,14 +505,26 @@
     """Module Definition Argument."""
 
     name: str = ""
     allocates: int | None = None
 
 
 @dataclass
+class ModuleDefinitionNumericArg:
+    """Module Definition Numeric Argument."""
+
+    # shortened version (MD-<int>_L-<int>) should be Value in 0.xml ModuleInstanceArgument (at least with ETS 5)
+    allocator_ref_id: str | None
+    # if allocator_ref_id is not used, this is 0.xml ModuleInstanceArgument Value
+    value: int | None
+    # RefId to Argument (<application>_MD-<int>_A-<int>) - Base value for arguments used in SubModules
+    base_value: str | None
+
+
+@dataclass
 class ComObject:
     """Class that represents a ComObject instance."""
 
     __slots__ = (
         "identifier",
         "name",
         "text",
```

### Comparing `xknxproject-3.7.0/xknxproject/models/static.py` & `xknxproject-3.7.1/xknxproject/models/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Contains static data from the project files that is not really important and doesn't change often."""
+
 from enum import Enum
 
 
 class SpaceType(Enum):
     """Supported space types according to Specs from XSD."""
 
     BUILDING = "Building"
```

### Comparing `xknxproject-3.7.0/xknxproject/util.py` & `xknxproject-3.7.1/xknxproject/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """XML utilities."""
+
 from __future__ import annotations
 
 import logging
 from typing import overload
 
 from xknxproject.const import MAIN_AND_SUB_DPT, MAIN_DPT
 from xknxproject.models import DPTType
@@ -48,21 +49,19 @@
             _LOGGER.warning(
                 'Could not parse DPTType from: "%s" in "%s"', _dpt, dpt_string
             )
     return supported_dpts
 
 
 @overload
-def parse_xml_flag(flag: str | None, default: bool) -> bool:
-    ...
+def parse_xml_flag(flag: str | None, default: bool) -> bool: ...
 
 
 @overload
-def parse_xml_flag(flag: str | None, default: None = None) -> bool | None:
-    ...
+def parse_xml_flag(flag: str | None, default: None = None) -> bool | None: ...
 
 
 def parse_xml_flag(flag: str | None, default: bool | None = None) -> bool | None:
     """Parse the XML flag to an optional boolean."""
     if flag is None:
         return default
     return flag == "Enabled"
```

### Comparing `xknxproject-3.7.0/xknxproject/xknxproj.py` & `xknxproject-3.7.1/xknxproject/xknxproj.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ETS Project Parser is a library to parse ETS project files."""
+
 from __future__ import annotations
 
 import logging
 from pathlib import Path
 import time
 
 from xknxproject.__version__ import __version__
```

### Comparing `xknxproject-3.7.0/xknxproject/xml/parser.py` & `xknxproject-3.7.1/xknxproject/xml/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Parser logic for ETS XML files."""
+
 from __future__ import annotations
 
 import html
 import logging
 from operator import attrgetter
 
 from striprtf.striprtf import rtf_to_text
@@ -185,42 +186,46 @@
                 device.manufacturer, ""
             )
 
             try:
                 product = products_dict[device.product_ref]
             except KeyError:
                 _LOGGER.warning(
-                    "Could not find hardware product for device %s with product_ref %s",
+                    "Could not find hardware product for device %s from %s with product_ref %s",
                     device.individual_address,
+                    device.manufacturer_name,
                     device.product_ref,
                 )
                 continue
             device.product_name = product.text
             device.hardware_name = product.hardware_name
             device.order_number = product.order_number
 
             try:
                 application_program_ref = hardware_application_map[
                     device.hardware_program_ref
                 ]
             except KeyError:
                 _LOGGER.warning(
-                    "Could not find application_program_ref for device %s with hardware_program_ref %s",
+                    "Could not find application_program_ref for device %s - %s - %s with hardware_program_ref %s",
                     device.individual_address,
+                    device.manufacturer_name,
+                    device.product_name,
                     device.hardware_program_ref,
                 )
                 continue
             device.application_program_ref = application_program_ref
             for com_object in device.com_object_instance_refs:
+                # TODO: try and except here
                 com_object.resolve_com_object_ref_id(
                     application_program_ref, self.knx_proj_contents
                 )
-            for module_instance_argument in device.module_instance_arguments():
+            for module_instance in device.module_instances:
                 # need to complete ref_id before parsing application program
-                module_instance_argument.complete_ref_id(application_program_ref)
+                module_instance.complete_arguments_ref_id(application_program_ref)
 
         # only parse each application program file once and only extract used infos
         application_programs = (
             ApplicationProgramLoader.get_application_program_files_for_devices(
                 devices=self.devices,
             )
         )
```

### Comparing `xknxproject-3.7.0/xknxproject/zip/extractor.py` & `xknxproject-3.7.1/xknxproject/zip/extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class to read KNXProj ZIP files."""
+
 from __future__ import annotations
 
 import base64
 from collections.abc import Iterator
 from contextlib import contextmanager
 import hashlib
 import logging
```

### Comparing `xknxproject-3.7.0/xknxproject.egg-info/PKG-INFO` & `xknxproject-3.7.1/xknxproject.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xknxproject
-Version: 3.7.0
+Version: 3.7.1
 Summary: A library to gather information from ETS project files used for KNX
 Author-email: Marvin Wichmann <me@marvin-wichmann.de>, Matthias Alphart <farmio@alphart.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 2, June 1991
         
          Copyright (C) 1989, 1991 Free Software Foundation, Inc.,
          51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA
```

### Comparing `xknxproject-3.7.0/xknxproject.egg-info/SOURCES.txt` & `xknxproject-3.7.1/xknxproject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

