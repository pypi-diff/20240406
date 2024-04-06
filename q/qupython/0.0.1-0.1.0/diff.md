# Comparing `tmp/qupython-0.0.1.tar.gz` & `tmp/qupython-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qupython-0.0.1.tar", last modified: Sun Nov 12 15:36:42 2023, max compression
+gzip compressed data, was "qupython-0.1.0.tar", last modified: Sat Apr  6 14:07:41 2024, max compression
```

## Comparing `qupython-0.0.1.tar` & `qupython-0.1.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 frank     (1000) frank     (1000)        0 2023-11-12 15:36:42.635502 qupython-0.0.1/
--rw-r--r--   0 frank     (1000) frank     (1000)     1070 2023-11-12 15:35:56.000000 qupython-0.0.1/LICENSE
--rw-r--r--   0 frank     (1000) frank     (1000)     5621 2023-11-12 15:36:42.634502 qupython-0.0.1/PKG-INFO
--rw-r--r--   0 frank     (1000) frank     (1000)     5091 2023-11-12 14:44:34.000000 qupython-0.0.1/README.md
--rw-r--r--   0 frank     (1000) frank     (1000)      516 2023-11-12 15:34:19.000000 qupython-0.0.1/pyproject.toml
-drwxr-xr-x   0 frank     (1000) frank     (1000)        0 2023-11-12 15:36:42.633502 qupython-0.0.1/qupython/
--rw-r--r--   0 frank     (1000) frank     (1000)       56 2023-11-04 13:04:24.000000 qupython-0.0.1/qupython/__init__.py
--rw-r--r--   0 frank     (1000) frank     (1000)     4009 2023-11-12 13:49:33.000000 qupython-0.0.1/qupython/construction.py
--rw-r--r--   0 frank     (1000) frank     (1000)      258 2023-11-05 15:34:41.000000 qupython-0.0.1/qupython/decorator.py
--rw-r--r--   0 frank     (1000) frank     (1000)     3599 2023-11-05 15:36:52.000000 qupython-0.0.1/qupython/err_msg.py
--rw-r--r--   0 frank     (1000) frank     (1000)     2230 2023-11-12 12:48:19.000000 qupython-0.0.1/qupython/function.py
--rw-r--r--   0 frank     (1000) frank     (1000)     5724 2023-11-12 14:29:49.000000 qupython-0.0.1/qupython/qubit.py
-drwxr-xr-x   0 frank     (1000) frank     (1000)        0 2023-11-12 15:36:42.634502 qupython-0.0.1/qupython.egg-info/
--rw-r--r--   0 frank     (1000) frank     (1000)     5621 2023-11-12 15:36:42.000000 qupython-0.0.1/qupython.egg-info/PKG-INFO
--rw-r--r--   0 frank     (1000) frank     (1000)      331 2023-11-12 15:36:42.000000 qupython-0.0.1/qupython.egg-info/SOURCES.txt
--rw-r--r--   0 frank     (1000) frank     (1000)        1 2023-11-12 15:36:42.000000 qupython-0.0.1/qupython.egg-info/dependency_links.txt
--rw-r--r--   0 frank     (1000) frank     (1000)        9 2023-11-12 15:36:42.000000 qupython-0.0.1/qupython.egg-info/top_level.txt
--rw-r--r--   0 frank     (1000) frank     (1000)       38 2023-11-12 15:36:42.635502 qupython-0.0.1/setup.cfg
-drwxr-xr-x   0 frank     (1000) frank     (1000)        0 2023-11-12 15:36:42.634502 qupython-0.0.1/test/
--rw-r--r--   0 frank     (1000) frank     (1000)     2590 2023-11-05 00:18:34.000000 qupython-0.0.1/test/test_public_api.py
--rw-r--r--   0 frank     (1000) frank     (1000)     3436 2023-11-12 14:36:25.000000 qupython-0.0.1/test/test_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:07:41.804134 qupython-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-06 14:07:17.000000 qupython-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-06 14:07:41.804134 qupython-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-04-06 14:07:17.000000 qupython-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-06 14:07:37.000000 qupython-0.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:07:41.800134 qupython-0.1.0/qupython/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-06 14:07:17.000000 qupython-0.1.0/qupython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-06 14:07:17.000000 qupython-0.1.0/qupython/construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-06 14:07:17.000000 qupython-0.1.0/qupython/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-06 14:07:17.000000 qupython-0.1.0/qupython/err_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-04-06 14:07:17.000000 qupython-0.1.0/qupython/function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2024-04-06 14:07:17.000000 qupython-0.1.0/qupython/qubit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-06 14:07:17.000000 qupython-0.1.0/qupython/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:07:41.804134 qupython-0.1.0/qupython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5427 2024-04-06 14:07:41.000000 qupython-0.1.0/qupython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-06 14:07:41.000000 qupython-0.1.0/qupython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 14:07:41.000000 qupython-0.1.0/qupython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-06 14:07:41.000000 qupython-0.1.0/qupython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 14:07:41.000000 qupython-0.1.0/qupython.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 14:07:41.804134 qupython-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:07:41.804134 qupython-0.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-06 14:07:17.000000 qupython-0.1.0/test/test_code_examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-06 14:07:17.000000 qupython-0.1.0/test/test_public_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-06 14:07:17.000000 qupython-0.1.0/test/test_readme.py
```

### Comparing `qupython-0.0.1/LICENSE` & `qupython-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qupython-0.0.1/PKG-INFO` & `qupython-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: qupython
-Version: 0.0.1
+Version: 0.1.0
 Summary: Write quantum programs directly in Python
 Author-email: Frank Harkins <frankharkins@hotmail.co.uk>
 Project-URL: Homepage, https://github.com/frankharkins/qupython
 Project-URL: Bug Tracker, https://github.com/frankharkins/qupython/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: qiskit
