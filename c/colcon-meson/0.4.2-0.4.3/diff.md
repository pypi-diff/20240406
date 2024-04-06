# Comparing `tmp/colcon-meson-0.4.2.tar.gz` & `tmp/colcon-meson-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colcon-meson-0.4.2.tar", last modified: Thu Sep 29 02:09:55 2022, max compression
+gzip compressed data, was "colcon-meson-0.4.3.tar", last modified: Sat Apr  6 17:55:29 2024, max compression
```

## Comparing `colcon-meson-0.4.2.tar` & `colcon-meson-0.4.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 02:09:55.165038 colcon-meson-0.4.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2022-09-19 22:21:44.000000 colcon-meson-0.4.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1050 2022-09-29 02:09:55.165038 colcon-meson-0.4.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      630 2022-09-19 22:21:44.000000 colcon-meson-0.4.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 02:09:55.161705 colcon-meson-0.4.2/colcon_meson/
--rw-r--r--   0 root         (0) root         (0)        0 2022-09-19 22:21:44.000000 colcon-meson-0.4.2/colcon_meson/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8340 2022-09-19 22:21:44.000000 colcon-meson-0.4.2/colcon_meson/build.py
--rw-r--r--   0 root         (0) root         (0)     3503 2022-09-19 22:21:44.000000 colcon-meson-0.4.2/colcon_meson/identification.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-09-29 02:09:55.165038 colcon-meson-0.4.2/colcon_meson.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1050 2022-09-29 02:09:55.000000 colcon-meson-0.4.2/colcon_meson.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      332 2022-09-29 02:09:55.000000 colcon-meson-0.4.2/colcon_meson.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-09-29 02:09:55.000000 colcon-meson-0.4.2/colcon_meson.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      217 2022-09-29 02:09:55.000000 colcon-meson-0.4.2/colcon_meson.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       54 2022-09-29 02:09:55.000000 colcon-meson-0.4.2/colcon_meson.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2022-09-29 02:09:55.000000 colcon-meson-0.4.2/colcon_meson.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      838 2022-09-29 02:09:55.165038 colcon-meson-0.4.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2022-09-19 22:21:44.000000 colcon-meson-0.4.2/setup.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-06 17:55:29.232943 colcon-meson-0.4.3/
+-rw-rw-r--   0 christian  (1000) christian  (1000)    11357 2024-03-31 16:27:09.000000 colcon-meson-0.4.3/LICENSE
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1073 2024-04-06 17:55:29.232943 colcon-meson-0.4.3/PKG-INFO
+-rw-rw-r--   0 christian  (1000) christian  (1000)      630 2024-03-31 16:27:09.000000 colcon-meson-0.4.3/README.md
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-06 17:55:29.228943 colcon-meson-0.4.3/colcon_meson/
+-rw-rw-r--   0 christian  (1000) christian  (1000)        0 2024-03-31 16:27:09.000000 colcon-meson-0.4.3/colcon_meson/__init__.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     8340 2024-03-31 16:27:09.000000 colcon-meson-0.4.3/colcon_meson/build.py
+-rw-rw-r--   0 christian  (1000) christian  (1000)     3928 2024-04-06 17:52:20.000000 colcon-meson-0.4.3/colcon_meson/identification.py
+drwxrwxr-x   0 christian  (1000) christian  (1000)        0 2024-04-06 17:55:29.232943 colcon-meson-0.4.3/colcon_meson.egg-info/
+-rw-rw-r--   0 christian  (1000) christian  (1000)     1073 2024-04-06 17:55:29.000000 colcon-meson-0.4.3/colcon_meson.egg-info/PKG-INFO
+-rw-rw-r--   0 christian  (1000) christian  (1000)      332 2024-04-06 17:55:29.000000 colcon-meson-0.4.3/colcon_meson.egg-info/SOURCES.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)        1 2024-04-06 17:55:29.000000 colcon-meson-0.4.3/colcon_meson.egg-info/dependency_links.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)      217 2024-04-06 17:55:29.000000 colcon-meson-0.4.3/colcon_meson.egg-info/entry_points.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)       54 2024-04-06 17:55:29.000000 colcon-meson-0.4.3/colcon_meson.egg-info/requires.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)       13 2024-04-06 17:55:29.000000 colcon-meson-0.4.3/colcon_meson.egg-info/top_level.txt
+-rw-rw-r--   0 christian  (1000) christian  (1000)      862 2024-04-06 17:55:29.232943 colcon-meson-0.4.3/setup.cfg
+-rw-rw-r--   0 christian  (1000) christian  (1000)       38 2024-03-31 16:27:09.000000 colcon-meson-0.4.3/setup.py
```

### Comparing `colcon-meson-0.4.2/LICENSE` & `colcon-meson-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `colcon-meson-0.4.2/PKG-INFO` & `colcon-meson-0.4.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: colcon-meson
-Version: 0.4.2
+Version: 0.4.3
 Summary: Extension for colcon to support Meson packages.
 Author: Christian Rauch
 Author-email: Rauch.Christian@gmx.de
 Maintainer: Christian Rauch
 Maintainer-email: Rauch.Christian@gmx.de
 License: Apache License, Version 2.0
 Project-URL: GitHub, https://github.com/colcon/colcon-meson
 Keywords: colcon
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # colcon-meson
 
 A colcon extension for building [Meson](https://mesonbuild.com) packages.
```

