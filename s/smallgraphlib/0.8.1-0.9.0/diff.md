# Comparing `tmp/smallgraphlib-0.8.1.tar.gz` & `tmp/smallgraphlib-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smallgraphlib-0.8.1.tar", max compression
+gzip compressed data, was "smallgraphlib-0.9.0.tar", max compression
```

## Comparing `smallgraphlib-0.8.1.tar` & `smallgraphlib-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0     1627 2022-06-15 15:12:16.000000 smallgraphlib-0.8.1/README.md
--rw-r--r--   0        0        0     1351 2024-03-09 23:49:50.999966 smallgraphlib-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      908 2023-03-20 07:12:41.389886 smallgraphlib-0.8.1/smallgraphlib/__init__.py
--rw-r--r--   0        0        0    15943 2024-03-09 23:48:30.711967 smallgraphlib-0.8.1/smallgraphlib/automatons.py
--rw-r--r--   0        0        0     9455 2023-03-26 20:14:38.759490 smallgraphlib-0.8.1/smallgraphlib/basic_graphs.py
--rw-r--r--   0        0        0    30565 2024-03-05 08:49:22.875965 smallgraphlib-0.8.1/smallgraphlib/core.py
--rw-r--r--   0        0        0      733 2023-03-26 21:52:27.177352 smallgraphlib-0.8.1/smallgraphlib/custom_types.py
--rw-r--r--   0        0        0     7409 2023-03-28 16:45:43.464186 smallgraphlib-0.8.1/smallgraphlib/graphs_constructors.py
--rw-r--r--   0        0        0     5459 2024-02-21 08:40:04.415994 smallgraphlib-0.8.1/smallgraphlib/huffman.py
--rw-r--r--   0        0        0    14591 2024-02-21 08:42:41.523994 smallgraphlib-0.8.1/smallgraphlib/labeled_graphs.py
--rw-r--r--   0        0        0     4344 2023-05-06 21:18:44.677477 smallgraphlib-0.8.1/smallgraphlib/latex_export.py
--rw-r--r--   0        0        0        0 2023-03-28 13:52:40.000000 smallgraphlib-0.8.1/smallgraphlib/py.typed
--rw-r--r--   0        0        0     5420 2023-03-22 21:03:51.695796 smallgraphlib-0.8.1/smallgraphlib/string2automaton.py
--rw-r--r--   0        0        0    17143 2024-03-09 23:43:44.771968 smallgraphlib-0.8.1/smallgraphlib/tikz_export.py
--rw-r--r--   0        0        0     2539 2024-02-21 08:42:59.931994 smallgraphlib-0.8.1/smallgraphlib/trees.py
--rw-r--r--   0        0        0     3637 2023-03-27 17:01:34.378737 smallgraphlib-0.8.1/smallgraphlib/utilities.py
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 smallgraphlib-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1627 2022-06-15 15:12:16.000000 smallgraphlib-0.9.0/README.md
+-rw-r--r--   0        0        0     1593 2024-04-06 07:52:03.054000 smallgraphlib-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      970 2024-03-20 07:13:24.463641 smallgraphlib-0.9.0/smallgraphlib/__init__.py
+-rw-r--r--   0        0        0    15567 2024-03-17 08:42:35.019482 smallgraphlib-0.9.0/smallgraphlib/automatons.py
+-rw-r--r--   0        0        0     9670 2024-03-17 08:42:35.019482 smallgraphlib-0.9.0/smallgraphlib/basic_graphs.py
+-rw-r--r--   0        0        0    34062 2024-03-17 09:03:06.835478 smallgraphlib-0.9.0/smallgraphlib/core.py
+-rw-r--r--   0        0        0      820 2024-03-17 08:42:35.019482 smallgraphlib-0.9.0/smallgraphlib/custom_types.py
+-rw-r--r--   0        0        0     3845 2024-03-17 08:42:35.023482 smallgraphlib-0.9.0/smallgraphlib/flow.py
+-rw-r--r--   0        0        0     7784 2024-03-13 13:46:33.779991 smallgraphlib-0.9.0/smallgraphlib/graphs_constructors.py
+-rw-r--r--   0        0        0     6357 2024-04-03 21:16:55.978309 smallgraphlib-0.9.0/smallgraphlib/huffman.py
+-rw-r--r--   0        0        0    15340 2024-04-06 07:25:25.430794 smallgraphlib-0.9.0/smallgraphlib/labeled_graphs.py
+-rw-r--r--   0        0        0     5591 2024-04-03 21:16:18.621814 smallgraphlib-0.9.0/smallgraphlib/latex_export.py
+-rw-r--r--   0        0        0        0 2023-03-28 13:52:40.000000 smallgraphlib-0.9.0/smallgraphlib/py.typed
+-rw-r--r--   0        0        0     5420 2024-03-13 13:46:02.775991 smallgraphlib-0.9.0/smallgraphlib/string2automaton.py
+-rw-r--r--   0        0        0    24051 2024-03-17 08:42:35.023482 smallgraphlib-0.9.0/smallgraphlib/tikz_export.py
+-rw-r--r--   0        0        0     2553 2024-03-13 15:59:44.631960 smallgraphlib-0.9.0/smallgraphlib/trees.py
+-rw-r--r--   0        0        0     4334 2024-03-13 08:50:48.387998 smallgraphlib-0.9.0/smallgraphlib/utilities.py
+-rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 smallgraphlib-0.9.0/PKG-INFO
```

### Comparing `smallgraphlib-0.8.1/README.md` & `smallgraphlib-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `smallgraphlib-0.8.1/pyproject.toml` & `smallgraphlib-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 [tool.poetry]
 name = "smallgraphlib"
-version = "0.8.1"
+version = "0.9.0"
 description = "Simple library for handling small graphs, including Tikz code generation."
 authors = ["Nicolas Pourcelot <nicolas.pourcelot@gmail.com>"]
 repository = "https://github.com/wxgeo/smallgraphlib"
 license = "GPL-3.0-or-later"
 readme = "README.md"
 keywords = ["graph", "tikz", "latex"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7"
 mypy = "^1.8"
-flake8 = "^6"
 black = "^22.1.0"
 tox = "^4.1.2"
 sphinx-autodoc-typehints = "^1.18.3"
 sphinx-rtd-theme = "^1.0.0"#
 myst-parser = "^0.18.0"
 # To test compatibility with sympy.
 sympy = "^1.10.1"
 # Version 7.29+ are buggy !
 python-semantic-release = "7.28.1"
+ruff = "^0.3.2"
+numpy = "^1.26.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
 version_variable = "pyproject.toml:version"
@@ -35,22 +36,37 @@
 [tool.mypy]
 implicit_optional = true
 warn_unused_ignores = true
 
 [tool.black]
 line-length = 110
 
+[tool.pytest.ini_options]
+doctest_optionflags = "NORMALIZE_WHITESPACE IGNORE_EXCEPTION_DETAIL"
+
+[tool.ruff]
+line-length = 110
+fix = true
+
+[tool.ruff.lint]
+ignore = ["E203"]
+
+[tool.ruff.lint.extend-per-file-ignores]
+"tests/test_latex_export.py" = ["E501"]
+
+
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 skipsdist = true
 envlist = py311
 
 [testenv]
 allowlist_externals = poetry
 commands =
     poetry install -v
     poetry run black smallgraphlib tests
+    poetry run ruff check smallgraphlib tests
     poetry run pytest tests
+    poetry run pytest --doctest-modules
     poetry run mypy smallgraphlib tests
-    poetry run flake8 --max-line-length 110 --ignore=E203,W503,W391 --per-file-ignores="tests/test_latex_export.py:E501"
 """
```

### Comparing `smallgraphlib-0.8.1/smallgraphlib/__init__.py` & `smallgraphlib-0.9.0/smallgraphlib/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from importlib import metadata
 
 from smallgraphlib.automatons import Acceptor, Transducer
 from smallgraphlib.basic_graphs import Graph, DirectedGraph
+from smallgraphlib.flow import FlowNetwork
 from smallgraphlib.labeled_graphs import (
     WeightedGraph,
     WeightedDirectedGraph,
     LabeledGraph,
     LabeledDirectedGraph,
 )
 from smallgraphlib.graphs_constructors import (
@@ -32,8 +33,9 @@
     "graph",
     "complete_bipartite_graph",
     "perfect_binary_tree",
     "Traversal",
     "InvalidGraphAttribute",
     "Acceptor",
     "Transducer",
+    "FlowNetwork",
 ]
```

### Comparing `smallgraphlib-0.8.1/smallgraphlib/automatons.py` & `smallgraphlib-0.9.0/smallgraphlib/automatons.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,34 @@
 from abc import ABC
-from typing import Iterable, Generic, TypeVar, NewType, cast, Final
+from typing import Iterable, Generic, TypeVar, NewType, cast
 
 from smallgraphlib.string2automaton import StringToAutomatonParser
 
-from smallgraphlib.custom_types import Node
-from smallgraphlib.labeled_graphs import LabeledEdge, LabeledDirectedGraph
-from smallgraphlib.utilities import cached_property
+from smallgraphlib.custom_types import Node, LabeledEdge
+from smallgraphlib.labeled_graphs import LabeledDirectedGraph
+from smallgraphlib.tikz_export import TikzTransducerPrinter, TikzAcceptorPrinter, TikzAutomatonPrinter
+from smallgraphlib.utilities import cached_property, set_repr
 
 _T = TypeVar("_T", bound="Automaton")
 Char = NewType("Char", str)
 
-GREEK_LETTERS: Final[tuple[str, ...]] = (
-    "alpha",
-    "beta",
-    "gamma",
-    "delta",
-    "epsilon",
-    "zeta",
-    "eta",
-    "theta",
-    "iota",
-    "kappa",
-    "lambda",
-    "mu",
-    "nu",
-    "xi",
-    "pi",
-    "rho",
-    "sigma",
-    "tau",
-    "upsilon",
-    "phi",
-    "chi",
-    "psi",
-    "omega",
-)
-
 
 class UnknownState(RuntimeError):
     """Error raised when a state is unknown to the automat."""
 
 
 class UnknownLetter(RuntimeError):
     """Error raised when a letter is unknown to the automat."""
 
 
 class Automaton(LabeledDirectedGraph, ABC, Generic[Node]):
+    """Base class for all automata. Don't use it directly."""
+
+    printer = TikzAutomatonPrinter  # type: ignore
+
     def __init__(
         self,
         states: Iterable[Node],
         *transitions: LabeledEdge,
         alphabet: Iterable[str] | str,
         initial_states: Iterable[Node],
         alphabet_name: str = None,
@@ -108,39 +87,20 @@
         if state_type:
             state_type += " "
         if state not in self.states:
             raise UnknownState(
                 f"Invalid {state_type}state: {state}. The states of this automaton are {self.states}."
             )
 
-    def _tikz_specific_node_style(self, node: Node) -> str:
-        styles = []
-        if node in self.initial_states:
-            styles.append("rectangle")
-        return ",".join(styles)
-
-    def _tikz_labels(self, node1, node2) -> list[str]:
-        labels = sorted(self.labels(node1, node2))
-        if (
-            self.alphabet_name is not None
-            and sorted(labels) == list(self.alphabet)
-            and len(self.alphabet) > 1
-        ):
-            return [self._latex(self.alphabet_name)]
-        return [",".join(self._latex(label) for label in labels)] if labels else []
-
-    @staticmethod
-    def _latex(label: str) -> str:
-        label = label.replace("#", r"\#")
-        if label in GREEK_LETTERS:
-            label = "\\" + label
-        return f"${label}$" if label else r"$\varepsilon$"
-
 
 class Acceptor(Automaton, Generic[Node]):
+    """An acceptor, i.e. a finite state automaton which defines a language by accepting or rejecting words."""
+
+    printer = TikzAcceptorPrinter  # type: ignore
+
     def __init__(
         self,
         states: Iterable[Node],
         *transitions: LabeledEdge,
         alphabet: Iterable[str] | str,
         initial_states: Iterable[Node],
         final_states: Iterable[Node],
@@ -161,20 +121,14 @@
             self._verify_state(state, state_type="final")
         self.final_states = frozenset(final_states)
 
     @cached_property
     def transitions(self) -> tuple[LabeledEdge, ...]:
         return self.labeled_edges
 
-    def _tikz_specific_node_style(self, node: Node) -> str:
-        styles = [super()._tikz_specific_node_style(node)]
-        if node in self.final_states:
-            styles.append("double,fill=lightgray")
-        return ",".join(styles)
-
     def recognize(self, word: str, _start: Iterable[Node] = None) -> bool:
         states = set(_start) if _start is not None else self.initial_states
         if word == "":
             # Any of the current states must be final.
             return len(states & self.final_states) != 0
         return any(self.recognize(word[1:], self.transition_func(state, Char(word[0]))) for state in states)
 
@@ -189,32 +143,43 @@
                 other.transition_func(state, letter) == self.transition_func(state, letter)
                 for letter in self.alphabet
                 for state in self.states
             )
         )
 
     def __repr__(self):