+Requires-Dist: qiskit-aer
 
 # quPython
 
-> Quantum programs directly in Python 
-
-> [!WARNING]  
-> This project is currently a proof-of-concept. It will be buggy and unstable.
+```
+pip install qupython
+```
 
 quPython compiles Python functions into quantum programs, executes the
 programs, and returns the results as `bool`-like objects.
 
-## What can it do?
-
 Initialize a `quPython.Qubit` object just like any other object and use it
-inside a `@quantum` function.
+inside a `@quantum` function. These are the only two imports you'll need.
 
 ```python
 from qupython import Qubit, quantum
 
 @quantum
 def random_bit():
     qubit = Qubit()         # Allocate new qubit
@@ -41,123 +40,100 @@
 program, executes it, and returns results.
 
 ```python
 >>> random_bit()
 True
 ```
 
-quPython makes writing quantum programs feel like any other Python program.
+## Python-like data management
 
-### Features and examples
-
-Allocate qubits as you go, and return classical bits as `bool`-like objects in
-whatever form you like.
+Create classes for quantum data just as you would conventional data. The
+following example creates a simple logical qubit class. See the [Logical qubit
+example](./examples/logical-qubit.md) for a more complete class.
 
 ```python
-@quantum
-def ghz(num_bits: int):
+from qupython import Qubit, quantum
+from qupython.typing import BitPromise
+
+class LogicalQubit:
     """
-    Create and measure a GHZ state
+    Simple logical qubit using the five-qubit code.
+    See https://en.wikipedia.org/wiki/Five-qubit_error_correcting_code
     """
-    qubits = [ Qubit() for _ in range(num_bits) ]
-    control, targets = qubits[0], qubits[1:]
-    control.h()
-    for target in targets:
-        target.x(conditions=[control])
-    return [ qubit.measure() for qubit in qubits ]
-```
-
-```
->>> ghz(8)
-[False, False, False, False, False, False, False, False]
+    def __init__(self):
+        """
+        Create new logical qubit and initialize to logical |0>.
+        Uses initialization procedure from https://quantumcomputing.stackexchange.com/a/14449
+        """
+        self.qubits = [Qubit() for _ in range(5)]
+        self.qubits[4].z()
+        for q in self.qubits[:4]:
+            q.h()
+            self.qubits[4].x(conditions=[q])
+        for a, b in [(0,4),(0,1),(2,3),(1,2),(3,4)]:
+            control = self.qubits[b]
+            self.qubits[a].z(conditions=[control])
+
+    def measure(self) -> BitPromise:
+        """
+        Measure logical qubit to single classical bit
+        """
+        out = Qubit().h()
+        for q in self.qubits:
+            q.z(conditions=[out])
+        return out.h().measure()
 ```
 
-Create classes for quantum data just as you would conventional data, and
-condition quantum gates on classical and quantum data in exactly the same way.
+This abstracts the bit-level operations away from the user.
 
 ```python
-class BellPair:
-    def __init__(self):
-        self.left = Qubit().h()
-        self.right = Qubit().x(conditions=[self.left])
-
 @quantum
-def teleportation_demo():
-    message = Qubit()
-
-    bell_pair = BellPair()
-    do_x = bell_pair.left.x(conditions=[message]).measure()
-    do_z = message.h().measure()
+def logical_qubit_demo() -> BitPromise:
+    q = LogicalQubit()
+    return q.measure()
+```
 
-    bell_pair.right.x(conditions=[do_x]).z(conditions=[do_z])
-    return bell_pair.right.measure()
+```python
+>>> logical_qubit_demo()
+False
 ```
 
-### Generate Qiskit circuits
+## Generate Qiskit circuits
 
 If you want, you can just use quPython to create Qiskit circuits with Pythonic
 syntax (rather than the assembly-like syntax of `qc.cx(0, 1)` in native
 Qiskit).
 
 ```python
 # Compile using quPython
-teleportation_demo.compile()
+logical_qubit_demo.compile()
 
 # Draw compiled Qiskit circuit
-teleportation_demo.circuit.draw()
+logical_qubit_demo.circuit.draw()
 ```
 
 ```
