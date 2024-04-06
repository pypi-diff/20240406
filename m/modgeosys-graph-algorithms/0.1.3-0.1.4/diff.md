# Comparing `tmp/modgeosys_graph_algorithms-0.1.3.tar.gz` & `tmp/modgeosys_graph_algorithms-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgeosys_graph_algorithms-0.1.3.tar", max compression
+gzip compressed data, was "modgeosys_graph_algorithms-0.1.4.tar", max compression
```

## Comparing `modgeosys_graph_algorithms-0.1.3.tar` & `modgeosys_graph_algorithms-0.1.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2570 2024-04-05 19:12:57.618449 modgeosys_graph_algorithms-0.1.3/README.md
--rw-r--r--   0        0        0      489 2024-04-06 00:11:53.088142 modgeosys_graph_algorithms-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.1.3/src/modgeosys/__init__.py
--rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.1.3/src/modgeosys/graph/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-03 15:51:00.826738 modgeosys_graph_algorithms-0.1.3/src/modgeosys/graph/a_star.py
--rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.1.3/src/modgeosys/graph/distance.py
--rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.1.3/src/modgeosys/graph/edge_validation.py
--rw-r--r--   0        0        0     1698 2024-04-05 22:46:21.217218 modgeosys_graph_algorithms-0.1.3/src/modgeosys/graph/prim.py
--rw-r--r--   0        0        0     4631 2024-04-05 16:19:14.785077 modgeosys_graph_algorithms-0.1.3/src/modgeosys/graph/types.py
--rw-r--r--   0        0        0     1100 2024-04-02 16:41:14.618923 modgeosys_graph_algorithms-0.1.3/tests/modgeosys/graph/conftest.py
--rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.1.3/tests/modgeosys/graph/generate_a_star_test_data.py
--rw-r--r--   0        0        0     2178 2024-04-03 15:49:02.994036 modgeosys_graph_algorithms-0.1.3/tests/modgeosys/graph/test_a_star.py
--rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.1.3/tests/modgeosys/graph/test_distance.py
--rw-r--r--   0        0        0      580 2024-04-05 17:10:40.308700 modgeosys_graph_algorithms-0.1.3/tests/modgeosys/graph/test_prim.py
--rw-r--r--   0        0        0     2680 2024-04-03 15:48:34.777853 modgeosys_graph_algorithms-0.1.3/tests/modgeosys/graph/test_types.py
--rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2570 2024-04-05 19:12:57.618449 modgeosys_graph_algorithms-0.1.4/README.md
+-rw-r--r--   0        0        0      489 2024-04-06 06:19:38.598603 modgeosys_graph_algorithms-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.1.4/src/modgeosys/__init__.py
+-rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-03 15:51:00.826738 modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/a_star.py
+-rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/distance.py
+-rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/edge_validation.py
+-rw-r--r--   0        0        0     1698 2024-04-05 22:46:21.217218 modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/prim.py
+-rw-r--r--   0        0        0     4631 2024-04-05 16:19:14.785077 modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/types.py
+-rw-r--r--   0        0        0     1100 2024-04-02 16:41:14.618923 modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/conftest.py
+-rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/generate_a_star_test_data.py
+-rw-r--r--   0        0        0     2178 2024-04-03 15:49:02.994036 modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_a_star.py
+-rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_distance.py
+-rw-r--r--   0        0        0      580 2024-04-05 17:10:40.308700 modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_prim.py
+-rw-r--r--   0        0        0     2680 2024-04-03 15:48:34.777853 modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_types.py
+-rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.1.4/PKG-INFO
```

### Comparing `modgeosys_graph_algorithms-0.1.3/README.md` & `modgeosys_graph_algorithms-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.3/src/modgeosys/graph/a_star.py` & `modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.3/src/modgeosys/graph/distance.py` & `modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.3/src/modgeosys/graph/prim.py` & `modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.3/src/modgeosys/graph/types.py` & `modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/types.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.3/tests/modgeosys/graph/conftest.py` & `modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/conftest.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.3/tests/modgeosys/graph/generate_a_star_test_data.py` & `modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/generate_a_star_test_data.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.3/tests/modgeosys/graph/test_a_star.py` & `modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.3/tests/modgeosys/graph/test_distance.py` & `modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.3/tests/modgeosys/graph/test_prim.py` & `modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.3/tests/modgeosys/graph/test_types.py` & `modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_types.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.3/PKG-INFO` & `modgeosys_graph_algorithms-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modgeosys-graph-algorithms
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Kevin Weller
 Author-email: klweller@icloud.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: heapdict (>=1.0.1,<2.0.0)
```