+        # Sort set elements to make doctests deterministic.
+        initial_states = set_repr(self.initial_states)
+        final_states = set_repr(self.final_states)
+        indicate_alphabet_name = (
+            "" if self.alphabet_name is None else f", alphabet_name={self.alphabet_name!r}"
+        )
+
         return (
             f"{self.__class__.__name__}({self.states!r}, "
             f"{', '.join(repr(transition) for transition in self.transitions)}, "
-            f"alphabet={''.join(self.alphabet)!r}, initial_states={set(self.initial_states)!r}, "
-            f"final_states={set(self.final_states)!r}, alphabet_name={self.alphabet_name!r})"
+            f"alphabet={''.join(self.alphabet)!r}, initial_states={initial_states}, "
+            f"final_states={final_states}{indicate_alphabet_name})"
         )
 
     @classmethod
     def from_string(
         cls,
         string: str,
         sep: tuple[str, str, str, str, str] = ("/", ":", ";", "--", "|"),
         alphabet: Iterable[str] = None,
         alphabet_name: str = None,
     ) -> "Acceptor":
         """Constructor used to generate an automaton from a string.
 
-            >>> Acceptor.from_string(">(I):a|b--1  /  (1):a--2;b--3  /  (2):a--1|I  /  3")
+            >>> s = ">(I):a|b--1  /  (1):a--2;b--3  /  (2):a--1|I  /  3"
+            >>> Acceptor.from_string(s)
+            Acceptor(('1', '2', '3', 'I'), ('1', '2', 'a'), ('1', '3', 'b'), ('2', '1', 'a'), ('2', 'I', 'a'),
+                     ('I', '1', 'a'), ('I', '1', 'b'),
+                     alphabet='ab', initial_states={'I'}, final_states={'1', '2', 'I'})
 
         will generate an automaton of 4 states: `I`, `1`, `2` and `3`,
         each state information being separated by `/`.
 
         Each state can be marked as initial or final:
 
             - The parentheses `()` around states `I`, `1` and `2` mean those states will be final.
@@ -231,19 +196,30 @@
         (transition without reading any letter).
 
         Separators may be changed using `sep` keyword:
 
             >>> Acceptor.from_string(
             ...    ">(I):a,b:1 ; (1):a:2+b:3 ; (2):a:1,I ; 3", sep=(";", ":", "+", ":", ",")
             ...    )
+            Acceptor(('1', '2', '3', 'I'), ('1', '2', 'a'), ('1', '3', 'b'), ('2', '1', 'a'), ('2', 'I', 'a'),
+                     ('I', '1', 'a'), ('I', '1', 'b'),
+                     alphabet='ab', initial_states={'I'}, final_states={'1', '2', 'I'})
 
         If a transition applies for every letter, one may use the alphabet name, `**` or `ALL`
         instead of listing all the letters.
 
-            >>> Acceptor.from_string(">I:a--1;b / (1):**--I")
+            >>> acceptor = Acceptor.from_string(">I:a--1;b / (1):**--I")
+            >>> acceptor
+            Acceptor(('1', 'I'), ('1', 'I', 'a'), ('1', 'I', 'b'), ('I', '1', 'a'), ('I', 'I', 'b'),
+            alphabet='ab', initial_states={'I'}, final_states={'1'})
+            >>> acceptor == Acceptor.from_string(">I:a--1;b / (1):ALL--I")
+            True
+            >>> Acceptor.from_string(">I:a--1;b / (1):S--I", alphabet_name="S")
+            Acceptor(('1', 'I'), ('1', 'I', 'a'), ('1', 'I', 'b'), ('I', '1', 'a'), ('I', 'I', 'b'),
+            alphabet='ab', initial_states={'I'}, final_states={'1'}, alphabet_name='S')
         """
         data = StringToAutomatonParser(sep).parse(string)
         if alphabet is None:
             # `**` notation stands for all alphabet's letters.
             alphabet = {letter for state, next_state, letter in data.transitions} - {
                 "**",
                 alphabet_name,
@@ -271,17 +247,19 @@
     """A deterministic transducer.
 
     A transducer is a finite states automaton which translates an input word into another word.
 
         >>> from smallgraphlib import Transducer
         >>> transducer = Transducer.from_string(">I:a--1;b / 1:b;a[#]--I")
         >>> transducer.translate("aababba")  # Count the number of "ba" substrings
-        "##"
+        '##'
     """
 
+    printer = TikzTransducerPrinter  # type: ignore
+
     def __init__(
         self,
         states: Iterable[Node],
         *transitions: tuple[Node, Node, str] | tuple[Node, Node, str, str],
         input_alphabet: Iterable[str] | str,
         output_alphabet: Iterable[str] | str,
         initial_state: Node,
@@ -347,46 +325,27 @@
         state = next(iter(self.initial_states))
         output = []
         for letter in word:
             output.append(self.next_word(state, letter))
             state = self.next_state(state, letter)
         return "".join(output)
 
-    def _tikz_labels(self, node1: Node, node2: Node) -> list[str]:
-        # Associate to each output word all the input letters than can produce it.
-        words: dict[str, set[Char]] = {}
-        for letter in self.alphabet:
-            if self.next_state(node1, letter) == node2:
-                words.setdefault(self.next_word(node1, letter), set()).add(letter)
-
-        labels: list[str] = []
-        for word, letters in words.items():
-            sorted_letters = sorted(letters)
-            if sorted_letters == list(self.alphabet) and self.alphabet_name is not None:
-                letters_str = self.alphabet_name
-            else:
-                letters_str = ",".join(sorted_letters)
-            letters_str = self._latex(letters_str)
-            if word:
-                letters_str += rf"\fbox{{{self._latex(word)}}}"
-            labels.append(letters_str)
-        return labels
-
     @classmethod
     def from_string(
         cls,
         string: str,
         sep: tuple[str, str, str, str, str] = ("/", ":", ";", "--", "|"),
         alphabet_name: str = None,
     ) -> "Transducer":
         """This constructor is used to generate transducers.
 
         For example, the following automaton prints a "#" character for each "ba" substring read.
 
             >>> Transducer.from_string(">I:a--1;b / 1:b;a[#]--I")
+            Transducer(('1', 'I'), ('1', '1', 'b'), ('1', 'I', 'a'), ('I', '1', 'a'), ('I', 'I', 'b'))
 
         Extensive syntax description can be found in `Acceptor.from_string()` documentation.
         """
 
         data = StringToAutomatonParser(sep).parse(string)
         # Extract output information from transitions labels
         transitions: list[tuple[str, str, str, str]] = []
```

### Comparing `smallgraphlib-0.8.1/smallgraphlib/basic_graphs.py` & `smallgraphlib-0.9.0/smallgraphlib/basic_graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,41 +2,39 @@
 # -*- coding: utf-8 -*-
 """
 Created on Sat May  7 12:24:58 2022
 
 @author: nicolas
 """
 from typing import (
-    Tuple,
-    Dict,
-    List,
     FrozenSet,
     Sequence,
+    Generic,
 )
 
 from smallgraphlib.core import (
     AbstractGraph,
     InvalidGraphAttribute,
 )
 from smallgraphlib.custom_types import Node, DirectedEdge, UndirectedEdge
 from smallgraphlib.utilities import (
     cached_property,
 )
 
 
-class Graph(AbstractGraph):
+class Graph(AbstractGraph, Generic[Node]):
     """A graph with undirected edges.
 
     >>> G = Graph((1, 2, 3), {1, 3}, {1, 2}, {2, 1}, {1})
     """
 
     @staticmethod
     def _get_edges_from_adjacency_matrix(
         matrix: Sequence[Sequence[int]],
-    ) -> List[Tuple[int, int]]:
+    ) -> list[tuple[int, int]]:
         edges = []
         for i in range(len(matrix)):
             for j in range(i + 1):  # we must only deal with i <= j, since it is an undirected graph.
                 if i == j:
                     if matrix[i][i] % 2 == 1:
                         raise ValueError(
                             "The adjacency matrix of an undirected graph must have "
@@ -54,16 +52,19 @@
                 edges.extend(edge_multiplicity * [(i + 1, j + 1)])
         return edges
 
     def is_isomorphic_to(self, other) -> bool:
         return super().is_isomorphic_to(other)
 
     def __repr__(self):
-        edges = (repr(set(edge)) for edge in self.edges)
-        return f"Graph({tuple(self.nodes)!r}, {', '.join(edges)})"
+        # Sort nodes in edges for undirected graphs, so that doctests
+        # can be deterministic.
+        edges_as_couples = sorted(sorted(edge) for edge in self.edges)
+        edges = ", ".join(f"{{{node1!r}, {node2!r}}}" for node1, node2 in edges_as_couples)
+        return f"Graph({tuple(self.nodes)!r}, {edges})"
 
     @property
     def is_directed(self):
         return False
 
     @staticmethod
     def _edge(node1: Node, node2: Node = None) -> UndirectedEdge:
@@ -83,16 +84,16 @@
         return self._count_odd_degrees() == 2
 
     @cached_property
     def is_connected(self):
         return self._test_connection_from_node(next(iter(self.nodes)))
 
     @cached_property
-    def greedy_coloring(self) -> Dict[Node, int]:
-        coloring: Dict[Node, int] = {}
+    def greedy_coloring(self) -> dict[Node, int]:
+        coloring: dict[Node, int] = {}
         # Sort nodes by reversed degree, then alphabetically
         nodes = sorted(self.nodes, key=(lambda _node: (-self.node_degree(_node), _node)))
         for node in nodes:
             color_num = 0
             while any(coloring.get(adjacent) == color_num for adjacent in self.successors(node)):
                 color_num += 1
             coloring[node] = color_num
@@ -129,36 +130,36 @@
         if not self.is_subgraph_stable(*nodes_group):
             return False
         if not self.is_subgraph_stable(*other_group):
             return False
         return all(self.are_adjacents(node1, node2) for node1 in nodes_group for node2 in other_group)
 
 
-class DirectedGraph(AbstractGraph):
+class DirectedGraph(AbstractGraph, Generic[Node]):
     """A graph with directed edges.
 
     >>> G = DirectedGraph((1, 2, 3), (1, 3), (1, 2), (2, 1), (1, 1))
     """
 
     @staticmethod
     def _get_edges_from_adjacency_matrix(
         matrix: Sequence[Sequence[int]],
-    ) -> List[Tuple[int, int]]:
+    ) -> list[tuple[int, int]]:
         edges = []
         for i in range(len(matrix)):
             for j in range(len(matrix)):
                 edge_multiplicity = matrix[i][j]
                 edges.extend(edge_multiplicity * [(i + 1, j + 1)])
         return edges
 
     def is_isomorphic_to(self, other) -> bool:
         return super().is_isomorphic_to(other)
 
     def __repr__(self):
-        edges = (repr(edge) for edge in self.edges)
+        edges = sorted(repr(edge) for edge in self.edges)
         return f"DirectedGraph({tuple(self.nodes)!r}, {', '.join(edges)})"
 
     @property
     def is_directed(self):
         return True
 
     @staticmethod
@@ -182,17 +183,17 @@
             elif out_degree == in_degree - 1 and not end_found:
                 end_found = True
             elif out_degree != in_degree:
                 return False
         return start_found and end_found
 
     @cached_property
-    def levels(self) -> Tuple[FrozenSet[Node], ...]:
+    def levels(self) -> tuple[FrozenSet[Node], ...]:
         graph = self.copy()
-        levels: List[FrozenSet] = []
+        levels: list[FrozenSet] = []
         while True:
             level = set()
             for node in graph.nodes:
                 if graph.out_degree(node) == 0:  # is node a sink ?
                     level.add(node)
             if len(level) == 0:
                 break
@@ -259,15 +260,15 @@
         for i in range(n):
             for j in range(n):
                 for k in range(n):
                     M[i][j] = M[i][j] or (M[i][k] and M[k][j])
         return M
 
     @cached_property
-    def transitive_closure_matrix(self) -> Tuple[Tuple[int, ...], ...]:
+    def transitive_closure_matrix(self) -> tuple[tuple[int, ...], ...]:
         """Return the matrix of the transitive closure."""
         # Make a mutable copy of the adjacency matrix.
         M = [list(line) for line in self.adjacency_matrix]
 
         while True:
             new_M = self._apply_transitivity_to(M)
             if new_M == M:
```

### Comparing `smallgraphlib-0.8.1/smallgraphlib/core.py` & `smallgraphlib-0.9.0/smallgraphlib/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,144 +7,160 @@
 from numbers import Integral
 from typing import (
     Tuple,
     FrozenSet,
     Set,
     Iterable,
     Any,
-    Dict,
-    List,
     Generic,
     Counter as CounterType,
     Optional,
     Iterator,
     Sequence,
     Type,
+    Callable,
+    Self,
 )
 
 from smallgraphlib.custom_types import _AbstractGraph, Node, Edge, EdgeLike
 from smallgraphlib.utilities import cached_property, Multiset, clear_cache
-from smallgraphlib.tikz_export import tikz_printer
+from smallgraphlib.tikz_export import TikzPrinter
 
 
 class Traversal(Enum):
     PREORDER = 0
     POSTORDER = 1
     INORDER = 2
 
 
 class NodeAlreadyFoundError(RuntimeError):
     pass
 
 
 class AbstractGraph(ABC, Generic[Node]):
+    printer = TikzPrinter
+
     def __init__(
         self,
         nodes: Iterable[Node],
         *edges: EdgeLike,
         sort_nodes: bool = True,
     ):
         """Create a graph of nodes, when nodes may be any hashable objects.
 
         Edges may be any iterable of two nodes.
 
         If the graph is directed and the edge is a set {A, B} of two nodes,
         then two edges are added, one from A to B and one from B to A.
         Note that in that case, adding {A} will result in two edges too.
         """
-        self._successors: Dict[Node, CounterType[Node]] = {}
+        self._successors: dict[Node, CounterType[Node]] = {}
         if self.is_directed:
-            self._predecessors: Dict[Node, CounterType[Node]] = {}
+            self._predecessors: dict[Node, CounterType[Node]] = {}
         else:
             self._predecessors = self._successors
         # Nodes must be added before edges.
         if sort_nodes:
             nodes = sorted(nodes)
         self.add_nodes(*nodes)
         self.add_edges(*edges)
 
     # ------------------
     # Other constructors
     # ------------------
 
     @classmethod
-    def from_dict(cls: Type[_AbstractGraph], d: dict[Node, Iterable[Node]]) -> _AbstractGraph:
-        """DirectedGraph.from_dict({1: [2, 3], 2: [], 3: [1]}) will generate a graph of
-        3 nodes, 1, 2 and 3, with edges 1->2, 1->3 and 3->1."""
+    def from_dict(
+        cls: Type[_AbstractGraph], d: dict[Node, Iterable[Node]] = None, /, **successors: Iterable[Node]
+    ) -> _AbstractGraph:
+        """Generate a graph from a dictionary of nodes, each node being associated with its successors.
+
+        For example `DirectedGraph.from_dict({1: [2, 3], 2: [], 3: [1]})` will generate a graph of
+        3 nodes, 1, 2 and 3, with edges 1->2, 1->3 and 3->1.
+
+            >>> from smallgraphlib import DirectedGraph
+            >>> DirectedGraph.from_dict({1: [2, 3], 2: [], 3: [1]})
+            DirectedGraph((1, 2, 3), (1, 2), (1, 3), (3, 1))
+            >>> DirectedGraph.from_dict(A="BC", B="", C="A")
+            DirectedGraph(('A', 'B', 'C'), ('A', 'B'), ('A', 'C'), ('C', 'A'))
+        """
+        if d is None:
+            d = {}
+        d.update(successors)  # type: ignore
         nodes: set[Node] = set()
-        edges: list[Tuple[Node, Node]] = []
+        edges: list[tuple[Node, Node]] = []
         for start, ends in d.items():
             nodes.add(start)
             nodes.update(ends)
             edges.extend((start, end) for end in ends)
         return cls(nodes, *edges)
 
     @classmethod
     def from_string(cls: Type[_AbstractGraph], string: str) -> _AbstractGraph:
         """DirectedGraph.from_string("A:B,C B:C C") will generate a graph of 3 nodes, A, B and C, with
         edges A->B, A->C and B->C."""
-        nodes: List[str] = []
-        edges: List[Tuple[str, str]] = []
+        nodes: list[str] = []
+        edges: list[tuple[str, str]] = []
         for substring in string.split():
             node, *remaining = substring.split(":", 1)
             nodes.append(node.strip())
             if remaining:
                 edges.extend((node, successor.strip()) for successor in remaining[0].split(","))
         return cls(nodes, *edges)
 
     @staticmethod
-    def _matrix_as_tuple_of_tuples(matrix: Iterable[Iterable]) -> Tuple[Tuple, ...]:
+    def _matrix_as_tuple_of_tuples(matrix: Iterable[Iterable]) -> tuple[Tuple, ...]:
         if hasattr(matrix, "tolist"):  # for numpy or sympy
             matrix = matrix.tolist()
-        M = tuple(tuple(iterable) for iterable in matrix)
+        tuple_matrix = tuple(tuple(iterable) for iterable in matrix)
         # Test if M is correct
-        n = len(M)
-        if any(len(line) != n for line in M):
+        n = len(tuple_matrix)
+        if any(len(line) != n for line in tuple_matrix):
             raise ValueError("All matrix lines must be the same length.")
-        return M
+        return tuple_matrix
 
     @staticmethod
     @abstractmethod
     def _get_edges_from_adjacency_matrix(
         matrix: Sequence[Sequence[int]],
-    ) -> List[Tuple[int, int]]:
+    ) -> list[tuple[int, int]]:
         ...
 
     @classmethod
     def from_matrix(
         cls: Type[_AbstractGraph], matrix: Iterable[Iterable[int]], nodes_names: Iterable[Node] = None
     ) -> _AbstractGraph:
         """Construct the graph corresponding to the given adjacency matrix.
 
         Matrix must be a matrix of positive integers
         (`int` or any integer type inheriting from `numbers.Integral`).
         """
         # Convert iterable to matrix.
