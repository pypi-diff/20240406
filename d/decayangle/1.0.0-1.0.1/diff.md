# Comparing `tmp/decayangle-1.0.0.tar.gz` & `tmp/decayangle-1.0.1.tar.gz`

## Comparing `decayangle-1.0.0.tar` & `decayangle-1.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 decayangle-1.0.0/.pylintrc
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 decayangle-1.0.0/docs/Makefile
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 decayangle-1.0.0/docs/conf.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 decayangle-1.0.0/docs/index.rst
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 decayangle-1.0.0/docs/make.bat
--rw-r--r--   0        0        0    17345 2020-02-02 00:00:00.000000 decayangle-1.0.0/notebooks/decay_example.ipynb
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 decayangle-1.0.0/src/decayangle/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 decayangle-1.0.0/src/decayangle/__init__.py
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 decayangle-1.0.0/src/decayangle/backend.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 decayangle-1.0.0/src/decayangle/config.py
--rw-r--r--   0        0        0    28941 2020-02-02 00:00:00.000000 decayangle-1.0.0/src/decayangle/decay_topology.py
--rw-r--r--   0        0        0    17593 2020-02-02 00:00:00.000000 decayangle-1.0.0/src/decayangle/kinematics.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 decayangle-1.0.0/src/decayangle/lorentz.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 decayangle-1.0.0/src/decayangle/numerics_helpers.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 decayangle-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 decayangle-1.0.0/tests/test_Nbody.py
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 decayangle-1.0.0/tests/test_decay.py
--rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 decayangle-1.0.0/tests/test_kinematics.py
--rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 decayangle-1.0.0/tests/test_lorentz.py
--rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 decayangle-1.0.0/tests/test_sorting.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 decayangle-1.0.0/tests/test_topology.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 decayangle-1.0.0/.gitignore
--rw-r--r--   0        0        0    10483 2020-02-02 00:00:00.000000 decayangle-1.0.0/LICENSE.md
--rw-r--r--   0        0        0    10973 2020-02-02 00:00:00.000000 decayangle-1.0.0/README.md
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 decayangle-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    12045 2020-02-02 00:00:00.000000 decayangle-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    21702 2020-02-02 00:00:00.000000 decayangle-1.0.1/.pylintrc
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 decayangle-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 decayangle-1.0.1/docs/conf.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 decayangle-1.0.1/docs/index.rst
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 decayangle-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0    17345 2020-02-02 00:00:00.000000 decayangle-1.0.1/notebooks/decay_example.ipynb
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/__init__.py
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/backend.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/config.py
+-rw-r--r--   0        0        0    31233 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/decay_topology.py
+-rw-r--r--   0        0        0    17593 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/kinematics.py
+-rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/lorentz.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 decayangle-1.0.1/src/decayangle/numerics_helpers.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/test_Nbody.py
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/test_decay.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/test_kinematics.py
+-rw-r--r--   0        0        0    12288 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/test_lorentz.py
+-rw-r--r--   0        0        0     2046 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/test_sorting.py
+-rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 decayangle-1.0.1/tests/test_topology.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 decayangle-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 decayangle-1.0.1/LICENSE.md
+-rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 decayangle-1.0.1/README.md
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 decayangle-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 decayangle-1.0.1/PKG-INFO
```

### Comparing `decayangle-1.0.0/.pylintrc` & `decayangle-1.0.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/docs/Makefile` & `decayangle-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/docs/conf.py` & `decayangle-1.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/docs/index.rst` & `decayangle-1.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/docs/make.bat` & `decayangle-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/notebooks/decay_example.ipynb` & `decayangle-1.0.1/notebooks/decay_example.ipynb`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/src/decayangle/config.py` & `decayangle-1.0.1/src/decayangle/config.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/src/decayangle/decay_topology.py` & `decayangle-1.0.1/src/decayangle/decay_topology.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Tuple, Union, Any, Dict, Optional
+from typing import List, Tuple, Union, Any, Dict, Optional, Generator, Callable
 from functools import cached_property
 from collections import namedtuple
 import numpy as np
 from jax import numpy as jnp
 import networkx as nx
 from decayangle.lorentz import LorentzTrafo
 from decayangle import kinematics as akm
@@ -10,32 +10,42 @@
 from decayangle.config import config as cfg
 
 cb = cfg.backend
 
 HelicityAngles = namedtuple("HelicityAngles", ["theta_rf", "psi_rf"])
 
 
-def flat(l):
+def flat(l) -> Generator:
     """Flatten a nested list
 
     Args:
         l (list): the list to flatten
 
     Returns:
-        list: the flattened list
+        list: the flattened list as a generator
     """
     if isinstance(l, (tuple, list)):
         for el in l:
             yield from flat(el)
     else:
         yield l
 
 
 class Node:
-
+    """
+    Class to represent a node in a decay topology. The node can have daughters, which are also nodes. 
+    The value of a node is either an integer or a tuple of integers. A tuple implies that the node will finally decay into the particles given in the tuple.
+    The ordering function is used to sort the daughters and the values of the composite nodes.
+
+    Attributes:
+        value (Union[int, Tuple[int]]): the value of the node
+        parent (Node): the parent node of the node
+        daughters (Tuple[Node]): the daughters of the node
+        ordering_function (function): function ordering the daughters and node values of the node
+    """
     @staticmethod
     def construct_topology(node: "Node", topology: Tuple[Union[int, tuple]]):
         """Construct a topology from a tuple of integers and tuples, in the form like the string representation of a topology
 
         i.e. ((1,2), 3)
         or ((1, (2, 3)), 4) for a four body decay
 
@@ -95,15 +105,15 @@
                     "Node value has to be smaller than 10000 to ensure consistent sorting of daughters"
                 )
             self.value = value
         self.__daughters = tuple()
         self.parent = None
 
     @property
-    def ordering_function(self):
+    def ordering_function(self) -> Callable:
         """Get the sorting key of the node.
         This is used to sort the daughters and make sure, that the order of the daughters is consistent.
 
         Returns:
             int: the sorting key
         """
         return self.__sorting_fun
@@ -155,15 +165,15 @@
             raise ValueError("Daughter has to be a Node")
 
         self.__daughters = self.__daughters + (daughter,)
         self.__daughters = self.__sorted_daughters()
         daughter.parent = self
 
     @property
-    def daughters(self) -> List["Node"]:
+    def daughters(self) -> Tuple["Node"]:
         """Get the daughters of the node
 
         Returns:
             List[Node]: the daughters of the node
         """
         return self.__daughters
 
@@ -171,15 +181,15 @@
         if len(self.daughters) == 0:
             return str(self.value)
         return (
             f"( {self.value} -> " + f"{', '.join([str(d) for d in self.daughters])} )"
         )
 
     @property
-    def final_state(self):
+    def final_state(self) -> bool:
         """Check if the node is a final state node by checking if it has daughters
 
         Returns:
             bool: True if the node is a final state node, False otherwise
         """
         return len(self.daughters) == 0
 
@@ -244,29 +254,29 @@
 
         Returns:
             the mass of the particle, as set by the momenta dictionary
             This expects the momenta to be jax or numpy compatible
         """
         return akm.mass(self.momentum(momenta))
 
-    def transform(self, trafo: LorentzTrafo, momenta: dict) -> dict:
+    def transform(self, trafo: LorentzTrafo, momenta: dict) -> Dict[int, Union[np.array, jnp.array]]:
         """Transform the momenta of the final state particles
 
         Args:
             trafo (LorentzTrafo): transformation to apply
             momenta (dict): the momenta of the final state particles
 
         Returns:
             dict: the transformed momenta
         """
         return {
             k: matrix_vector_product(trafo.matrix_4x4, v) for k, v in momenta.items()
         }
 
-    def boost(self, target: Union["Node", int], momenta: dict):
+    def boost(self, target: Union["Node", int], momenta: dict) -> LorentzTrafo:
         """Get the boost from this node to a target node
         The momenta dictionary will define the initial configuration.
         It is expected, that the momenta are jax or numpy compatible and that the momenta are given in the rest frame of this node.
         """
         if not cb.allclose(
             akm.gamma(self.momentum(momenta)),
             cb.ones_like(akm.gamma(self.momentum(momenta))),
@@ -312,17 +322,19 @@
         if nth_daughter >= len(self.daughters):
             raise ValueError(
                 f"Node {self} does not have a daughter with index {nth_daughter}"
             )
         rotation, _, _ = self.rotate_to(self.daughters[nth_daughter], momenta)
         return self.transform(rotation, momenta)
 
-    def helicity_angles(self, momenta: dict):
+    def helicity_angles(self, momenta: dict) -> HelicityAngles:
         """
-        Get the helicity angles for every internal node
+        Get the helicity angles for the daughters of this node.
+        The angles are with respect to the first daughter. 
+        Here the ordering scheme can be important.
 
         Parameters:
             momenta: Dictionary of momenta for the final state particles
 
         Returns:
             Helicity angles for the final state particles
 
@@ -366,14 +378,26 @@
         psi_rf, theta_rf = akm.rotate_to_z_axis(target.momentum(momenta))
         rotation = LorentzTrafo(zero, zero, zero, zero, theta_rf, psi_rf)
 
         return rotation, theta_rf, psi_rf
 
 
 class Topology:
+    """ A class to represent a decay topology as a tree of nodes.
+    The tree is constructed from a root node, which has daughters, which can have daughters and so on.
+    The final state nodes are the nodes without daughters.
+    The ordering function is used to sort the daughters of the nodes and the values of the composite nodes.
+
+    Properties:
+        root (Node): the root node of the topology
+        final_state_nodes (List[Node]): the final state nodes of the topology
+        ordering_function (function): function ordering the daughters and node values of the topology
+    
+    """
+
     def __init__(
         self,
         root: Union[Node, int],
         decay_topology: Optional[List[Union[int, tuple]]] = None,
         ordering_function=None,
     ):
         self.__root = Node.get_node(root)
@@ -406,15 +430,15 @@
 
         Returns:
             List[Node]: the final state nodes of the topology
         """
         return [n for n in self.preorder() if n.final_state]
 
     @property
-    def ordering_function(self):
+    def ordering_function(self) -> Callable:
         """The sorting key of the topology
 
         Returns:
             int: the sorting key of the topology
         """
         return self.__sorting_fun
 
@@ -444,15 +468,15 @@
         Returns:
             bool: True if the node is contained in the topology, False otherwise
         """
         contained_node = Node.get_node(contained_node)
         contained_node.ordering_function = self.ordering_function
         return self.root.contains(contained_node)
 
-    def to_rest_frame(self, momenta: dict):
+    def to_rest_frame(self, momenta: dict) -> Dict[int, Union[np.array, jnp.array]]:
         """Transform the momenta to the rest frame of the root node
 
         Args:
             momenta (dict): the momenta of the final state particles
 
         Returns:
             dict: the momenta in the rest frame of the root node
@@ -476,15 +500,15 @@
         """nodes of the tree
 
         Returns:
             Dict[Union[tuple, int], Node]: A dict of the nodes with the node value as key
         """
         return {n.value: n for n in self.preorder()}
 
-    def helicity_angles(self, momenta: dict) -> Dict[Tuple[int, int], HelicityAngles]:
+    def helicity_angles(self, momenta: dict) -> Dict[Tuple[Union[tuple ,int], Union[tuple ,int]], HelicityAngles]:
         """
         Get a tree with the helicity angles for every internal node
 
         Parameters:
             momenta: Dictionary of momenta for the final state particles
 
         Returns:
@@ -656,19 +680,26 @@
                     r_node.add_daughter(l2)
                     r_node.add_daughter(r2)
                 topologies.append((l_node, r_node))
     return topologies
 
 class TopologyCollection:
     """
-    A group of topologies with the same start node and final state nodes
+    A group of topologies with the same start node and final state nodes. Mostly used to filter topologies based on the internal nodes they contain.
+    Also ensures, that all topologies are for the same final state nodes and start node.
+
+    Attributes:
+        start_node (int): the start node of the topologies. Has to be the same for all topologies.
+        final_state_nodes (list): the final state nodes of the topologies. Have to be the same for all topologies.
+        topologies (list): the topologies of the collection
+        ordering_function (function): function ordering the daughters and node values of the topologies. Will overwrite the ordering function of the topologies.
     """
 
     @staticmethod
-    def filter_list(topologies: List[Node], contained_node: Node):
+    def filter_list(topologies: List[Node], contained_node: Node) -> List[Topology]:
         """
         Filter the topologies based on the number of contained steps.
 
         Args:
             contained_step (list): sub topology for which to filter
         """
         return [t for t in topologies if t.contains(contained_node)]
@@ -708,15 +739,15 @@
         self.node_numbers = dict(enumerate([self.start_node] + self.final_state_nodes))
         if ordering_function is not None:
             self.ordering_function = ordering_function
         else:
             self.ordering_function = cfg.ordering_function
 
     @property
-    def ordering_function(self):
+    def ordering_function(self) -> Callable:
         """The sorting key of the topology, used to sort the daughters of the nodes and the values of the composite nodes
 
         Returns:
             A function returning an integer and accepting an integer or tuple as input
         """
         return self.__sorting_fun
 
@@ -751,26 +782,26 @@
         return [
             Topology(node, ordering_function=self.ordering_function)
             for node in topologies_with_root_node
         ]
 
     @property
     def topologies(self) -> List[Topology]:
-        """returns all possible topologies for the given final state nodes
+        """Returns all possible topologies for the given final state nodes or the topologies provided at initialization
 
         Returns:
-            List[Topology]: all possible topologies for the given final state nodes
+            List[Topology]: the topologies of the collection
         """
         if self.__topologies is None:
             self.__topologies = self.__generate_topologies()
         return self.__topologies
 
-    def filter(self, *contained_nodes: Node):
+    def filter(self, *contained_nodes: Node) -> List[Topology]:
         """
-        Filter the topologies based on the number of contained steps.
+        Filter the topologies based on the number of contained intermediate nodes.
 
         Args:
             contained_nodes (tuple[Node]): nodes which should be contained in the topologies
         """
         topologies = self.topologies
         for contained_node in contained_nodes:
             topologies = self.filter_list(topologies, contained_node)
```

