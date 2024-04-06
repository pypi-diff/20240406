# Comparing `tmp/phasegen-0.0.3b0.tar.gz` & `tmp/phasegen-0.0.4b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phasegen-0.0.3b0.tar", max compression
+gzip compressed data, was "phasegen-0.0.4b0.tar", max compression
```

## Comparing `phasegen-0.0.3b0.tar` & `phasegen-0.0.4b0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      726 2024-04-06 17:13:58.155945 phasegen-0.0.3b0/README.md
--rw-r--r--   0        0        0     4631 2024-04-06 17:13:58.167945 phasegen-0.0.3b0/phasegen/__init__.py
--rw-r--r--   0        0        0    15046 2024-04-06 17:13:58.167945 phasegen-0.0.3b0/phasegen/coalescent_models.py
--rw-r--r--   0        0        0    14599 2024-04-06 17:13:58.167945 phasegen-0.0.3b0/phasegen/comparison.py
--rw-r--r--   0        0        0    37008 2024-04-06 17:13:58.167945 phasegen-0.0.3b0/phasegen/demography.py
--rw-r--r--   0        0        0    93405 2024-04-06 17:13:58.167945 phasegen-0.0.3b0/phasegen/distributions.py
--rw-r--r--   0        0        0     1601 2024-04-06 17:13:58.167945 phasegen-0.0.3b0/phasegen/expm.py
--rw-r--r--   0        0        0    25126 2024-04-06 17:13:58.167945 phasegen-0.0.3b0/phasegen/inference.py
--rw-r--r--   0        0        0     2378 2024-04-06 17:13:58.167945 phasegen-0.0.3b0/phasegen/lineage.py
--rw-r--r--   0        0        0     2745 2024-04-06 17:13:58.167945 phasegen-0.0.3b0/phasegen/locus.py
--rw-r--r--   0        0        0     2653 2024-04-06 17:13:58.167945 phasegen-0.0.3b0/phasegen/norms.py
--rw-r--r--   0        0        0    16983 2024-04-06 17:13:58.171945 phasegen-0.0.3b0/phasegen/rewards.py
--rw-r--r--   0        0        0     1121 2024-04-06 17:13:58.171945 phasegen-0.0.3b0/phasegen/serialization.py
--rw-r--r--   0        0        0    11098 2024-04-06 17:13:58.171945 phasegen-0.0.3b0/phasegen/spectrum.py
--rw-r--r--   0        0        0    29122 2024-04-06 17:13:58.171945 phasegen-0.0.3b0/phasegen/state_space.py
--rw-r--r--   0        0        0    53272 2024-04-06 17:13:58.171945 phasegen-0.0.3b0/phasegen/state_space_old.py
--rw-r--r--   0        0        0     1230 2024-04-06 17:13:58.171945 phasegen-0.0.3b0/phasegen/utils.py
--rw-r--r--   0        0        0     4478 2024-04-06 17:13:58.171945 phasegen-0.0.3b0/phasegen/visualization.py
--rw-r--r--   0        0        0      931 2024-04-06 17:13:58.171945 phasegen-0.0.3b0/pyproject.toml
--rw-r--r--   0        0        0     1744 1970-01-01 00:00:00.000000 phasegen-0.0.3b0/PKG-INFO
+-rw-r--r--   0        0        0      725 2024-04-06 17:31:18.139292 phasegen-0.0.4b0/README.md
+-rw-r--r--   0        0        0     4631 2024-04-06 17:31:18.151292 phasegen-0.0.4b0/phasegen/__init__.py
+-rw-r--r--   0        0        0    15046 2024-04-06 17:31:18.151292 phasegen-0.0.4b0/phasegen/coalescent_models.py
+-rw-r--r--   0        0        0    14599 2024-04-06 17:31:18.151292 phasegen-0.0.4b0/phasegen/comparison.py
+-rw-r--r--   0        0        0    37008 2024-04-06 17:31:18.151292 phasegen-0.0.4b0/phasegen/demography.py
+-rw-r--r--   0        0        0    93421 2024-04-06 17:31:18.151292 phasegen-0.0.4b0/phasegen/distributions.py
+-rw-r--r--   0        0        0     1652 2024-04-06 17:31:18.151292 phasegen-0.0.4b0/phasegen/expm.py
+-rw-r--r--   0        0        0    25126 2024-04-06 17:31:18.155292 phasegen-0.0.4b0/phasegen/inference.py
+-rw-r--r--   0        0        0     2378 2024-04-06 17:31:18.155292 phasegen-0.0.4b0/phasegen/lineage.py
+-rw-r--r--   0        0        0     2745 2024-04-06 17:31:18.155292 phasegen-0.0.4b0/phasegen/locus.py
+-rw-r--r--   0        0        0     2653 2024-04-06 17:31:18.155292 phasegen-0.0.4b0/phasegen/norms.py
+-rw-r--r--   0        0        0    16983 2024-04-06 17:31:18.155292 phasegen-0.0.4b0/phasegen/rewards.py
+-rw-r--r--   0        0        0     1121 2024-04-06 17:31:18.155292 phasegen-0.0.4b0/phasegen/serialization.py
+-rw-r--r--   0        0        0    11098 2024-04-06 17:31:18.155292 phasegen-0.0.4b0/phasegen/spectrum.py
+-rw-r--r--   0        0        0    29122 2024-04-06 17:31:18.155292 phasegen-0.0.4b0/phasegen/state_space.py
+-rw-r--r--   0        0        0    53272 2024-04-06 17:31:18.155292 phasegen-0.0.4b0/phasegen/state_space_old.py
+-rw-r--r--   0        0        0     1230 2024-04-06 17:31:18.155292 phasegen-0.0.4b0/phasegen/utils.py
+-rw-r--r--   0        0        0     4478 2024-04-06 17:31:18.155292 phasegen-0.0.4b0/phasegen/visualization.py
+-rw-r--r--   0        0        0      931 2024-04-06 17:31:18.155292 phasegen-0.0.4b0/pyproject.toml
+-rw-r--r--   0        0        0     1743 1970-01-01 00:00:00.000000 phasegen-0.0.4b0/PKG-INFO
```

### Comparing `phasegen-0.0.3b0/README.md` & `phasegen-0.0.4b0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # PhaseGen  <img align="right" width="100" src="https://raw.githubusercontent.com/Sendrowski/PhaseGen/master/docs/logo.png">
 
 [![Documentation Status](https://readthedocs.org/projects/phasegen/badge/?version=latest)](https://phasegen.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/phasegen.svg)](https://badge.fury.io/py/phasegen)
 
 
-``phasegen`` is a package for simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios. It used phase-type theory do so. ``phasegen`` supports a wide range of demographic models and coalescent tree statistics.
+``phasegen`` is a package for simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios. ``phasegen`` leverages phase-type theory and supports a wide range of demographic models and coalescent tree statistics.
 
 Please see the [documentation](https://phasegen.readthedocs.io/en/latest/) for all the details.
```

### Comparing `phasegen-0.0.3b0/phasegen/__init__.py` & `phasegen-0.0.4b0/phasegen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 PhaseGen package.
 """
 
 __author__ = "Janek Sendrowski"
 __contact__ = "sendrowski.janek@gmail.com"
 __date__ = "2023-04-09"
 
-__version__ = '0.0.3-beta'
+__version__ = '0.0.4-beta'
 
 import logging
 import os
 import sys
 
 import jsonpickle.ext.numpy as jsonpickle_numpy
 from tqdm import tqdm
```

### Comparing `phasegen-0.0.3b0/phasegen/coalescent_models.py` & `phasegen-0.0.4b0/phasegen/coalescent_models.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/comparison.py` & `phasegen-0.0.4b0/phasegen/comparison.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/demography.py` & `phasegen-0.0.4b0/phasegen/demography.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/distributions.py` & `phasegen-0.0.4b0/phasegen/distributions.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from abc import ABC, abstractmethod
 from collections.abc import Mapping
 from functools import cached_property, cache
 from math import factorial
 from typing import Generator, List, Callable, Tuple, Dict, Collection, Iterable, Iterator
 
 import numpy as np
-import tskit
 from numpy.polynomial.hermite_e import HermiteE
 from scipy import special
 from scipy.ndimage import gaussian_filter1d
 from scipy.stats import norm
 
 from .coalescent_models import StandardCoalescent, CoalescentModel, BetaCoalescent, DiracCoalescent
 from .demography import Demography, PopSizeChanges
@@ -2441,14 +2440,15 @@
             """
             Simulate statistics.
 
             :param _:
             :return: Statistics.
             """
             import msprime as ms
+            import tskit
 
             # simulate trees
             g: Generator = ms.sim_ancestry(
                 sequence_length=self.locus_config.n,
                 recombination_rate=self.locus_config.recombination_rate,
                 samples=samples,
                 num_replicates=num_replicates,
@@ -2550,15 +2550,15 @@
             desc="Simulating trees"
         ))
 
         # store results
         self.heights, self.total_branch_lengths, self.sfs_counts = res[0].T, res[1].T, res[2:].T
 
     @staticmethod
-    def _expand_trees(ts: tskit.TreeSequence) -> Iterator[tskit.Tree]:
+    def _expand_trees(ts: 'tskit.TreeSequence') -> Iterator['tskit.Tree']:
         """
         Expand tree sequence to `n` trees where `n` is the number of loci.
 
         :param ts: Tree sequence.
         :return: List of trees.
         """
         for tree in ts.trees():
```

### Comparing `phasegen-0.0.3b0/phasegen/expm.py` & `phasegen-0.0.4b0/phasegen/expm.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,16 +53,17 @@
         :return: Matrix exponential
         """
         return scipy.linalg.expm(m)
 
 
 class Backend(ABC):
     """
-    Base class for backends.
+    Backend for matrix exponentiation.
     """
+    #: Backend for matrix exponentiation
     backend: MatrixExponentiation = SciPyExpm
 
     @classmethod
     @abstractmethod
     def expm(cls, m: np.ndarray) -> np.ndarray:
         """
         Compute the matrix exponential.
```

### Comparing `phasegen-0.0.3b0/phasegen/inference.py` & `phasegen-0.0.4b0/phasegen/inference.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/lineage.py` & `phasegen-0.0.4b0/phasegen/lineage.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/locus.py` & `phasegen-0.0.4b0/phasegen/locus.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/norms.py` & `phasegen-0.0.4b0/phasegen/norms.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/rewards.py` & `phasegen-0.0.4b0/phasegen/rewards.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/serialization.py` & `phasegen-0.0.4b0/phasegen/serialization.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/spectrum.py` & `phasegen-0.0.4b0/phasegen/spectrum.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/state_space.py` & `phasegen-0.0.4b0/phasegen/state_space.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/state_space_old.py` & `phasegen-0.0.4b0/phasegen/state_space_old.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/utils.py` & `phasegen-0.0.4b0/phasegen/utils.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/phasegen/visualization.py` & `phasegen-0.0.4b0/phasegen/visualization.py`

 * *Files identical despite different names*

### Comparing `phasegen-0.0.3b0/pyproject.toml` & `phasegen-0.0.4b0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "phasegen"
-version = "0.0.3-beta"
+version = "0.0.4-beta"
 description = "Simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios."
 authors = ["Sendrowski <sendrowski.janek@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
```

### Comparing `phasegen-0.0.3b0/PKG-INFO` & `phasegen-0.0.4b0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phasegen
-Version: 0.0.3b0
+Version: 0.0.4b0
 Summary: Simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios.
 License: MIT
 Author: Sendrowski
 Author-email: sendrowski.janek@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,11 +26,11 @@
 
 # PhaseGen  <img align="right" width="100" src="https://raw.githubusercontent.com/Sendrowski/PhaseGen/master/docs/logo.png">
 
 [![Documentation Status](https://readthedocs.org/projects/phasegen/badge/?version=latest)](https://phasegen.readthedocs.io/en/latest/?badge=latest)
 [![PyPI version](https://badge.fury.io/py/phasegen.svg)](https://badge.fury.io/py/phasegen)
 
 
-``phasegen`` is a package for simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios. It used phase-type theory do so. ``phasegen`` supports a wide range of demographic models and coalescent tree statistics.
+``phasegen`` is a package for simulation and inference on exact solutions of coalescent distributions under diverse demographic scenarios. ``phasegen`` leverages phase-type theory and supports a wide range of demographic models and coalescent tree statistics.
 
 Please see the [documentation](https://phasegen.readthedocs.io/en/latest/) for all the details.
```

