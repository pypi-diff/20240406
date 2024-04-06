# Comparing `tmp/omnibelt-0.8.3.tar.gz` & `tmp/omnibelt-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omnibelt-0.8.3.tar", last modified: Wed Feb 14 16:13:01 2024, max compression
+gzip compressed data, was "omnibelt-0.8.4.tar", last modified: Sat Apr  6 12:18:18 2024, max compression
```

## Comparing `omnibelt-0.8.3.tar` & `omnibelt-0.8.4.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-14 16:13:01.980234 omnibelt-0.8.3/
--rw-r--r--   0 fleeb     (7343) is        (1040)     1067 2023-08-30 14:46:29.000000 omnibelt-0.8.3/LICENSE
--rw-r--r--   0 fleeb     (7343) is        (1040)     1428 2024-02-14 16:13:01.980234 omnibelt-0.8.3/PKG-INFO
--rw-r--r--   0 fleeb     (7343) is        (1040)     1046 2023-09-15 10:14:28.000000 omnibelt-0.8.3/README.md
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-14 16:13:01.980234 omnibelt-0.8.3/omnibelt/
--rw-r--r--   0 fleeb     (7343) is        (1040)     3023 2024-02-14 16:12:42.000000 omnibelt-0.8.3/omnibelt/__init__.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    23793 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/basic_containers.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     3378 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/containers.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     3584 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/crafts.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1684 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/errors.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    27196 2023-09-15 09:53:43.000000 omnibelt-0.8.3/omnibelt/exporting.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     3013 2023-09-15 09:53:43.000000 omnibelt-0.8.3/omnibelt/exporting_common.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    16842 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/farming.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    13046 2023-11-26 13:15:41.000000 omnibelt-0.8.3/omnibelt/filesystem.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     3307 2024-02-14 10:31:17.000000 omnibelt-0.8.3/omnibelt/flow.py
--rw-r--r--   0 fleeb     (7343) is        (1040)      334 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/hashing.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     4324 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/logging.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     5663 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/logic.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    35399 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/nodes.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     7801 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/operators.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    20294 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/ordered_set.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    18477 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/packing.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     2038 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/patterns.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     3913 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/propagators.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    12961 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/pure_packing.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     8403 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/registries.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     4483 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/structured.py
--rw-r--r--   0 fleeb     (7343) is        (1040)      264 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/timing.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     2054 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/transactions.py
--rw-r--r--   0 fleeb     (7343) is        (1040)    43501 2024-02-13 14:35:58.000000 omnibelt-0.8.3/omnibelt/tricks.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     6575 2023-09-12 17:14:31.000000 omnibelt-0.8.3/omnibelt/typing.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     9138 2023-11-30 16:25:31.000000 omnibelt-0.8.3/omnibelt/utils.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1761 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/viz.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     6097 2023-08-30 14:46:29.000000 omnibelt-0.8.3/omnibelt/wrappers.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-14 16:13:01.980234 omnibelt-0.8.3/omnibelt.egg-info/
--rw-r--r--   0 fleeb     (7343) is        (1040)     1428 2024-02-14 16:13:01.000000 omnibelt-0.8.3/omnibelt.egg-info/PKG-INFO
--rw-r--r--   0 fleeb     (7343) is        (1040)      905 2024-02-14 16:13:01.000000 omnibelt-0.8.3/omnibelt.egg-info/SOURCES.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)        1 2024-02-14 16:13:01.000000 omnibelt-0.8.3/omnibelt.egg-info/dependency_links.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)       99 2024-02-14 16:13:01.000000 omnibelt-0.8.3/omnibelt.egg-info/requires.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)        9 2024-02-14 16:13:01.000000 omnibelt-0.8.3/omnibelt.egg-info/top_level.txt
--rw-r--r--   0 fleeb     (7343) is        (1040)      634 2024-02-14 16:13:01.980234 omnibelt-0.8.3/setup.cfg
--rw-r--r--   0 fleeb     (7343) is        (1040)       41 2023-09-15 10:04:42.000000 omnibelt-0.8.3/setup.py
-drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-02-14 16:13:01.980234 omnibelt-0.8.3/tests/
--rw-r--r--   0 fleeb     (7343) is        (1040)      883 2023-08-30 14:46:29.000000 omnibelt-0.8.3/tests/test_basics.py
--rw-r--r--   0 fleeb     (7343) is        (1040)      666 2023-08-30 14:46:29.000000 omnibelt-0.8.3/tests/test_packing.py
--rw-r--r--   0 fleeb     (7343) is        (1040)      535 2023-08-30 14:46:29.000000 omnibelt-0.8.3/tests/test_transactions.py
--rw-r--r--   0 fleeb     (7343) is        (1040)     1018 2023-08-30 14:46:29.000000 omnibelt-0.8.3/tests/test_wrappers.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:18:18.605839 omnibelt-0.8.4/
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1067 2023-08-30 14:46:29.000000 omnibelt-0.8.4/LICENSE
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1428 2024-04-06 12:18:18.605839 omnibelt-0.8.4/PKG-INFO
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1046 2023-09-15 10:14:28.000000 omnibelt-0.8.4/README.md
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:18:18.605839 omnibelt-0.8.4/omnibelt/
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3045 2024-04-06 12:17:36.000000 omnibelt-0.8.4/omnibelt/__init__.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    23793 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/basic_containers.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3378 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/containers.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3584 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/crafts.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1684 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/errors.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    27196 2023-09-15 09:53:43.000000 omnibelt-0.8.4/omnibelt/exporting.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3013 2023-09-15 09:53:43.000000 omnibelt-0.8.4/omnibelt/exporting_common.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    16842 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/farming.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    13145 2024-03-15 17:11:57.000000 omnibelt-0.8.4/omnibelt/filesystem.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3307 2024-02-14 10:31:17.000000 omnibelt-0.8.4/omnibelt/flow.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      334 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/hashing.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     4324 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/logging.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     5663 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/logic.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    35399 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/nodes.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     7801 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/operators.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    20294 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/ordered_set.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    18477 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/packing.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2038 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/patterns.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     3913 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/propagators.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    12961 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/pure_packing.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     8835 2024-04-04 10:29:36.000000 omnibelt-0.8.4/omnibelt/registries.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     4483 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/structured.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      264 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/timing.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     2054 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/transactions.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)    44744 2024-03-24 12:25:51.000000 omnibelt-0.8.4/omnibelt/tricks.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     6575 2023-09-12 17:14:31.000000 omnibelt-0.8.4/omnibelt/typing.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     9419 2024-03-15 10:43:25.000000 omnibelt-0.8.4/omnibelt/utils.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1761 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/viz.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     6097 2023-08-30 14:46:29.000000 omnibelt-0.8.4/omnibelt/wrappers.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:18:18.605839 omnibelt-0.8.4/omnibelt.egg-info/
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1428 2024-04-06 12:18:18.000000 omnibelt-0.8.4/omnibelt.egg-info/PKG-INFO
+-rw-r--r--   0 fleeb     (7343) is        (1040)      905 2024-04-06 12:18:18.000000 omnibelt-0.8.4/omnibelt.egg-info/SOURCES.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        1 2024-04-06 12:18:18.000000 omnibelt-0.8.4/omnibelt.egg-info/dependency_links.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)       99 2024-04-06 12:18:18.000000 omnibelt-0.8.4/omnibelt.egg-info/requires.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)        9 2024-04-06 12:18:18.000000 omnibelt-0.8.4/omnibelt.egg-info/top_level.txt
+-rw-r--r--   0 fleeb     (7343) is        (1040)      634 2024-04-06 12:18:18.609839 omnibelt-0.8.4/setup.cfg
+-rw-r--r--   0 fleeb     (7343) is        (1040)       41 2023-09-15 10:04:42.000000 omnibelt-0.8.4/setup.py
+drwxr-xr-x   0 fleeb     (7343) is        (1040)        0 2024-04-06 12:18:18.605839 omnibelt-0.8.4/tests/
+-rw-r--r--   0 fleeb     (7343) is        (1040)      883 2023-08-30 14:46:29.000000 omnibelt-0.8.4/tests/test_basics.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      666 2023-08-30 14:46:29.000000 omnibelt-0.8.4/tests/test_packing.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)      535 2023-08-30 14:46:29.000000 omnibelt-0.8.4/tests/test_transactions.py
+-rw-r--r--   0 fleeb     (7343) is        (1040)     1018 2023-08-30 14:46:29.000000 omnibelt-0.8.4/tests/test_wrappers.py
```

### Comparing `omnibelt-0.8.3/LICENSE` & `omnibelt-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/PKG-INFO` & `omnibelt-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnibelt
-Version: 0.8.3
+Version: 0.8.4
 Summary: "Omni-belt: A Tool-belt containing pure python utilities for downstream projects"
 Home-page: https://github.com/felixludos/omni-belt
 Author: Felix Leeb
 Author-email: felixludos.info@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `omnibelt-0.8.3/README.md` & `omnibelt-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/__init__.py` & `omnibelt-0.8.4/omnibelt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.3'
+__version__ = '0.8.4'
 
 from .flow import safe_self_execute, multi_index, cwd, include_module, lengen
 from .logging import get_printer, get_global_setting, get_global_settings, set_global_setting, set_printer_setting
 from .typing import primitives, unspecified_argument, join_classes, replace_class, \
 	duplicate_class, duplicate_func, duplicate_instance, wrap_class, mix_into, \
 	conditional_method, lambda_conditional_method, agnosticmethod, agnostic, agnosticproperty, isiterable
 from .filesystem import create_dir, crawl, spawn_path_options, load_yaml, save_yaml, \
@@ -19,15 +19,15 @@
 from .ordered_set import OrderedSet
 from .farming import WorkerPool
 from .exporting import AbstractExporter, AbstractExportManager, SimpleExporterBase
 from .exporting import export, load_export, set_export_manager, ExportManager
 from .tricks import self_aware, clsdec, innerchild, method_wrapper, ClassDescriptable, classdescriptor, \
 	extract_function_signature, capturable_super, captured_super, auto_init, dynamic_capture, \
 	smartproperty, autoproperty, referenceproperty, defaultproperty, TrackSmart, Tracer, \
-	Modifiable, inject_modifiers, ClassHierarchy, method_decorator, args2kwargs
+	Modifiable, inject_modifiers, ClassHierarchy, method_decorator, args2kwargs, extract_missing_args
 from .propagators import method_propagator
 from .operators import operation_base, auto_operation, Operationalized, DecoratedOperational, \
 	AbstractOperational, AbstractOperator
 
 from .packing import Packable, primitive, Primitive, SERIALIZABLE, JSONABLE, pack, unpack
 from .packing import save_pack, load_pack, json_pack, json_unpack
 # from .pure_packing import pack, unpack, json_unpack, json_pack
```