### Comparing `decayangle-1.0.0/src/decayangle/kinematics.py` & `decayangle-1.0.1/src/decayangle/kinematics.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/src/decayangle/lorentz.py` & `decayangle-1.0.1/src/decayangle/lorentz.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,24 @@
 
 cb = cfg.backend
 
 WignerAngles = namedtuple("WignerAngles", ["phi_rf", "theta_rf", "psi_rf"])
 
 
 class LorentzTrafo:
+    """
+    A class to represent a Lorentz transformation. It is initialized with either 6 values or 2 matrices.
+    The matrices are the 2x2 SU(2) matrix and the 4x4 O(3) matrix.
+    Both representations are held in the class and can be accessed via the attributes matrix_2x2 and matrix_4x4.
+
+    The 4x4 matrix is used to perfrom the Lorentz transformation on a 4-vector and to decode the parameters of the transformation up to a rotation of 2 pi.
+    The 2x2 matrix can then be used to determine if a rotation of 2 pi has been performed, as this implies matrix_2x2(decoded params) = -matrix_2x2(original params).
+    This is important information for fermions. 
+    """
+
     def __init__(self, *args, **kwargs):
         if len(args) > 0:
             phi, theta, xi, phi_rf, theta_rf, psi_rf = args
             self.matrix_4x4 = build_4_4(phi, theta, xi, phi_rf, theta_rf, psi_rf)
             self.matrix_2x2 = build_2_2(phi, theta, xi, phi_rf, theta_rf, psi_rf)
         matrix_2x2 = kwargs.get("matrix_2x2", None)
         matrix_4x4 = kwargs.get("matrix_4x4", None)
