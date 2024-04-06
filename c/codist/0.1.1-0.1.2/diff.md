# Comparing `tmp/codist-0.1.1.tar.gz` & `tmp/codist-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codist-0.1.1.tar", last modified: Fri Apr  5 00:23:18 2024, max compression
+gzip compressed data, was "codist-0.1.2.tar", last modified: Sat Apr  6 12:00:37 2024, max compression
```

## Comparing `codist-0.1.1.tar` & `codist-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-05 00:23:18.117203 codist-0.1.1/
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3829 2024-04-05 00:23:18.116978 codist-0.1.1/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3446 2024-04-04 10:33:01.000000 codist-0.1.1/README.md
--rw-r--r--   0 jfin305  (1356368322) 1403514002      561 2024-04-05 00:22:33.000000 codist-0.1.1/pyproject.toml
--rw-r--r--   0 jfin305  (1356368322) 1403514002       38 2024-04-05 00:23:18.117252 codist-0.1.1/setup.cfg
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-05 00:23:18.113749 codist-0.1.1/src/
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-05 00:23:18.114667 codist-0.1.1/src/codist/
--rw-r--r--   0 jfin305  (1356368322) 1403514002      168 2024-04-05 00:21:58.000000 codist-0.1.1/src/codist/__init__.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002      618 2024-04-04 23:27:33.000000 codist-0.1.1/src/codist/ast.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     7963 2024-04-05 00:13:19.000000 codist-0.1.1/src/codist/distance.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     2012 2024-04-05 00:05:36.000000 codist-0.1.1/src/codist/tree.py
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-05 00:23:18.116744 codist-0.1.1/src/codist.egg-info/
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3829 2024-04-05 00:23:18.000000 codist-0.1.1/src/codist.egg-info/PKG-INFO
--rw-r--r--   0 jfin305  (1356368322) 1403514002      304 2024-04-05 00:23:18.000000 codist-0.1.1/src/codist.egg-info/SOURCES.txt
--rw-r--r--   0 jfin305  (1356368322) 1403514002        1 2024-04-05 00:23:18.000000 codist-0.1.1/src/codist.egg-info/dependency_links.txt
--rw-r--r--   0 jfin305  (1356368322) 1403514002        7 2024-04-05 00:23:18.000000 codist-0.1.1/src/codist.egg-info/top_level.txt
-drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-05 00:23:18.116306 codist-0.1.1/tests/
--rw-r--r--   0 jfin305  (1356368322) 1403514002      350 2024-04-04 03:47:43.000000 codist-0.1.1/tests/test_ast.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     3541 2024-04-04 22:53:09.000000 codist-0.1.1/tests/test_distance.py
--rw-r--r--   0 jfin305  (1356368322) 1403514002     1204 2024-04-04 10:36:27.000000 codist-0.1.1/tests/test_trees.py
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-06 12:00:37.557444 codist-0.1.2/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     1076 2024-04-05 00:24:06.000000 codist-0.1.2/LICENSE
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     5814 2024-04-06 12:00:37.557195 codist-0.1.2/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     4155 2024-04-06 10:24:02.000000 codist-0.1.2/README.md
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      561 2024-04-06 12:00:11.000000 codist-0.1.2/pyproject.toml
+-rw-r--r--   0 jfin305  (1356368322) 1403514002       38 2024-04-06 12:00:37.557492 codist-0.1.2/setup.cfg
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-06 12:00:37.554213 codist-0.1.2/src/
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-06 12:00:37.555319 codist-0.1.2/src/codist/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      168 2024-04-05 00:21:58.000000 codist-0.1.2/src/codist/__init__.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      618 2024-04-06 11:58:16.000000 codist-0.1.2/src/codist/ast.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     8188 2024-04-06 11:59:53.000000 codist-0.1.2/src/codist/distance.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     2010 2024-04-06 05:31:00.000000 codist-0.1.2/src/codist/tree.py
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-06 12:00:37.556941 codist-0.1.2/src/codist.egg-info/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     5814 2024-04-06 12:00:37.000000 codist-0.1.2/src/codist.egg-info/PKG-INFO
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      312 2024-04-06 12:00:37.000000 codist-0.1.2/src/codist.egg-info/SOURCES.txt
+-rw-r--r--   0 jfin305  (1356368322) 1403514002        1 2024-04-06 12:00:37.000000 codist-0.1.2/src/codist.egg-info/dependency_links.txt
+-rw-r--r--   0 jfin305  (1356368322) 1403514002        7 2024-04-06 12:00:37.000000 codist-0.1.2/src/codist.egg-info/top_level.txt
+drwxr-xr-x   0 jfin305  (1356368322) 1403514002        0 2024-04-06 12:00:37.556591 codist-0.1.2/tests/
+-rw-r--r--   0 jfin305  (1356368322) 1403514002      350 2024-04-04 03:47:43.000000 codist-0.1.2/tests/test_ast.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     3541 2024-04-04 22:53:09.000000 codist-0.1.2/tests/test_distance.py
+-rw-r--r--   0 jfin305  (1356368322) 1403514002     1204 2024-04-04 10:36:27.000000 codist-0.1.2/tests/test_trees.py
```

### Comparing `codist-0.1.1/PKG-INFO` & `codist-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: codist
-Version: 0.1.1
-Summary: AST edit distance
-Project-URL: repository, https://github.com/James-Ansley/codist
-Classifier: Development Status :: 1 - Planning
-Classifier: Topic :: Utilities
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-
 # CoDist
 
 CoDist (Code Distance) is a library that provides functions to calculate the
 edit distance and edit paths of abstract syntax trees.
 
 While this library is primarily concerned with AST edit distances, it can handle
 any generic tree of the form: `Tree[T] = tuple[T, tuple[Tree[T], ...]]`