### Comparing `omnibelt-0.8.3/omnibelt/basic_containers.py` & `omnibelt-0.8.4/omnibelt/basic_containers.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/containers.py` & `omnibelt-0.8.4/omnibelt/containers.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/crafts.py` & `omnibelt-0.8.4/omnibelt/crafts.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/errors.py` & `omnibelt-0.8.4/omnibelt/errors.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/exporting.py` & `omnibelt-0.8.4/omnibelt/exporting.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/exporting_common.py` & `omnibelt-0.8.4/omnibelt/exporting_common.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/farming.py` & `omnibelt-0.8.4/omnibelt/farming.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/filesystem.py` & `omnibelt-0.8.4/omnibelt/filesystem.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,19 +178,23 @@
 		out = ordered_dump(data, stream=bf, Dumper=yaml.SafeDumper,
 							default_flow_style=default_flow_style, **kwargs)
 	else:
 		out = yaml.safe_dump(data, bf, default_flow_style=default_flow_style, **kwargs)
 	return bf.getvalue()
 
 
-def load_csv_rows(path):
+def load_csv_rows(path, **kwargs):
 	import pandas as pd
-	tbl = pd.read_csv(path)
+	tbl = pd.read_csv(path, **kwargs)
 	for _, row in tbl.iterrows():
