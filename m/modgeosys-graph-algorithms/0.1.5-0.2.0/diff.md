# Comparing `tmp/modgeosys_graph_algorithms-0.1.5.tar.gz` & `tmp/modgeosys_graph_algorithms-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modgeosys_graph_algorithms-0.1.5.tar", max compression
+gzip compressed data, was "modgeosys_graph_algorithms-0.2.0.tar", max compression
```

## Comparing `modgeosys_graph_algorithms-0.1.5.tar` & `modgeosys_graph_algorithms-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     3296 2024-04-06 06:24:37.507965 modgeosys_graph_algorithms-0.1.5/README.md
--rw-r--r--   0        0        0      489 2024-04-06 06:24:55.656051 modgeosys_graph_algorithms-0.1.5/pyproject.toml
--rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.1.5/src/modgeosys/__init__.py
--rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/__init__.py
--rw-r--r--   0        0        0     2969 2024-04-03 15:51:00.826738 modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/a_star.py
--rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/distance.py
--rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/edge_validation.py
--rw-r--r--   0        0        0     1698 2024-04-05 22:46:21.217218 modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/prim.py
--rw-r--r--   0        0        0     4631 2024-04-05 16:19:14.785077 modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/types.py
--rw-r--r--   0        0        0     1100 2024-04-02 16:41:14.618923 modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/conftest.py
--rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/generate_a_star_test_data.py
--rw-r--r--   0        0        0     2178 2024-04-03 15:49:02.994036 modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_a_star.py
--rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_distance.py
--rw-r--r--   0        0        0      580 2024-04-05 17:10:40.308700 modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_prim.py
--rw-r--r--   0        0        0     2680 2024-04-03 15:48:34.777853 modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_types.py
--rw-r--r--   0        0        0     3681 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3535 2024-04-06 17:32:32.989368 modgeosys_graph_algorithms-0.2.0/README.md
+-rw-r--r--   0        0        0      489 2024-04-06 19:06:02.327222 modgeosys_graph_algorithms-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       49 2024-01-20 21:48:11.836178 modgeosys_graph_algorithms-0.2.0/src/modgeosys/__init__.py
+-rw-r--r--   0        0        0       29 2024-01-20 21:50:16.898870 modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/__init__.py
+-rw-r--r--   0        0        0     3088 2024-04-06 18:54:45.417423 modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/a_star.py
+-rw-r--r--   0        0        0      635 2024-04-02 16:41:14.666923 modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/distance.py
+-rw-r--r--   0        0        0      176 2024-04-03 04:46:47.958690 modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/edge_validation.py
+-rw-r--r--   0        0        0     1696 2024-04-06 19:04:49.983022 modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/prim.py
+-rw-r--r--   0        0        0     4729 2024-04-06 18:49:38.140617 modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/types.py
+-rw-r--r--   0        0        0     1529 2024-04-06 18:55:42.785567 modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/conftest.py
+-rw-r--r--   0        0        0      980 2024-01-14 23:04:31.215810 modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/generate_a_star_test_data.py
+-rw-r--r--   0        0        0     7194 2024-04-06 19:01:38.862501 modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_a_star.py
+-rw-r--r--   0        0        0     1860 2024-04-02 16:41:14.626923 modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_distance.py
+-rw-r--r--   0        0        0      580 2024-04-05 17:10:40.308700 modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_prim.py
+-rw-r--r--   0        0        0     2955 2024-04-06 18:58:26.381989 modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_types.py
+-rw-r--r--   0        0        0     3920 1970-01-01 00:00:00.000000 modgeosys_graph_algorithms-0.2.0/PKG-INFO
```

### Comparing `modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/a_star.py` & `modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/a_star.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,53 @@
 from dataclasses import dataclass
 
 from heapdict import heapdict
 
 from modgeosys.graph.types import Edge, Graph, HeuristicDistanceCallable, NoNavigablePathError
 
 
-def a_star(graph: Graph, start_node_index: int, goal_node_index: int, heuristic_distance: HeuristicDistanceCallable) -> list[Edge]:
+@dataclass(order=True)
+class Hop:
+    """A wrapper for an edge that includes the f() function, and the g and h values to support A*."""
+    edge: Edge
+    g: int | float
+    h: int | float
+    cached_f: int | float | None = None
+
+    def f(self) -> int | float:
+        """Calculate the combined cost of the edge."""
+        self.cached_f = self.g + self.h
+        return self.cached_f
+
+    def __eq__(self, other):
+        return self.edge == other.edge and self.cached_f == other.cached_f and self.g == other.g and self.h == other.h
+
+    def __repr__(self):
+        return f'Hop(edge={self.edge}, cached_f={self.cached_f}, g={self.g}, h={self.h})'
+
+    def __hash__(self):
+        return hash(self.edge)
+
+    def __copy__(self):
+        return Hop(edge=self.edge, g=self.g, h=self.h)
+
+    def __deepcopy__(self, memo: Mapping | None = None):
+        return Hop(edge=self.edge, g=self.g, h=self.h)
+
+
+def a_star(graph: Graph, start_node_index: int, goal_node_index: int, heuristic_distance: HeuristicDistanceCallable) -> list[Hop]:
     """Implement the A* algorithm for finding the shortest path between two nodes in a graph."""
 
     # Grab the nodes and adjacency map from the graph.
     nodes         = graph.nodes
     adjacency_map = graph.adjacency_map()
 
     # Initialize the edge hop lists.
     unhopped   = list(graph.edges)
