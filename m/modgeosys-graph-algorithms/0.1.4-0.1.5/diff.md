# Comparing `tmp/modgeosys_graph_algorithms-0.1.4.tar.gz` & `tmp/modgeosys_graph_algorithms-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgeosys_graph_algorithms-0.1.4.tar", max compression
+gzip compressed data, was "modgeosys_graph_algorithms-0.1.5.tar", max compression
```

## Comparing `modgeosys_graph_algorithms-0.1.4.tar` & `modgeosys_graph_algorithms-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2570 2024-04-05 19:12:57.618449 modgeosys_graph_algorithms-0.1.4/README.md
--rw-r--r--   0        0        0      489 2024-04-06 06:19:38.598603 modgeosys_graph_algorithms-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.1.4/src/modgeosys/__init__.py
--rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-03 15:51:00.826738 modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/a_star.py
--rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/distance.py
--rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/edge_validation.py
--rw-r--r--   0        0        0     1698 2024-04-05 22:46:21.217218 modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/prim.py
--rw-r--r--   0        0        0     4631 2024-04-05 16:19:14.785077 modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/types.py
--rw-r--r--   0        0        0     1100 2024-04-02 16:41:14.618923 modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/conftest.py
--rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/generate_a_star_test_data.py
--rw-r--r--   0        0        0     2178 2024-04-03 15:49:02.994036 modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_a_star.py
--rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_distance.py
--rw-r--r--   0        0        0      580 2024-04-05 17:10:40.308700 modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_prim.py
--rw-r--r--   0        0        0     2680 2024-04-03 15:48:34.777853 modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_types.py
--rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3296 2024-04-06 06:24:37.507965 modgeosys_graph_algorithms-0.1.5/README.md
+-rw-r--r--   0        0        0      489 2024-04-06 06:24:55.656051 modgeosys_graph_algorithms-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.1.5/src/modgeosys/__init__.py
+-rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-03 15:51:00.826738 modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/a_star.py
+-rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/distance.py
+-rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/edge_validation.py
+-rw-r--r--   0        0        0     1698 2024-04-05 22:46:21.217218 modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/prim.py
+-rw-r--r--   0        0        0     4631 2024-04-05 16:19:14.785077 modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/types.py
+-rw-r--r--   0        0        0     1100 2024-04-02 16:41:14.618923 modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/conftest.py
+-rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/generate_a_star_test_data.py
+-rw-r--r--   0        0        0     2178 2024-04-03 15:49:02.994036 modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_a_star.py
+-rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_distance.py
+-rw-r--r--   0        0        0      580 2024-04-05 17:10:40.308700 modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_prim.py
+-rw-r--r--   0        0        0     2680 2024-04-03 15:48:34.777853 modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_types.py
+-rw-r--r--   0        0        0     3681 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.1.5/PKG-INFO
```

### Comparing `modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/a_star.py` & `modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/distance.py` & `modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/prim.py` & `modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.4/src/modgeosys/graph/types.py` & `modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/types.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/conftest.py` & `modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/conftest.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/generate_a_star_test_data.py` & `modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/generate_a_star_test_data.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_a_star.py` & `modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_a_star.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_distance.py` & `modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_prim.py` & `modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.4/tests/modgeosys/graph/test_types.py` & `modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_types.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.4/PKG-INFO` & `modgeosys_graph_algorithms-0.1.5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,63 +1,57 @@
-Metadata-Version: 2.1
-Name: modgeosys-graph-algorithms
-Version: 0.1.4
-Summary: 
-Author: Kevin Weller
-Author-email: klweller@icloud.com
-Requires-Python: >=3.12,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: heapdict (>=1.0.1,<2.0.0)
-Requires-Dist: numpy (>=1.26.3,<2.0.0)
-Description-Content-Type: text/markdown
-
 # modgeosys-graph-algorithms: Graph Algorithms
 
 A repository for [hopefully] clean, readable, and easily-called implementations of some navigation,
 path planning, and obstacle avoidance algorithms I will be using in the near future, written in modern
 Python and/or Rust with Python bindings. I'll be adding more algorithm implementations over time.
 
 ## Algorithms: Currently implemented + planned
 * [A*](https://en.wikipedia.org/wiki/A*_search_algorithm) - Graph path search algorithm.
-  * code-complete in both Python and Rust.
+  * Code-complete in both Python and Rust.
   * Needs a more thorough test suite.
 * [Prim's algorithm](https://en.wikipedia.org/wiki/Prim's_algorithm) - Prim's Minimum Spanning Tree algorithm.
-  * Planned.
+  * Code-complete in Python.
+  * Tested on toy dataset in test suite.
+  * Tested on larger sample (pickled) dataset, not yet incorporated into test suite.
 
 ## Usage
 
-### A\* (Python)
+### A\*
+
+#### Python
 
 ```python
-from modgeosys.graph.a_star import a_star
+from pprint import pprint
+
 from modgeosys.graph.types import Node, Edge, Graph
 from modgeosys.graph.distance import manhattan_distance, euclidean_distance
 
-# Define a graph.
+from modgeosys.graph.a_star import a_star
+
+# Define a toy graph.
 nodes = [Node(coordinates=(0.0, 0.0)),
          Node(coordinates=(0.0, 2.0)),
          Node(coordinates=(1.0, 0.0)),
          Node(coordinates=(2.0, 1.0)),
          Node(coordinates=(2.0, 3.0))]
 edges = (Edge(weight=2.0, node_indices=frozenset((0, 1))),
          Edge(weight=1.0, node_indices=frozenset((0, 2))),
          Edge(weight=1.0, node_indices=frozenset((2, 3))),
          Edge(weight=3.0, node_indices=frozenset((1, 4))),
          Edge(weight=1.0, node_indices=frozenset((3, 4))))
-graph = Graph(nodes=nodes, edges=edges)
+toy_graph = Graph(nodes=nodes, edges=edges)
 
 # Call the A* function.
-path = a_star(graph=graph, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
-
-# Report the resulting path.
-print(path)
+path = a_star(graph=toy_graph, start_node_index=0, goal_node_index=4, heuristic_distance=manhattan_distance)
+print(f'A* Path:')
+pprint(path)
+print()
 ```
 
-### A\* (Rust)
+#### Rust
 ```rust
 use std::collections::HashSet;
 
 use modgeosys_graph::a_star::a_star;
 use modgeosys_graph::types::{Node, Edge, Graph};
 use modgeosys_graph::distance::manhattan_distance;
 
@@ -79,7 +73,30 @@
   // Call the A* function.
   let path = a_star(&graph, 0, 4, manhattan_distance).unwrap();
 
   // Report the resulting path.
   println!("{:?}", path);
 }
 ```
+
+### Prim's algorithm
+
+#### Python
+
+```python
+import pickle
+from pprint import pprint
+
+from modgeosys.graph.types import Node, Edge, Graph
+from modgeosys.graph.distance import manhattan_distance, euclidean_distance
+
+from modgeosys.graph.prim import prim
+
+# Load a bigger graph from a pickle file.
+with open('python/data/graph.pickle', 'rb') as f:
+    larger_graph = pickle.load(f)
+
+# Call the Prim function.
+minimum_spanning_tree = prim(graph=larger_graph, start_node_index=0)
+print('Prim Minimum Spanning Tree:')
+print(minimum_spanning_tree)
+```
```