-		yield row.to_dict()
+		data = row.to_dict()
+		for k, v in data.items():
+			if v != v:
+				data[k] = None
+		yield data
 
 
 def load_yaml(path, ordered=False):
 	path = str(path)
 	with open(path, 'r') as f:
 		if ordered:
 			return ordered_load(f, yaml.SafeLoader)
```

### Comparing `omnibelt-0.8.3/omnibelt/flow.py` & `omnibelt-0.8.4/omnibelt/flow.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/logging.py` & `omnibelt-0.8.4/omnibelt/logging.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/logic.py` & `omnibelt-0.8.4/omnibelt/logic.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/nodes.py` & `omnibelt-0.8.4/omnibelt/nodes.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/operators.py` & `omnibelt-0.8.4/omnibelt/operators.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/ordered_set.py` & `omnibelt-0.8.4/omnibelt/ordered_set.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/packing.py` & `omnibelt-0.8.4/omnibelt/packing.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/patterns.py` & `omnibelt-0.8.4/omnibelt/patterns.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/propagators.py` & `omnibelt-0.8.4/omnibelt/propagators.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/pure_packing.py` & `omnibelt-0.8.4/omnibelt/pure_packing.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/registries.py` & `omnibelt-0.8.4/omnibelt/registries.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 			self._sister_registry_object.__setitem__(v, k, sync=False)
 
 
 	def is_known(self, x):
 		return x in self or x in self.backward()
 
 