-                    ┌───┐┌─┐                           
-q_0: ────────────■──┤ H ├┤M├───────────────────────────
-          ┌───┐  │  └───┘└╥┘┌──────────┐┌──────────┐┌─┐
-q_1: ─────┤ X ├──┼────────╫─┤0         ├┤0         ├┤M├
-     ┌───┐└─┬─┘┌─┴─┐ ┌─┐  ║ │          ││          │└╥┘
-q_2: ┤ H ├──■──┤ X ├─┤M├──╫─┤          ├┤          ├─╫─
-     └───┘     └───┘ └╥┘  ║ │  If_else ││          │ ║ 
-c_0: ═════════════════╬═══╬═╡          ╞╡  If_else ╞═╩═
-                      ║   ║ │          ││          │   
-c_1: ═════════════════╩═══╬═╡0         ╞╡          ╞═══
-                          ║ └──────────┘│          │   
-c_2: ═════════════════════╩═════════════╡0         ╞═══
-                                        └──────────┘   
+     ┌───┐                                                       
+q_0: ┤ H ├────────────■────────■───────────■─────■───────────────
+     ├───┤            │        │           │     │               
+q_1: ┤ H ├──■─────────┼────────┼──■──■──■──┼─────┼───────────────
+     ├───┤  │         │        │  │  │  │  │     │               
+q_2: ┤ H ├──┼────■────┼────────┼──┼──■──┼──■──■──┼───────────────
+     ├───┤┌─┴─┐┌─┴─┐┌─┴─┐┌───┐ │  │     │     │  │               
+q_3: ┤ Z ├┤ X ├┤ X ├┤ X ├┤ X ├─┼──■──■──┼─────┼──┼─────■─────────
+     ├───┤└───┘└───┘└───┘└─┬─┘ │     │  │     │  │     │ ┌───┐┌─┐
+q_4: ┤ H ├─────────────────┼───┼─────┼──■─────■──■──■──■─┤ H ├┤M├
+     ├───┤                 │   │     │              │    └───┘└╥┘
+q_5: ┤ H ├─────────────────■───■─────■──────────────■──────────╫─
+     └───┘                                                     ║ 
+c: 1/══════════════════════════════════════════════════════════╩═
+                                                               0 
 ```
 
 You can compile the function without executing it, optimize the cirucit,
 execute it however you like, then use quPython to interpret the results.
 
 ```python
 from qiskit_aer.primitives import Sampler
-qiskit_result = Sampler().run(teleportation_demo.circuit).result()
-teleportation_demo.interpret_result(qiskit_result)  # returns `False`
-```
-
-## How it works
-
-> For contributors (or the curious)
-
-To see how quPython works, we'll use the `Qubit` object outside a `@quantum`
-function. `Qubit` objects store a list of operations that act on them.
-
-```python
->>> qubit = Qubit()
->>> qubit.h()
->>> qubit.operations
-[quPythonInstruction(h, [<qupython.qubit.Qubit object at 0x7fddf68504d0>])]
+qiskit_result = Sampler().run(logical_qubit_demo.circuit).result()
+logical_qubit_demo.interpret_result(qiskit_result)  # returns `False`
 ```
-
-The only way to get a classical data type from a quantum program is the
-`Qubit.measure` method. We give the appearance that this returns a `bool`, but
-it actually returns a `QubitPromise` object, which saves a link to the measure
-operation that created it.
-
-```python
->>> promise = qubit.measure()
->>> promise
-QubitPromise(<qupython.qubit.quPythonMeasurement object at 0x7fddf0ddbbd0>)
-```
-
-When the user calls a `@quantum` function, quPython intercepts the output,
-finds any `QubitPromise` objects, then traces back the `Qubits` those promises
-came from. With this information, quPython can construct the `QuantumCircuit`
-needed to fulfil the promises. quPython then executes the circuit and fills in
-the `QubitPromise` values.
```

### Comparing `qupython-0.0.1/README.md` & `qupython-0.1.0/qupython.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,34 @@
-# quPython
+Metadata-Version: 2.1
+Name: qupython
+Version: 0.1.0
+Summary: Write quantum programs directly in Python
+Author-email: Frank Harkins <frankharkins@hotmail.co.uk>
+Project-URL: Homepage, https://github.com/frankharkins/qupython
+Project-URL: Bug Tracker, https://github.com/frankharkins/qupython/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: qiskit
+Requires-Dist: qiskit-aer
 
-> Quantum programs directly in Python 
+# quPython
 
-> [!WARNING]  
-> This project is currently a proof-of-concept. It will be buggy and unstable.
+```
+pip install qupython
+```
 
 quPython compiles Python functions into quantum programs, executes the
 programs, and returns the results as `bool`-like objects.
 
-## What can it do?
-
 Initialize a `quPython.Qubit` object just like any other object and use it
-inside a `@quantum` function.
+inside a `@quantum` function. These are the only two imports you'll need.
 
 ```python
 from qupython import Qubit, quantum
 
 @quantum
 def random_bit():
     qubit = Qubit()         # Allocate new qubit
@@ -27,123 +40,100 @@
 program, executes it, and returns results.
 
 ```python
 >>> random_bit()
 True
 ```
 
-quPython makes writing quantum programs feel like any other Python program.
-
-### Features and examples
+## Python-like data management
 
-Allocate qubits as you go, and return classical bits as `bool`-like objects in
-whatever form you like.
+Create classes for quantum data just as you would conventional data. The
+following example creates a simple logical qubit class. See the [Logical qubit
+example](./examples/logical-qubit.md) for a more complete class.
 
 ```python