@@ -22,14 +10,88 @@
 
 ```
 pip install codist
 ```
 
 ## Usage
 
+### Tree Edit Distance
+
+Trees are represented as tuples: `Tree[T] = tuple[T, tuple[Tree[T], ...]]`.
+
+For example, the following two trees from the original Zhang Shasha paper:
+
+<div style="display: flex; gap: 0.5ch; justify-content: center;">
+<img src="assets/graph_1.png" style="max-width: 47%; height: 14em;"/>
+<img src="assets/graph_2.png" style="max-width: 47%; height: 14em;"/>
+</div>
+
+Can be represented with the following tuples:
+
+```python
+tree1 = ("f", (("d", (("a", ()), ("c", (("b", ()),)))), ("e", ())))
+tree2 = ("f", (("c", (("d", (("a", ()), ("b", ())),),),), ("e", ())))
+```
+
+A small helper function, `t`, has been provided to make tree construction less
+verbose:
+
+```python
+from codist import t
+
+tree1 = t("f", t("d", t("a"), t("c", t("b"))), t("e"))
+tree2 = t("f", t("c", t("d", t("a"), t("b"))), t("e"))
+```
+
+The distance between these two trees can be taken with the `tree_dist` function:
+
+```python
+from codist import tree_dist
+
+dist = tree_dist(tree1, tree2)
+print("The distance is:", dist)  # The distance is 2
+```
+
+A custom set of cost functions can be provided with a `Cost` object:
+
+```python
+from codist import Cost, tree_dist
+
+cost = Cost(
+    delete=lambda n: 3,
+    insert=lambda n: 3,
+    relabel=lambda n1, n2: 0 if n1 == n2 else 2,
+)
+
+dist = tree_dist(tree1, tree2, cost=cost)
+print("The distance is:", dist)  # The distance is 6
+```
+
+By default, all change operations have a cost of 1 except for the case of
+γ(a -> a) which is 0.
+
+The edit path can be obtained with the `tree_edit` function which returns the
+tree distance and a tuple of change operations:
+
+```python
+from codist import tree_edit
+
+dist, path = tree_edit(tree1, tree2)
+path = tuple(c for c in path if c[0] != c[1])
+print("The distance is:", dist)  # The distance is 2
+print("The changes are:", path)  # The changes are: (('c', 'Λ'), ('Λ', 'c'))
+```
+
+Change operations are 2-tuples of the form: `tuple[T | Lambda, T | Lambda]`
+where `Lambda` is a singleton defined in the `distance` module.
+
+The `tree_edit` function can also take a cost object.
+
+### AST Edit Distance
+
 Currently, only AST node _type_ information is compared. A silhouette of an AST
 (an AST containing only type information) is constructed with
 the `parse_ast_silhouette` function.
 
 ```python
 from pprint import pprint
 from codist.ast import parse_ast_silhouette
@@ -88,74 +150,8 @@
         ('AugAssign',
          (('Name', (('Store', ()),)),
           ('Add', ()),
           ('List', (('Name', (('Load', ()),)), ('Load', ()))))))))),
     ('Return', (('Name', (('Load', ()),)),)))),))
 ```
 