-        M = cls._matrix_as_tuple_of_tuples(matrix)
+        tuple_matrix = cls._matrix_as_tuple_of_tuples(matrix)
         # Test if M is correct
-        n = len(M)
-        for line in M:
+        n = len(tuple_matrix)
+        for line in tuple_matrix:
             for val in line:
                 if not (isinstance(val, Integral) and int(val) >= 0):
                     raise ValueError(f"All matrix values must be positive integers, but {val!r} is not.")
 
-        edges = cls._get_edges_from_adjacency_matrix(M)
+        edges = cls._get_edges_from_adjacency_matrix(tuple_matrix)
 
         g = cls(range(1, n + 1), *edges)
         if nodes_names:
             g.rename_nodes(dict(enumerate(list(nodes_names)[: len(g.nodes)], start=1)))
         return g
 
     # ------------
     # Node methods
     # ------------
 
     # Nodes must be ordered, to generate the matrix, so do *not* return a set.
     @cached_property
-    def nodes(self) -> Tuple[Node, ...]:
+    def nodes(self) -> tuple[Node, ...]:
         return tuple(self._successors)
 
     @cached_property
     def nodes_set(self) -> FrozenSet[Node]:
         return frozenset(self.nodes)
 
     def _add_node(self, node: Node) -> None:
@@ -180,15 +196,15 @@
             for node, counter in list(dictionary.items()):  # make a copy, since we modify the dictionary.
                 if node == old_name:
                     dictionary[new_name] = dictionary.pop(old_name)
                 if old_name in counter:
                     counter[new_name] = counter.pop(old_name)
 
     @clear_cache
-    def rename_nodes(self, node_names: Dict[Node, Node]) -> None:
+    def rename_nodes(self, node_names: dict[Node, Node]) -> None:
         if not node_names:
             return
         # First, we must assure the atomicity of the renaming operation:
         # it should not fail half-way if a node is not found, or if two renaming rules will conflict...
         # This is an incorrect renaming for example:
         # {A -> E, B -> E}
         # ({A -> E, A -> F} would be incorrect too, but can't occur with dict.)
@@ -219,30 +235,30 @@
                 f"Names conflict in renaming, when trying to apply the following names {conflicts}."
             )
 
         # The renaming operation must look simultaneous:
         # for example, we must avoid that applying {A -> B, B -> C} will result in A −> C !
         # The solution is to use temporary names when renaming.
         # Something like {A -> tmp_B, B -> tmp_C} and then {tmp_B -> B, tmp_C -> C}.
-        remaining_translation: List[Node] = []
+        remaining_translation: list[Node] = []
         # Use list() to make a copy of the dictionary keys and values, since we modify the dictionary.
         for i, (old_name, new_name) in enumerate(list(node_names.items())):
             self.rename_node(old_name, "\00" + str(i))
             remaining_translation.append(new_name)
         for i, new_name in enumerate(remaining_translation):
             self.rename_node("\00" + str(i), remaining_translation[i])
 
     def shuffle_nodes(self):
         """Shuffle nodes.
 
         >>> from smallgraphlib import random_graph
         >>> g = random_graph(4, 7)
         >>> g2 = g.copy()
         >>> g2.shuffle_nodes()
-        >>> g == g2
+        >>> g == g2  # doctest: +SKIP
         ...  # probably False
         >>> g.is_isomorphic_to(g2)
         True
         """
         # Sort nodes before shuffling, to make shuffling deterministic with a given random.seed.
         # nodes = sorted(self.nodes)
         nodes = list(self.nodes)
@@ -250,15 +266,15 @@
         self.rename_nodes(dict((old_name, new_name) for old_name, new_name in zip(self.nodes, nodes)))
 
     # ------------
     # Edge methods
     # ------------
 
     @cached_property
-    def edges(self) -> Tuple[Edge, ...]:
+    def edges(self) -> tuple[Edge, ...]:
         edges_count: CounterType[Edge] = Multiset()
         for node in self.nodes:
             for successor in self.successors(node):
                 edge: Edge = self._edge(node, successor)
                 edges_count[edge] += self.count_edges(node, successor)
         if not self.is_directed:
             for key in edges_count:
@@ -266,15 +282,15 @@
         return tuple(edges_count.elements())
 
     @cached_property
     def edges_set(self) -> FrozenSet[Edge]:
         return frozenset(self.edges)
 
     @staticmethod