-    hopped     = []
+    hops       = []
 
     # Current node begins with the starting node.
     current_node_index = start_node_index
 
     # Initialize the f heapdict and cumulative g value.
     f = heapdict()
     g = 0
@@ -43,41 +72,13 @@
         # Pick the edge with the lowest f value.
         _, best_hop = f.popitem()
 
         # Update cumulative g, the index of the currently-visited node, and the edge hop lists.
         g                  = best_hop.g
         current_node_index = best_hop.edge.index_of_other_node(current_node_index)
         unhopped.remove(best_hop.edge)
-        hopped.append(best_hop)
+        hops.append(best_hop)
 
         # Clear the auto-sorted f heapdict for reuse with the next hop calculation.
         f.clear()
 
-    return hopped
-
-
-
-@dataclass(order=True)
-class Hop:
-    """A wrapper for an edge that includes the f() function, and the g and h values to support A*."""
-    edge: Edge
-    g: int | float
-    h: int | float
-
-    def f(self) -> int | float:
-        """Calculate the combined cost of the edge."""
-        return self.g + self.h
-
-    def __eq__(self, other):
-        return self.edge == other.edge and self.g == other.g and self.h == other.h
-
-    def __repr__(self):
-        return f'Edge(edge={self.edge}, f={self.f()}, g={self.g}, h={self.h})'
-
-    def __hash__(self):
-        return hash(self.edge)
-
-    def __copy__(self):
-        return Hop(edge=self.edge, g=self.g, h=self.h)
-
-    def __deepcopy__(self, memo: Mapping | None = None):
-        return Hop(edge=self.edge, g=self.g, h=self.h)
+    return hops
```

### Comparing `modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/distance.py` & `modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/prim.py` & `modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/prim.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def prim(graph: Graph, start_node_index: int, edge_is_valid: ValidEdgeCallable = edge_is_always_valid) -> set[Edge]:
     """Implement Prim's algorithm for finding the minimum spanning tree of a graph."""
 
     nodes = graph.nodes
     edges = graph.edges
 
     included_node_indices = {start_node_index}
-    excluded_node_indices = (set(range(len(nodes))) - included_node_indices)
+    excluded_node_indices = set(range(len(nodes))) - included_node_indices
 
     included_edges = set()
     excluded_edges = set(edges)
 
     while excluded_node_indices:
 
         candidate_edges = sorted(edge for edge in excluded_edges if edge.node_indices & included_node_indices)
```

### Comparing `modgeosys_graph_algorithms-0.1.5/src/modgeosys/graph/types.py` & `modgeosys_graph_algorithms-0.2.0/src/modgeosys/graph/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,17 @@
 
 @dataclass(order=True)
 class Edge:
     """An edge in a graph."""
     weight: int | float
     node_indices: frozenset[int] = field(compare=False)
 
+    def __post_init__(self):
+        self.weight = float(self.weight)  # Convert weight to float
+
     def index_of_other_node(self, current_index: int) -> int:
         """Given one node index, return the other node index."""
         node_indices = list(self.node_indices)
         return node_indices[1] if node_indices[0] == current_index else node_indices[0]
 
     def __eq__(self, other):
         return self.weight == other.weight and self.node_indices == other.node_indices
```

### Comparing `modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/generate_a_star_test_data.py` & `modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/generate_a_star_test_data.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_distance.py` & `modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_distance.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_prim.py` & `modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_prim.py`

 * *Files identical despite different names*

### Comparing `modgeosys_graph_algorithms-0.1.5/tests/modgeosys/graph/test_types.py` & `modgeosys_graph_algorithms-0.2.0/tests/modgeosys/graph/test_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,14 +22,24 @@
 
 def test_edge_creation():
     edge = Edge(weight=10.0, node_indices=frozenset((1, 2)))
     assert edge.weight == 10.0
     assert edge.node_indices == frozenset((1, 2))
 
 
+def test_edge_creation_with_int_weight():
+    edge = Edge(weight=10, node_indices=frozenset((1, 2)))
+    assert edge.weight == 10.0
+
+
+def test_edge_creation_with_string_weight():
+    edge = Edge(weight='10.0', node_indices=frozenset((1, 2)))
+    assert edge.weight == 10.0
+
+
 def test_edge_index_of_other_node():
     edge = Edge(weight=10.0, node_indices=frozenset((1, 2)))
     assert edge.index_of_other_node(1) == 2
     assert edge.index_of_other_node(2) == 1
 
 
 def test_edge_equality():
```