```

### Comparing `decayangle-1.0.0/src/decayangle/numerics_helpers.py` & `decayangle-1.0.1/src/decayangle/numerics_helpers.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/tests/test_Nbody.py` & `decayangle-1.0.1/tests/test_Nbody.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/tests/test_decay.py` & `decayangle-1.0.1/tests/test_decay.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/tests/test_kinematics.py` & `decayangle-1.0.1/tests/test_kinematics.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/tests/test_lorentz.py` & `decayangle-1.0.1/tests/test_lorentz.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/tests/test_sorting.py` & `decayangle-1.0.1/tests/test_sorting.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/tests/test_topology.py` & `decayangle-1.0.1/tests/test_topology.py`

 * *Files identical despite different names*

### Comparing `decayangle-1.0.0/README.md` & `decayangle-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -215,8 +215,8 @@
 - [ThreeBodyDecays.jl](https://github.com/mmikhasenko/ThreeBodyDecays.jl), 
 - [SymbolicThreeBodyDecays.jl](https://github.com/mmikhasenko/SymbolicThreeBodyDecays.jl),
 - [ComPWA/ampform-dpd](https://github.com/ComPWA/ampform-dpd).
 Consistency of the `decayangle` framework with these appoaches is validated in the tests.
 
 ## License
 
-`decayangle` is distributed under the terms of the [Apache2.0](https://www.apache.org/licenses/LICENSE-2.0) license.
+`decayangle` is distributed under the terms of the [MIT](https://mit-license.org/) license.
```

### Comparing `decayangle-1.0.0/pyproject.toml` & `decayangle-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,21 +9,22 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/decayangle"]
 
 [project]
 name = "decayangle"
 description = 'A tool for wigner rotations in n-body decays'
-version = '1.0.0'
+version = '1.0.1'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Kai Habermann", email = "kai.habermann@gmx.net" },
+  { name = "Mikhail Mikhasenko", email = "mikhail.mikhasenko@cern.ch"},
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
@@ -60,8 +61,8 @@
 ]
 
 [tool.hatch.envs.test.scripts]
 cov = 'pytest --cov-report=term-missing --cov-config=pyproject.toml --cov --cov=tests'
 
 [[tool.hatch.envs.test.matrix]]
 python = ["312", "38", "39", "311", "310"]
-version = ["1.0.0"]
+version = ["1.0.1"]
```

### Comparing `decayangle-1.0.0/PKG-INFO` & `decayangle-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: decayangle
-Version: 1.0.0
+Version: 1.0.1
 Summary: A tool for wigner rotations in n-body decays
 Project-URL: Documentation, https://kaihabermann.github.io/decayangle/
 Project-URL: Issues, https://github.com/KaiHabermann/decayangle/issues
 Project-URL: Source, https://github.com/KaiHabermann/decayangle
-Author-email: Kai Habermann <kai.habermann@gmx.net>
+Author-email: Kai Habermann <kai.habermann@gmx.net>, Mikhail Mikhasenko <mikhail.mikhasenko@cern.ch>
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -242,8 +242,8 @@
 - [ThreeBodyDecays.jl](https://github.com/mmikhasenko/ThreeBodyDecays.jl), 
 - [SymbolicThreeBodyDecays.jl](https://github.com/mmikhasenko/SymbolicThreeBodyDecays.jl),
 - [ComPWA/ampform-dpd](https://github.com/ComPWA/ampform-dpd).
 Consistency of the `decayangle` framework with these appoaches is validated in the tests.
 
 ## License
 
-`decayangle` is distributed under the terms of the [Apache2.0](https://www.apache.org/licenses/LICENSE-2.0) license.
+`decayangle` is distributed under the terms of the [MIT](https://mit-license.org/) license.
```