-The distance between two ASTs can be computed with the `tree_dist` function.
-
-```python
-from codist import tree_dist
-
-print("The above trees have a distance of:", tree_dist(ast1, ast2))
-```
-
-Would print:
-
-```text
-The above trees have a distance of: 8
-```
-
-The edit path and distance between two trees can be computed with
-the `tree_edit` function. For convenience, this function also computes the
-edit distance:
-
-```python
-from codist import tree_edit
-
-dist, path = tree_edit(ast1, ast2)
-print("The above trees have a distance of:", dist)
-print("And an edit path of:")
-pprint(tuple(e for e in path if e[0] != e[1]))
-```
-
-which prints:
-
-
-```
-The above trees have a distance of: 8
-And an edit path of:
-(('Gt', 'GtE'),
- ('Load', 'Store'),
- ('Load', 'Add'),
- ('Attribute', 'Λ'),
- ('Λ', 'Load'),
- ('Λ', 'List'),
- ('Call', 'AugAssign'),
- ('Expr', 'Λ'))
-```
-
-A custom set of `Cost` functions can be provided to change the weights of
-insertions, deletions, and relabelings. By default, all change operations are 1
-except for the case of γ(a -> a) which is 0. To change the cost, construct
-a `Cost` object:
-
-```python
-from codist import Cost
-
-cost = Cost(
-    delete=(lambda n: 3),
-    insert=(lambda n: 3),
-    relabel=(lambda n1, n2: 0 if n1 == n2 else 2),
-)
-
-dist = tree_dist(ast1, ast2, cost=cost)
-
-print("The above trees have a distance of:", dist)
-```
-
-Which prints:
-
-```
-The above trees have a distance of: 20
-```
+The distance between these ASTs can be taken as above.
```

### Comparing `codist-0.1.1/pyproject.toml` & `codist-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "codist"
-version = "0.1.1"
+version = "0.1.2"
 description = "AST edit distance"
 
 readme = "README.md"
 requires-python = ">=3.12"
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `codist-0.1.1/src/codist/ast.py` & `codist-0.1.2/src/codist/ast.py`

 * *Files identical despite different names*

### Comparing `codist-0.1.1/src/codist/distance.py` & `codist-0.1.2/src/codist/distance.py`

 * *Files 12% similar despite different names*