-@quantum
-def ghz(num_bits: int):
+from qupython import Qubit, quantum
+from qupython.typing import BitPromise
+
+class LogicalQubit:
     """
-    Create and measure a GHZ state
+    Simple logical qubit using the five-qubit code.
+    See https://en.wikipedia.org/wiki/Five-qubit_error_correcting_code
     """
-    qubits = [ Qubit() for _ in range(num_bits) ]
-    control, targets = qubits[0], qubits[1:]
-    control.h()
-    for target in targets:
-        target.x(conditions=[control])
-    return [ qubit.measure() for qubit in qubits ]
-```
-
-```
->>> ghz(8)
-[False, False, False, False, False, False, False, False]
+    def __init__(self):
+        """
+        Create new logical qubit and initialize to logical |0>.
+        Uses initialization procedure from https://quantumcomputing.stackexchange.com/a/14449
+        """
+        self.qubits = [Qubit() for _ in range(5)]
+        self.qubits[4].z()
+        for q in self.qubits[:4]:
+            q.h()
+            self.qubits[4].x(conditions=[q])
+        for a, b in [(0,4),(0,1),(2,3),(1,2),(3,4)]:
+            control = self.qubits[b]
+            self.qubits[a].z(conditions=[control])
+
+    def measure(self) -> BitPromise:
+        """
+        Measure logical qubit to single classical bit
+        """
+        out = Qubit().h()
+        for q in self.qubits:
+            q.z(conditions=[out])
+        return out.h().measure()
 ```
 
-Create classes for quantum data just as you would conventional data, and
-condition quantum gates on classical and quantum data in exactly the same way.
+This abstracts the bit-level operations away from the user.
 
 ```python
-class BellPair:
-    def __init__(self):
-        self.left = Qubit().h()
-        self.right = Qubit().x(conditions=[self.left])
-
 @quantum
-def teleportation_demo():
-    message = Qubit()
-
-    bell_pair = BellPair()
-    do_x = bell_pair.left.x(conditions=[message]).measure()
-    do_z = message.h().measure()
+def logical_qubit_demo() -> BitPromise:
+    q = LogicalQubit()
+    return q.measure()
+```
 
-    bell_pair.right.x(conditions=[do_x]).z(conditions=[do_z])
-    return bell_pair.right.measure()
+```python
+>>> logical_qubit_demo()
+False
 ```
 
-### Generate Qiskit circuits
+## Generate Qiskit circuits
 
 If you want, you can just use quPython to create Qiskit circuits with Pythonic
 syntax (rather than the assembly-like syntax of `qc.cx(0, 1)` in native
 Qiskit).
 
 ```python
 # Compile using quPython
-teleportation_demo.compile()
+logical_qubit_demo.compile()
 
 # Draw compiled Qiskit circuit
-teleportation_demo.circuit.draw()
+logical_qubit_demo.circuit.draw()
 ```
 
 ```
-                    ┌───┐┌─┐                           
-q_0: ────────────■──┤ H ├┤M├───────────────────────────
-          ┌───┐  │  └───┘└╥┘┌──────────┐┌──────────┐┌─┐
-q_1: ─────┤ X ├──┼────────╫─┤0         ├┤0         ├┤M├
-     ┌───┐└─┬─┘┌─┴─┐ ┌─┐  ║ │          ││          │└╥┘
-q_2: ┤ H ├──■──┤ X ├─┤M├──╫─┤          ├┤          ├─╫─
-     └───┘     └───┘ └╥┘  ║ │  If_else ││          │ ║ 
-c_0: ═════════════════╬═══╬═╡          ╞╡  If_else ╞═╩═
-                      ║   ║ │          ││          │   
-c_1: ═════════════════╩═══╬═╡0         ╞╡          ╞═══
-                          ║ └──────────┘│          │   
-c_2: ═════════════════════╩═════════════╡0         ╞═══
-                                        └──────────┘   
+     ┌───┐                                                       
+q_0: ┤ H ├────────────■────────■───────────■─────■───────────────
+     ├───┤            │        │           │     │               
+q_1: ┤ H ├──■─────────┼────────┼──■──■──■──┼─────┼───────────────
+     ├───┤  │         │        │  │  │  │  │     │               
+q_2: ┤ H ├──┼────■────┼────────┼──┼──■──┼──■──■──┼───────────────
+     ├───┤┌─┴─┐┌─┴─┐┌─┴─┐┌───┐ │  │     │     │  │               
+q_3: ┤ Z ├┤ X ├┤ X ├┤ X ├┤ X ├─┼──■──■──┼─────┼──┼─────■─────────
+     ├───┤└───┘└───┘└───┘└─┬─┘ │     │  │     │  │     │ ┌───┐┌─┐
+q_4: ┤ H ├─────────────────┼───┼─────┼──■─────■──■──■──■─┤ H ├┤M├
+     ├───┤                 │   │     │              │    └───┘└╥┘
+q_5: ┤ H ├─────────────────■───■─────■──────────────■──────────╫─
+     └───┘                                                     ║ 
+c: 1/══════════════════════════════════════════════════════════╩═
+                                                               0 
 ```
 
 You can compile the function without executing it, optimize the cirucit,
 execute it however you like, then use quPython to interpret the results.
 
 ```python
 from qiskit_aer.primitives import Sampler