-	def find(self, x, default=unspecified_argument):
+	def find(self, x, default: Any = unspecified_argument):
 		if x in self:
 			return self[x]
 		if x in self.backward():
 			return self.backward()[x]
 		if default is not unspecified_argument:
 			return default
 		raise self.NotFoundError(x)
@@ -161,17 +161,29 @@
 		assert isinstance(value, cls.entry_cls)
 		if key == getattr(value, cls._key_name):
 			return getattr(value, cls._sister_key_name)
 		return getattr(value, cls._key_name)
 
 
 	def get_value(self, key, default=unspecified_argument):
-		if default is unspecified_argument:
-			return getattr(self.find(key), self._sister_key_name)
-		return getattr(self.find(key), self._sister_key_name, default)
+		entry = self.find(key, None)
+		if entry is not None:
+			return getattr(entry, self._sister_key_name)
+		if default is not unspecified_argument:
+			return default
+		raise self.NotFoundError(key)
+
+
+	def get_key(self, value, default=unspecified_argument):
+		if value in self.backward():
+			entry = self.backward()[value]
+			return getattr(entry, self._key_name)
+		elif default is not unspecified_argument:
+			return default
+		raise self.NotFoundError(value)
 
 
 	def update(self, other, sync=True):
 		if sync:
 			self._sister_registry_object.update({self._get_sister_entry_key(k, v): v
 			                                     for k, v in other.items()}, sync=False)
 		return super().update(other, sync=False)
@@ -259,16 +271,19 @@
 
 class Class_Registry(Entry_Double_Registry, sister_component='cls'):
 
 	def __init_subclass__(cls, sister_component='cls', components=[], required=[]):
 		super().__init_subclass__(primary_component='name', sister_component=sister_component,
 		                          components=components, required=required)
 
-	def get_class(self, key, default=unspecified_argument):
-		return self.get_value(key, default=default)
+	def get_class(self, name: str, default=unspecified_argument):
+		return self.get_value(name, default=default)
+
+	def get_name(self, cls: type, default=unspecified_argument):
+		return self.get_key(cls, default=default)
 
 	class DecoratorBase(Entry_Double_Registry.DecoratorBase):
 		def _register(self, val, name=None, **params):
 			if name is None:
 				name = val.__name__
 			return super()._register(val, name=name, **params)
```

### Comparing `omnibelt-0.8.3/omnibelt/structured.py` & `omnibelt-0.8.4/omnibelt/structured.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/transactions.py` & `omnibelt-0.8.4/omnibelt/transactions.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/tricks.py` & `omnibelt-0.8.4/omnibelt/tricks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1314,14 +1314,41 @@
 		return fixed_args, fixed_kwargs, missing
 	if allow_positional:
 		return fixed_args, fixed_kwargs
 	assert len(fixed_args) == 0, f'fixed_args: {fixed_args}'
 	return fixed_kwargs
 
 
+def extract_missing_args(fn: Union[Callable, Type], args=None, kwargs=None, *, include_existing=False, skip_first=None):
+	empty_args, existing, missing = extract_function_signature(fn, args, kwargs,
+															   default_fn=lambda key, default: inspect.Parameter.empty,
+															   include_missing=True,
+															   allow_positional=False, allow_rest=True,
+															   force_no_positional=True, skip_first=skip_first)
+	assert len(empty_args) == 0
+
+	if include_existing:
+		return existing, missing
+	return missing
+
+
+
+# def extract_missing_args(fn: Union[Callable, Type],
+#                                args: Optional[Tuple] = None, kwargs: Optional[Dict[str, Any]] = None, *,
+#                                allow_rest: bool = True, including_existing: bool = True, skip_first=None) \
+# 		-> Union[List[inspect.Parameter], Tuple[List[inspect.Parameter], Dict[str, Any]]]:
+
+# 	empty_args, existing, missing = extract_function_signature(fn, args, kwargs, include_missing=True,
+# 															   allow_rest=allow_rest, skip_first=skip_first,
+# 															   force_no_positional=True)
+# 	assert len(empty_args) == 0
+# 	if including_existing:
+# 		return missing, existing
+# 	return missing
+
 
 # class Property(object):
 #     "Emulate PyProperty_Type() in Objects/descrobject.c"
 #
 #     def __init__(self, fget=None, fset=None, fdel=None, doc=None):
 #         self.fget = fget
 #         self.fset = fset