```diff
@@ -71,55 +71,56 @@
     :param tree2: the target tree
     :param cost: a Cost object defining cost functions
 
     :returns: The edit distance between ``tree1`` and ``tree2``
     """
     postorder1 = tree.postorder(tree1)
     postorder2 = tree.postorder(tree2)
-    keyroots1 = tree.keyroots(tree1)
-    keyroots2 = tree.keyroots(tree2)
     l1 = tree.leftmosts(tree1)
     l2 = tree.leftmosts(tree2)
 
+    delete = cost.delete
+    insert = cost.insert
+    relabel = cost.relabel
+
     memo = [[0 for _ in postorder2] for _ in postorder1]
 
     def _tree_dist(i, j):
         forest_dist = [
             [0 for _ in range(j - l2[j] + 2)]
             for _ in range(i - l1[i] + 2)
         ]
 
-        for (i1, ni) in enumerate(range(l1[i], i + 1), start=1):
-            forest_dist[i1][0] = \
-                forest_dist[i1 - 1][0] + cost.delete(postorder1[ni])
-
-        for (j1, nj) in enumerate(range(l2[j], j + 1), start=1):
-            forest_dist[0][j1] = \
-                forest_dist[0][j1 - 1] + cost.insert(postorder2[nj])
+        for i1, ni in enumerate(range(l1[i], i + 1), start=1):
+            forest_dist[i1][0] = forest_dist[i1 - 1][0] + delete(postorder1[ni])
+
+        for j1, nj in enumerate(range(l2[j], j + 1), start=1):
+            forest_dist[0][j1] = forest_dist[0][j1 - 1] + insert(postorder2[nj])
 
-        for (i1, ni) in enumerate(range(l1[i], i + 1), start=1):
+        for i1, ni in enumerate(range(l1[i], i + 1), start=1):
             for (j1, nj) in enumerate(range(l2[j], j + 1), start=1):
+                node_i = postorder1[ni]
+                node_j = postorder2[nj]
                 if l1[ni] == l1[i] and l2[nj] == l2[j]:
-                    forest_dist[i1][j1] = min(
-                        forest_dist[i1 - 1][j1] + cost.delete(postorder1[ni]),
-                        forest_dist[i1][j1 - 1] + cost.insert(postorder2[nj]),
-                        forest_dist[i1 - 1][j1 - 1]
-                        + cost.relabel(postorder1[ni], postorder2[nj]),
+                    memo[ni][nj] = forest_dist[i1][j1] = min(
+                        forest_dist[i1 - 1][j1] + delete(node_i),
+                        forest_dist[i1][j1 - 1] + insert(node_j),
+                        forest_dist[i1 - 1][j1 - 1] + relabel(node_i, node_j),
                     )
-                    memo[ni][nj] = forest_dist[i1][j1]
                 else:
+                    m = l1[ni] - l1[i]
+                    n = l2[nj] - l2[j]
                     forest_dist[i1][j1] = min(
-                        forest_dist[i1 - 1][j1] + cost.delete(postorder1[ni]),
-                        forest_dist[i1][j1 - 1] + cost.insert(postorder2[nj]),
-                        forest_dist[l1[ni] - l1[i]][l2[nj] - l2[j]]
-                        + memo[ni][nj]
+                        forest_dist[i1 - 1][j1] + delete(node_i),
+                        forest_dist[i1][j1 - 1] + insert(node_j),
+                        forest_dist[m][n] + memo[ni][nj]
                     )
 
-    for ki in keyroots1:
-        for kj in keyroots2:
+    for ki in tree.keyroots(tree1):
+        for kj in tree.keyroots(tree2):
             _tree_dist(ki, kj)
 
     return memo[-1][-1]
 
 
 def tree_edit[T](
       tree1: Tree[T],
@@ -136,84 +137,95 @@
     :returns: A tuple containing the edit distance between
         ``tree1`` and ``tree2`` and a tuple of `Change` operations where each
         change operation is a 2-tuple of the form ``(T | Lambda -> T | Lambda)``
         where ``Lambda`` is a singleton string: ``"Λ"``
     """
     postorder1 = tree.postorder(tree1)
     postorder2 = tree.postorder(tree2)
-    keyroots1 = tree.keyroots(tree1)
-    keyroots2 = tree.keyroots(tree2)
     l1 = tree.leftmosts(tree1)
     l2 = tree.leftmosts(tree2)
 
+    delete = cost.delete
+    insert = cost.insert
+    relabel = cost.relabel
+
     memo = [[0 for _ in postorder2] for _ in postorder1]
     ops = [[[] for _ in postorder2] for _ in postorder1]
 
     def _tree_dist(i, j):
         forest_dist = [
             [0 for _ in range(j - l2[j] + 2)]
             for _ in range(i - l1[i] + 2)
         ]
-        opt_parts = [[[] for _ in range(j - l2[j] + 2)]
+        opt_parts = [[() for _ in range(j - l2[j] + 2)]
                      for _ in range(i - l1[i] + 2)]
 
-        for (i1, ni) in enumerate(range(l1[i], i + 1), start=1):
+        for i1, ni in enumerate(range(l1[i], i + 1), start=1):
             node = postorder1[ni]
-            forest_dist[i1][0] = \
-                forest_dist[i1 - 1][0] + cost.delete(node)
-            opt_parts[i1][0] = [*opt_parts[i1 - 1][0], (node, Lambda)]
+            forest_dist[i1][0] = forest_dist[i1 - 1][0] + delete(node)
+            opt_parts[i1][0] = ((i1 - 1, 0), ((node, Lambda),))
 
-        for (j1, nj) in enumerate(range(l2[j], j + 1), start=1):
+        for j1, nj in enumerate(range(l2[j], j + 1), start=1):
             node = postorder2[nj]
-            forest_dist[0][j1] = \
-                forest_dist[0][j1 - 1] + cost.insert(node)
-            opt_parts[0][j1] = [*opt_parts[0][j1 - 1], (Lambda, node)]
+            forest_dist[0][j1] = forest_dist[0][j1 - 1] + insert(node)
+            opt_parts[0][j1] = ((0, j1 - 1), ((Lambda, node),))
 
-        for (i1, ni) in enumerate(range(l1[i], i + 1), start=1):
-            for (j1, nj) in enumerate(range(l2[j], j + 1), start=1):
+        for i1, ni in enumerate(range(l1[i], i + 1), start=1):
+            for j1, nj in enumerate(range(l2[j], j + 1), start=1):
                 left = postorder1[ni]
                 right = postorder2[nj]
                 if l1[ni] == l1[i] and l2[nj] == l2[j]:
-                    costs = [
-                        forest_dist[i1 - 1][j1] + cost.delete(left),
-                        forest_dist[i1][j1 - 1] + cost.insert(right),
-                        forest_dist[i1 - 1][j1 - 1]
-                        + cost.relabel(left, right),
-                    ]
-                    forest_dist[i1][j1] = min(costs)
+                    min_cost, forest_dist[i1][j1] = min(enumerate((
+                        forest_dist[i1 - 1][j1] + delete(left),
+                        forest_dist[i1][j1 - 1] + insert(right),
+                        forest_dist[i1 - 1][j1 - 1] + relabel(left, right),
+                    )), key=lambda e: e[1])
                     memo[ni][nj] = forest_dist[i1][j1]
-                    min_cost = min((0, 1, 2), key=lambda i_: costs[i_])
                     if min_cost == 0:
-                        opt_parts[i1][j1] = \
-                            [*opt_parts[i1 - 1][j1], (left, Lambda)]
+                        change = (left, Lambda)
+                        opt_parts[i1][j1] = ((i1 - 1, j1), (change,))
                     elif min_cost == 1:
-                        opt_parts[i1][j1] = \
-                            [*opt_parts[i1][j1 - 1], (Lambda, right)]
+                        change = (Lambda, right)
+                        opt_parts[i1][j1] = ((i1, j1 - 1), (change,))
                     else:
-                        opt_parts[i1][j1] = \
-                            [*opt_parts[i1 - 1][j1 - 1], (left, right)]
-                    ops[ni][nj] = opt_parts[i1][j1]
+                        change = (left, right)
+                        opt_parts[i1][j1] = ((i1 - 1, j1 - 1), (change,))
+                    ops[ni][nj] = change_path(opt_parts, i1, j1)
                 else:
                     m = l1[ni] - l1[i]
                     n = l2[nj] - l2[j]
-                    costs = [
-                        forest_dist[i1 - 1][j1] + cost.delete(left),
-                        forest_dist[i1][j1 - 1] + cost.insert(right),
+                    min_cost, forest_dist[i1][j1] = min(enumerate((
+                        forest_dist[i1 - 1][j1] + delete(left),
+                        forest_dist[i1][j1 - 1] + insert(right),
                         forest_dist[m][n] + memo[ni][nj],
-                    ]
-                    forest_dist[i1][j1] = min(costs)
-                    min_cost = min((0, 1, 2), key=lambda i_: costs[i_])
+                    )), key=lambda e: e[1])
                     if min_cost == 0:
-                        opt_parts[i1][j1] = \
-                            [*opt_parts[i1 - 1][j1], (left, Lambda)]
+                        change = (left, Lambda)
+                        opt_parts[i1][j1] = ((i1 - 1, j1), (change,))
                     elif min_cost == 1:
-                        opt_parts[i1][j1] = \
-                            [*opt_parts[i1][j1 - 1], (Lambda, right)]
+                        change = (Lambda, right)
+                        opt_parts[i1][j1] = ((i1, j1 - 1), (change,))
                     else:
-                        opt_parts[i1][j1] = \
-                            [*opt_parts[m][n], *ops[ni][nj]]
+                        next_op, changes = opt_parts[m][n]
+                        opt_parts[i1][j1] = (next_op, changes + ops[ni][nj])
 
-    for ki in keyroots1:
-        for kj in keyroots2:
+    for ki in tree.keyroots(tree1):
+        for kj in tree.keyroots(tree2):
             _tree_dist(ki, kj)
 
     return memo[-1][-1], tuple(ops[-1][-1])
+
+
+def change_path(ops, i, j) -> tuple[Change, ...]:
+    next_op, change = ops[i][j]
+    result = [*change[::-1]]
+    stack = [next_op]
+    while stack:
+        (i, j) = stack.pop()
+        current = ops[i][j]
+        if i < 0 or j < 0 or current == ():
+            continue
+        next_op, change = current
+        if change is not None:
+            result.extend(change[::-1])
+        stack.append(next_op)
+    return tuple(reversed(result))
```

### Comparing `codist-0.1.1/src/codist/tree.py` & `codist-0.1.2/src/codist/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 #: A tree is any tuple of the form: ``Tree[T] = tuple[T, tuple[Tree[T], ...]]``
 Tree: type["tuple[T, tuple[Tree[T], ...]]"]
 
 type Tree[T: Hashable] = tuple[T, tuple[Tree[T], ...]]
 
 
 def t[T](
-      value: T,
+      root: T,
       *children: Tree[T],
 ) -> Tree[T]:
     """Small convenience function to help construct trees"""
-    return value, children
+    return root, children
 
 
 def postorder[T](tree: Tree[T]) -> tuple[T, ...]:
     """A postorder traversal of the node data in ``tree``"""
     s1 = [tree]
     s2 = []
     while s1:
```

### Comparing `codist-0.1.1/tests/test_distance.py` & `codist-0.1.2/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `codist-0.1.1/tests/test_trees.py` & `codist-0.1.2/tests/test_trees.py`

 * *Files identical despite different names*