### Comparing `colcon-meson-0.4.2/README.md` & `colcon-meson-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `colcon-meson-0.4.2/colcon_meson/build.py` & `colcon-meson-0.4.3/colcon_meson/build.py`

 * *Files identical despite different names*

### Comparing `colcon-meson-0.4.2/colcon_meson/identification.py` & `colcon-meson-0.4.3/colcon_meson/identification.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,18 +38,30 @@
         elif isinstance(cur, mparser.StringNode):
             return self._holderify(cur.value)
         elif isinstance(cur, mparser.ArrayNode):
             return self.evaluate_arraystatement(cur)
         return None
 
     def function_call(self, node: mparser.FunctionNode) -> typing.Optional[InterpreterObject]:
-        func_name = node.func_name
+        node_func_name = f"{type(node.func_name).__module__}.{type(node.func_name).__qualname__}"
+        if node_func_name == "str":
+            # meson <= 1.2
+            func_name = node.func_name
+        elif node_func_name == "mesonbuild.mparser.IdNode":
+            # meson >= 1.3
+            func_name = node.func_name.value
+        else:
+            raise AttributeError("Cannot determine meson project name.")
+
+        assert type(func_name) == str
+
         reduced_pos = [self.evaluate_statement(arg) for arg in node.args.arguments]
         reduced_pos = list(filter(None, reduced_pos))
         args = self._unholder_args(reduced_pos, {})[0]
+
         if func_name == "project":
             self.data["name"] = args[0]
         elif func_name == "dependency":
             self.data["dependencies"].update(args)
         elif func_name == "subdir":
             subpath = os.path.join(self.source_root, args[0])
             parser = CustomInterpreter(subpath, "", "")
```

### Comparing `colcon-meson-0.4.2/colcon_meson.egg-info/PKG-INFO` & `colcon-meson-0.4.3/colcon_meson.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: colcon-meson
-Version: 0.4.2
+Version: 0.4.3
 Summary: Extension for colcon to support Meson packages.
 Author: Christian Rauch
 Author-email: Rauch.Christian@gmx.de
 Maintainer: Christian Rauch
 Maintainer-email: Rauch.Christian@gmx.de
 License: Apache License, Version 2.0
 Project-URL: GitHub, https://github.com/colcon/colcon-meson
 Keywords: colcon
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # colcon-meson
 
 A colcon extension for building [Meson](https://mesonbuild.com) packages.
```

### Comparing `colcon-meson-0.4.2/setup.cfg` & `colcon-meson-0.4.3/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [metadata]
 name = colcon-meson
-version = 0.4.2
+version = 0.4.3
 project_urls = 
 	GitHub = https://github.com/colcon/colcon-meson
 author = Christian Rauch
 author_email = Rauch.Christian@gmx.de
 maintainer = Christian Rauch
 maintainer_email = Rauch.Christian@gmx.de
 license = Apache License, Version 2.0
 description = Extension for colcon to support Meson packages.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = colcon
 
 [options]
+python_requires = >=3.6
 install_requires = 
 	colcon-core >= 0.10.0
 	colcon-library-path
 	meson >= 0.60.0
 packages = find:
 
 [options.entry_points]
```