-    def _get_edge_extremities(edge: EdgeLike) -> Tuple[Node, Node]:
+    def _get_edge_extremities(edge: EdgeLike) -> tuple[Node, Node]:
         nodes = iter(edge)
         start = next(nodes)
         try:
             end = next(nodes)
         except StopIteration:
             end = start
         try:
@@ -332,31 +348,31 @@
             return False
 
         if self.order == 0:
             return other.order == 0
 
         def count_in_and_out_degrees(
             graph: AbstractGraph,
-        ) -> CounterType[Tuple[int, int]]:
+        ) -> CounterType[tuple[int, int]]:
             return Counter((graph.in_out_degree(node_) for node_ in graph.nodes))
 
         if count_in_and_out_degrees(self) != count_in_and_out_degrees(other):
             return False
         assert self.order == other.order and self.degree == other.degree
 
-        degrees_to_nodes_for_other_graph: Dict[Tuple[int, int], List[Node]] = {}
+        degrees_to_nodes_for_other_graph: dict[tuple[int, int], list[Node]] = {}
         for node in other.nodes:
             degrees_to_nodes_for_other_graph.setdefault(other.in_out_degree(node), []).append(node)
         nodes_to_degrees_for_self = {node: self.in_out_degree(node) for node in self.nodes}
 
         remaining_self_nodes = set(self.nodes)
         remaining_other_nodes = set(other.nodes)
-        used_nodes: List[Node] = [remaining_self_nodes.pop()]
-        corresponding_nodes_possibilities: Dict[Node, Optional[List[Node]]] = {}
-        reversed_mapping: Dict[Node, Node] = {}
+        used_nodes: list[Node] = [remaining_self_nodes.pop()]
+        corresponding_nodes_possibilities: dict[Node, Optional[list[Node]]] = {}
+        reversed_mapping: dict[Node, Node] = {}
         order = self.order
 
         adjacency_test_methods = [(self.successors, other.successors)]
         # If graph is undirected, predecessors are also successors, so no need to test twice.
         if self.is_directed:
             adjacency_test_methods.append((self.predecessors, other.predecessors))
 
@@ -497,75 +513,79 @@
         if not count_undirected_loops_twice and node1 == node2 and not self.is_directed:
             n //= 2
         return n
 
     def weight(self, node1: Node, node2: Node) -> float:
         if node1 == node2:
             return 0
-        elif self.are_adjacents(node1, node2):
+        elif node2 in self.successors(node1):
             return 1
         else:
             return math.inf
 
     @cached_property
     def weight_matrix(self):
         return tuple(tuple(self.weight(node1, node2) for node2 in self.nodes) for node1 in self.nodes)
 
-    def labels(self, node1: Node, node2: Node) -> List[str]:
+    def labels(self, node1: Node, node2: Node) -> list[str]:
         n = self.count_edges(node1, node2, count_undirected_loops_twice=False)
         return n * [""]
 
     def node_degree(self, node: Node) -> int:
         if self.is_directed:
             return self.in_degree(node) + self.out_degree(node)
         return self.out_degree(node)
 
     @property
-    def all_degrees(self) -> Dict[Node, int]:
+    def all_degrees(self) -> dict[Node, int]:
         return {node: self.node_degree(node) for node in self.nodes}
 
     @property
-    def all_in_degrees(self) -> Dict[Node, int]:
+    def all_in_degrees(self) -> dict[Node, int]:
         return {node: self.in_degree(node) for node in self.nodes}
 
     @property
-    def all_out_degrees(self) -> Dict[Node, int]:
+    def all_out_degrees(self) -> dict[Node, int]:
         return {node: self.out_degree(node) for node in self.nodes}
 
     def in_degree(self, node: Node) -> int:
         return sum(self._predecessors[node].values())
 
     def out_degree(self, node: Node) -> int:
         return sum(self._successors[node].values())
 
-    def in_out_degree(self, node: Node) -> Tuple[int, int]:
+    def in_out_degree(self, node: Node) -> tuple[int, int]:
         return self.in_degree(node), self.out_degree(node)
 
     def successors(self, node: Node) -> Set[Node]:
         return set(self._successors[node])
 
     def predecessors(self, node: Node) -> Set[Node]:
         return set(self._predecessors[node])
 
     def copy(self):
         return self.__class__(self.nodes, *self.edges)
 
     @cached_property
-    def adjacency_matrix(self) -> Tuple[Tuple[int, ...], ...]:
+    def adjacency_matrix(self) -> tuple[tuple[int, ...], ...]:
         """Get the adjacency matrix of the graph.
 
         If operations on the matrix are needed, the matrix should be converted to a `numpy` or `sympy` matrix:
 
-            >>> import numpy  # doctest: +SKIP
+            >>> import numpy
             >>> from smallgraphlib import complete_graph
-            >>> M = numpy.matrix(complete_graph(3).adjacency_matrix)
-            >>> M**2
-            matrix([[2, 1, 1],
-                    [1, 2, 1],
-                    [1, 1, 2]])
+            >>> raw_matrix = complete_graph(3).adjacency_matrix
+            >>> raw_matrix * raw_matrix
+            Traceback (most recent call last):
+            TypeError: can't multiply sequence by non-int of type 'tuple'
+            >>> M = numpy.array(raw_matrix)
+            >>> M @ M  # `@` is the operator corresponding to matrix multiplication
+            array([[2, 1, 1],
+                   [1, 2, 1],
+                   [1, 1, 2]])
 
         Return:
             A matrix of integers, as a tuple of tuples.
         """
         return tuple(tuple(self.count_edges(start, end) for end in self.nodes) for start in self.nodes)
 
     @abstractmethod
@@ -583,22 +603,22 @@
         ...
 
     @staticmethod
     @abstractmethod
     def _edge(node1: Node, node2: Node = None) -> Edge:
         ...
 
-    def _dijkstra(self, start: Node, end: Node = None) -> Tuple[Dict[Node, float], Dict[Node, List[Node]]]:
+    def _dijkstra(self, start: Node, end: Node = None) -> tuple[dict[Node, float], dict[Node, list[Node]]]:
         """Implementation of Dijkstra Algorithm."""
         if start not in self.nodes:
             raise ValueError(f"Unknown node {start!r}.")
         if end is not None and end not in self.nodes:
             raise ValueError(f"Unknown node {end!r}.")
-        lengths: Dict[Node, float] = {node: (0 if node == start else math.inf) for node in self.nodes}
-        last_step: Dict[Node, List[Node]] = {node: [] for node in self.nodes}
+        lengths: dict[Node, float] = {node: (0 if node == start else math.inf) for node in self.nodes}
+        last_step: dict[Node, list[Node]] = {node: [] for node in self.nodes}
         never_selected_nodes = set(self.nodes)
         selected_node = start
         while selected_node != end and len(never_selected_nodes) > 1:
             never_selected_nodes.remove(selected_node)
             for successor in self.successors(selected_node) & never_selected_nodes:
                 weight = self.weight(selected_node, successor)
                 if weight < 0:
@@ -615,27 +635,40 @@
     # TODO: put in cache all distances from `start` node when running Dijkstra algorithm.
     #
     def distance(self, start: Node, end: Node) -> float:
         """Implementation of Dijkstra Algorithm."""
         lengths, _ = self._dijkstra(start, end)
         return lengths[end]
 
-    @cached_property
-    def distance_matrix(self):
-        return tuple(tuple(self.distance(node1, node2) for node2 in self.nodes) for node1 in self.nodes)
+    # @cached_property
+    # def distance_matrix(self):
+    #     return tuple(tuple(self.distance(node1, node2) for node2 in self.nodes) for node1 in self.nodes)
+
+    @cached_property
+    def distance_matrix(self) -> tuple[tuple[float, ...], ...]:
+        """Compute the distance matrix, using Roy-Floyd-Warshall algorithm."""
+        matrix = [list(row) for row in self.weight_matrix]
+        n = self.order
+        for k in range(n):
+            for i in range(n):
+                for j in range(n):
+                    # Try to use node k to find a shorter path.
+                    matrix[i][j] = min(matrix[i][j], matrix[i][k] + matrix[k][j])
+        # Making result immutable is much safer for user, since we use caching.
+        return tuple(tuple(row) for row in matrix)
 
     @cached_property
     def diameter(self) -> float:
         return max(self.distance(node1, node2) for node1 in self.nodes for node2 in self.nodes)
 
-    def shortest_paths(self, start: Node, end: Node) -> Tuple[float, List[List[Node]]]:
+    def shortest_paths(self, start: Node, end: Node) -> tuple[float, list[list[Node]]]:
         """Implementation of Dijkstra Algorithm."""
         lengths, last_step = self._dijkstra(start, end)
 
-        def generate_paths(path: List[Node]) -> List[List[Node]]:
+        def generate_paths(path: list[Node]) -> list[list[Node]]:
             if path[0] == start:
                 return [path]
             paths = []
             for predecessor in last_step[path[0]]:
                 paths.extend(generate_paths([predecessor] + path))
             return paths
 
@@ -646,16 +679,16 @@
         start: Node = None,
         *,
         error_if_already_visited=False,
     ) -> Iterator[Node]:
         """Return a node iterator, using a prefix DFS."""
         if start is None:
             start = self.nodes[0]
-        stack: List[Node] = [start]
-        previous_nodes: List[Optional[Node]] = [None]
+        stack: list[Node] = [start]
+        previous_nodes: list[Optional[Node]] = [None]
         # If the graph isn't a rooted tree, there is no notion of parent.
         # If we want to use DFS to test if the graph is a tree, we must try to visit all adjacents nodes
         # except the one we come from, and see if there were already visited.
         # So we must keep track of the node we come from for each node of the stack.
         visited: Set[Node] = set()
         while stack:
             node = stack.pop()
@@ -696,15 +729,15 @@
                 for successor in self._successors[node]:
                     yield from postorder_dfs(successor)
                 yield node
 
         def inorder_dfs(node: Node) -> Iterator[Node]:
             visited.add(node)
             # Eliminate visited nodes from the list of successors *before* splitting it.
