# Comparing `tmp/modgeosys_graph_algorithms-0.1.0.tar.gz` & `tmp/modgeosys_graph_algorithms-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgeosys_graph_algorithms-0.1.0.tar", max compression
+gzip compressed data, was "modgeosys_graph_algorithms-0.1.1.tar", max compression
```

## Comparing `modgeosys_graph_algorithms-0.1.0.tar` & `modgeosys_graph_algorithms-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2570 2024-04-05 19:12:57.618449 modgeosys_graph_algorithms-0.1.0/README.md
--rw-r--r--   0        0        0      489 2024-04-05 19:12:46.626416 modgeosys_graph_algorithms-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.1.0/src/modgeosys/__init__.py
--rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.1.0/src/modgeosys/graph/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-03 15:51:00.826738 modgeosys_graph_algorithms-0.1.0/src/modgeosys/graph/a_star.py
--rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.1.0/src/modgeosys/graph/distance.py
--rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.1.0/src/modgeosys/graph/edge_validation.py
--rw-r--r--   0        0        0     1445 2024-04-05 17:13:55.581222 modgeosys_graph_algorithms-0.1.0/src/modgeosys/graph/prim.py
--rw-r--r--   0        0        0     4631 2024-04-05 16:19:14.785077 modgeosys_graph_algorithms-0.1.0/src/modgeosys/graph/types.py
--rw-r--r--   0        0        0     1100 2024-04-02 16:41:14.618923 modgeosys_graph_algorithms-0.1.0/tests/modgeosys/graph/conftest.py
--rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.1.0/tests/modgeosys/graph/generate_a_star_test_data.py
--rw-r--r--   0        0        0     2178 2024-04-03 15:49:02.994036 modgeosys_graph_algorithms-0.1.0/tests/modgeosys/graph/test_a_star.py
--rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.1.0/tests/modgeosys/graph/test_distance.py
--rw-r--r--   0        0        0      580 2024-04-05 17:10:40.308700 modgeosys_graph_algorithms-0.1.0/tests/modgeosys/graph/test_prim.py
--rw-r--r--   0        0        0     2680 2024-04-03 15:48:34.777853 modgeosys_graph_algorithms-0.1.0/tests/modgeosys/graph/test_types.py
--rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2570 2024-04-05 19:12:57.618449 modgeosys_graph_algorithms-0.1.1/README.md
+-rw-r--r--   0        0        0      489 2024-04-05 22:47:03.101333 modgeosys_graph_algorithms-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.1.1/src/modgeosys/__init__.py
+-rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.1.1/src/modgeosys/graph/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-03 15:51:00.826738 modgeosys_graph_algorithms-0.1.1/src/modgeosys/graph/a_star.py
+-rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.1.1/src/modgeosys/graph/distance.py
+-rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.1.1/src/modgeosys/graph/edge_validation.py
+-rw-r--r--   0        0        0     1698 2024-04-05 22:46:21.217218 modgeosys_graph_algorithms-0.1.1/src/modgeosys/graph/prim.py
+-rw-r--r--   0        0        0     4631 2024-04-05 16:19:14.785077 modgeosys_graph_algorithms-0.1.1/src/modgeosys/graph/types.py
+-rw-r--r--   0        0        0     1100 2024-04-02 16:41:14.618923 modgeosys_graph_algorithms-0.1.1/tests/modgeosys/graph/conftest.py
+-rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.1.1/tests/modgeosys/graph/generate_a_star_test_data.py
+-rw-r--r--   0        0        0     2178 2024-04-03 15:49:02.994036 modgeosys_graph_algorithms-0.1.1/tests/modgeosys/graph/test_a_star.py
+-rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.1.1/tests/modgeosys/graph/test_distance.py
+-rw-r--r--   0        0        0      580 2024-04-05 17:10:40.308700 modgeosys_graph_algorithms-0.1.1/tests/modgeosys/graph/test_prim.py
+-rw-r--r--   0        0        0     2680 2024-04-03 15:48:34.777853 modgeosys_graph_algorithms-0.1.1/tests/modgeosys/graph/test_types.py
+-rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.1.1/PKG-INFO
```

### Comparing `modgeosys_graph_algorithms-0.1.0/README.md` & `modgeosys_graph_algorithms-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.0/src/modgeosys/graph/a_star.py` & `modgeosys_graph_algorithms-0.1.1/src/modgeosys/graph/a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.0/src/modgeosys/graph/distance.py` & `modgeosys_graph_algorithms-0.1.1/src/modgeosys/graph/distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.0/src/modgeosys/graph/prim.py` & `modgeosys_graph_algorithms-0.1.1/src/modgeosys/graph/prim.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,21 +15,27 @@
 
     included_edges = set()
     excluded_edges = set(edges)
 
     while excluded_node_indices:
 
         candidate_edges = sorted(edge for edge in excluded_edges if edge.node_indices & included_node_indices)
-
         best_edge = None
 
         for edge in candidate_edges:
+
             if edge_is_valid(edge):
+
                 best_edge = edge
-                new_node_index = next(iter(best_edge.node_indices - included_node_indices))
+                indices = best_edge.node_indices - included_node_indices
+                if len(indices) != 1:
+                    # We've discovered a cycle.  Remove the edge from consideration, and move on.
+                    excluded_edges.remove(best_edge)
+                    continue
+                new_node_index = next(iter(indices))
 
                 included_node_indices.add(new_node_index)
                 excluded_node_indices.remove(new_node_index)
                 included_edges.add(best_edge)
                 excluded_edges.remove(best_edge)
 
                 break
```

### Comparing `modgeosys_graph_algorithms-0.1.0/src/modgeosys/graph/types.py` & `modgeosys_graph_algorithms-0.1.1/src/modgeosys/graph/types.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.0/tests/modgeosys/graph/conftest.py` & `modgeosys_graph_algorithms-0.1.1/tests/modgeosys/graph/conftest.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.0/tests/modgeosys/graph/generate_a_star_test_data.py` & `modgeosys_graph_algorithms-0.1.1/tests/modgeosys/graph/generate_a_star_test_data.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.0/tests/modgeosys/graph/test_a_star.py` & `modgeosys_graph_algorithms-0.1.1/tests/modgeosys/graph/test_a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.0/tests/modgeosys/graph/test_distance.py` & `modgeosys_graph_algorithms-0.1.1/tests/modgeosys/graph/test_distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.0/tests/modgeosys/graph/test_prim.py` & `modgeosys_graph_algorithms-0.1.1/tests/modgeosys/graph/test_prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.0/tests/modgeosys/graph/test_types.py` & `modgeosys_graph_algorithms-0.1.1/tests/modgeosys/graph/test_types.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.0/PKG-INFO` & `modgeosys_graph_algorithms-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modgeosys-graph-algorithms
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Kevin Weller
 Author-email: klweller@icloud.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: heapdict (>=1.0.1,<2.0.0)
```