```

### Comparing `omnibelt-0.8.3/omnibelt/typing.py` & `omnibelt-0.8.4/omnibelt/typing.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/utils.py` & `omnibelt-0.8.4/omnibelt/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 
 # from omnibelt import safe_self_execute
 import re
+import builtins
 import ast
 from typing import Iterator, Hashable, Any
 import sys
 from collections import OrderedDict
 from string import Formatter
 from tqdm import tqdm
 from tqdm.notebook import tqdm as tqdm_notebook
@@ -79,16 +80,22 @@
 	Evaluates the keys in the given string as expressions using the given variables
 	"""
 	fmt = Formatter()
 	vals = {key:eval(key, vars) for _, key, _, _ in fmt.parse(s)}
 	return s.format(**vals)
 
 
+_builtin_vars = dir(builtins)
 
 class PowerFormatter(Formatter):
+	@staticmethod
+	def _ignore_variable(var: str):
+		return var in _builtin_vars
+
+
 	def parse(self, s):
 		nodes = self.parse_bracket_tree(s)
 
 		idx = 0
 		for start, end, children in nodes:
 			if children is None:
 				if end > idx:
@@ -188,15 +195,18 @@
 				try:
 					scope[key] = src[key]
 				except KeyError:
 					pass
 				else:
 					break
 			if key not in scope:
-				raise KeyError(f'Variable {key!r} not found in provided args or kwargs')
+				if key in __builtins__:
+					scope[key] = __builtins__[key]
+				else:
+					raise KeyError(f'Variable {key!r} not found in provided args or kwargs')
 		return scope
 
 	def get_field(self, field_name, args, kwargs):
 		try:
 			scope = self.variable_scope(field_name, args, kwargs)
 			out = eval(field_name, scope)
 		except SyntaxError:
@@ -222,26 +232,26 @@
 		nodes = self.parse_bracket_tree(s)
 		past = set()
 		for start, end, children in nodes:
 			if children is None:
 				continue
 			elif len(children):
 				for var in self.variables(s[start + 1:end], allow_repeats=allow_repeats):
-					if var not in past:
+					if var not in past and not self._ignore_variable(var):
 						if not allow_repeats:
 							past.add(var)
 						yield var
 			else:
 				content, spec, conv = self.parse_field(s[start + 1:end])
 				try:
 					vars = self._expression_variables(content)
 				except SyntaxError:
 					continue
 				for var in vars:
-					if var not in past:
+					if var not in past and not self._ignore_variable(var):
 						if not allow_repeats:
 							past.add(var)
 						yield var
 
 
 
 # test_cases = {
```

### Comparing `omnibelt-0.8.3/omnibelt/viz.py` & `omnibelt-0.8.4/omnibelt/viz.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt/wrappers.py` & `omnibelt-0.8.4/omnibelt/wrappers.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/omnibelt.egg-info/PKG-INFO` & `omnibelt-0.8.4/omnibelt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omnibelt
-Version: 0.8.3
+Version: 0.8.4
 Summary: "Omni-belt: A Tool-belt containing pure python utilities for downstream projects"
 Home-page: https://github.com/felixludos/omni-belt
 Author: Felix Leeb
 Author-email: felixludos.info@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `omnibelt-0.8.3/omnibelt.egg-info/SOURCES.txt` & `omnibelt-0.8.4/omnibelt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/setup.cfg` & `omnibelt-0.8.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/tests/test_basics.py` & `omnibelt-0.8.4/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/tests/test_packing.py` & `omnibelt-0.8.4/tests/test_packing.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/tests/test_transactions.py` & `omnibelt-0.8.4/tests/test_transactions.py`

 * *Files identical despite different names*

### Comparing `omnibelt-0.8.3/tests/test_wrappers.py` & `omnibelt-0.8.4/tests/test_wrappers.py`

 * *Files identical despite different names*