-qiskit_result = Sampler().run(teleportation_demo.circuit).result()
-teleportation_demo.interpret_result(qiskit_result)  # returns `False`
-```
-
-## How it works
-
-> For contributors (or the curious)
-
-To see how quPython works, we'll use the `Qubit` object outside a `@quantum`
-function. `Qubit` objects store a list of operations that act on them.
-
-```python
->>> qubit = Qubit()
->>> qubit.h()
->>> qubit.operations
-[quPythonInstruction(h, [<qupython.qubit.Qubit object at 0x7fddf68504d0>])]
+qiskit_result = Sampler().run(logical_qubit_demo.circuit).result()
+logical_qubit_demo.interpret_result(qiskit_result)  # returns `False`
 ```
-
-The only way to get a classical data type from a quantum program is the
-`Qubit.measure` method. We give the appearance that this returns a `bool`, but
-it actually returns a `QubitPromise` object, which saves a link to the measure
-operation that created it.
-
-```python
->>> promise = qubit.measure()
->>> promise
-QubitPromise(<qupython.qubit.quPythonMeasurement object at 0x7fddf0ddbbd0>)
-```
-
-When the user calls a `@quantum` function, quPython intercepts the output,
-finds any `QubitPromise` objects, then traces back the `Qubits` those promises
-came from. With this information, quPython can construct the `QuantumCircuit`
-needed to fulfil the promises. quPython then executes the circuit and fills in
-the `QubitPromise` values.
```

### Comparing `qupython-0.0.1/pyproject.toml` & `qupython-0.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 [project]
 name = "qupython"
-version = "0.0.1"
-authors = [
-  { name="Frank Harkins", email="frankharkins@hotmail.co.uk" },
-]
+version = "0.1.0"
 description = "Write quantum programs directly in Python"
 readme = "README.md"
 requires-python = ">=3.8"
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-]
+classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
+dependencies = [ "qiskit", "qiskit-aer",]
+[[project.authors]]
+name = "Frank Harkins"
+email = "frankharkins@hotmail.co.uk"
 
 [project.urls]
-"Homepage" = "https://github.com/frankharkins/qupython"
+Homepage = "https://github.com/frankharkins/qupython"
 "Bug Tracker" = "https://github.com/frankharkins/qupython/issues"
```

### Comparing `qupython-0.0.1/qupython/construction.py` & `qupython-0.1.0/qupython/construction.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Functions for compiling quantum circuits from QubitPromise objects
+# Functions for compiling quantum circuits from BitPromise objects
 
 import contextlib
 import qiskit
 from collections.abc import Mapping, Iterable
-from .qubit import Qubit, QubitPromise, quPythonInstruction, quPythonMeasurement
+from .qubit import Qubit, BitPromise, quPythonInstruction, quPythonMeasurement
 from .err_msg import ERR_MSG
 
 
 def _get_promises(obj):
     """
-    Recursively search Python object for `QubitPromises`.
+    Recursively search Python object for `BitPromise` objects.
     """
     # TODO: unit test
     if obj is None:
         return set()
 
     if isinstance(obj, (int, float, bool, str)):
         return set()
 
     if isinstance(obj, Qubit):
         raise ValueError(ERR_MSG["ReturnQubitFromQuantumFunction"])
-    if isinstance(obj, QubitPromise):
+    if isinstance(obj, BitPromise):
         return set([obj])
 
     if hasattr(obj, "__dict__"):
         obj = obj.__dict__
 
     if isinstance(obj, Mapping):
         promises = set()
@@ -43,73 +43,61 @@
 
 
 def _get_bits_from_promises(promises):
     """
     Find all qubits needed to fulfil all promises. This includes any qubits
     that interact with measured qubits.
     """
-    # TODO: unit test
-    # TODO: this does not work if a measurement is conditioned on a promise
-    # that isn't in `promises`. Qubits and promises are now too similar and
-    # should inherit from the same class. For example, we need
-    # `get_linked_bits` to search through both qubits and promises.
-    initial_bits = set(promises)
+    initial_bits=set(promises)
     all_bits = initial_bits.copy()
     for bit in initial_bits:
-        all_bits |= bit.get_linked_bits()
+        all_bits |= bit.get_linked_bits(already_found=all_bits)
     return all_bits
 
 
 def _waiting_for_bits(instruction):
     """
     Check if instruction can be applied to circuit.
     """
     for bit in instruction.qubits+instruction.promises:
-        if bit.operations.index(instruction) != bit.op_pointer:
+        if bit.operations[bit.op_pointer] != instruction:
             return True
     return False
 
 
 def _add_instructions_to_circuit(circuit, qubit):
     """
     Keep adding this Qubit's instructions to the circuit until complete, or
     waiting for another bit or qubit.
     """
     for op in qubit.operations[qubit.op_pointer :]:
         if _waiting_for_bits(op):
             return
+        for bit in op.qubits+op.promises:
+            bit.op_pointer += 1
         if isinstance(op, quPythonMeasurement):
-            qubit.op_pointer += 1
             for promise in op.promises:
                 circuit.measure(qubit.index, promise.index)
-                promise.op_pointer += 1
             continue
