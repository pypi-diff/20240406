# Comparing `tmp/expr_codegen-0.6.0.tar.gz` & `tmp/expr_codegen-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "expr_codegen-0.6.0.tar", last modified: Wed Mar  6 06:34:49 2024, max compression
+gzip compressed data, was "expr_codegen-0.6.1.tar", last modified: Sat Apr  6 05:08:13 2024, max compression
```

## Comparing `expr_codegen-0.6.0.tar` & `expr_codegen-0.6.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 06:34:49.312000 expr_codegen-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-03-06 06:34:49.312000 expr_codegen-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 06:34:49.308000 expr_codegen-0.6.0/expr_codegen/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6998 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/codes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/dag.py
--rw-r--r--   0 runner    (1001) docker     (127)    14425 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/expr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 06:34:49.312000 expr_codegen-0.6.0/expr_codegen/latex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/latex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/latex/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 06:34:49.312000 expr_codegen-0.6.0/expr_codegen/pandas/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/pandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/pandas/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/pandas/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/pandas/template.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 06:34:49.312000 expr_codegen-0.6.0/expr_codegen/polars/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/polars/code.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/polars/printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/polars/template.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/expr_codegen/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 06:34:49.312000 expr_codegen-0.6.0/expr_codegen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-03-06 06:34:49.000000 expr_codegen-0.6.0/expr_codegen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-06 06:34:49.000000 expr_codegen-0.6.0/expr_codegen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 06:34:49.000000 expr_codegen-0.6.0/expr_codegen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-06 06:34:49.000000 expr_codegen-0.6.0/expr_codegen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-06 06:34:49.000000 expr_codegen-0.6.0/expr_codegen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-03-06 06:34:44.000000 expr_codegen-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 06:34:49.312000 expr_codegen-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7588 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/expr_codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/codes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4560 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/dag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14433 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/expr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/expr_codegen/latex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/latex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/latex/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11190 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/expr_codegen/pandas/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/pandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/pandas/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7188 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/pandas/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/pandas/template.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/expr_codegen/polars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3816 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/polars/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/polars/printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/polars/template.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6101 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/expr_codegen/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/expr_codegen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9952 2024-04-06 05:08:13.000000 expr_codegen-0.6.1/expr_codegen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-06 05:08:13.000000 expr_codegen-0.6.1/expr_codegen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 05:08:13.000000 expr_codegen-0.6.1/expr_codegen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-06 05:08:13.000000 expr_codegen-0.6.1/expr_codegen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-06 05:08:13.000000 expr_codegen-0.6.1/expr_codegen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-06 05:08:08.000000 expr_codegen-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 05:08:13.058371 expr_codegen-0.6.1/setup.cfg
```

### Comparing `expr_codegen-0.6.0/LICENSE` & `expr_codegen-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/PKG-INFO` & `expr_codegen-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expr_codegen
-Version: 0.6.0
+Version: 0.6.1
 Summary: symbol expression to polars expression tool
 Author-email: wukan <wu-kan@163.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, wukan
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `expr_codegen-0.6.0/README.md` & `expr_codegen-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/expr_codegen/codes.py` & `expr_codegen-0.6.1/expr_codegen/codes.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,20 @@
                     t.id = self.targets_map.get(t.id, t.id)
                     self.targets_new.add(t.id)
             else:
                 self.targets_old.add(target.id)
                 target.id = self.targets_map.get(target.id, target.id)
                 self.targets_new.add(target.id)
 
+        # 处理 alpha=close 这种情况
+        if isinstance(node.value, ast.Name):
+            self.args_old.add(node.value.id)
+            node.value.id = self.args_map.get(node.value.id, node.value.id)
+            self.args_new.add(node.value.id)
+
         self.generic_visit(node)
         return node
 
     def visit_Compare(self, node):
         # 比较符的左右也可能是变量，要处理
         if isinstance(node.left, ast.Name):
             self.args_old.add(node.left.id)
```

### Comparing `expr_codegen-0.6.0/expr_codegen/dag.py` & `expr_codegen-0.6.1/expr_codegen/dag.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/expr_codegen/expr.py` & `expr_codegen-0.6.1/expr_codegen/expr.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,15 +348,15 @@
     for node in preorder_traversal(e):
         # print(node)
         if len(node.args) == 0:
             continue
         node_name = get_node_name(node)
         node_args0_name = get_node_name(node.args[0])
         if node_name == node_args0_name:
-            if node.name in ('cs_rank', 'sign', 'Abs'):
+            if node.name in ('cs_rank', 'sign', 'Abs', 'abs_'):
                 replacements.append((node, node.args[0]))
     for node, replacement in replacements:
         print(node, '  ->  ', replacement)
         e = e.xreplace({node: replacement})
     return e
```

### Comparing `expr_codegen-0.6.0/expr_codegen/latex/printer.py` & `expr_codegen-0.6.1/expr_codegen/latex/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/expr_codegen/model.py` & `expr_codegen-0.6.1/expr_codegen/model.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/expr_codegen/pandas/code.py` & `expr_codegen-0.6.1/expr_codegen/pandas/code.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/expr_codegen/pandas/printer.py` & `expr_codegen-0.6.1/expr_codegen/pandas/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/expr_codegen/pandas/template.py.j2` & `expr_codegen-0.6.1/expr_codegen/pandas/template.py.j2`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/expr_codegen/polars/code.py` & `expr_codegen-0.6.1/expr_codegen/polars/code.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/expr_codegen/polars/printer.py` & `expr_codegen-0.6.1/expr_codegen/polars/printer.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/expr_codegen/polars/template.py.j2` & `expr_codegen-0.6.1/expr_codegen/polars/template.py.j2`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/expr_codegen/tool.py` & `expr_codegen-0.6.1/expr_codegen/tool.py`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/expr_codegen.egg-info/PKG-INFO` & `expr_codegen-0.6.1/expr_codegen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: expr_codegen
-Version: 0.6.0
+Version: 0.6.1
 Summary: symbol expression to polars expression tool
 Author-email: wukan <wu-kan@163.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, wukan
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `expr_codegen-0.6.0/expr_codegen.egg-info/SOURCES.txt` & `expr_codegen-0.6.1/expr_codegen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `expr_codegen-0.6.0/pyproject.toml` & `expr_codegen-0.6.1/pyproject.toml`

 * *Files identical despite different names*

