# Comparing `tmp/peakrdl-halcpp-0.3.5.tar.gz` & `tmp/peakrdl-halcpp-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakrdl-halcpp-0.3.5.tar", last modified: Mon Aug 28 15:09:21 2023, max compression
+gzip compressed data, was "peakrdl-halcpp-0.4.0.tar", last modified: Sat Apr  6 19:24:07 2024, max compression
```

## Comparing `peakrdl-halcpp-0.3.5.tar` & `peakrdl-halcpp-0.4.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 15:09:21.435665 peakrdl-halcpp-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (999)    35122 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)      101 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (999)     1915 2023-08-28 15:09:21.435665 peakrdl-halcpp-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      556 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-28 15:09:21.435665 peakrdl-halcpp-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     1956 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 15:09:21.431665 peakrdl-halcpp-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 15:09:21.431665 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/
--rw-r--r--   0 runner    (1001) docker     (999)       22 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/__about__.py
--rw-r--r--   0 runner    (1001) docker     (999)       34 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1958 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/__peakrdl__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3174 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)    12709 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/haladdrmap.py
--rw-r--r--   0 runner    (1001) docker     (999)     1692 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/halutils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 15:09:21.431665 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/include/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/include/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1098 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/include/addrmap_node.h
--rw-r--r--   0 runner    (1001) docker     (999)      351 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/include/arch_io.h
--rw-r--r--   0 runner    (1001) docker     (999)     3223 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/include/array_nodes.h
--rw-r--r--   0 runner    (1001) docker     (999)     4933 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/include/field_node.h
--rw-r--r--   0 runner    (1001) docker     (999)      728 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/include/halcpp_base.h
--rw-r--r--   0 runner    (1001) docker     (999)     1542 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/include/halcpp_utils.h
--rw-r--r--   0 runner    (1001) docker     (999)     3277 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/include/reg_node.h
--rw-r--r--   0 runner    (1001) docker     (999)      525 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/include/regfile_node.h
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 15:09:21.435665 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/templates/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3616 2023-08-28 15:09:18.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/templates/addrmap.j2
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-28 15:09:21.431665 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     1915 2023-08-28 15:09:21.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      927 2023-08-28 15:09:21.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-28 15:09:21.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       66 2023-08-28 15:09:21.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       41 2023-08-28 15:09:21.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       15 2023-08-28 15:09:21.000000 peakrdl-halcpp-0.3.5/src/peakrdl_halcpp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:24:07.098778 peakrdl-halcpp-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35122 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-06 19:24:07.094778 peakrdl-halcpp-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 19:24:07.098778 peakrdl-halcpp-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:24:07.090778 peakrdl-halcpp-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:24:07.090778 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/__peakrdl__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5869 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16602 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/halnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/halutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:24:07.094778 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/include/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/include/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/include/addrmap_node.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/include/arch_io.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7366 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/include/array_nodes.h
+-rw-r--r--   0 runner    (1001) docker     (127)    10912 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/include/field_node.h
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/include/halcpp_base.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/include/halcpp_utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/include/mem_node.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7050 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/include/reg_node.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/include/regfile_node.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:24:07.094778 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-06 19:24:05.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/templates/addrmap.h.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 19:24:07.094778 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-06 19:24:06.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-06 19:24:07.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 19:24:06.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-06 19:24:06.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-06 19:24:06.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 19:24:06.000000 peakrdl-halcpp-0.4.0/src/peakrdl_halcpp.egg-info/top_level.txt
```

### Comparing `peakrdl-halcpp-0.3.5/LICENSE` & `peakrdl-halcpp-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peakrdl-halcpp-0.3.5/PKG-INFO` & `peakrdl-halcpp-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-halcpp
-Version: 0.3.5
+Version: 0.4.0
 Summary: Generate CPP Hardware Abstraction Layer libraries
 Home-page: https://github.com/Risto97/PeakRDL-halcpp
 Author: Risto Pejasinovic
 Author-email: risto.pejasinovic@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/Risto97/PeakRDL-halcpp
 Project-URL: Tracker, https://github.com/Risto97/PeakRDL-halcpp/issues