-            successors: List[Node] = [
+            successors: list[Node] = [
                 successor for successor in self._successors[node] if successor not in visited
             ]
             for successor in successors[:1]:
                 yield from inorder_dfs(successor)
             yield node
             for successor in successors[1:]:
                 yield from inorder_dfs(successor)
@@ -743,21 +776,65 @@
         visited: Set[Node] = set()
         while queue:
             node = queue.popleft()
             visited.add(node)
             yield node
             queue.extend(successor for successor in self._successors[node] if successor not in visited)
 
-    def _tikz_specific_node_style(self, node: Node) -> str:
-        """Overwrite this method to add a specific tikz style to some nodes."""
-        return ""
-
-    def _tikz_labels(self, node1: Node, node2: Node) -> list[str]:
-        """Overwrite this method to modify tikz value for some labels."""
-        return self.labels(node1, node2)
+    def find_path(
+        self,
+        start: Node,
+        end: Node,
+        _filter_edges: Callable[[Self, Node, Node], bool] = (lambda _, __, ___: True),
+        _filter_nodes: Callable[[Self, Node], bool] | Iterable[Node] = (),
+    ) -> list[Node]:
+        """Return a path between nodes `start` and `end`, if any, or an empty list.
+
+        If defined, `_filter_edges` is a boolean function, which takes three arguments: the calling class,
+        the current node and its successor.
+        If `_filter(self, node1, node2)` returns `False`, the edge (node1, node2), if it exists, will be ignored.
+        """
+        previous: dict[Node, Node] = {}
+        queue: deque[Node] = deque([start])
+        if callable(_filter_nodes):
+            _filter_nodes = set(node for node in self.nodes if _filter_nodes(self, node))
+        else:
+            _filter_nodes = set(_filter_nodes)
+        while end not in previous and len(queue) > 0:
+            # BFS
+            node = queue.popleft()
+            for successor in self.successors(node):
+                if _filter_edges(self, node, successor) and node not in _filter_nodes:
+                    # If successor was never seen before, append it to queue.
+                    if successor not in previous:
+                        previous[successor] = node
+                        queue.append(successor)
+        if end in previous:
+            path = [end]
+            while path[-1] != start:
+                path.append(previous[path[-1]])
+            return list(reversed(path))
+        return []
+
+    # ------------------
+    #    Tikz support
+    # ==================
+
+    # def _tikz_specific_node_style(self, node: Node) -> str:
+    #     """Overwrite this method to add a specific tikz style to some nodes."""
+    #     return ""
+    #
+    # def _tikz_labels(self, node1: Node, node2: Node) -> list[str]:
+    #     """Overwrite this method to modify tikz value for some labels."""
+    #     return self.labels(node1, node2)
+    #
+    # def _tikz_angles(self, node: Node) -> dict[Node, float]:
+    #     """Overwrite this method to modify tikz automatic nodes' placement."""
+    #     theta = 360 / self.order
+    #     return {node: i * theta for i, node in enumerate(self.nodes)}
 
     def as_tikz(self, *, shuffle_nodes=False, border: str = None, options="") -> str:
         r"""Generate tikz code corresponding to this graph.
 
         `Tikz` package must be loaded in the latex preamble, with `arrows.meta` library::
 
             \usepackage{tikz}
@@ -767,12 +844,12 @@
 
             \usepackage[outline]{contour}
             \contourlength{0.5pt}
 
         If set, `border` have to be a combination of tikz path drawing styles,
         like "dotted", or "dashed,blue".
         """
-        return tikz_printer.tikz_code(self, shuffle_nodes=shuffle_nodes, border=border, options=options)
+        return self.printer(self, shuffle_nodes=shuffle_nodes).tikz_code(border=border, options=options)
 
 
 class InvalidGraphAttribute(AttributeError):
     """This error is raised when a method or property can't return a value for a particular graph."""
```

### Comparing `smallgraphlib-0.8.1/smallgraphlib/custom_types.py` & `smallgraphlib-0.9.0/smallgraphlib/custom_types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from typing import TypeVar, Tuple, FrozenSet, Union, Set, Iterable, Any, Dict, List, TYPE_CHECKING
+from typing import TypeVar, FrozenSet, Union, Set, Iterable, Any, TYPE_CHECKING
 
 from smallgraphlib.utilities import ComparableAndHashable
 
 if TYPE_CHECKING:
     from smallgraphlib.core import AbstractGraph
 
 _AbstractGraph = TypeVar("_AbstractGraph", bound="AbstractGraph")
 Node = TypeVar("Node", bound=ComparableAndHashable)
 # Node = TypeVar("Node", bound=typing.Hashable)  # too subtile for Pycharm ? ;-(
-DirectedEdge = Tuple[Node, Node]
+DirectedEdge = tuple[Node, Node]
 UndirectedEdge = FrozenSet[Node]
 Edge = Union[DirectedEdge, UndirectedEdge]
 EdgeLike = Union[Edge, Set[Node], Iterable[Node]]
-Label = Any
-InternalGraphRepresentation = Dict[Node, Dict[Node, Union[int, List[Label]]]]
-Point = Tuple[float, float]
-Segment = Tuple[Point, Point]
+Label_ = Any
+InternalGraphRepresentation = dict[Node, dict[Node, Union[int, list[Label_]]]]
+Point = tuple[float, float]
+Segment = tuple[Point, Point]
+Label = TypeVar("Label")
+LabeledEdge = tuple[Node, Node, Label]
+WeightedEdge = tuple[Node, Node, float]
```

### Comparing `smallgraphlib-0.8.1/smallgraphlib/graphs_constructors.py` & `smallgraphlib-0.9.0/smallgraphlib/graphs_constructors.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import random
-from typing import List, Tuple, Iterable
+from typing import Iterable
 
 
 from smallgraphlib.custom_types import Node, Edge
 from smallgraphlib.core import AbstractGraph
 from smallgraphlib.basic_graphs import Graph, DirectedGraph
 from smallgraphlib.labeled_graphs import (
     LabeledDirectedGraph,
@@ -15,17 +15,22 @@
 from smallgraphlib.tikz_export import _TIKZ_EXPORT_MAX_MULTIPLE_EDGES_SUPPORT
 
 
 def graph(nodes=None, *edges, directed=False, **labeled_edges):
     """Factory function to create graphs with various syntaxes.
 
     >>> graph("A:B,C B:C C")
+    Graph(('A', 'B', 'C'), {'A', 'B'}, {'A', 'C'}, {'B', 'C'})
     >>> graph(AB=5, BC=7, AC=8, directed=True)
-    >>> graph("A:B=5,C=8 B:C=inf", directed=True)
-    >>> graph("A:B='some text with space',C=text_without_space B:C=2.5 D")
+    WeightedDirectedGraph(('A', 'B', 'C'), ('A', 'B', 5), ('A', 'C', 8), ('B', 'C', 7))
+    >>> graph("A:B=5,C=8 B:C=inf C", directed=True)
+    WeightedDirectedGraph(('A', 'B', 'C'), ('A', 'B', 5), ('A', 'C', 8), ('B', 'C', inf))
+    >>> graph("A:B='some text with space',C=text_without_space B:C=2.5 C D")
+    LabeledGraph(('A', 'B', 'C', 'D'), ('A', 'B', 'some text with space'),
+                 ('A', 'C', 'text_without_space'), ('B', 'C', 2.5))
 
     This is intended mainly for quick interactive use (or one-time-use scripts),
     since its interface is not very clean and may change frequently.
 
     You should use the constructors provided by the various graph classes
     if you need a stable API.
     """
@@ -68,16 +73,16 @@
 
 
 def perfect_binary_tree(height: int):
     """Return a perfect binary tree of given height.
 
     In a perfect binary tree, each node has two children, except in last level.
     """
-    nodes: List[int] = []
-    edges: List[Edge] = []
+    nodes: list[int] = []
+    edges: list[Edge] = []
     for level in range(height):
         nodes.extend(range(1 << level, 1 << level + 1))
     for level in range(height - 1):
         for i in range(1 << level, 1 << level + 1):
             edges.append((i, i << 1))
             edges.append((i, (i << 1) + 1))
 
@@ -142,16 +147,16 @@
             max_multiple_loops = degree
 
     max_degree = order * max_multiple_loops + (order * (order - 1) * max_multiple_edges) // 2
 
     if degree > max_degree:
         raise ValueError(f"Degree must not exceed {max_degree} with given contraints.")
 
-    nodes: List[int] = list(range(1, order + 1))
-    edges: List[Tuple[int, int]] = []
+    nodes: list[int] = list(range(1, order + 1))
+    edges: list[tuple[int, int]] = []
 
     # fmt: off
     # Keep track of remaining edges possibilities, for each (start, end) nodes couple.
     # Only nodes which accept edges will be kept (all except the last one
     # for undirected simple graph, since start < end).
     counters = {
         start: counter
```

### Comparing `smallgraphlib-0.8.1/smallgraphlib/huffman.py` & `smallgraphlib-0.9.0/smallgraphlib/huffman.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,37 @@
 from collections import Counter
 from operator import attrgetter
+from typing import Generic
 
 from smallgraphlib.custom_types import Node
 
 
-class Tree:
+class Tree(Generic[Node]):
+    """A tree defined as a recursive structure."""
+
     def __init__(self, root: Node, *branches: "Tree") -> None:
         self.root = root
         self.branches: tuple["Tree", ...] = branches
 
 
-class HuffmanTree(Tree):
+class HuffmanTree(Tree[tuple[int, str]]):
     def __init__(self, *branches: "HuffmanTree", char: str = None, weight: int = None) -> None:
-        self.branches: tuple["HuffmanTree", ...]
+        self.branches: tuple["HuffmanTree", ...] = branches  # Just for Pycharm to handle correctly the type!
         if len(branches) == 2:
             if char is not None or weight is not None:
                 raise ValueError("Char and weight can't be set, except for leaves.")
         elif len(branches) == 0:
             if char is None or weight is None:
                 raise ValueError("Char and weight must be set for leaves.")
         else:
             raise ValueError(f"There must be either 0 or 2 branches, not {len(branches)}.")
         char = min(branch.char for branch in branches) if branches else char
         weight = sum(branch.weight for branch in branches) if branches else weight
+        assert char is not None
+        assert weight is not None
         super().__init__((weight, char), *branches)
 
     @classmethod
     def from_text(cls, text: str) -> "HuffmanTree":
         trees = {
             HuffmanTree(char=letter, weight=occurrences) for letter, occurrences in Counter(text).items()
         }
@@ -38,19 +43,19 @@
             tree2 = min(trees, key=sort_func)
             trees.remove(tree2)
             trees.add(HuffmanTree(tree1, tree2))
         assert len(trees) == 1
         return trees.pop()
 
     @property
-    def weight(self):
+    def weight(self) -> int:
         return self.root[0]
 
     @property
-    def char(self):
+    def char(self) -> str:
         return self.root[1]
 
     @property
     def is_leaf(self) -> bool:
         return len(self.branches) == 0
 
     @property
@@ -115,33 +120,51 @@
             return {self.char: ""}
         return {
             key: str(i) + value
             for i, branch in enumerate(self.branches)
             for key, value in branch.labels.items()
         }
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         if self.is_leaf:
-            return f"HuffmanTree(char={self.char}, weight={self.weight})"
+            return f"HuffmanTree(char={self.char!r}, weight={self.weight})"
         return f"HuffmanTree({self.left_branch!r}, {self.right_branch!r})"
 
-    def __str__(self):
+    def __str__(self) -> str:
         lines = []
+        if self.is_leaf:
+            return f"({self.char})"
         shift = len(str(self.weight)) + 1
         for n, line in enumerate(str(self.left_branch).split("\n")):
             if n == 0:
                 # lines.append("\u252C\u2500\u2500" + line)
                 lines.append(f"{self.weight}\u2500\u2500" + line)
             else:
                 lines.append("\u2502" + shift * " " + line)
         for n, line in enumerate(str(self.right_branch).split("\n")):
             if n == 0:
                 lines.append("\u2514" + shift * "\u2500" + line)
             else:
                 lines.append((shift + 1) * " " + line)
         return "\n".join(lines)
 
+    def as_dict(self):
+        if self.is_leaf:
+            return {self.root: []}
+        else:
+            return (
+                {self.root: [branch.root for branch in self.branches]}
+                | self.left_branch.as_dict()
+                | self.right_branch.as_dict()
+            )
+
+    # def __eq__(self, other):
+    #     return isinstance(other, HuffmanTree) and (
+    #         (self.is_leaf and other.is_leaf and self.root == other.root)
+    #         or (other.left_branch == self.left_branch and other.right_branch == self.right_branch)
+    #     )
+
 
 def encode(text: str) -> str:
     """Return a string of `0` and `1` representing the bits of a text encoded using Huffman algorithm."""
     tree = HuffmanTree.from_text(text)
     return tree.encode(text)
```

### Comparing `smallgraphlib-0.8.1/smallgraphlib/labeled_graphs.py` & `smallgraphlib-0.9.0/smallgraphlib/labeled_graphs.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import ast
 import math
 import re
 from abc import ABC, abstractmethod
 from itertools import chain
 from math import inf
 from numbers import Real
-from typing import Iterable, Tuple, Dict, List, TypeVar, Generic, Any, Sequence, Type
+from typing import Iterable, TypeVar, Generic, Any, Sequence, Type
 
 from smallgraphlib.basic_graphs import Graph, DirectedGraph
 from smallgraphlib.core import AbstractGraph, InvalidGraphAttribute
-from smallgraphlib.custom_types import Node, Edge
+from smallgraphlib.custom_types import Node, Edge, Label, LabeledEdge, WeightedEdge
+from smallgraphlib.tikz_export import TikzLabeledGraphPrinter
 from smallgraphlib.utilities import cached_property
 
 _AbstractLabeledGraph = TypeVar("_AbstractLabeledGraph", bound="AbstractLabeledGraph")
 _AbstractWeightedGraph = TypeVar("_AbstractWeightedGraph", bound="AbstractWeightedGraph")
-Label = TypeVar("Label")
-LabeledEdge = Tuple[Node, Node, Label]
-WeightedEdge = Tuple[Node, Node, float]
 
 
-class AbstractLabeledGraph(AbstractGraph, ABC, Generic[Label]):
+class AbstractLabeledGraph(AbstractGraph, ABC, Generic[Node, Label]):
     """Abstract class for all labeled graphs, don't use it directly."""
 
+    printer = TikzLabeledGraphPrinter
+
     def __init__(
         self,
         nodes: Iterable[Node],
         *labeled_edges: LabeledEdge,
         sort_nodes: bool = True,
     ):
-        edges: List[Edge] = []
-        self._labels: Dict[Edge, List[Label]] = {}
+        edges: list[Edge] = []
+        self._labels: dict[Edge, list[Label]] = {}
         for *edge, label in labeled_edges:
             edges.append(edge)  # type: ignore
             self._labels.setdefault(self._edge(*edge), []).append(label)
 
         super().__init__(nodes, *edges, sort_nodes=sort_nodes)
 
     def __eq__(self, other: Any):
@@ -41,66 +41,84 @@
             sorted(self.labels(*edge)) == sorted(other.labels(*edge)) for edge in self.edges
         )
 
     def __repr__(self):
         labeled_edges = (repr(labeled_edge) for labeled_edge in self.labeled_edges)
         return f"{self.__class__.__name__}({tuple(self.nodes)!r}, {', '.join(labeled_edges)})"
 
+    def copy(self):
+        return self.__class__(self.nodes, *self.labeled_edges)
+
     @cached_property
     def labeled_edges(self) -> tuple[LabeledEdge, ...]:
         # noinspection PyTypeChecker
         return tuple(
             sorted(
                 (
-                    *edge,
+                    *(
+                        sorted(edge) if isinstance(edge, (set, frozenset)) else edge
+                    ),  # Sorting nodes will help in making doctests deterministic.
                     label,
                 )
                 for edge, labels in self._labels.items()
                 for label in labels
             )
         )
 
+    def as_dict(self) -> dict[tuple[Node, Node], Label]:
+        return {(node1, node2): label for node1, node2, label in self.labeled_edges}
+
     @classmethod
     def from_dict(
-        cls: Type[_AbstractLabeledGraph], edge_label_dict: dict = None, /, **edge_label
+        cls: Type[_AbstractLabeledGraph],
+        edge_label_dict: dict[str | tuple[Node, Node], Label] = None,  # type: ignore
+        /,
+        **edge_label: Label,  # type: ignore
     ) -> _AbstractLabeledGraph:
         """Construct a directed graph using a {edge_name: label} dictionnary (or keywords).
 
-        All edges' names must be two letters strings (like "AB"), each letter representing a node.
+        All edges' names must be either:
+            - two letters strings (like "AB"), each letter representing a node,
+            - or a couple of nodes (like ("A", "B") or (1, 2)).
         Nodes' names are automatically deduced from edges' names.
 
         >>> g1 = LabeledGraph.from_dict(AB=1, AC=3, BC=4)
         >>> g2 = LabeledGraph.from_dict({"AB": 1, "AC": 3, "BC": 4})
-        >>> g1 == g2
+        >>> g3 = LabeledGraph.from_dict({("A", "B"): 1, ("A", "C"): 3, ("B", "C"): 4})
+        >>> g1 == g2 == g3
         True
         >>> g1.nodes
         ('A', 'B', 'C')
         """
         if edge_label_dict is None:
             edge_label_dict = {}
-        edge_label_dict.update(edge_label)
+        edge_label_dict.update(edge_label)  # type: ignore
         nodes = set(chain(*(edge for edge in edge_label_dict)))
         return cls(nodes, *((*edge, label) for edge, label in edge_label_dict.items()))
 
     @classmethod
     def from_string(cls: Type[_AbstractLabeledGraph], string: str) -> _AbstractLabeledGraph:
         """LabeledGraph.from_string("A:B=label,C='other label' B:C=5 C D:C")
         will generate a graph of 4 nodes, A, B, C and D, with edges A->B, A->C, B->C and C->D
         and respective labels 'label', 'other label', 5 and `None`.
 
+        >>> LabeledGraph.from_string("A:B=label,C='other label' B:C=5 C D:C")
+        LabeledGraph(('A', 'B', 'C', 'D'), ('A', 'B', 'label'), ('A', 'C', 'other label'),
+                     ('B', 'C', 5), ('C', 'D', None))
+
         Note that labels containing a space must be surrounded by single or double quotes.
         Labels containing only digits will be converted to numbers (integers or floats),
         except if surrounded by quotes.
 
         If no label is given, `None` is stored by default.
         """
         # Convert spaces inside labels to null characters, to make splitting easier.
         string = re.sub("""'[^']*'|"[^"]*""", (lambda m: m.group().replace(" ", "\x00")), string)
-        nodes: List[str] = []
-        edges: List[Tuple[str, str, Any]] = []
+        nodes: list[str] = []
+        edges: list[tuple[str, str, Any]] = []
         label: Any
         for substring in string.split():
             node, *remaining = substring.split(":", 1)
             nodes.append(node.strip())
             if remaining:
                 for successor_and_label in remaining[0].split(","):
                     successor, *after_successor = successor_and_label.split("=", 1)
@@ -113,22 +131,22 @@
                             if label == "inf":
                                 label = math.inf
                             elif label == "-inf":
                                 label = -math.inf
                     else:
                         label = None
                     edges.append((node, successor.strip(), label))
-        return cls(nodes, *edges)  # type: ignore
+        return cls(nodes, *edges)
 
-    def labels(self, node1: Node, node2: Node) -> List[str]:
+    def labels(self, node1: Node, node2: Node) -> list[str]:
         labels = self._labels.get(self._edge(node1, node2), [])
         assert len(labels) == self.count_edges(node1, node2, count_undirected_loops_twice=False)
         return [str(label if label is not None else "") for label in labels]
 
-    def rename_nodes(self, node_names: Dict[Node, Node]) -> None:
+    def rename_nodes(self, node_names: dict[Node, Node]) -> None:
         super().rename_nodes(node_names)
         # Rename nodes in self._labels dict.
         old_labels = self._labels.copy()
         self._labels.clear()
         for edge, label in old_labels.items():
             new_edge = self._edge(*(node_names[node] for node in edge))
             self._labels[new_edge] = label
@@ -143,18 +161,18 @@
 
 
 class LabeledGraph(AbstractLabeledGraph, Graph):
     """A labeled undirected graph."""
 
 
 class LabeledDirectedGraph(AbstractLabeledGraph, DirectedGraph):
-    pass
+    """A labeled directed graph."""
 
 
-class AbstractWeightedGraph(AbstractLabeledGraph, ABC):
+class AbstractWeightedGraph(AbstractLabeledGraph, ABC, Generic[Node, Label]):
     """Abstract class for all weighted graphs, don't use it directly."""
 
     def __init__(
         self,
         nodes: Iterable[Node],
         *weighted_edges: WeightedEdge,
         sort_nodes: bool = True,
@@ -174,15 +192,15 @@
             else:
                 # We must support sympy.oo, but isinstance(sympy.oo, Real) return False.
                 return float(value) == math.inf and value != "inf"  # do not accept string "inf" !
         except (TypeError, ValueError):
             return False
 
     @property
-    def weights(self) -> Dict[Edge, List[float]]:
+    def weights(self) -> dict[Edge, list[float]]:
         return self._labels
 
     def weight(self, node1: Node, node2: Node, *, aggregator=min, default: float = inf) -> float:
         """
         Return the weight of the edge joining node1 and node2.
 
         Args:
@@ -195,41 +213,24 @@
             float
         """
         if node1 == node2:
             return 0
         values = self.weights.get(self._edge(node1, node2), [default])
         return aggregator(values)
 
-    def _tikz_labels(self, node1: Node, node2: Node) -> list[str]:
-        """Overwrite this method to modify tikz value for some labels."""
-        labels = self._labels.get(self._edge(node1, node2), [])
-
-        def format_(label):
-            # Note: math.isinf() supports `sympy.oo` too.
-            if label is None:
-                return ""
-            elif math.isinf(label) and label > 0:
-                return r"$\infty$"
-            elif math.isinf(label) and label < 0:
-                return r"$-\infty$"
-            else:
-                return str(label)
-
-        return [format_(label) for label in labels]
-
     @cached_property
     def total_weight(self) -> float:
         """Return the sum of all edges weights."""
         return sum(sum(values) for values in self.weights.values())
 
     @staticmethod
     @abstractmethod
     def _get_edges_from_weights_matrix(
         matrix: Sequence[Sequence[float]],
-    ) -> List[Tuple[int, int, float]]:
+    ) -> list[tuple[int, int, float]]:
         ...
 
     @classmethod
     def from_matrix(
         cls: Type[_AbstractWeightedGraph],
         matrix: Iterable[Iterable[float]],
         nodes_names: Iterable[Node] = None,
@@ -246,27 +247,35 @@
         for line in M:
             for val in line:
                 if not cls._is_weight(val):
                     raise ValueError(f"All matrix values must be positive real numbers, but {val!r} is not.")
 
         edges = cls._get_edges_from_weights_matrix(M)
 
-        g = cls(range(1, n + 1), *edges)  # type: ignore
+        g = cls(range(1, n + 1), *edges)
         if nodes_names:
-            g.rename_nodes(dict(enumerate(list(nodes_names)[: len(g.nodes)], start=1)))  # type: ignore
+            g.rename_nodes(dict(enumerate(list(nodes_names)[: len(g.nodes)], start=1)))
         return g
 
+    def get_path_capacity(self, path: list[Node]):
+        """Return the capacity of the path, which is the smallest weight of any of its edges."""
+        return min(self.weight(node1, node2) for node1, node2 in zip(path[:-1], path[1:]))
+
+    def get_path_weight(self, path: list[Node]):
+        """Return the weight of the path, which is the sum of those of its edges."""
+        return sum(self.weight(node1, node2) for node1, node2 in zip(path[:-1], path[1:]))
+
 
-class WeightedGraph(AbstractWeightedGraph, LabeledGraph):
+class WeightedGraph(AbstractWeightedGraph, LabeledGraph, Generic[Node]):
     """A weighted undirected graph, i.e. an undirected graph where all edges have a positive weight."""
 
     @staticmethod
     def _get_edges_from_weights_matrix(
         matrix: Sequence[Sequence[float]],
-    ) -> List[Tuple[int, int, float]]:
+    ) -> list[tuple[int, int, float]]:
         edges = []
         for i in range(len(matrix)):
             for j in range(i + 1):  # we must only deal with i <= j, since it is an undirected graph.
                 weight = matrix[i][j]
                 if i == j:
                     if weight != 0:
                         raise ValueError(
@@ -290,21 +299,21 @@
 
         A spanning tree of a graph G is a subgraph of G who is a tree and contains all the nodes of G.
 
         If the graph is not connected, raise an `InvalidGraphAttribute`.
         """
         # Nodes and edges of the spanning tree.
         last_connected_node = self.nodes[0]
-        connected_nodes: List[Node] = [last_connected_node]  # type: ignore
-        weighted_edges: List[WeightedEdge] = []
+        connected_nodes: list[Node] = [last_connected_node]
+        weighted_edges: list[WeightedEdge] = []
 
         # Nodes which may be connected, with the current cost of connection, i.e. the minimal edge's weight
         # enabling to connect it to the spanning tree.
-        cheapest_cost: Dict[Node, float] = {}  # type: ignore
-        cheapest_edge: Dict[Node, Node] = {}  # type: ignore
+        cheapest_cost: dict[Node, float] = {}
+        cheapest_edge: dict[Node, Node] = {}
         unreached_nodes = set(self.nodes) - set(connected_nodes)
 
         while True:
             # Update frontier
             for successor in self.successors(last_connected_node):
                 if successor not in connected_nodes:
                     cost = self.weight(last_connected_node, successor)
@@ -332,21 +341,21 @@
 
         if unreached_nodes:
             raise InvalidGraphAttribute("This graph has no spanning tree since it is not connected.")
 
         return WeightedGraph(connected_nodes, *weighted_edges)
 
 
-class WeightedDirectedGraph(AbstractWeightedGraph, LabeledDirectedGraph):
+class WeightedDirectedGraph(AbstractWeightedGraph, LabeledDirectedGraph, Generic[Node]):
     """A directed graph with weights (i.e. positive floats) associated to its edges."""
 
     @staticmethod
     def _get_edges_from_weights_matrix(
         matrix: Sequence[Sequence[float]],
-    ) -> List[Tuple[int, int, float]]:
+    ) -> list[tuple[int, int, float]]:
         edges = []
         for i in range(len(matrix)):
             for j in range(len(matrix)):
                 weight = matrix[i][j]
                 if i == j:
                     if weight != 0:
                         raise ValueError(
```

### Comparing `smallgraphlib-0.8.1/smallgraphlib/latex_export.py` & `smallgraphlib-0.9.0/smallgraphlib/latex_export.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,38 @@
 import math
 from typing import Iterable
 
+from smallgraphlib.basic_graphs import Graph
+
 from smallgraphlib.core import AbstractGraph
 from smallgraphlib.custom_types import Node
 
+COLORS = [
+    "red",
+    "blue",
+    "green",
+    "orange",
+    "magenta",
+    "cyan",
+    "violet",
+    "brown",
+    "pink",
+    "yellow",
+    "purple",
+    "gray",
+    "black",
+    "silver",
+    "sienna",
+    "white",
+    "maroon",
+    "beige",
+    "salmon",
+    "olive",
+]
+
 
 def latex_Dijkstra(graph: AbstractGraph[Node], start: Node, end: Node = None) -> str:
     """Generate the LaTeX code of a table corresponding to Dijkstra algorithm's steps.
 
     If `end` is `None`, only stop when the shorter path to all other nodes have been found.
     """
     nodes = graph.nodes
@@ -102,7 +127,31 @@
             lines.append(
                 f"Shorter(s) path(s) from ${start}$ to ${target}$: "
                 f"${shortest_paths()}$ (length: {distance})."
             )
             lines.append("")
 
     return "\n" + "\n".join(lines)
+
+
+def latex_WelshPowell(graph: Graph[Node]) -> str:
+    """Generate the LaTeX code of a table ordering nodes by degrees and attributing each a color."""
+    nodes: list[str] = []
+    degrees: list[str] = []
+    colors: list[str] = []
+    for node, color_num in graph.greedy_coloring.items():
+        nodes.append(node)
+        degrees.append(str(graph.all_degrees[node]))
+        colors.append(COLORS[color_num] if color_num < len(COLORS) else str(color_num))
+    return "\n".join(
+        [
+            r"\begin{tabular}{|l|*{" + str(graph.order) + "}{c|}}",
+            r"\hline",
+            r"\cellcolor{blue!10} nodes & " + " & ".join(nodes) + r"\\",
+            r"\hline",
+            r"\cellcolor{blue!10} degrees & " + " & ".join(degrees) + r"\\",
+            r"\hline",
+            r"\cellcolor{blue!10} colors & " + " & ".join(colors) + r"\\",
+            r"\hline",
+            r"\end{tabular}",
+        ]
+    )
```

### Comparing `smallgraphlib-0.8.1/smallgraphlib/string2automaton.py` & `smallgraphlib-0.9.0/smallgraphlib/string2automaton.py`

 * *Files identical despite different names*

### Comparing `smallgraphlib-0.8.1/smallgraphlib/tikz_export.py` & `smallgraphlib-0.9.0/smallgraphlib/tikz_export.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,49 @@
 import math
 import random
-from typing import Generic, TYPE_CHECKING
+from typing import Generic, TYPE_CHECKING, Final
 
-from smallgraphlib.utilities import frange
+from smallgraphlib.utilities import frange, cached_property, clear_cache
 
-from smallgraphlib.custom_types import Node, Segment, Point
+from smallgraphlib.custom_types import Node, Segment, Point, Label
 
 if TYPE_CHECKING:
     from smallgraphlib.core import AbstractGraph
-
+    from smallgraphlib.labeled_graphs import AbstractLabeledGraph
+    from smallgraphlib.automatons import Automaton, Transducer, Char, Acceptor
+    from smallgraphlib.flow import FlowNetwork
 
 _TIKZ_EXPORT_MAX_MULTIPLE_EDGES_SUPPORT = 3
 
+GREEK_LETTERS: Final[tuple[str, ...]] = (
+    "alpha",
+    "beta",
+    "gamma",
+    "delta",
+    "epsilon",
+    "zeta",
+    "eta",
+    "theta",
+    "iota",
+    "kappa",
+    "lambda",
+    "mu",
+    "nu",
+    "xi",
+    "pi",
+    "rho",
+    "sigma",
+    "tau",
+    "upsilon",
+    "phi",
+    "chi",
+    "psi",
+    "omega",
+)
+
 
 def segments_intersection(segment1: Segment, segment2: Segment, eps: float = 10**-8) -> Point | None:
     (xA, yA), (xB, yB) = segment1
     (xC, yC), (xD, yD) = segment2
     # solve: s*A + (1 - s)*B = t*C + (1 - t)*D  <==>  s*(A - B) + t*(D - C) = D - B
     #                                           <==>  s*xBA + t*xCD = xBD  and  s*yBA + t*yCD = yBD
     xCD, yCD = xD - xC, yD - yC
@@ -185,41 +213,64 @@
 class TikzPrinter(Generic[Node]):
     lines: list[str]
     # `nodes_positions` stores the cartesian coordinates of each of the graph's node.
     nodes_positions: dict[Node, Point]
     # The places already occupied by labels are stored in `labels_positions`, to avoid placing another
     # label there.
     labels_positions: list[Point]
-    graph: "AbstractGraph[Node]"
-    angles: dict[Node, float]
     # Nodes numeration (useful in particular when they are shuffled):
     index: dict[Node, int]
-    nodes: list[Node]
     # For debugging:
     _cartography: dict[tuple[Node, ...], Point]
 
+    def __init__(self, graph: "AbstractGraph[Node]", shuffle_nodes=False):
+        self.graph: "AbstractGraph[Node]" = graph
+        self._reset()
+        self.shuffle_nodes: bool = shuffle_nodes
+
+    @clear_cache
     def _reset(self):
         self.lines = []
         self.nodes_positions = {}
         self.labels_positions = []
         self._cartography = {}
-        self.angles = {}
         self.index = {}
 
     @staticmethod
     def latex_preamble_additions() -> list[str]:
         """Return the lines of LaTeX code to insert in the LaTeX preamble."""
         return [
             r"\usepackage{tikz}",
             r"\usetikzlibrary{arrows.meta}",
             r"\usepackage[outline]{contour}",
             r"\contourlength{0.15em}",
         ]
 
-    def tikz_code(self, graph, *, shuffle_nodes=False, border: str = None, options="") -> str:
+    @cached_property
+    def angles(self) -> dict[Node, float]:
+        """Overwrite this method to modify tikz automatic nodes' placement."""
+        theta = 360 / self.graph.order
+        return {node: i * theta for i, node in enumerate(self.nodes)}
+
+    @cached_property
+    def nodes(self) -> tuple[Node, ...]:
+        nodes = list(self.graph.nodes)
+        if self.shuffle_nodes:
+            random.shuffle(nodes)
+        return tuple(nodes)
+
+    def specific_node_style(self, node: Node) -> str:
+        """Overwrite this method to add a specific tikz style to some nodes."""
+        return ""
+
+    def labels(self, node1: Node, node2: Node) -> list[str]:
+        """Overwrite this method to modify tikz value for some labels."""
+        return self.graph.labels(node1, node2)
+
+    def tikz_code(self, *, border: str = None, options="") -> str:
         r"""Generate tikz code corresponding to this graph.
 
         `Tikz` package must be loaded in the latex preamble, with `arrows.meta` library::
 
             \usepackage{tikz}
             \usetikzlibrary{arrows.meta}
 
@@ -231,40 +282,37 @@
         If set, `border` have to be a combination of tikz path drawing styles,
         like "dotted", or "dashed,blue".
         """
         if border:
             return "".join(
                 [
                     rf"\begin{{tikzpicture}}\node[rounded corners,draw,inner sep=2pt,{border}]{{",
-                    self.tikz_code(graph, shuffle_nodes=shuffle_nodes, options=options),
+                    self.tikz_code(options=options),
                     r"};\end{tikzpicture}",
                 ]
             )
-        self.graph = graph
         self._reset()
         self.lines = [
             r"\providecommand{\contour}[2]{#2}"  # avoid an error if package contour is not loaded.
             r"\begin{tikzpicture}[solid,black,"
             r"every node/.style = {font={\scriptsize}},"
             r"vertex/.style = {draw, circle,font={\scriptsize},inner sep=2},"
             "directed/.style = {-{Stealth[scale=1.1]}},"
             "reversed/.style = {{Stealth[scale=1.1]}-},"
             "undirected/.style = {},"
             f"{options}"
             "]"
         ]
-        theta = 360 / self.graph.order
-        nodes = self.nodes = list(self.graph.nodes)
-        if shuffle_nodes:
-            random.shuffle(nodes)
+        # theta = 360 / self.graph.order
+        nodes = self.nodes  # = list(self.graph.nodes)
         self.index = {node: i for i, node in enumerate(nodes)}
         # All nodes are placed around a circle, creating a regular polygon.
         for i, node in enumerate(nodes):
-            angle = self.angles[node] = i * theta
-            specific_style = self.graph._tikz_specific_node_style(node)
+            angle = self.angles[node]
+            specific_style = self.specific_node_style(node)
             self.lines.append(rf"\node[vertex,{specific_style}] ({node}) at ({angle}:1cm) {{${node}$}};")
 
         for node in nodes:
             alpha = math.radians(self.angles[node])
             self.nodes_positions[node] = math.cos(alpha), math.sin(alpha)
 
         # Detect edges' intersections, to avoid positioning labels there.
@@ -311,16 +359,15 @@
                     self._generate_edge(node1, node2)
 
         self.lines.append(r"\end{tikzpicture}")
         return "\n".join(self.lines)
 
     def _generate_loop(self, node: Node) -> None:
         style = "directed" if self.graph.is_directed else "undirected"
-        # n: int = self._tikz_count_edges(node, node)
-        for i, label in enumerate(self.graph._tikz_labels(node, node), start=1):
+        for i, label in enumerate(self.labels(node, node), start=1):
             self.lines.append(
                 rf"\draw[{style}] ({node}) to "
                 f"[out={self.angles[node] - 45},in={self.angles[node] + 45},looseness={1 + i * 4}] "
                 rf"node[midway] {{\contour{{white}}{{{label}}}}} "
                 f"({node});"
             )
 
@@ -334,15 +381,15 @@
         node2_is_left_neighbour = (self.index[node1] - self.index[node2] + 1) % len(self.nodes) == 0
 
         if self.graph.is_directed:
             data = [("directed", node1, node2), ("reversed", node2, node1)]
         else:
             data = [("undirected", node1, node2)]
         for direction, nodeA, nodeB in data:
-            _labels = self.graph._tikz_labels(nodeA, nodeB)
+            _labels = self.labels(nodeA, nodeB)
             labels.extend(_labels)
             styles += len(_labels) * [direction]
         n = len(styles)
         if n == 0:
             bendings = []
         elif n == 1:
             bendings = [0]  # strait line by default
@@ -375,8 +422,134 @@
                 self._cartography[(node1, node2)] = xy
                 label_tikz_code = rf"node[pos={pos}] {{\contour{{white}}{{{label}}}}}"
             direction = "left" if bending > 0 else "right"
             tikz_bending = f"bend {direction}={abs(bending)}" if bending != 0 else ""
             self.lines.append(rf"\draw[{style}] ({node1}) to[{tikz_bending}] {label_tikz_code} ({node2});")
 
 
-tikz_printer: TikzPrinter = TikzPrinter()
+class TikzLabeledGraphPrinter(TikzPrinter, Generic[Node, Label]):
+    def __init__(self, graph: "AbstractLabeledGraph[Node, Label]", shuffle_nodes=False):
+        self.graph: "AbstractLabeledGraph[Node, Label]" = graph  # For Pycharm
+        super().__init__(graph, shuffle_nodes=shuffle_nodes)
+
+    def labels(self, node1: Node, node2: Node) -> list[str]:
+        """Overwrite this method to modify tikz value for some labels."""
+        labels = self.graph._labels.get(self.graph._edge(node1, node2), [])
+
+        def format_(label):
+            # Note: math.isinf() supports `sympy.oo` too.
+            if label is None:
+                return ""
+            elif math.isinf(label) and label > 0:
+                return r"$\infty$"
+            elif math.isinf(label) and label < 0:
+                return r"$-\infty$"
+            else:
+                return str(label)
+
+        return [format_(label) for label in labels]
+
+
+class TikzAutomatonPrinter(TikzPrinter, Generic[Node]):
+    def __init__(self, graph: "Automaton[Node]", shuffle_nodes=False):
+        self.graph: "Automaton[Node]" = graph  # For Pycharm
+        super().__init__(graph, shuffle_nodes=shuffle_nodes)
+
+    def specific_node_style(self, node: Node) -> str:
+        styles = []
+        if node in self.graph.initial_states:
+            styles.append("rectangle")
+        return ",".join(styles)
+
+    def labels(self, node1, node2) -> list[str]:
+        labels = sorted(self.graph.labels(node1, node2))
+        if (
+            self.graph.alphabet_name is not None
+            and sorted(labels) == list(self.graph.alphabet)
+            and len(self.graph.alphabet) > 1
+        ):
+            return [self._latex(self.graph.alphabet_name)]
+        return [",".join(self._latex(label) for label in labels)] if labels else []
+
+    @staticmethod
+    def _latex(label: str) -> str:
+        label = label.replace("#", r"\#")
+        if label in GREEK_LETTERS:
+            label = "\\" + label
+        return f"${label}$" if label else r"$\varepsilon$"
+
+
+class TikzAcceptorPrinter(TikzAutomatonPrinter, Generic[Node]):
+    def __init__(self, graph: "Acceptor[Node]", shuffle_nodes=False):
+        self.graph: "Acceptor[Node]" = graph  # For Pycharm
+        super().__init__(graph, shuffle_nodes=shuffle_nodes)
+
+    def specific_node_style(self, node: Node) -> str:
+        styles = [super().specific_node_style(node)]
+        if node in self.graph.final_states:
+            styles.append("double,fill=lightgray")
+        return ",".join(styles)
+
+
+class TikzTransducerPrinter(TikzAutomatonPrinter, Generic[Node]):
+    def __init__(self, graph: "Transducer[Node]", shuffle_nodes=False):
+        self.graph: "Transducer[Node]" = graph  # For Pycharm
+        super().__init__(graph, shuffle_nodes=shuffle_nodes)
+
+    def labels(self, node1: Node, node2: Node) -> list[str]:
+        # Associate to each output word all the input letters than can produce it.
+        words: dict[str, set[Char]] = {}
+        for letter in self.graph.alphabet:
+            if self.graph.next_state(node1, letter) == node2:
+                words.setdefault(self.graph.next_word(node1, letter), set()).add(letter)
+
+        labels: list[str] = []
+        for word, letters in words.items():
+            sorted_letters = sorted(letters)
+            if sorted_letters == list(self.graph.alphabet) and self.graph.alphabet_name is not None:
+                letters_str = self.graph.alphabet_name
+            else:
+                letters_str = ",".join(sorted_letters)
+            letters_str = self._latex(letters_str)
+            if word:
+                letters_str += rf"\fbox{{{self._latex(word)}}}"
+            labels.append(letters_str)
+        return labels
+
+
+class TikzFlowNetworkPrinter(TikzPrinter, Generic[Node]):
+    def __init__(self, graph: "FlowNetwork[Node]", shuffle_nodes=False):
+        self.graph: "FlowNetwork[Node]" = graph  # For Pycharm
+        super().__init__(graph, shuffle_nodes=shuffle_nodes)
+
+    @cached_property
+    def nodes(self) -> tuple[Node, ...]:
+        """Return nodes in a nice order for tikz export."""
+        source = self.graph.source
+        sink = self.graph.sink
+        # When exporting graph as a tikz picture, all nodes are displayed on a circle.
+        # However, since it is a network flow, it is better to display source and sink at both extremities
+        # of the drawing (source at left, sink at right).
+        # We'll try to display nodes in a nice way too, detecting paths, to minimize edges' crossings,
+        # # though it's not so obvious...
+        angles: dict[Node, float] = {
+            source: 180,  # Display the source at the extreme-left of the graph.
+            sink: 0,  # Display the sink at the extreme-right of the graph.
+        }
+        path = self.graph.find_path(source, sink)
+        assert path[0] == source and path[-1] == sink
+        # If we find a path from source to sink, we display its nodes from left to right, on the top of the graph.
+        # We must remove source and sink from path, since there are already handled.
+        paths: tuple[list[Node], list[Node]] = (
+            path[1:-1],
+            self.graph.find_path(source, sink, _filter_nodes=path[1:-1])[1:-1],
+        )
+        assert len(paths) == 2
+        remaining_nodes = self.graph.nodes_set - set(paths[0]) - set(paths[1]) - {source, sink}
+        for i, node in enumerate(remaining_nodes):
+            paths[i % 2].append(node)
+
+        for j, path in enumerate(paths):
+            theta = 180 / (len(path) + 1)
+            for i, node in enumerate(reversed(path) if j == 0 else path, start=1):
+                angles[node] = j * 180 + i * theta
+        return tuple(node for angle, node in sorted((angle, node) for node, angle in angles.items()))
```

### Comparing `smallgraphlib-0.8.1/smallgraphlib/trees.py` & `smallgraphlib-0.9.0/smallgraphlib/trees.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,60 +1,60 @@
 from numbers import Real
-from typing import Iterable, Any, Dict, Set, Tuple, Iterator
+from typing import Iterable, Any, Set, Iterator, Generic
 
 from smallgraphlib import Graph, WeightedGraph, LabeledGraph
 from smallgraphlib.core import (
     AbstractGraph,
     InvalidGraphAttribute,
     Traversal,
 )
 from smallgraphlib.custom_types import Node, Edge
 
 
-class Tree:
+class Tree(Generic[Node]):
     """A rooted tree."""
 
     def __init__(
         self,
         nodes: Iterable[Node],
         root: Node = None,
         *edges: Edge,
-        nodes_labels: Dict[Node, Any] = None,
-        edges_labels: Dict[Edge, Any] = None,
+        nodes_labels: dict[Node, Any] = None,
+        edges_labels: dict[Edge, Any] = None,
     ):
         if root is None:
             root = next(iter(nodes))
         self._root = root
         if edges_labels is None:
-            self._graph = Graph(nodes, *edges)
+            self._graph: Graph[Node] = Graph(nodes, *edges)
         else:
             edges_labels = edges_labels.copy()
             labeled_edges = []
             for edge in edges:
                 labeled_edges.append((*edge, edges_labels.pop(edge, None)))
             if edges_labels:  # should be empty now
                 raise ValueError("Unknown edges: " + ", ".join(str(edge) for edge in edges_labels))
             if all(isinstance(value, Real) for value in edges_labels.values()):
                 self._graph = WeightedGraph(nodes, *labeled_edges)
             else:
                 self._graph = LabeledGraph(nodes, *labeled_edges)
 
     @property
-    def root(self) -> Node:  # type: ignore
+    def root(self) -> Node:
         return self._root
 
-    def as_graph(self) -> AbstractGraph:
+    def as_graph(self) -> AbstractGraph[Node]:
         return self._graph.copy()
 
     @property
-    def nodes(self) -> Tuple[Node, ...]:
+    def nodes(self) -> tuple[Node, ...]:
         return self._graph.nodes
 
     @property
-    def edges(self) -> Tuple[Edge, ...]:
+    def edges(self) -> tuple[Edge, ...]:
         return self._graph.edges
 
     def children(self, node: Node) -> Set[Node]:
         return self._graph.successors(node)
 
     def parent(self, node: Node) -> Node:
         if node == self.root:
```

### Comparing `smallgraphlib-0.8.1/smallgraphlib/utilities.py` & `smallgraphlib-0.9.0/smallgraphlib/utilities.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,23 +23,30 @@
 
 
 def cached_property(f):
     return property(cached(f))
 
 
 def clear_cache(f):
-    """Decorator to indicate that a function must invalidate the cache."""
+    """Decorator to indicate that a method must invalidate the class cache when called.
+
+    If the class have a method `on_clear_cache()`, it will be called too.
+    """
 
     @wraps(f)
     def cached_f(self=None, *args, **kw):
         result = f(self, *args, **kw)
         try:
             self._cache.clear()
         except AttributeError:
             self._cache = {}
+        try:
+            self.on_clear_cache()
+        except AttributeError:
+            pass
         return result
 
     return cached_f
 
 
 # class HasInternalCache:
 #     def put_in_cache(self, key, value):
@@ -65,16 +72,16 @@
         >>> s = Multiset(("a", "a", "b"))
         >>> s
         Multiset({'a': 2, 'b': 1})
         >>> s["b"] -= 1
         >>> s
         Multiset({'a': 2})
         >>> s["b"] -= 1
-        ...
-        ValueError: Multiset value can't be negative for key 'b'.
+        Traceback (most recent call last):
+        ValueError: Multiset value must be a positive integer, not -1.
 
     Trying to set negative values will raise a ValueError.
 
     Like `Counter`, `Multiset` is a `dict` subclass, so you may use dict methods on it.
 
     If you access it using the `dict` interface, be careful when iterating over keys.
     Modifying values when iterating over keys is unsafe, since if a value becomes zero,
@@ -122,7 +129,24 @@
 
 def frange(start: float, end: float, step: float = 1) -> Generator[float, None, None]:
     """Generate float values from `start` (included) to `end` (excluded) with an increment of `step`."""
     count = start
     while count < end:
         yield count
         count += step
+
+
+def set_repr(obj: object) -> str:
+    """Represent sets and (unnested) frozensets in a deterministic way, by sorting elements.
+
+    >>> set_repr({4, 3, 2})
+    '{2, 3, 4}'
+    >>> set_repr(frozenset({3, 2, 4}))
+    '{2, 3, 4}'
+
+    For any other objects, it just calls python default repr().
+    >>> set_repr(45.)
+    '45.0'
+    """
+    if isinstance(obj, (set, frozenset)):
+        return f"{{{', '.join(set_repr(elt) for elt in sorted(obj))}}}"
+    return repr(obj)
```

### Comparing `smallgraphlib-0.8.1/PKG-INFO` & `smallgraphlib-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smallgraphlib
-Version: 0.8.1
+Version: 0.9.0
 Summary: Simple library for handling small graphs, including Tikz code generation.
 Home-page: https://github.com/wxgeo/smallgraphlib
 License: GPL-3.0-or-later
 Keywords: graph,tikz,latex
 Author: Nicolas Pourcelot
 Author-email: nicolas.pourcelot@gmail.com
 Requires-Python: >=3.10,<4.0
```