-        if op.promises:
-            # TODO: neaten up
-            with contextlib.ExitStack() as stack:
-                for promise in op.promises:
-                    stack.enter_context(
-                        circuit.if_test((promise.index, int(not promise.inverse)))
-                    )
-                circuit.append(op.qiskit_instruction, [q.index for q in op.qubits])
-
-        else:
+        with contextlib.ExitStack() as stack:
+            for promise in op.promises:
+                stack.enter_context(
+                    circuit.if_test((promise.index, int(not promise.inverse)))
+                )
             circuit.append(op.qiskit_instruction, [q.index for q in op.qubits])
-        for bit in op.qubits+op.promises:
-            bit.op_pointer += 1
 
 
 def _construct_circuit(promises):
     """
-    Compile quantum circuit needed to fulfil QubitPromise values.
+    Compile quantum circuit needed to fulfil BitPromise values.
     """
     # TODO: unit test
     bits = _get_bits_from_promises(promises)
     qubits = [b for b in bits if isinstance(b, Qubit)]
-    promises = [p for p in bits if isinstance(p, QubitPromise)]
+    promises = [p for p in bits if isinstance(p, BitPromise)]
     for index, qubit in enumerate(qubits):
         qubit.index = index  # Map qupython.Qubit to circuit qubit
         qubit.op_pointer = 0  # To keep track of compiled operations
     for index, promise in enumerate(promises):
         promise.index = index  # Map promise to circuit clbit
         promise.op_pointer = 0