@@ -16,14 +16,15 @@
         It is based on C++ 17<br/>
         
         ### Jump straight to project [documentation](https://risto97.github.io/PeakRDL-halcpp/) to learn more.
         
         #### For installation instruction click [here](https://risto97.github.io/PeakRDL-halcpp/docs/getting_started/installation).
         #### For an instruction on how to run a simple example click [here](https://risto97.github.io/PeakRDL-halcpp/docs/getting_started/example)
         
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `peakrdl-halcpp-0.3.5/README.md` & `peakrdl-halcpp-0.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,7 +5,8 @@
 PeakRDL-halcpp is a generator for hardware abstraction layer for peripherals that enables low-level interaction with hardware.
 It is based on C++ 17<br/>
 
 ### Jump straight to project [documentation](https://risto97.github.io/PeakRDL-halcpp/) to learn more.
 
 #### For installation instruction click [here](https://risto97.github.io/PeakRDL-halcpp/docs/getting_started/installation).
 #### For an instruction on how to run a simple example click [here](https://risto97.github.io/PeakRDL-halcpp/docs/getting_started/example)
+
```

### Comparing `peakrdl-halcpp-0.3.5/setup.py` & `peakrdl-halcpp-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     package_dir={'': 'src'},
     packages=setuptools.find_packages("src"),
     include_package_data=True,
     python_requires='>=3.6',
     install_requires=[
         "systemrdl-compiler>=1.25.0",
         "Jinja2>=3.0.0",
+        "peakrdl>=1.1.0",
     ],
     entry_points = {
         "peakrdl.exporters": [
             'halcpp = peakrdl_halcpp.__peakrdl__:Exporter'
         ]
     },
     classifiers=(
```

### Comparing `peakrdl-halcpp-0.3.5/src/peakrdl_halcpp/__peakrdl__.py` & `peakrdl-halcpp-0.4.0/src/peakrdl_halcpp/__peakrdl__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,54 @@
 from typing import TYPE_CHECKING
 
-from peakrdl.plugins.exporter import ExporterSubcommandPlugin #pylint: disable=import-error
-from peakrdl.config import schema #pylint: disable=import-error
+from peakrdl.plugins.exporter import ExporterSubcommandPlugin  # pylint: disable=import-error
 
-# from peakrdl.main import main
-from .exporter import  HalExporter
-import sys
+from .exporter import HalExporter
 
 if TYPE_CHECKING:
     import argparse
     from systemrdl.node import AddrmapNode
 
 
 class Exporter(ExporterSubcommandPlugin):
-    short_desc = "Generate CPP Hardware Abstraction Layer libraries"
-    long_desc = "Generate CPP Hardware Abstraction Layer libraries"
+    """Generates C++ Hardware Abstraction Layer (HAL) libraries."""
 
+    short_desc = 'Generates C++ Hardware Abstraction Layer (HAL) libraries.'
+    long_desc = 'Generates C++ Hardware Abstraction Layer (HAL) libraries.'
 
     def add_exporter_arguments(self, arg_group: 'argparse.ArgumentParser') -> None:
-
+        """Adds custom arguments to the plugin."""
         arg_group.add_argument(
-                "--ext",
-                nargs="*", 
-                help="list of addrmap modules that have implemented <name>_EXT class in <name>_ext.h header file, used for extending functionality"
-                )
+            "--ext",
+            nargs="*",
+            help="List of addrmap modules that have implemented <name>_HAL_EXT class in \
+                <name>_hal_ext.h header file, used for extending functionality."
+        )
 
         arg_group.add_argument(
             "--list-files",
             dest="list_files",
             default=False,
             action="store_true",
-            help="Dont generate files, but instead just list the files that will be generated, and external files that need to be included"
+            help="Dont generate files, but instead just list the files that will be \
+                generated, and external files that need to be included."
         )
 
         arg_group.add_argument(
-            "--keep-buses",
-            dest="keep_buses",
+            "--skip-buses",
+            dest="skip_buses",
             default=False,
             action="store_true",
-            help="If there is an addrmap containing only addrmaps, not registers, by default it will be ommited in hierarchy, it is possible to keep it by passing --keep-buses flag"
+            help="Addrmaps containing only addrmaps, not registers, can be removed by \
+                passing --skip-buses flag."
         )
 
-
     def do_export(self, top_node: 'AddrmapNode', options: 'argparse.Namespace') -> None:
+        """Plugin entry function."""
         hal = HalExporter()
         hal.export(
-            nodes=top_node,
+            node=top_node,
             outdir=options.output,
             list_files=options.list_files,
-            ext=options.ext,
-            keep_buses=options.keep_buses,
+            ext_modules=options.ext,
+            skip_buses=options.skip_buses,
         )
-
-        # if "-DUSE_ZICSR=1" not in sys.argv:
-        #     sys.argv.append("-DUSE_ZICSR=1")
-        #     main()
```

### Comparing `peakrdl-halcpp-0.3.5/src/peakrdl_halcpp.egg-info/PKG-INFO` & `peakrdl-halcpp-0.4.0/src/peakrdl_halcpp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-halcpp
-Version: 0.3.5
+Version: 0.4.0
 Summary: Generate CPP Hardware Abstraction Layer libraries
 Home-page: https://github.com/Risto97/PeakRDL-halcpp
 Author: Risto Pejasinovic
 Author-email: risto.pejasinovic@gmail.com
 License: UNKNOWN
 Project-URL: Source, https://github.com/Risto97/PeakRDL-halcpp
 Project-URL: Tracker, https://github.com/Risto97/PeakRDL-halcpp/issues
@@ -16,14 +16,15 @@
         It is based on C++ 17<br/>
         
         ### Jump straight to project [documentation](https://risto97.github.io/PeakRDL-halcpp/) to learn more.
         
         #### For installation instruction click [here](https://risto97.github.io/PeakRDL-halcpp/docs/getting_started/installation).
         #### For an instruction on how to run a simple example click [here](https://risto97.github.io/PeakRDL-halcpp/docs/getting_started/example)
         
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `peakrdl-halcpp-0.3.5/src/peakrdl_halcpp.egg-info/SOURCES.txt` & `peakrdl-halcpp-0.4.0/src/peakrdl_halcpp.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 MANIFEST.in
 README.md
 setup.py
 src/peakrdl_halcpp/__about__.py
 src/peakrdl_halcpp/__init__.py
 src/peakrdl_halcpp/__peakrdl__.py
 src/peakrdl_halcpp/exporter.py
-src/peakrdl_halcpp/haladdrmap.py
+src/peakrdl_halcpp/halnode.py
 src/peakrdl_halcpp/halutils.py
 src/peakrdl_halcpp.egg-info/PKG-INFO
 src/peakrdl_halcpp.egg-info/SOURCES.txt
 src/peakrdl_halcpp.egg-info/dependency_links.txt
 src/peakrdl_halcpp.egg-info/entry_points.txt
 src/peakrdl_halcpp.egg-info/requires.txt
 src/peakrdl_halcpp.egg-info/top_level.txt
 src/peakrdl_halcpp/include/__init__.py
 src/peakrdl_halcpp/include/addrmap_node.h
 src/peakrdl_halcpp/include/arch_io.h
 src/peakrdl_halcpp/include/array_nodes.h
 src/peakrdl_halcpp/include/field_node.h
 src/peakrdl_halcpp/include/halcpp_base.h
 src/peakrdl_halcpp/include/halcpp_utils.h
+src/peakrdl_halcpp/include/mem_node.h
 src/peakrdl_halcpp/include/reg_node.h
 src/peakrdl_halcpp/include/regfile_node.h
 src/peakrdl_halcpp/templates/__init__.py
-src/peakrdl_halcpp/templates/addrmap.j2
+src/peakrdl_halcpp/templates/addrmap.h.j2
```