```

### Comparing `qupython-0.0.1/qupython/err_msg.py` & `qupython-0.1.0/qupython/err_msg.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Experimental extra-long error messages
 # fmt: off
 
 from textwrap import dedent
 
 ERR_MSG = {
-  "QubitPromiseNotResolved":
+  "BitPromiseNotResolved":
   """
-  You can't cast QubitPromise to a bool until it's resolved.
+  You can't cast BitPromise to a bool until it's resolved.
 
-  You're trying to cast a QubitPromise (the output of .measure()) to a bool,
-  but QubitPromises don't have a value until after the function completes.
+  You're trying to cast a BitPromise (the output of .measure()) to a bool, but
+  BitPromise objects don't have a value until after the function completes.
 
     @quantum
     def random_action():
         a = Qubit()
         if a.measure():  # Problem
             do_thing()
         return
@@ -24,15 +24,15 @@
     def random_bit():
         a = Qubit()
         return a.measure()
 
     if random_bit():
         do_thing()
 
-  There is an exception to this: The quPython compiler recognises QubitPromise
+  There is an exception to this: The quPython compiler recognises BitPromise
   objects that condition qubit gates, so you can do the following.
 
     a, b = Qubit(), Qubit()
     # Measure one qubit and condition X-gate on measurement result
     promise = a.measure()
     b.x(conditions=[promise])
   """,
@@ -64,18 +64,18 @@
   Compilation and execution happens when the @quantum function completes, so
   quPython raises this message to prevent you from accidentally handling
   compiled Qubit objects.
   """,
 
   "CantSearchObjectForPromises":
   """
-  Can't search through object {obj} for QubitPromises.
+  Can't search through object {obj} for BitPromise objects.
 
   When a @quantum function returns something, quPython intercepts it and
-  searches for any QubitPromise objects. It then compiles and executes the
+  searches for any BitPromise objects. It then compiles and executes the
   quantum program needed to fulfil these promises.
 
   For some reason, quPython can't search the object(s) you're returning.
   Consider returning a different data structure, or raising a bug report if you
   belive this object should be searchable.
   """,
```

### Comparing `qupython-0.0.1/qupython/function.py` & `qupython-0.1.0/qupython/function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Class for @quantum functions
 
 import qiskit
 from qiskit_aer.primitives import Sampler
-from .qubit import QubitPromise, quPythonInstruction, quPythonMeasurement
+from .qubit import quPythonInstruction, quPythonMeasurement
 from .construction import _get_promises, _construct_circuit
 from .err_msg import ERR_MSG
 
 
 class quPythonFunctionError(Exception):
     pass
```

### Comparing `qupython-0.0.1/qupython/qubit.py` & `qupython-0.1.0/qupython/qubit.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,113 +1,112 @@
 import qiskit.circuit.library as clib
 from .err_msg import ERR_MSG
 
 
-class QubitPromiseNotResolvedError(Exception):
+class BitPromiseNotResolvedError(Exception):
     pass
 
 class _Bit:
     operations: list
 
-    def get_linked_bits(self, already_found=set()):
+    def get_linked_bits(self, already_found=None):
         # TODO: unit test
-        # TODO: neaten up
-        # TODO: optimize
-        linked_bits = already_found.copy() or set([self])
-        for op in self.operations:
-            linked_bits |= set(op.qubits)
-            linked_bits |= set(op.promises)
-
-        new_bits = linked_bits - already_found
-        while new_bits:
-            for bit in new_bits.copy():
-                new_bits |= bit.get_linked_bits(already_found=linked_bits)
-            new_bits = new_bits - linked_bits
-            linked_bits |= new_bits
-        return linked_bits
+        searched_bits = set()
+        all_known_bits = { self }
+        while len(searched_bits) < len(all_known_bits):
+            for bit in (all_known_bits - searched_bits):
+                for op in bit.operations:
+                    all_known_bits |= set(op.qubits + op.promises)
+                searched_bits.add(bit)
+        return all_known_bits
 
 
-class QubitPromise(_Bit):
+class BitPromise(_Bit):
     """
     Placeholder for qubit measurement results.
 
     Each promise belongs to exactly one measurement instruction. At the end of
     a `@quantum` function, quPython executes the circuit needed to fulfil any
     returned promises.
 
-    After the values are determined, a `QubitPromise` tries to behave as much
+    After the values are determined, a `BitPromise` tries to behave as much
     like a `bool` as possible. Unfortunately, there are some quirks because
-    `QubitPromises` need to have unique hashes before circuit compilation, but
-    `bool`s all have the same hash (0 or 1) and you can't change an object's
-    hash without breaking basic Python functionality. The following code
-    snippet shows an example.
+    `BitPromise` objects need to have unique hashes before circuit compilation,
+    but `bool`s all have the same hash (0 or 1) and you can't change an
+    object's hash without breaking basic Python functionality. The following
+    code snippet shows an example.
 
     ```
     # Create fulfilled qubit promise
-    promise = QubitPromise(None)
+    promise = BitPromise(None)
     promise.value = True
 
     # Show unexpected behavior
     promise == True  # True
     promise in (True, False)  # False
     ```
 
-    Currently not sure what the best behavior is. Options are:
-      * Keep it like this, and encourage users to cast to `bool` ASAP
-      * Keep like this, but have quPython return a new copy of the data with
-        _actual_ `bool`s
-      * Something else?
+    For best results, cast to `bool` as soon as possible after the function
+    completes.
+
+    If you have better ideas on how to handle this, let me know at
+    https://github.com/frankharkins/qupython/issues/new
     """
 
     def __init__(self, measurement_instruction, inverse=False):
         self.operations = [measurement_instruction]
         self.inverse = inverse
         self.value = None
 
     def __bool__(self):
         if self.value is None:
-            raise QubitPromiseNotResolvedError(ERR_MSG["QubitPromiseNotResolved"])
+            raise BitPromiseNotResolvedError(ERR_MSG["BitPromiseNotResolved"])
         return self.value
 
+    def __int__(self):
+        return int(bool(self))
+
     def __eq__(self, other):
         if self.value is None:
             return id(self) == id(other)
         return self.value == other
 
     def __hash__(self):
         return id(self)
 
     def __repr__(self):
         if self.value is None:
-            return f"QubitPromise({self.operations})"
+            return f"BitPromise({self.operations})"
         return repr(self.value)
 
     def __invert__(self):
-        new_promise = QubitPromise(
-            self.measurement_instruction,
+        # TODO: This is a bit inefficient as it adds a new measurement each
+        # time we invert the promise
+        measurement_instruction = self.operations[0]
+        new_promise = BitPromise(
+            measurement_instruction,
             inverse= not self.inverse
         )
-        self.measurement_instruction.append(new_promise)
+        measurement_instruction.promises.append(new_promise)
         return new_promise
 
 
-
 class quPythonInstruction:
     def __init__(self, qiskit_instruction, qubits, promises=[]):
         self.qiskit_instruction = qiskit_instruction
         self.qubits = qubits
         self.promises = promises
 
     def __repr__(self):
         return f"quPythonInstruction({self.qiskit_instruction.name}, {self.qubits})"
 
 
 class quPythonMeasurement:
     def __init__(self, qubit):
-        self.promises = [QubitPromise(self)]
+        self.promises = [BitPromise(self)]
         self.qubits = [qubit]
 
 
 class Qubit(_Bit):
     def __init__(self, name=None):
         self.name = name
         self.operations = []
@@ -118,31 +117,31 @@
         raise ValueError(
             "Can't cast Qubit to bool; use `.measure()` to measure"
             " the qubit instead."
         )
 
     def _separate_conditions(self, conditions):
         qubits = [c for c in conditions if isinstance(c, Qubit)]
-        promises = [c for c in conditions if isinstance(c, QubitPromise)]
-        rest = [c for c in conditions if not isinstance(c, (Qubit, QubitPromise))]
-        return qubits, promises, rest
+        promises = [c for c in conditions if isinstance(c, BitPromise)]
+        build_time_conditions = [c for c in conditions if not isinstance(c, (Qubit, BitPromise))]
+        return qubits, promises, build_time_conditions
 
     def _create_1q_gate_methods(self):
         """
         Generate methods such as self.h, self.p, etc.
         This method runs on object initialization.
         """
 
         # TODO: unit test
         # TODO: neaten up
         def _create_method(gate):
             def add_gate(*args, **kwargs):
                 conditions = kwargs.pop("conditions", [])
-                qubits, promises, rest = self._separate_conditions(conditions)
-                if not all(rest):
+                qubits, promises, build_time_conditions = self._separate_conditions(conditions)
+                if not all(build_time_conditions):
                     return
                 qiskit_inst = gate(*args, **kwargs)
                 if qubits:
                     qiskit_inst = qiskit_inst.control(len(qubits))
                 inst = quPythonInstruction(
                     qiskit_instruction=qiskit_inst,
                     qubits=qubits + [self],
@@ -171,12 +170,12 @@
             (clib.RZGate, "rz"),
             (clib.UGate, "u"),
         ]:
             setattr(self, name, _create_method(gate))
 
     def measure(self):
         """
-        Add measure instruction to Qubit and return QubitPromise
+        Add measure instruction to Qubit and return BitPromise
         """
         inst = quPythonMeasurement(self)
         self.operations.append(inst)
         return inst.promises[0]
```

### Comparing `qupython-0.0.1/test/test_public_api.py` & `qupython-0.1.0/test/test_public_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,14 +39,25 @@
             qc = lotsa_swaps.circuit
             self.assertEqual(qc.num_qubits, n)
             self.assertEqual(
                     len(qc.data),
                     n + 3*(n//2)
             )
 
+    def test_clbit_negation(self):
+        @quantum
+        def my_fun():
+            q = Qubit().h()
+            m = q.measure()
+            q.x(conditions=[~m])
+            return q.measure()
+        for _ in range(20):
+            result = bool(my_fun())
+            self.assertEqual(result, True)
+
 class QuantumFunctionCallable(unittest.TestCase):
     def test_ordering(self):
         @quantum
         def get_bits():
             qubits = [ Qubit() for _ in range(10) ]
             qubits[0].x()
             return [ qubit.measure() for qubit in qubits ]
```

### Comparing `qupython-0.0.1/test/test_readme.py` & `qupython-0.1.0/test/test_readme.py`

 * *Files 20% similar despite different names*

```diff
@@ -42,72 +42,75 @@
         # === End code example ===
 
         function_output = random_bit()
         self.assertTrue(
             function_output == True or function_output == False
         )
 
+
         # === Begin code example ===
-        @quantum
-        def ghz(num_bits: int):
+        from qupython import Qubit, quantum
+        from qupython.typing import BitPromise
+
+        class LogicalQubit:
             """
-            Create and measure a GHZ state
+            Simple logical qubit using the five-qubit code.
+            See https://en.wikipedia.org/wiki/Five-qubit_error_correcting_code
             """
-            qubits = [ Qubit() for _ in range(num_bits) ]
-            control, targets = qubits[0], qubits[1:]
-            control.h()
-            for target in targets:
-                target.x(conditions=[control])
-            return [ qubit.measure() for qubit in qubits ]
+            def __init__(self):
+                """
+                Create new logical qubit and initialize to logical |0>.
+                Uses initialization procedure from https://quantumcomputing.stackexchange.com/a/14449
+                """
+                self.qubits = [Qubit() for _ in range(5)]
+                self.qubits[4].z()
+                for q in self.qubits[:4]:
+                    q.h()
+                    self.qubits[4].x(conditions=[q])
+                for a, b in [(0,4),(0,1),(2,3),(1,2),(3,4)]:
+                    control = self.qubits[b]
+                    self.qubits[a].z(conditions=[control])
+
+            def measure(self) -> BitPromise:
+                """
+                Measure logical qubit to single classical bit
+                """
+                out = Qubit().h()
+                for q in self.qubits:
+                    q.z(conditions=[out])
+                return out.h().measure()
         # === End code example ===
 
-        for _ in range(10):
-            result = ghz(10)
-            self.assertTrue(
-                all(result) or all(not r for r in result)
-            )
-
         # === Begin code example ===
-        class BellPair:
-            def __init__(self):
-                self.left = Qubit().h()
-                self.right = Qubit().x(conditions=[self.left])
-
         @quantum
-        def teleportation_demo():
-            message = Qubit()
-
-            bell_pair = BellPair()
-            do_x = bell_pair.left.x(conditions=[message]).measure()
-            do_z = message.h().measure()
-
-            bell_pair.right.x(conditions=[do_x]).z(conditions=[do_z])
-            return bell_pair.right.measure()
+        def logical_qubit_demo() -> BitPromise:
+            q = LogicalQubit()
+            return q.measure()
         # === End code example ===
 
         for _ in range(15):
             self.assertFalse(
-                teleportation_demo()
+                logical_qubit_demo()
             )
 
         # === Begin code example ===
         # Compile using quPython
-        teleportation_demo.compile()
+        logical_qubit_demo.compile()
 
         # Draw compiled Qiskit circuit
-        teleportation_demo.circuit.draw()
+        logical_qubit_demo.circuit.draw()
         # === End code example ===
 
         self.assertIsInstance(
-            teleportation_demo.circuit,
+            logical_qubit_demo.circuit,
             qiskit.QuantumCircuit
         )
 
         # === Begin code example ===
         from qiskit_aer.primitives import Sampler
-        qiskit_result = Sampler().run(teleportation_demo.circuit).result()
-        teleportation_demo.interpret_result(qiskit_result)  # returns `False`
+        qiskit_result = Sampler().run(logical_qubit_demo.circuit).result()
+        logical_qubit_demo.interpret_result(qiskit_result)  # returns `False`
         # === End code example ===
 
         self.assertFalse(
-            teleportation_demo.interpret_result(qiskit_result)
+            logical_qubit_demo.interpret_result(qiskit_result)
         )
```

