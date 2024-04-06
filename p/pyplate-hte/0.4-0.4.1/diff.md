# Comparing `tmp/pyplate-hte-0.4.tar.gz` & `tmp/pyplate-hte-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyplate-hte-0.4.tar", last modified: Tue Apr  2 16:58:44 2024, max compression
+gzip compressed data, was "pyplate-hte-0.4.1.tar", last modified: Sat Apr  6 16:12:44 2024, max compression
```

## Comparing `pyplate-hte-0.4.tar` & `pyplate-hte-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-02 16:58:44.520273 pyplate-hte-0.4/
--rw-r--r--   0 marvinj    (502) staff       (20)    10945 2024-02-29 20:48:18.000000 pyplate-hte-0.4/LICENSE.txt
--rw-r--r--   0 marvinj    (502) staff       (20)    15332 2024-04-02 16:58:44.518910 pyplate-hte-0.4/PKG-INFO
--rw-r--r--   0 marvinj    (502) staff       (20)     2582 2024-04-02 16:53:28.000000 pyplate-hte-0.4/README.md
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-02 16:58:44.429279 pyplate-hte-0.4/pyplate/
--rw-r--r--   0 marvinj    (502) staff       (20)     1531 2024-04-02 16:53:28.000000 pyplate-hte-0.4/pyplate/__init__.py
--rw-r--r--   0 marvinj    (502) staff       (20)    13085 2024-02-29 20:48:18.000000 pyplate-hte-0.4/pyplate/experiment_design.py
--rw-r--r--   0 marvinj    (502) staff       (20)   105779 2024-04-02 16:53:28.000000 pyplate-hte-0.4/pyplate/pyplate.py
--rw-r--r--   0 marvinj    (502) staff       (20)      815 2024-04-02 16:53:28.000000 pyplate-hte-0.4/pyplate/pyplate.yaml
--rw-r--r--   0 marvinj    (502) staff       (20)    14316 2024-02-29 20:48:18.000000 pyplate-hte-0.4/pyplate/slicer.py
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-02 16:58:44.517501 pyplate-hte-0.4/pyplate_hte.egg-info/
--rw-r--r--   0 marvinj    (502) staff       (20)    15332 2024-04-02 16:58:44.000000 pyplate-hte-0.4/pyplate_hte.egg-info/PKG-INFO
--rw-r--r--   0 marvinj    (502) staff       (20)      668 2024-04-02 16:58:44.000000 pyplate-hte-0.4/pyplate_hte.egg-info/SOURCES.txt
--rw-r--r--   0 marvinj    (502) staff       (20)        1 2024-04-02 16:58:44.000000 pyplate-hte-0.4/pyplate_hte.egg-info/dependency_links.txt
--rw-r--r--   0 marvinj    (502) staff       (20)       20 2024-04-02 16:58:44.000000 pyplate-hte-0.4/pyplate_hte.egg-info/requires.txt
--rw-r--r--   0 marvinj    (502) staff       (20)        8 2024-04-02 16:58:44.000000 pyplate-hte-0.4/pyplate_hte.egg-info/top_level.txt
--rw-r--r--   0 marvinj    (502) staff       (20)      687 2024-04-02 16:53:28.000000 pyplate-hte-0.4/pyproject.toml
--rw-r--r--   0 marvinj    (502) staff       (20)       38 2024-04-02 16:58:44.520513 pyplate-hte-0.4/setup.cfg
-drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-02 16:58:44.515740 pyplate-hte-0.4/tests/
--rw-r--r--   0 marvinj    (502) staff       (20)    10643 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_Container.py
--rw-r--r--   0 marvinj    (502) staff       (20)     1975 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_Experiment.py
--rw-r--r--   0 marvinj    (502) staff       (20)     6029 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_ExperimentalSpace.py
--rw-r--r--   0 marvinj    (502) staff       (20)      987 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_Factor.py
--rw-r--r--   0 marvinj    (502) staff       (20)     5193 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_Plate.py
--rw-r--r--   0 marvinj    (502) staff       (20)     6666 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_Recipe.py
--rw-r--r--   0 marvinj    (502) staff       (20)     6292 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_Slicer.py
--rw-r--r--   0 marvinj    (502) staff       (20)     3477 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_Substance.py
--rw-r--r--   0 marvinj    (502) staff       (20)     2827 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_convert.py
--rw-r--r--   0 marvinj    (502) staff       (20)     3702 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_create_solution.py
--rw-r--r--   0 marvinj    (502) staff       (20)     1340 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_dilute.py
--rw-r--r--   0 marvinj    (502) staff       (20)    24056 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_recipe_amount_used.py
--rw-r--r--   0 marvinj    (502) staff       (20)    10202 2024-04-02 16:53:28.000000 pyplate-hte-0.4/tests/test_recipe_volume_used.py
--rw-r--r--   0 marvinj    (502) staff       (20)     5701 2024-02-29 20:48:18.000000 pyplate-hte-0.4/tests/test_transfers.py
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-06 16:12:44.267452 pyplate-hte-0.4.1/
+-rw-r--r--   0 marvinj    (502) staff       (20)    10945 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/LICENSE.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)    15334 2024-04-06 16:12:44.266542 pyplate-hte-0.4.1/PKG-INFO
+-rw-r--r--   0 marvinj    (502) staff       (20)     2582 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/README.md
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-06 16:12:44.231970 pyplate-hte-0.4.1/pyplate/
+-rw-r--r--   0 marvinj    (502) staff       (20)     1768 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/pyplate/__init__.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    12603 2024-04-06 15:54:04.000000 pyplate-hte-0.4.1/pyplate/experiment_design.py
+-rw-r--r--   0 marvinj    (502) staff       (20)   108858 2024-04-06 15:54:04.000000 pyplate-hte-0.4.1/pyplate/pyplate.py
+-rw-r--r--   0 marvinj    (502) staff       (20)      860 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/pyplate/pyplate.yaml
+-rw-r--r--   0 marvinj    (502) staff       (20)    14316 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/pyplate/slicer.py
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-06 16:12:44.265408 pyplate-hte-0.4.1/pyplate_hte.egg-info/
+-rw-r--r--   0 marvinj    (502) staff       (20)    15334 2024-04-06 16:12:44.000000 pyplate-hte-0.4.1/pyplate_hte.egg-info/PKG-INFO
+-rw-r--r--   0 marvinj    (502) staff       (20)      668 2024-04-06 16:12:44.000000 pyplate-hte-0.4.1/pyplate_hte.egg-info/SOURCES.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)        1 2024-04-06 16:12:44.000000 pyplate-hte-0.4.1/pyplate_hte.egg-info/dependency_links.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)       20 2024-04-06 16:12:44.000000 pyplate-hte-0.4.1/pyplate_hte.egg-info/requires.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)        8 2024-04-06 16:12:44.000000 pyplate-hte-0.4.1/pyplate_hte.egg-info/top_level.txt
+-rw-r--r--   0 marvinj    (502) staff       (20)      689 2024-04-06 16:11:48.000000 pyplate-hte-0.4.1/pyproject.toml
+-rw-r--r--   0 marvinj    (502) staff       (20)       38 2024-04-06 16:12:44.267587 pyplate-hte-0.4.1/setup.cfg
+drwxr-xr-x   0 marvinj    (502) staff       (20)        0 2024-04-06 16:12:44.264119 pyplate-hte-0.4.1/tests/
+-rw-r--r--   0 marvinj    (502) staff       (20)    10740 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Container.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     1975 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Experiment.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     6029 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_ExperimentalSpace.py
+-rw-r--r--   0 marvinj    (502) staff       (20)      987 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Factor.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     5325 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Plate.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     6607 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Recipe.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     6292 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Slicer.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     3477 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_Substance.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     2827 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_convert.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     3762 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_create_solution.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     1352 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_dilute.py
+-rw-r--r--   0 marvinj    (502) staff       (20)    25879 2024-04-06 15:54:04.000000 pyplate-hte-0.4.1/tests/test_recipe_amount_used.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     1392 2024-04-06 15:54:04.000000 pyplate-hte-0.4.1/tests/test_recipe_volume_used.py
+-rw-r--r--   0 marvinj    (502) staff       (20)     5796 2024-04-06 15:39:49.000000 pyplate-hte-0.4.1/tests/test_transfers.py
```

### Comparing `pyplate-hte-0.4/LICENSE.txt` & `pyplate-hte-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4/PKG-INFO` & `pyplate-hte-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplate-hte
-Version: 0.4
+Version: 0.4.1
 Summary: A Python tool for designing chemistry experiments in plate format
 Author: Eugene Kwan and James Marvin
 Author-email: ekwan16@gmail.com
 License:   				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pyplate-hte-0.4/README.md` & `pyplate-hte-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4/pyplate/__init__.py` & `pyplate-hte-0.4.1/pyplate/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,21 +20,27 @@
         try:
             with file_path.open('r') as config_file:
                 yaml_config = yaml.safe_load(config_file)
         except yaml.YAMLError as exc:
             raise RuntimeError("Config file could not be read.") from exc
 
         self.internal_precision = yaml_config['internal_precision']
-        self.moles_prefix = yaml_config['moles_storage']
-        assert self.moles_prefix[1:] == 'mol'
-        self.volume_prefix = yaml_config['volume_storage']
-        assert self.volume_prefix[1:] == 'L'
-        self.default_density = float(yaml_config['default_density'])
+        self.moles_storage_unit = yaml_config['moles_storage_unit']
+        assert self.moles_storage_unit[-3:] == 'mol'
+        self.moles_display_unit = yaml_config['moles_display_unit']
+        assert self.moles_display_unit[-3:] == 'mol'
+        self.volume_storage_unit = yaml_config['volume_storage_unit']
+        assert self.volume_storage_unit[-1] == 'L'
+        self.volume_display_unit = yaml_config['volume_display_unit']
+        assert self.volume_display_unit[-1] == 'L'
+
+        self.default_solid_density = float(yaml_config['default_solid_density'])
+        self.default_enzyme_density = float(yaml_config['default_enzyme_density'])
         self.default_weight_volume_units = yaml_config['default_weight_volume_units']
-        self.default_moles_unit = yaml_config['default_moles_unit']
-        self.default_volume_unit = yaml_config['default_volume_unit']
+
+
         self.default_colormap = yaml_config['default_colormap']
         self.default_diverging_colormap = yaml_config['default_diverging_colormap']
         self.precisions = yaml_config['precisions']
 
 
 from .pyplate import Substance, Container, Plate, Recipe
```

### Comparing `pyplate-hte-0.4/pyplate/experiment_design.py` & `pyplate-hte-0.4.1/pyplate/experiment_design.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,101 +1,109 @@
-from typing import Union, Optional, List
+from typing import Union, Optional, List, Callable
 
 from pyplate import Substance, Container
 import itertools
 
 
 class Factor:
     """"
-    A factor is a variable that is under the control of the experimenter.
-    It has a name (must be unique to a given experimental space), a list
-    of possible values, and a verifier function.
-    verifier takes a well object and a desired value and returns True if
-    the well is consistent with the description.
+    A factor is a variable that is under the control of the experimenter. It has a name (must be unique to a given
+    experimental space) and a list of possible values.
 
     :param name: The name of the factor
     :type name: str
     :param possible_values: A list of possible values for the factor
     :type possible_values: list[str | Substance]
-    :param verifier: A function that takes a well and a value and returns True if the well is consistent with the value
-    :type verifier: callable
     """
 
-    name: str
-    possible_values: list[str | Substance]
-    verifier: callable
-
-    def __init__(self, name: str, possible_values: list[str | Substance], verifier: callable):
+    def __init__(self, name: str, possible_values: list[str | Substance | float | int]):
         self.name = name
         self.possible_values = possible_values
-        self.verifier = verifier
+
+    def get_level_factory(self):
+        non_null_level = next(value for value in self.possible_values if value is not None)
+        if isinstance(non_null_level, tuple):
+            if isinstance(non_null_level[0], Substance) and isinstance(non_null_level[1], float | int):
+                def get_level(container):
+                    for substance, amount in filter(None, self.possible_values):
+                        if container.contents[substance] == amount:
+                            return substance, amount
+                    return "Factor not found"
+
+                return get_level
+        elif isinstance(non_null_level, Substance):
+            def get_level(container):
+                for substance in filter(None, self.possible_values):
+                    if substance in container.contents:
+                        return substance
+                return "Factor not found"
+
+            return get_level
+        else:
+            def get_level(container):
+                return container.experimental_conditions.get(self.name, "Factor not found")
+
+            return get_level
 
     def __repr__(self):
-        return f"Factor({self.name}, {self.possible_values}, {self.verifier})"
+        return f"Factor({self.name}, {self.possible_values})"
 
     def __str__(self):
         return f"Factor: {self.name} with possible values {self.possible_values}"
 
     def __eq__(self, other):
         return (self.name == other.name
-                and self.possible_values == other.possible_values
-                and self.verifier == other.verifier)
+                and self.possible_values == other.possible_values)
 
     def __hash__(self):
-        return hash((self.name, tuple(self.possible_values), self.verifier))
+        return hash((self.name, tuple(self.possible_values)))
 
 
 class Experiment:
     """
-    An experiment represents a single experiment within an experimental space. It has
-    a dictionary of factors and their values. It's experiment_id is a unique identifier
-    for the experiment within the experimental space. The replicate_idx distinguishes
-    between multiple replicates of the same experiment. The well object is a reference
-    to the well in which the experiment was performed.
-
-    :param factors: A dictionary of factors and their values
-    :type factors: dict
-    :param experiment_id: A unique identifier for the experiment within the experimental space
-    :type experiment_id: int
-    :param replicate_idx: A unique identifier for the replicate of the experiment
-    :type replicate_idx: int
-    :param well: A reference to the well in which the experiment was performed
-    :type well: Container
-    """
+    An Experiment represents a single experiment within an experimental space. It keeps track of Factors and their
+    desired values for a single run. Each experiment has a unique identifier, as well as a replicate identifier to
+    distinguish between Experiments conducted with the same factors in replicate. Experiments maintain a reference to the
+    Container they were performed in.
 
-    factors: dict[str, [str | Substance]]
-    experiment_id: int
-    replicate_idx: int
-    well: Optional[Container]
+    """
 
     def __init__(self, factors: dict[str, [str | Substance]], experiment_id: int, replicate_idx: int,
-                 well: Optional[Container] = None):
+                 verifier: Callable[[Container], bool], well: Optional[Container] = None):
         self.factors = factors
         self.experiment_id = experiment_id
         self.replicate_idx = replicate_idx
         self.well = well
+        self.verifier = verifier
 
-    def map_well(self, well: Container) -> None:
+    def map_container(self, well: Container) -> None:
         """
         Map the experiment to a well. This is useful for keeping track of
         which well an experiment was performed in.
 
         :param well: The well to map to
         :type well: Container
         :return: None
         """
         self.well = well
 
+    def check_well(self, well=None):
+        if well:
+            return self.verifier(well)
+        else:
+            return self.verifier(self.well)
+
     def __repr__(self):
         return f"Experiment({self.factors}, {self.experiment_id}, {self.replicate_idx}, {self.well})"
 
     def __str__(self):
         return (f"Experiment: {self.factors} "
-                f"with experiment_id {self.experiment_id} "
-                f"and replicate_idx {self.replicate_idx}")
+                f"with experiment_id {self.experiment_id}, "
+                f"replicate_idx {self.replicate_idx}, "
+                f"mapped to well {self.well}")
 
     def __getitem__(self, key):
         return self.factors[key]
 
     def __setitem__(self, key, value):
         self.factors[key] = value
 
@@ -116,33 +124,36 @@
 
     def __hash__(self):
         return hash((frozenset(self.factors.items()), self.experiment_id, self.replicate_idx, self.well))
 
 
 class ExperimentalSpace:
     """
-    An experimental space is a collection of experiments that share the same factors.
-    It a list of factors, a list of blocks, and a list of all experiments. The blocks
-    allow for grouping of experiments with similar fixed factors.
+An experimental space is a collection of experiments that share the same factors. Experiments within a space may be
+blocked together based on their factors use.
 
     :param factors: A set of factors that define the experimental space
     :type factors: set[Factor]
     :param experiment_id_generator: A function that generates unique experiment ids
     :type experiment_id_generator: callable
     """
 
     factors: set[Factor]
     blocks: list[Experiment]
-    experiments: list[Experiment]
+    experiments: dict[tuple[str, float | str | Substance], Experiment]
     blocks: Optional[list[Experiment]]
     experiments: Optional[list[Experiment]]
 
-    def __init__(self, factors: set[Factor], experiment_id_generator: callable):
-        self.factors = factors
+    def __init__(self, factors: set[Factor], experiment_id_generator: Callable,
+                 factor_rules: Callable[[Experiment], bool]):
+        self.factors = set()
+        for factor in factors:
+            self.register_factor(factor)
         self.experiment_id_generator = experiment_id_generator
+        self.factor_rules = factor_rules
         self.blocks = None
         self.experiments = None
 
     def register_factor(self, factor: Factor) -> None:
         """
         Register a factor with the experimental space. Ensures that factor
         names are unique.
@@ -161,52 +172,57 @@
         adding experiments without `generate_experiments`.
 
         :param experiment: The experiment to add
         :type experiment: Experiment
         :return: None
         """
         if not self.experiments:
-            self.experiments = []
+            self.experiments = {}
         if experiment.factors.keys() != {x.name for x in self.factors}:
             raise ValueError(f"Experiment factors {experiment.factors.keys()}"
                              f" do not match experimental space factors {self.factors}")
         for factor_name in experiment.factors:
-            factor_object = self.get_registered_factor(factor_name)
+            factor_object = self.get_factor(factor_name)
             if experiment[factor_name] not in factor_object.possible_values:
                 raise ValueError(f"Experiment factor {factor_name} value {experiment[factor_name]}"
                                  f" not in possible values {factor_object.possible_values}")
-        self.experiments.append(experiment)
+        if not self.factor_rules(experiment):
+            raise ValueError(f"Experiment does not satisfy factor rules, make sure you don't have any conflicting "
+                             f"factors.")
+        factor_combination = sorted(experiment.factors.items())
+        self.experiments[factor_combination] = experiment
 
     def filter_experiments(self, filter_function: callable) -> None:
         """
         Filter the experiments in the experimental space. This is useful for
         removing experiments that do not meet certain criteria.
 
         :param filter_function: A function that takes an experiment and returns True if it should be kept
         :type filter_function: callable
         :return: None
         """
         self.experiments = [x for x in self.experiments if filter_function(x)]
 
-    def get_registered_factor(self, factor_name) -> Factor:
+    def get_factor(self, factor_name) -> Factor:
         """
         Get a registered factor by name.
 
         :param factor_name: The name of the factor to get
         :type factor_name: str
         :return: The factor object
         :rtype: Factor
         """
         for factor in self.factors:
             if factor.name == factor_name:
                 return factor
         raise ValueError(f"Factor {factor_name} not found in experimental space")
 
     def generate_experiments(self, factors: dict[str, [str | Substance]],
-                             n_replicates: int, blocking_factors: list[str]) -> list[list[Experiment]]:
+                             n_replicates: int, blocking_factors: list[str],
+                             experiment_verifier: Callable[[Container], bool]) -> list[list[Experiment]]:
         """
         Generate experiments for the experimental space. This is useful for
         generating a full factorial design of a subset of the experimental space.
 
         :param factors: A list of factors to generate experiments for (must be a subset of the experimental space factors)
         :type factors: dict[str, [str | Substance]]
         :param n_replicates: The number of replicates to generate for each experiment
@@ -216,16 +232,17 @@
         :return: A list of blocks, where each block is a list of experiments
         """
         filtered_factors = {}
         for factor in self.factors:
             if factors[factor.name] == "all":
                 filtered_factors[factor.name] = factor.possible_values
             else:
-                filtered_factors[factor.name] = [value for value in factor.possible_values if value in factors[factor.name]]
-        
+                filtered_factors[factor.name] = [value for value in factor.possible_values if
+                                                 value in factors[factor.name]]
+
         # Initialize blocks
         blocks = {}
 
         """
         The following lines return a list of tuples shown below, assuming you block on Factor 1 and Factor 2:
         [
             [
@@ -244,75 +261,46 @@
 
         # If needed form blocking combinations
         blocking_combinations = list(itertools.product(*[filtered_factors[name] for name in blocking_factors]))
 
         # Iterate over each combination of blocking factors
         for block_combination in blocking_combinations:
             block = []
-            
+
             # Filter out the current blocking factors and create combinations of other factors
-            non_blocking_factors = {name: values for name, values in filtered_factors.items() if name not in blocking_factors}
+            non_blocking_factors = {name: values for name, values in filtered_factors.items() if
+                                    name not in blocking_factors}
             other_combinations = list(itertools.product(*non_blocking_factors.values()))
 
             # Generate experiments for each combination
             for comb in other_combinations:
                 factors_dict = dict(zip(non_blocking_factors.keys(), comb))
-                
+
                 # Set the values of the blocking factors
                 for bf, value in zip(blocking_factors, block_combination):
                     factors_dict[bf] = value
 
                 # Create replicates for each unique combination
                 for rep in range(n_replicates):
-                    experiment = Experiment(factors=factors_dict, replicate_idx=rep+1, experiment_id=self.experiment_id_generator())
-                    block.append(experiment)
+                    experiment = Experiment(factors=factors_dict, replicate_idx=rep + 1,
+                                            experiment_id=self.experiment_id_generator(), verifier=experiment_verifier)
+                    if self.factor_rules(experiment):
+                        block.append(experiment)
+                        factor_key = sorted(factors_dict.items())
+                        self.experiments[factor_key] = experiment
 
             # Use the blocking factor combination as the key for the blocks dictionary
             blocks[block_combination] = block
 
         return blocks
-    
-        #Another implementation
-        # experiment_factor_values = {}
-        # for factor in self.factors:
-        #     if factors[factor.name] == "all":
-        #         experiment_factor_values[factor.name] = factor.possible_values
-        #     else:
-        #         experiment_factor_values[factor.name] = [value for value in factor.possible_values if
-        #                                                  value in factors[factor.name]]
-
-        # non_blocking_factor_values = dict(filter(lambda x: x[0] not in blocking_factors, experiment_factor_values.items()))
-        # blocking_factor_values = dict(filter(lambda x: x[0] in blocking_factors, experiment_factor_values.items()))
-
-        # # Initialize blocks
-        # blocks = []
-
-        """
-        The following lines return a list of tuples shown below, assuming you block on Factor 1 and Factor 2:
-        [
-            [
-                [("Factor 1", "value 1"), ("Factor 2", "value 1"), ("Factor 3", "value 1")],
-                [("Factor 1", "value 1"), ("Factor 2", "value 1"), ("Factor 3", "value 2")],
-            ],
-            [
-                [("Factor 1", "value 1"), ("Factor 2", "value 2"), ("Factor 3", "value 1")],
-                [("Factor 1", "value 1"), ("Factor 2", "value 2"), ("Factor 3", "value 2")],
-            ],
-            ...
-        ]
-        
-        Easy to use this to create dicts and thus experiments
-        """
-        # blocking_factor_combos = [list(zip(blocking_factor_values.keys(), values)) for values in itertools.product(*blocking_factor_values.values())]
-        # non_blocking_factor_combos = [list(zip(non_blocking_factor_values.keys(), values)) for values in itertools.product(*non_blocking_factor_values.values())]
-
-        # for blocking_combo in blocking_factor_combos:
-        #     block = []
-        #     for non_blocking_combo in non_blocking_factor_combos:
-        #         for rep in range(n_replicates):
-        #             experiment = Experiment(dict(blocking_combo + non_blocking_combo), self.experiment_id_generator(), rep + 1)
-        #             block.append(experiment)
-        #     blocks.append(block)
-
-        # return blocks
-    
 
+    def map_experiments(self, containers: list[Container]):
+        for container in containers:
+            factor_combination = []
+            for factor in self.factors:
+                get_level = factor.get_level_factory()
+                factor_value = get_level(container)
+                if factor_value == "Factor not found":
+                    continue
+                factor_combination.append((factor.name, factor_value))
+            factor_combination = sorted(factor_combination, key=lambda x: x[0])
+            self.experiments[factor_combination].map_container(container)
```

### Comparing `pyplate-hte-0.4/pyplate/pyplate.py` & `pyplate-hte-0.4.1/pyplate/pyplate.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,18 +275,18 @@
         if not isinstance(value, (int, float)):
             raise TypeError("Value must be a float.")
         if not isinstance(unit, str):
             raise TypeError("Unit must be a str.")
 
         if unit[-1] == 'L':
             prefix_value = Unit.convert_prefix_to_multiplier(unit[:-1])
-            result = value * prefix_value / Unit.convert_prefix_to_multiplier(config.volume_prefix[0])
+            result = value * prefix_value / Unit.convert_prefix_to_multiplier(config.volume_storage_unit[0])
         else:  # moles
             prefix_value = Unit.convert_prefix_to_multiplier(unit[:-3])
-            result = value * prefix_value / Unit.convert_prefix_to_multiplier(config.moles_prefix[0])
+            result = value * prefix_value / Unit.convert_prefix_to_multiplier(config.moles_storage_unit[0])
         return round(result, config.internal_precision)
 
     @staticmethod
     def convert_from_storage(value: float, unit: str) -> float:
         """
 
         Converts value from storage format.
@@ -302,53 +302,55 @@
         if not isinstance(value, (int, float)):
             raise TypeError("Value must be a float.")
         if not isinstance(unit, str):
             raise TypeError("Unit must be a str.")
 
         if unit[-1] == 'L':
             prefix_value = Unit.convert_prefix_to_multiplier(unit[:-1])
-            result = value * Unit.convert_prefix_to_multiplier(config.volume_prefix[0]) / prefix_value
+            result = value * Unit.convert_prefix_to_multiplier(config.volume_storage_unit[0]) / prefix_value
         else:  # moles
             prefix_value = Unit.convert_prefix_to_multiplier(unit[:-3])
-            result = value * Unit.convert_prefix_to_multiplier(config.moles_prefix[0]) / prefix_value
+            result = value * Unit.convert_prefix_to_multiplier(config.moles_storage_unit[0]) / prefix_value
         return round(result, config.internal_precision)
 
     @staticmethod
     def convert_from_storage_to_standard_format(what: Substance | Container, quantity: float) -> Tuple[float, str]:
         """
         Converts a quantity of a substance or container to a standard format.
-        Example: (water, 1e6) -> (18.015, 'mL'), (NaCl, 1e6) -> (58.443, 'g')
+        Example: (water, 1e6) -> (18.015, 'mL'), (NaCl, 1e6) -> (58.443, 'g'), (Amylase, 1) -> (1, 'U')
+
         Args:
             what: Substance or Container
             quantity: Quantity in storage format.
 
         Returns: Tuple of quantity and unit.
 
         """
         if isinstance(what, Substance):
             if what.is_enzyme():
                 unit = 'U'
             elif what.is_solid():
                 unit = 'g'
                 # convert moles to grams
                 # molecular weight is in g/mol
-                quantity *= Unit.convert_prefix_to_multiplier(config.moles_prefix[0]) * what.mol_weight
+                quantity *= Unit.convert_prefix_to_multiplier(config.moles_storage_unit[0]) * what.mol_weight
             elif what.is_liquid():
                 unit = 'L'
                 # convert moles to liters
                 # molecular weight is in g/mol
                 # density is in g/mL
-                quantity *= (Unit.convert_prefix_to_multiplier(config.moles_prefix[0])
+                quantity *= (Unit.convert_prefix_to_multiplier(config.moles_storage_unit[0])
                              * what.mol_weight / what.density / 1e3)
             else:
+                # This shouldn't happen.
                 raise TypeError("Invalid type for what.")
         elif isinstance(what, Container):
             # Assume the container contains a liquid
             unit = 'L'
-            quantity *= Unit.convert_prefix_to_multiplier(config.volume_prefix[0])
+            quantity *= Unit.convert_prefix_to_multiplier(config.volume_storage_unit[0])
         else:
             raise TypeError("Invalid type for what.")
 
         multiplier = 1
         while quantity < 1 and multiplier > 1e-6:
             quantity *= 1e3
             multiplier /= 1e3
@@ -533,15 +535,15 @@
             raise TypeError("Molecular weight must be a float.")
 
         if not mol_weight > 0:
             raise ValueError("Molecular weight must be positive.")
 
         substance = Substance(name, Substance.SOLID, molecule)
         substance.mol_weight = mol_weight
-        substance.density = config.default_density
+        substance.density = config.default_solid_density
         return substance
 
     @staticmethod
     def liquid(name: str, mol_weight: float, density: float, molecule=None) -> Substance:
         """
         Creates a liquid substance.
 
@@ -584,15 +586,15 @@
         Returns: New substance.
 
         """
         if not isinstance(name, str):
             raise TypeError("Name must be a str.")
 
         substance = Substance(name, Substance.ENZYME, molecule)
-        substance.density = config.default_density
+        substance.density = config.default_enzyme_density
         return substance
 
     def is_solid(self) -> bool:
         """
         Return true if `Substance` is a solid.
         """
         return self._type == Substance.SOLID
@@ -641,14 +643,15 @@
         max_volume, _ = Unit.parse_quantity(max_volume)
         if max_volume <= 0:
             raise ValueError("Maximum volume must be positive.")
         self.name = name
         self.contents: Dict[Substance, float] = {}
         self.volume = 0.0
         self.max_volume = Unit.convert_to_storage(max_volume, 'L')
+        self.experimental_conditions = {}
         if initial_contents:
             if not isinstance(initial_contents, Iterable):
                 raise TypeError("Initial contents must be iterable.")
             for entry in initial_contents:
                 if not isinstance(entry, Iterable) or not len(entry) == 2:
                     raise TypeError("Element in initial_contents must be a (Substance, str) tuple.")
                 substance, quantity = entry
@@ -700,16 +703,16 @@
         if not isinstance(quantity, str):
             raise TypeError("Quantity must be a str.")
 
         if source.is_enzyme():
             volume_to_add = 0
             amount_to_add = Unit.convert(source, quantity, 'U')
         else:
-            volume_to_add = Unit.convert(source, quantity, config.volume_prefix)
-            amount_to_add = Unit.convert(source, quantity, config.moles_prefix)
+            volume_to_add = Unit.convert(source, quantity, config.volume_storage_unit)
+            amount_to_add = Unit.convert(source, quantity, config.moles_storage_unit)
         if self.volume + volume_to_add > self.max_volume:
             raise ValueError("Exceeded maximum volume")
         self.volume = round(self.volume + volume_to_add, config.internal_precision)
         self.contents[source] = round(self.contents.get(source, 0) + amount_to_add, config.internal_precision)
 
     def _transfer(self, source_container: Container, quantity: str) -> Tuple[Container, Container]:
         """
@@ -734,15 +737,15 @@
                 raise ValueError(f"Not enough mixture left in source container ({source_container.name}). " +
                                  f"Only {Unit.convert_from_storage(source_container.volume, 'mL')} mL available, " +
                                  f"{Unit.convert_from_storage(volume_to_transfer, 'mL')} mL needed.")
             ratio = volume_to_transfer / source_container.volume
 
         elif unit == 'g':
             mass_to_transfer = round(quantity_to_transfer, config.internal_precision)
-            total_mass = sum(Unit.convert(substance, f"{amount} {config.moles_prefix}", "g") for
+            total_mass = sum(Unit.convert(substance, f"{amount} {config.moles_storage_unit}", "g") for
                              substance, amount in source_container.contents.items())
             ratio = mass_to_transfer / total_mass
         elif unit == 'mol':
             moles_to_transfer = Unit.convert_to_storage(quantity_to_transfer, 'mol')
             total_moles = sum(amount for substance, amount in source_container.contents.items()
                               if not substance.is_enzyme())
             ratio = moles_to_transfer / total_moles
@@ -761,24 +764,24 @@
             if source_container.contents[substance] == -0.0:
                 source_container.contents[substance] = 0.0
         if source_container.has_liquid():
             transfer = Unit.convert_from_storage(ratio * source_container.volume, 'L')
             transfer, unit = Unit.get_human_readable_unit(transfer, 'L')
         else:
             # total mass in source container times ratio
-            mass = sum(Unit.convert(substance, f"{amount} {config.moles_prefix if not substance.is_enzyme() else 'U'}",
+            mass = sum(Unit.convert(substance, f"{amount} {config.moles_storage_unit if not substance.is_enzyme() else 'U'}",
                                     "mg") for substance, amount in source_container.contents.items())
             transfer, unit = Unit.get_human_readable_unit(mass * ratio, 'mg')
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
         to.instructions += f"\nTransfer {round(transfer, precision)} {unit} of {source_container.name} to {to.name}"
-        to.volume = round(sum(Unit.convert(substance, f"{amount} {config.moles_prefix}", config.volume_prefix) for
+        to.volume = round(sum(Unit.convert(substance, f"{amount} {config.moles_storage_unit}", config.volume_storage_unit) for
                               substance, amount in to.contents.items()), config.internal_precision)
         if to.volume > to.max_volume:
             raise ValueError(f"Exceeded maximum volume in {to.name}.")
-        source_container.volume = sum(Unit.convert(substance, f"{amount} {config.moles_prefix}", config.volume_prefix)
+        source_container.volume = sum(Unit.convert(substance, f"{amount} {config.moles_storage_unit}", config.volume_storage_unit)
                                       for substance, amount in source_container.contents.items())
         source_container.volume = round(source_container.volume, config.internal_precision)
         return source_container, to
 
     def _transfer_slice(self, source_slice: Plate | PlateSlicer, quantity: str) -> Tuple[Plate, Container]:
         """
         Move quantity ('10 mL', '5 mg') from each well in a slice to self.
@@ -894,24 +897,42 @@
         if not isinstance(solute, Substance):
             raise TypeError("Solute must be a Substance.")
         if not isinstance(units, str):
             raise TypeError("Units must be a str.")
 
         mult, *units = Unit.parse_concentration('1 ' + units)
 
-        numerator = Unit.convert(solute, f"{self.contents.get(solute, 0)} {config.moles_prefix}", units[0])
+        numerator = Unit.convert(solute, f"{self.contents.get(solute, 0)} {config.moles_storage_unit}", units[0])
         if units[1].endswith('L'):
             denominator = Unit.convert_from_storage(self.volume, units[1])
         else:
             denominator = sum(
-                Unit.convert(substance, f"{amount} {config.moles_prefix}", units[1]) for substance, amount in
+                Unit.convert(substance, f"{amount} {config.moles_storage_unit}", units[1]) for substance, amount in
                 self.contents.items())
 
         return round(numerator / denominator / mult, config.internal_precision)
 
+    def get_volume(self, unit: str = None) -> float:
+        """
+        Get the volume of the container.
+
+        Args:
+            unit: Unit to return volume in. Defaults to volume_display_unit from config.
+
+        Returns: Volume of the container.
+
+        """
+        if unit is None:
+            unit = config.volume_display_unit
+
+        if not isinstance(unit, str):
+            raise TypeError("Unit must be a str.")
+
+        return Unit.convert_from_storage(self.volume, unit)
+
     @staticmethod
     def create_solution(solute: Substance, solvent: Substance, name: str = None, **kwargs) -> Container:
         """
         Create a solution.
 
         Two out of concentration, quantity, and total_quantity must be specified.
 
@@ -958,15 +979,15 @@
 
             if ratio <= 0:
                 raise ValueError("Solution is impossible to create.")
 
             if numerator == 'U':
                 if not solute.is_enzyme():
                     raise TypeError("Solute must be an enzyme.")
-                solvent_quantity = Unit.convert(solvent, f"{quantity} {quantity_unit}", config.moles_prefix)
+                solvent_quantity = Unit.convert(solvent, f"{quantity} {quantity_unit}", config.moles_storage_unit)
                 units = ratio * solvent_quantity
                 return Container(name,
                                  initial_contents=((solute, f"{units} U"), (solvent, f"{quantity} {quantity_unit}")))
 
             if quantity_unit == 'g':
                 ratio *= solute.mol_weight / solvent.mol_weight
             elif quantity_unit == 'mol':
@@ -998,89 +1019,151 @@
             value, unit = Unit.convert_from_storage_to_standard_format(substance, value)
             precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
             contents.append(f"{round(value, precision)} {unit} of {substance.name}")
         result.instructions = "Add " + ", ".join(contents) + " to a container."
         return result
 
     @staticmethod
-    def create_solution_from(source: Container, solute: Substance, concentration: str, solvent: Substance,
-                             quantity: str, name=None) -> Tuple[Container, Container]:
-        # TODO: consider case of different solvent
+    def create_solution_from(source: Container, solute: Substance, concentration: str, solvent: Substance | Container,
+                             quantity: str, name=None) -> (Tuple[Container, Container] |
+                                                           Tuple[Container, Container, Container]):
         """
-        Create a diluted solution from an existing solution.
+        Create a diluted solution from an existing solution or solutions.
 
 
         Arguments:
             source: Solution to dilute.
             solute: What to dissolve.
             concentration: Desired concentration. ('1 M', '0.1 umol/10 uL', etc.)
-            solvent: What to dissolve with.
+            solvent: What to dissolve with (if it is a Container, it can contain some solute).
             quantity: Desired total quantity. ('3 mL', '10 g')
             name: Optional name for new container.
 
         Returns:
-            Residual from the source container and a new container with desired solution.
+            Residual from the source container (and possibly the solvent container)
+             and a new container with the desired solution.
+
+        Raises:
+            ValueError: If the solution is impossible to create.
         """
 
         if not isinstance(source, Container):
             raise TypeError("Source must be a Container.")
         if not isinstance(solute, Substance):
             raise TypeError("Solute must be a Substance.")
         if not isinstance(concentration, str):
             raise TypeError("Concentration must be a str.")
-        if not isinstance(solvent, Substance):
-            raise TypeError("Solvent must be a Substance.")
+        if not isinstance(solvent, (Substance, Container)):
+            raise TypeError("Solvent must be a Substance or Container.")
         if not isinstance(quantity, str):
             raise TypeError("Quantity must be a str.")
         if name and not isinstance(name, str):
             raise TypeError("Name must be a str.")
 
         quantity_value, quantity_unit = Unit.parse_quantity(quantity)
         if quantity_value <= 0:
             raise ValueError("Quantity must be positive.")
 
         if solute not in source.contents:
-            raise ValueError(f"Container does not contain {solute.name}.")
+            raise ValueError(f"Source container does not contain {solute.name}.")
+
+        if solvent == solute:
+            raise ValueError("Solute and solvent must be different.")
 
         if not name:
             name = f"solution of {solute.name} in {solvent.name}"
 
-        new_ratio, numerator, denominator = Unit.calculate_concentration_ratio(solute, concentration, solvent)
-        current_ratio = source.contents[solute] / sum(source.contents[substance] for
-                                                      substance in source.contents if not substance.is_enzyme())
-        if new_ratio <= 0:
-            raise ValueError("Solution is impossible to create.")
+        # x is amount of source solution in mL, y is amount of solvent in mL
+        mass = sum(Unit.convert_from(substance, value, config.moles_storage_unit, 'g') for substance, value in
+                   source.contents.items())
+        moles = sum(Unit.convert_from(substance, value, config.moles_storage_unit, 'mol') for substance, value in
+                    source.contents.items())
+        volume = Unit.convert_from_storage(source.volume, 'mL')
+        d_x = mass / volume
+        mw_x = mass / moles
+        m_x = Unit.convert_from_storage(source.contents.get(solute, 0), 'mol') / (volume / 1000)
+
+        if isinstance(solvent, Container):
+            mass = sum(Unit.convert_from(substance, value, config.moles_storage_unit, 'g') for substance, value in
+                       solvent.contents.items())
+            moles = sum(Unit.convert_from(substance, value, config.moles_storage_unit, 'mol') for substance, value in
+                        solvent.contents.items())
+            volume = Unit.convert_from_storage(solvent.volume, 'mL')
+            d_y = mass / volume
+            mw_y = mass / moles
+            m_y = Unit.convert_from_storage(solvent.contents.get(solute, 0), 'mol') / (volume / 1000)
+        else:
+            d_y = solvent.density
+            mw_y = solvent.mol_weight
+            m_y = 0  # no solute in solvent
+
+        mw_s = solute.mol_weight
+        d_s = solute.density
+
+        concentration, numerator, denominator = Unit.parse_concentration(concentration)
+        a = numpy.array([[0., 0.], [0., 0.]])
+        b = numpy.array([0., 0.])
+
+        if numerator == 'mol':
+            top = numpy.array([m_x / 1000., m_y / 1000.])
+        elif numerator == 'g':
+            top = numpy.array([m_x * mw_s / 1000., m_y * mw_s / 1000.])
+        elif numerator == 'L':
+            # (mL/1000) * mol/L * g/mol * mL/g = mL / 1000 = L
+            top = numpy.array([m_x * mw_s / (d_s * 1e6), m_y * mw_s / (d_s * 1e6)])
+        else:
+            raise ValueError("Invalid numerator.")
+        if denominator == 'mol':
+            bottom = numpy.array([d_x / mw_x, d_y / mw_y])
+        elif denominator == 'g':
+            bottom = numpy.array([d_x, d_y])
+        elif denominator == 'L':
+            bottom = numpy.array([1 / 1000., 1 / 1000.])
+        else:
+            raise ValueError("Invalid denominator.")
 
-        if abs(new_ratio - current_ratio) <= 1e-3:
-            new_ratio = current_ratio
+        # concentration = top / bottom -> concentration * bottom - top = 0
+        a[0] = concentration * bottom - top
 
-        if new_ratio > current_ratio:
-            raise ValueError("Desired concentration is higher than current concentration.")
+        quantity_value, quantity_unit = Unit.parse_quantity(quantity)
 
-        potential_solution = Container.create_solution(solute, solvent, concentration=concentration,
-                                                       total_quantity=quantity)
-        ratio = potential_solution.contents[solute] / source.contents[solute]
-        solution = Container(name, max_volume=f"{source.max_volume} {config.volume_prefix}")
-
-        residual, solution = Container.transfer(source, solution, f"{source.volume * ratio} {config.volume_prefix}")
-        solution = solution.fill_to(solvent, quantity)
-
-        contents = [(*Unit.convert_from_storage_to_standard_format(solution, solution.volume), source.name),
-                    (*Unit.convert_from_storage_to_standard_format(solvent, solution.contents[solvent]), solvent.name)]
-        max_volume, unit = Unit.convert_from_storage_to_standard_format(solution, solution.max_volume)
-        sub_instructions = []
-        for value, sub_unit, substance in contents:
-            precision = config.precisions[sub_unit] if sub_unit in config.precisions else config.precisions['default']
-            sub_instructions.append(f"{round(value, precision)} {sub_unit} of {substance}")
-        precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
-        solution.instructions = ("Add "
-                                 + ", ".join(sub_instructions)
-                                 + f" to a {round(max_volume, precision)} {unit} container.")
+        if quantity_unit == 'g':
+            a[1] = numpy.array([d_x, d_y])
+        elif quantity_unit == 'L':
+            a[1] = numpy.array([1 / 1000., 1 / 1000.])
+        elif quantity_value == 'mol':
+            a[1] = numpy.array([d_x / mw_x, d_y / mw_y])
+
+        b[1] = quantity_value
+        x, y = numpy.linalg.solve(a, b)
+        if x < 0 or y < 0:
+            raise ValueError("Solution is impossible to create.")
 
-        return residual, solution.fill_to(solvent, quantity)
+        if isinstance(solvent, Substance):
+            if y:
+                new_solution = Container(name, initial_contents=[(solvent, f"{y} mL")])
+            else:
+                new_solution = Container(name)
+            if x:
+                source, new_solution = Container.transfer(source, new_solution, f"{x} mL")
+        else:
+            new_solution = Container(name)
+            if x:
+                source, new_solution = Container.transfer(source, new_solution, f"{x} mL")
+            if y:
+                solvent, new_solution = Container.transfer(solvent, new_solution, f"{y} mL")
+
+        precision = config.precisions['mL'] if 'mL' in config.precisions else config.precisions['default']
+        new_solution.instructions = f"Add {round(y, precision)} mL of {solvent.name} to" + \
+                                    f" {round(x, precision)} mL of {source.name}."
+
+        if isinstance(solvent, Substance):
+            return source, new_solution
+        else:
+            return source, solvent, new_solution
 
     def remove(self, what: (Substance | int) = Substance.LIQUID) -> Container:
         """
         Removes substances from `Container`
 
         Arguments:
             what: What to remove. Can be a type of substance or a specific substance. Defaults to LIQUID.
@@ -1089,16 +1172,16 @@
 
         """
         new_container = deepcopy(self)
         new_container.contents = {substance: value for substance, value in self.contents.items()
                                   if what not in (substance._type, substance)}
         new_container.volume = 0
         for substance, value in new_container.contents.items():
-            substance_unit = 'U' if substance.is_enzyme() else config.moles_prefix
-            new_container.volume += Unit.convert_from(substance, value, substance_unit, config.volume_prefix)
+            substance_unit = 'U' if substance.is_enzyme() else config.moles_storage_unit
+            new_container.volume += Unit.convert_from(substance, value, substance_unit, config.volume_storage_unit)
 
         new_container.instructions = self.instructions
         classes = {Substance.SOLID: 'solid', Substance.LIQUID: 'liquid', Substance.ENZYME: 'enzyme'}
         if what in classes:
             new_container.instructions += f"Remove all {classes[what]}s."
         else:
             new_container.instructions += f"Remove all {what.name}s."
@@ -1144,15 +1227,15 @@
             return deepcopy(self)
 
         if new_ratio > current_ratio:
             raise ValueError("Desired concentration is higher than current concentration.")
 
         current_umoles = Unit.convert_from_storage(self.contents.get(solvent, 0), 'umol')
         required_umoles = Unit.convert_from_storage(self.contents[solute], 'umol') / new_ratio - current_umoles
-        new_volume = self.volume + Unit.convert(solvent, f"{required_umoles} umol", config.volume_prefix)
+        new_volume = self.volume + Unit.convert(solvent, f"{required_umoles} umol", config.volume_storage_unit)
 
         if new_volume > self.max_volume:
             raise ValueError("Dilute solution will not fit in container.")
 
         if name:
             # Note: this copies the container twice
             destination = deepcopy(self)
@@ -1184,15 +1267,15 @@
 
         quantity, quantity_unit = Unit.parse_quantity(quantity)
         if quantity <= 0:
             raise ValueError("Quantity must be positive.")
         if quantity_unit not in ('L', 'g', 'mol'):
             raise ValueError("We can only fill to mass or volume.")
 
-        current_quantity = sum(Unit.convert(substance, f"{value} {config.moles_prefix}", quantity_unit)
+        current_quantity = sum(Unit.convert(substance, f"{value} {config.moles_storage_unit}", quantity_unit)
                                for substance, value in self.contents.items() if not substance.is_enzyme())
 
         required_quantity = quantity - current_quantity
         result = self._add(solvent, f"{required_quantity} {quantity_unit}")
         required_volume = Unit.convert(solvent, f"{required_quantity} {quantity_unit}", 'L')
         required_volume, unit = Unit.get_human_readable_unit(required_volume, 'L')
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
@@ -1291,49 +1374,49 @@
 
     def __getitem__(self, item) -> PlateSlicer:
         return PlateSlicer(self, item)
 
     def __repr__(self):
         return f"Plate: {self.name}"
 
-    def volumes(self, substance: (Substance | Iterable[Substance]) = None, unit: str = None) -> numpy.ndarray:
+    def get_volumes(self, substance: (Substance | Iterable[Substance]) = None, unit: str = None) -> numpy.ndarray:
         """
 
         Arguments:
             unit: unit to return volumes in.
             substance: (optional) Substance to display volumes of.
 
         Returns:
             numpy.ndarray of volumes for each well in desired unit.
 
         """
 
         # Arguments are type checked in PlateSlicer.volumes
-        return self[:].volumes(substance=substance, unit=unit)
+        return self[:].get_volumes(substance=substance, unit=unit)
 
     def substances(self) -> set[Substance]:
         """
 
         Returns: A set of substances present in the slice.
 
         """
         return self[:].substances()
 
-    def moles(self, substance: (Substance | Iterable[Substance]), unit: str = None) -> numpy.ndarray:
+    def get_moles(self, substance: (Substance | Iterable[Substance]), unit: str = None) -> numpy.ndarray:
         """
 
         Arguments:
             unit: unit to return moles in. ('mol', 'mmol', 'umol', etc.)
             substance: Substance to display moles of.
 
         Returns: moles of substance in each well.
         """
 
         # Arguments are type checked in PlateSlicer.moles
-        return self[:].moles(substance=substance, unit=unit)
+        return self[:].get_moles(substance=substance, unit=unit)
 
     def dataframe(self, unit: str, substance: (str | Substance | Iterable[Substance]) = 'all', cmap: str = None) \
             -> pandas.io.formats.style.Styler:
         """
 
         Arguments:
             unit: unit to return quantities in.
@@ -1342,22 +1425,22 @@
 
         Returns: Shaded dataframe of quantities in each well.
 
         """
         # Types are checked in PlateSlicer.dataframe
         return self[:].dataframe(substance=substance, unit=unit, cmap=cmap)
 
-    def volume(self, unit: str = 'uL') -> float:
+    def get_volume(self, unit: str = 'uL') -> float:
         """
         Arguments:
             unit: unit to return volumes in.
 
         Returns: total volume stored in slice in uL.
         """
-        return self.volumes(unit=unit).sum()
+        return self.get_volumes(unit=unit).sum()
 
     @staticmethod
     def transfer(source: Container | Plate | PlateSlicer, destination: Plate | PlateSlicer, quantity: str) \
             -> Tuple[Container | Plate | PlateSlicer, Plate]:
         """
         Move quantity ('10 mL', '5 mg') from source to destination,
         returning copies of the objects with amounts adjusted accordingly.
@@ -1637,15 +1720,15 @@
         if not name:
             name = f"solution of {solute.name} in {solvent.name}"
 
         new_ratio, numerator, denominator = Unit.calculate_concentration_ratio(solute, concentration, solvent)
         if new_ratio <= 0:
             raise ValueError("Solution is impossible to create.")
 
-        new_container = Container(name, max_volume=f"{source.max_volume} {config.volume_prefix}")
+        new_container = Container(name, max_volume=f"{source.max_volume} {config.volume_storage_unit}")
         self.uses(new_container)
         self.steps.append(RecipeStep('solution_from', source, new_container, solute, concentration, solvent, quantity))
 
         return new_container
 
     def remove(self, destination: Container | Plate | PlateSlicer, what=Substance.LIQUID) -> None:
         """
@@ -1880,30 +1963,30 @@
                 dest_name = dest.name
                 solute, concentration, solvent, new_name = step.operands
                 step.frm.append(None)
                 step.to[0] = self.results[dest_name]
                 self.used.add(dest_name)
                 self.results[dest_name] = self.results[dest_name].dilute(solute, concentration, solvent, new_name)
                 amount_added = self.results[dest_name].contents[solvent] - step.to[0].contents.get(solvent, 0)
-                amount_added = Unit.convert_from(solvent, amount_added, config.moles_prefix, 'L')
+                amount_added = Unit.convert_from(solvent, amount_added, config.moles_storage_unit, 'L')
                 amount_added, unit = Unit.get_human_readable_unit(amount_added, 'L')
                 precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
                 step.instructions = (f"Dilute {solute.name} in {dest_name} to {concentration}" +
                                      f" by adding {round(amount_added, precision)} {unit} of {solvent.name}.")
                 step.substances_used.add(solvent)
                 step.to.append(self.results[dest_name])
             elif operator == 'fill_to':
                 dest = step.to[0]
                 dest_name = dest.plate.name if isinstance(dest, PlateSlicer) else dest.name
                 solvent, quantity = step.operands
                 step.frm.append(None)
                 step.to[0] = self.results[dest_name]
                 self.used.add(dest_name)
                 amount_added = self.results[dest_name].contents[solvent] - step.to[0].contents.get(solvent, 0)
-                amount_added = Unit.convert_from(solvent, amount_added, config.moles_prefix, 'L')
+                amount_added = Unit.convert_from(solvent, amount_added, config.moles_storage_unit, 'L')
                 amount_added, unit = Unit.get_human_readable_unit(amount_added, 'L')
                 precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
                 step.instructions = (f"Fill {dest.name} with {solvent.name} up to {quantity}"
                                      f" by adding {round(amount_added, precision)} {unit}.")
 
                 if isinstance(dest, PlateSlicer):
                     dest = deepcopy(dest)
@@ -1934,17 +2017,17 @@
             unit: Unit to return amount in.
             destinations: Containers or plates to check. Defaults to "plates".
 
         Returns: Amount of substance used in the recipe.
 
         """
         if unit is None:
-            unit = 'U' if substance.is_enzyme() else config.default_moles_unit
+            unit = 'U' if substance.is_enzyme() else config.moles_display_unit
 
-        from_unit = 'U' if substance.is_enzyme() else config.moles_prefix
+        from_unit = 'U' if substance.is_enzyme() else config.moles_storage_unit
 
         dest_names = set()
         if destinations == "plates":
             dest_names = set(elem.name for elem in self.results.values() if isinstance(elem, Plate))
         elif isinstance(destinations, Iterable):
             for container in destinations:
                 if container.name not in self.used:
@@ -1998,18 +2081,18 @@
             container: Container to check.
             timeframe: 'all' or a stage defined in the recipe.
             unit: Unit to return amount in.
         """
 
         def helper(entry):
             substance, quantity = entry
-            return Unit.convert_from(substance, quantity, 'U' if substance.is_enzyme() else config.moles_prefix, unit)
+            return Unit.convert_from(substance, quantity, 'U' if substance.is_enzyme() else config.moles_storage_unit, unit)
 
         if unit is None:
-            unit = config.default_volume_unit
+            unit = config.volume_display_unit
         if not isinstance(unit, str):
             raise TypeError("Unit must be a str.")
         if not isinstance(container, Container):
             raise TypeError("Container must be a Container.")
         if not isinstance(timeframe, str):
             raise TypeError("Timeframe must be a str.")
         if timeframe not in self.stages.keys():
@@ -2068,19 +2151,19 @@
             raise TypeError("Colormap must be a str.")
 
         def helper(elem):
             """ Returns amount of substance in elem. """
             if substance == 'all':
                 amount = 0
                 for subst, quantity in elem.contents.items():
-                    substance_unit = 'U' if subst.is_enzyme() else config.moles_prefix
+                    substance_unit = 'U' if subst.is_enzyme() else config.moles_storage_unit
                     amount += Unit.convert_from(subst, quantity, substance_unit, unit)
                 return amount
             else:
-                substance_unit = 'U' if substance.is_enzyme() else config.moles_prefix
+                substance_unit = 'U' if substance.is_enzyme() else config.moles_storage_unit
                 return Unit.convert_from(substance, elem.contents.get(substance, 0), substance_unit, unit)
 
         if isinstance(timeframe, str):
             start_index = self.stages[timeframe].start
             end_index = self.stages[timeframe].stop
             if start_index is None:
                 start_index = 0
@@ -2303,113 +2386,112 @@
             raise TypeError("Colormap must be a str.")
 
         def helper(elem):
             """ Returns amount of substance in elem. """
             if substance == 'all':
                 amount = 0
                 for subst, quantity in elem.contents.items():
-                    substance_unit = 'U' if subst.is_enzyme() else config.moles_prefix
+                    substance_unit = 'U' if subst.is_enzyme() else config.moles_storage_unit
                     amount += Unit.convert_from(subst, quantity, substance_unit, unit)
                 return amount
             elif isinstance(substance, Iterable):
                 amount = 0
                 for subst in substance:
-                    substance_unit = 'U' if subst.is_enzyme() else config.moles_prefix
+                    substance_unit = 'U' if subst.is_enzyme() else config.moles_storage_unit
                     amount += Unit.convert_from(subst, elem.contents.get(subst, 0), substance_unit, unit)
                 return amount
             else:
-                substance_unit = 'U' if substance.is_enzyme() else config.moles_prefix
+                substance_unit = 'U' if substance.is_enzyme() else config.moles_storage_unit
                 return Unit.convert_from(substance, elem.contents.get(substance, 0), substance_unit, unit)
 
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
         df = self.get_dataframe().apply(numpy.vectorize(helper, cache=True, otypes='d'))
         vmin, vmax = df.min().min(), df.max().max()
         styler = df.style.format(precision=precision).background_gradient(cmap, vmin=vmin, vmax=vmax)
         return styler
 
-    def volumes(self, substance: (Substance | Iterable[Substance]) = None, unit: str = None) -> numpy.ndarray:
+    def get_volumes(self, substance: (Substance | Iterable[Substance]) = None, unit: str = None) -> numpy.ndarray:
         """
 
         Arguments:
             unit:  unit to return volumes in.
             substance: (optional) Substance to display volumes of.
 
         Returns:
             numpy.ndarray of volumes for each well in uL
 
         """
         if unit is None:
-            unit = config.default_volume_unit
+            unit = config.volume_display_unit
 
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
 
         if substance is None:
-            return numpy.vectorize(lambda elem: Unit.convert_from_storage(elem.volume, unit), cache=True,
-                                   otypes='d')(self.get()).round(precision)
+            return numpy.vectorize(lambda elem: elem.get_volume(unit),
+                                   cache=True, otypes='d')(self.get()).round(precision)
 
         if isinstance(substance, Substance):
             substance = [substance]
 
         if not (substance is None or
                 (isinstance(substance, Iterable) and all(isinstance(x, Substance) for x in substance))):
             raise TypeError("Substance must be a Substance or an Iterable of Substances.")
         if not isinstance(unit, str):
             raise TypeError("Unit must be a str.")
 
-
         def helper(elem):
             amount = 0
             """ Returns volume of elem. """
             if substance is None:
                 for subs, quantity in elem.contents.items():
-                    substance_unit = 'U' if subs.is_enzyme() else config.moles_prefix
+                    substance_unit = 'U' if subs.is_enzyme() else config.moles_storage_unit
                     amount += Unit.convert_from(subs, quantity, substance_unit, unit)
             else:
                 for subs in substance:
-                    substance_unit = 'U' if subs.is_enzyme() else config.moles_prefix
+                    substance_unit = 'U' if subs.is_enzyme() else config.moles_storage_unit
                     amount += Unit.convert_from(subs, elem.contents.get(subs, 0), substance_unit, unit)
             return amount
 
         return numpy.vectorize(helper, cache=True, otypes='d')(self.get()).round(precision)
 
     def substances(self) -> set[Substance]:
         """
 
         Returns: A set of substances present in the plate.
 
         """
         substances_arr = numpy.vectorize(lambda elem: set(elem.contents.keys()), cache=True)(self.get())
         return set.union(*substances_arr.flatten())
 
-    def moles(self, substance: (Substance | Iterable[Substance]), unit: str = 'mol') -> numpy.ndarray:
+    def get_moles(self, substance: (Substance | Iterable[Substance]), unit: str = 'mol') -> numpy.ndarray:
         """
         Arguments:
             unit: unit to return moles in. ('mol', 'mmol', 'umol', etc.)
             substance: Substance to display moles of.
 
         Returns: moles of substance in each well.
         """
 
         if isinstance(substance, Substance):
             substance = [substance]
         if unit is None:
-            unit = config.default_moles_unit
+            unit = config.moles_display_unit
 
         if not isinstance(substance, Iterable) or not all(isinstance(x, Substance) for x in substance):
             raise TypeError(f"Substance must be a Substance or an Iterable of Substances.")
         if not isinstance(unit, str):
             raise TypeError(f"Unit must be a str.")
 
         precision = config.precisions[unit] if unit in config.precisions else config.precisions['default']
 
         def helper(elem):
             amount = 0
             for subs in substance:
                 if not subs.is_enzyme():
-                    amount += Unit.convert_from(subs, elem.contents.get(subs, 0), config.moles_prefix, unit)
+                    amount += Unit.convert_from(subs, elem.contents.get(subs, 0), config.moles_storage_unit, unit)
             return amount
 
         return numpy.vectorize(helper, cache=True, otypes='d')(self.get()).round(precision)
 
     def remove(self, what: (Substance | int) = Substance.LIQUID):
         """
         Removes substances from slice
```

### Comparing `pyplate-hte-0.4/pyplate/pyplate.yaml` & `pyplate-hte-0.4.1/pyplate/pyplate.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # How many digits of precision to maintain in internal calculations
 internal_precision: 10
+
 # How many digits of precision to return to the user
 precisions:
   default: 3
   uL: 1
   umol: 1
   mg: 2
+
 # How to store volumes and moles internally
 # uL means we will store volumes as microliters
-volume_storage: uL
-#volume_storage_unit
-#volume_display_unit
-
-#... moles
+volume_storage_unit: uL
+# uL means we will return volumes as microliters
+volume_display_unit: uL
 
 # umol means we will store moles as micromoles
-moles_storage: umol
+moles_storage_unit: umol
+# umol means we will return moles as micromoles
+moles_display_unit: umol
+
 # density for solids/biologics in g/mL or U/mL. Can be set to float('inf') to give solids and biologics zero volume.
-default_density: 1
+default_solid_density: 1
+default_enzyme_density: 1
+
 # units for %w/v
 default_weight_volume_units: g/mL
 
-# default units to be returned to the user
-default_moles_unit: mol
-default_volume_unit: uL
-
 # default colormap to be used in visualizations
 default_colormap: Purples
-default_diverging_colormap: PuOr
+default_diverging_colormap: PuOr
```

### Comparing `pyplate-hte-0.4/pyplate/slicer.py` & `pyplate-hte-0.4.1/pyplate/slicer.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4/pyplate_hte.egg-info/PKG-INFO` & `pyplate-hte-0.4.1/pyplate_hte.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyplate-hte
-Version: 0.4
+Version: 0.4.1
 Summary: A Python tool for designing chemistry experiments in plate format
 Author: Eugene Kwan and James Marvin
 Author-email: ekwan16@gmail.com
 License:   				Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `pyplate-hte-0.4/pyplate_hte.egg-info/SOURCES.txt` & `pyplate-hte-0.4.1/pyplate_hte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4/pyproject.toml` & `pyplate-hte-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=63.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyplate-hte"
-version = "0.4"
+version = "0.4.1"
 description = "A Python tool for designing chemistry experiments in plate format"
 readme = "README.md"
 license = {file = "LICENSE.txt"}
 authors = [
     {name = "Eugene Kwan and James Marvin"},
     {email = "ekwan16@gmail.com"}
 ]
```

### Comparing `pyplate-hte-0.4/tests/test_Container.py` & `pyplate-hte-0.4.1/tests/test_Container.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,31 +50,31 @@
         Container.transfer(salt_water, water_stock, 1)
 
     initial_hashes = hash(water_stock), hash(salt_water)
     # water_stock is 10 mL, salt_water is 100 mL and 50 mmol
     salt_water_volume = Unit.convert_from_storage(salt_water.volume, 'mL')
     container1, container2 = Container.transfer(salt_water, water_stock, f"{salt_water_volume*0.1} mL")
     # 10 mL of water and 5 mol of salt should have been transferred
-    assert container1.volume == Unit.convert(water, '90 mL', config.volume_prefix)\
-           + Unit.convert(salt, '45 mmol', config.volume_prefix)
-    assert container1.contents[water] == Unit.convert(water, '90 mL', config.moles_prefix)
-    assert container1.contents[salt] == Unit.convert(salt, '45 mmol', config.moles_prefix)
-    assert container2.volume == Unit.convert(water, '20 mL', config.volume_prefix)\
-           + Unit.convert(salt, '5 mmol', config.volume_prefix)
+    assert container1.volume == Unit.convert(water, '90 mL', config.volume_storage_unit) \
+           + Unit.convert(salt, '45 mmol', config.volume_storage_unit)
+    assert container1.contents[water] == Unit.convert(water, '90 mL', config.moles_storage_unit)
+    assert container1.contents[salt] == Unit.convert(salt, '45 mmol', config.moles_storage_unit)
+    assert container2.volume == Unit.convert(water, '20 mL', config.volume_storage_unit)\
+           + Unit.convert(salt, '5 mmol', config.volume_storage_unit)
     assert salt in container2.contents and container2.contents[salt] == \
-           Unit.convert(salt, '5 mmol', config.moles_prefix)
-    assert container2.contents[water] == pytest.approx(Unit.convert(water, '20 mL', config.moles_prefix))
+           Unit.convert(salt, '5 mmol', config.moles_storage_unit)
+    assert container2.contents[water] == pytest.approx(Unit.convert(water, '20 mL', config.moles_storage_unit))
 
     # Original containers should be unchanged.
     assert initial_hashes == (hash(water_stock), hash(salt_water))
 
     salt_stock = Container('salt stock', initial_contents=[(salt, '10 g')])
     container1, container2 = Container.transfer(salt_stock, salt_water, '1 g')
     assert container2.contents[salt] == \
-           pytest.approx(salt_water.contents[salt] + Unit.convert(salt, '1 g', config.moles_prefix))
+           pytest.approx(salt_water.contents[salt] + Unit.convert(salt, '1 g', config.moles_storage_unit))
 
 
 def test_create_stock_solution(water, salt, salt_water):
     """
 
     Tests if transfers between `Container`s works properly.
 
@@ -117,15 +117,15 @@
         container._self_add(water, 5)
 
     # Use the _self_add method to add the substance to the container
     container._self_add(water, '5 mL')
 
     # Check if the substance was correctly added to the container
     assert water in container.contents
-    assert pytest.approx(container.contents[water]) == Unit.convert(water, '5 mL', config.moles_prefix)
+    assert pytest.approx(container.contents[water]) == Unit.convert(water, '5 mL', config.moles_storage_unit)
     assert pytest.approx(container.volume) == Unit.convert_to_storage(5, 'mL')
 
     # Try to add more substance than the container can hold
     with pytest.raises(ValueError, match='Exceeded maximum volume'):
         container._self_add(water, '10 mL')
 
 
@@ -155,23 +155,23 @@
         container2 = Container('container2', '10 mL')
         # Use the _transfer method to transfer the substance from the first to the second container
         container1, container2 = container2._transfer(container1, f"2 {unit}")
 
         # Check if the substance was correctly transferred
         assert water in container2.contents
         assert (pytest.approx(container2.contents[water]) ==
-                Unit.convert(water, f"2 {unit}", config.moles_prefix))
+                Unit.convert(water, f"2 {unit}", config.moles_storage_unit))
         assert (pytest.approx(container2.volume) ==
-                Unit.convert(water, f"2 {unit}", config.volume_prefix))
+                Unit.convert(water, f"2 {unit}", config.volume_storage_unit))
 
         # Check if the volume of the first container was correctly reduced
         assert (pytest.approx(container1.contents[water]) ==
-                Unit.convert(water, f"3 {unit}", config.moles_prefix))
+                Unit.convert(water, f"3 {unit}", config.moles_storage_unit))
         assert (pytest.approx(container1.volume) ==
-                Unit.convert(water, f"3 {unit}", config.volume_prefix))
+                Unit.convert(water, f"3 {unit}", config.volume_storage_unit))
 
     container1 = Container('container1', '10 mL', initial_contents=[(water, '5 mL')])
     container2 = Container('container2', '10 mL')
 
     # Try to transfer more substance than the first container holds
     with pytest.raises(ValueError, match='Not enough mixture left in source container'):
         container2._transfer(container1, '10 mL')
@@ -216,15 +216,15 @@
     # Create a stock solution of 1 M salt water
     stock = Container.create_solution(salt, water, concentration='1 M', total_quantity='100 mL')
 
     # Create a solution of 0.5 M salt water from the stock solution
     stock, solution = Container.create_solution_from(stock, salt,'0.5 M', water, '50 mL')
 
     # Should contain 25 mmol of salt and have a total volume of 50 mL
-    assert pytest.approx(Unit.convert(salt, '25 mmol', config.moles_prefix)) == solution.contents[salt]
-    assert pytest.approx(Unit.convert(water, '50 mL', config.volume_prefix)) == solution.volume
+    assert pytest.approx(Unit.convert(salt, '25 mmol', config.moles_storage_unit)) == solution.contents[salt]
+    assert pytest.approx(Unit.convert(water, '50 mL', config.volume_storage_unit)) == solution.volume
     assert pytest.approx(Unit.convert_from_storage(solution.volume, 'mL')) == 50.0
 
     # stock should have a volume of 75 mL and 75 mmol of salt
     # Try to create a solution with more volume than the source container holds
     with pytest.raises(ValueError, match='Not enough mixture left in source container'):
         Container.create_solution_from(stock, salt, '1 M', water, '100 mL')
```

### Comparing `pyplate-hte-0.4/tests/test_Experiment.py` & `pyplate-hte-0.4.1/tests/test_Experiment.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4/tests/test_ExperimentalSpace.py` & `pyplate-hte-0.4.1/tests/test_ExperimentalSpace.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4/tests/test_Factor.py` & `pyplate-hte-0.4.1/tests/test_Factor.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4/tests/test_Plate.py` & `pyplate-hte-0.4.1/tests/test_Plate.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,74 +42,74 @@
     with pytest.raises(ValueError, match='duplicate column names found'):
         Plate('plate', '10 uL', columns=['a', 'a'])
 
 
 def test_volume_and_volumes(salt, water, dmso, empty_plate):
     """
 
-    Test volume() and volumes() for a plate.
+    Test get_volume() and get_volumes() for a plate.
 
     """
     epsilon = 1e-3
     with pytest.raises(TypeError, match="Substance must be a Substance"):
-        empty_plate.volumes('1')
+        empty_plate.get_volumes('1')
 
     zeros = numpy.zeros(empty_plate.wells.shape)
     uL = numpy.ones(empty_plate.wells.shape)
     config.precisions['uL'] = 3
     # set precision to 3 decimal places for 'uL' for testing
 
-    salt_volume = round(Unit.convert(salt, '5 umol', 'uL'), 20)
-    assert empty_plate.volume() == 0
-    assert numpy.array_equal(empty_plate.volumes(), zeros)
-    assert numpy.array_equal(empty_plate.volumes(water), zeros)
+    salt_volume = round(Unit.convert(salt, '5 umol', 'uL'), 3)
+    assert empty_plate.get_volume() == 0
+    assert numpy.array_equal(empty_plate.get_volumes(), zeros)
+    assert numpy.array_equal(empty_plate.get_volumes(water), zeros)
 
     salt_container = Container('salt', initial_contents=((salt, '1 mol'),))
     salt_container, new_plate = Plate.transfer(salt_container, empty_plate, '5 umol')
-    assert new_plate.volume() == pytest.approx((salt_volume * uL).sum(), epsilon)
-    assert numpy.allclose(new_plate.volumes(), salt_volume * uL)
-    assert numpy.array_equal(new_plate.volumes(water), zeros)
-    assert numpy.allclose(new_plate.volumes(salt), salt_volume * uL, atol=epsilon)
+    assert new_plate.get_volume() == pytest.approx((salt_volume * uL).sum(), epsilon)
+    assert numpy.allclose(new_plate.get_volumes(unit='uL'), salt_volume * uL)
+    assert numpy.array_equal(new_plate.get_volumes(water), zeros)
+    assert numpy.allclose(new_plate.get_volumes(salt, unit='uL'), salt_volume * uL, atol=epsilon)
 
     water_container = Container('water', initial_contents=((water, '1 L'),))
     water_container, new_plate = Plate.transfer(water_container, new_plate, '50 uL')
-    assert new_plate.volume() == pytest.approx((salt_volume * uL).sum() + (50 * uL).sum(), epsilon)
-    assert numpy.allclose(new_plate.volumes(), (salt_volume + 50) * uL)
-    assert numpy.allclose(new_plate.volumes(water), 50 * uL)
-    assert numpy.allclose(new_plate.volumes(salt), salt_volume * uL, atol=1e-3)
+    assert new_plate.get_volume() == pytest.approx((salt_volume * uL).sum() + (50 * uL).sum(), epsilon)
+    assert numpy.allclose(new_plate.get_volumes(), (salt_volume + 50) * uL)
+    assert numpy.allclose(new_plate.get_volumes(water), 50 * uL)
+    assert numpy.allclose(new_plate.get_volumes(salt), salt_volume * uL, atol=1e-3)
 
     dmso_container = Container('dmso', initial_contents=((dmso, '1 L'), ))
     dmso_container, new_plate = Plate.transfer(dmso_container, new_plate, '25 uL')
-    assert new_plate.volume() == pytest.approx((salt_volume * uL).sum() + (75 * uL).sum(), epsilon)
-    assert numpy.allclose(new_plate.volumes(), (salt_volume + 75) * uL)
-    assert numpy.allclose(new_plate.volumes(water), 50 * uL)
-    assert numpy.allclose(new_plate.volumes(dmso), 25 * uL)
-    assert numpy.allclose(new_plate.volumes(salt), salt_volume * uL, atol=epsilon)
-    assert numpy.allclose(new_plate.volumes(water, unit='mL'), 0.05 * uL)
+    assert new_plate.get_volume() == pytest.approx((salt_volume * uL).sum() + (75 * uL).sum(), epsilon)
+    assert numpy.allclose(new_plate.get_volumes(), (salt_volume + 75) * uL)
+    assert numpy.allclose(new_plate.get_volumes(water), 50 * uL)
+    assert numpy.allclose(new_plate.get_volumes(dmso), 25 * uL)
+    assert numpy.allclose(new_plate.get_volumes(salt), salt_volume * uL, atol=epsilon)
+    assert numpy.allclose(new_plate.get_volumes(water, unit='mL'), 0.05 * uL)
 
 
 def test_moles(salt, water, empty_plate):
     """
 
     Test moles() for a plate.
 
     """
     with pytest.raises(TypeError, match="Substance must be a Substance"):
-        empty_plate.moles('1')
+        empty_plate.get_moles('1')
 
     zeros = numpy.zeros(empty_plate.wells.shape)
     ones = numpy.ones(empty_plate.wells.shape)
-    assert numpy.array_equal(empty_plate.moles(salt), zeros)
+    assert numpy.array_equal(empty_plate.get_moles(salt), zeros)
 
     salt_container = Container('salt', initial_contents=((salt, '1 mol'),))
     salt_container, new_plate = Plate.transfer(salt_container, empty_plate, '5 umol')
-    assert numpy.array_equal(new_plate.moles(salt, 'umol'), 5 * ones)
-    assert numpy.array_equal(new_plate.moles(water), zeros)
+    assert numpy.array_equal(new_plate.get_moles(salt, 'umol'), 5 * ones)
+    assert numpy.array_equal(new_plate.get_moles(water), zeros)
 
     water_container = Container('water', initial_contents=((water, '1 L'),))
     water_container, new_plate = Plate.transfer(water_container, new_plate, '1 mmol')
-    assert numpy.array_equal(new_plate.moles(salt, 'umol'), 5 * ones)
-    assert numpy.array_equal(new_plate.moles(water), 0.001 * ones)
+    assert numpy.array_equal(new_plate.get_moles(salt, 'umol'), 5 * ones)
+    assert numpy.array_equal(new_plate.get_moles(water, unit='mmol'), ones)
 
     water_container = Container('water', initial_contents=((water, '1 L'),))
     water_container, new_plate = Plate.transfer(water_container, new_plate, '5 uL')
-    new_plate.moles(water)
+    new_plate.get_moles(water)
```

### Comparing `pyplate-hte-0.4/tests/test_Recipe.py` & `pyplate-hte-0.4.1/tests/test_Recipe.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,46 +65,46 @@
         recipe.transfer(salt_water, container, 1)
     recipe.transfer(salt_water, container, '10 mL')
     # Container should still be empty until we bake.
     assert container.volume == 0
     results = recipe.bake()
     new_salt_water = results[salt_water.name]
     container = results[container.name]
-    assert container.volume == Unit.convert_to_storage(10, 'mL')
-    assert salt_water.volume - new_salt_water.volume == Unit.convert_to_storage(10, 'mL')
+    assert container.get_volume(unit='mL') == 10
+    assert salt_water.get_volume(unit='mL') - new_salt_water.get_volume(unit='mL') == 10
 
     # transfer() cannot ba called once the recipe is baked.
     with pytest.raises(RuntimeError, match="This recipe is locked"):
         recipe.transfer(salt_water, container, '10 mL')
     recipe = Recipe()
     plate = Plate('plate', max_volume_per_well='1 mL')
     recipe.uses(salt_water, plate)
     recipe.transfer(salt_water, plate, '5 uL')
     recipe.transfer(salt_water, plate[1, 1], '1 uL')
     results = recipe.bake()
     new_salt_water = results[salt_water.name]
     new_plate = results[plate.name]
     # 5 uL transferred to 96 wells and 1 uL to one well.
-    assert salt_water.volume - new_salt_water.volume == pytest.approx(Unit.convert_to_storage(5 * 96 + 1, 'uL'))
-    volumes = new_plate.volumes(unit='uL')
+    assert salt_water.get_volume(unit='uL') - new_salt_water.get_volume(unit='uL') == pytest.approx(5 * 96 + 1)
+    volumes = new_plate.get_volumes(unit='uL')
     # plate[1, 1] should have 6 uL, all others 5 uL
     assert volumes[0, 0] == 6
     assert volumes[0, 1] == 5
 
     container = Container('container')
     recipe = Recipe()
     recipe.uses(container, new_plate)
     recipe.transfer(new_plate[1, 1], container, '2 uL')
     recipe.transfer(new_plate[1:2, 1:2], container, '1 uL')
     results = recipe.bake()
     container = results[container.name]
     new_plate2 = results[new_plate.name]
     # 2 uL from plate[1, 1] and 1 uL from four wells.
-    assert container.volume == Unit.convert_to_storage(2 + 4, 'uL')
-    assert new_plate.volume('uL') - new_plate2.volume('uL') == 2 + 4
+    assert container.get_volume('uL') == 2 + 4
+    assert new_plate.get_volume('uL') - new_plate2.get_volume('uL') == 2 + 4
 
 
 def test_create_container(water, salt):
     """
 
     Test create_container within a Recipe.
 
@@ -153,9 +153,9 @@
     container3 = recipe.create_container('container3', initial_contents=[(water, '10 mL'), (salt, '5 mmol')])
     recipe.used = set(recipe.results.keys())
     assert container3.volume == 0
     results = recipe.bake()
     container = results[container.name]
     container2 = results[container2.name]
     container3 = results[container3.name]
-    assert Unit.convert_to_storage(10, 'mL') + Unit.convert(salt, '5 mmol', config.volume_prefix) == container3.volume
+    assert 10 + Unit.convert(salt, '5 mmol', 'mL') == container3.get_volume(unit='mL')
     assert container3.contents.get(salt, None) == Unit.convert_to_storage(5, 'mmol')
```

### Comparing `pyplate-hte-0.4/tests/test_Slicer.py` & `pyplate-hte-0.4.1/tests/test_Slicer.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4/tests/test_Substance.py` & `pyplate-hte-0.4.1/tests/test_Substance.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4/tests/test_convert.py` & `pyplate-hte-0.4.1/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `pyplate-hte-0.4/tests/test_create_solution.py` & `pyplate-hte-0.4.1/tests/test_create_solution.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,46 +16,46 @@
     """
     solvents = [water, dmso]
     solutes = [salt, triethylamine, sodium_sulfate]
     units = ['g', 'mol', 'mL']
     for numerator, denominator, quantity_unit in product(units, repeat=3):
         for solute in solutes:
             for solvent in solvents:
-                if numerator == 'mL' and solute.is_solid() and config.default_density == float('inf'):
+                if numerator == 'mL' and solute.is_solid() and config.default_solid_density == float('inf'):
                     continue
                 con = Container.create_solution(solute, solvent, concentration=f"0.001 {numerator}/{denominator}",
                                                 total_quantity=f"10 {quantity_unit}")
                 assert all(value > 0 for value in con.contents.values())
-                total = sum(Unit.convert(substance, f"{value} {config.moles_prefix}", quantity_unit) for
+                total = sum(Unit.convert(substance, f"{value} {config.moles_storage_unit}", quantity_unit) for
                             substance, value in con.contents.items())
                 assert abs(total - 10) < epsilon, f"Making 10 {quantity_unit} of a 0.001 {numerator}/{denominator}" \
                                                   f" solution of {solute} and {solvent} failed."
-                conc = Unit.convert(solute, f"{con.contents[solute]} {config.moles_prefix}", numerator) / \
-                    sum(Unit.convert(substance, f"{value} {config.moles_prefix}", denominator)
+                conc = Unit.convert(solute, f"{con.contents[solute]} {config.moles_storage_unit}", numerator) / \
+                       sum(Unit.convert(substance, f"{value} {config.moles_storage_unit}", denominator)
                         for substance, value in con.contents.items())
                 assert abs(conc - 0.001) < epsilon
 
                 con = Container.create_solution(solute, solvent, concentration=f"0.01 {numerator}/10 {denominator}",
                                                 total_quantity=f"10 {quantity_unit}")
-                total = sum(Unit.convert(substance, f"{value} {config.moles_prefix}", quantity_unit) for
+                total = sum(Unit.convert(substance, f"{value} {config.moles_storage_unit}", quantity_unit) for
                             substance, value in con.contents.items())
                 assert abs(total - 10) < epsilon
-                conc = Unit.convert(solute, f"{con.contents[solute]} {config.moles_prefix}", numerator) / \
-                    sum(Unit.convert(substance, f"{value} {config.moles_prefix}", denominator)
+                conc = Unit.convert(solute, f"{con.contents[solute]} {config.moles_storage_unit}", numerator) / \
+                       sum(Unit.convert(substance, f"{value} {config.moles_storage_unit}", denominator)
                         for substance, value in con.contents.items())
                 assert abs(conc - 0.01/10) < epsilon
 
     # Solute is an enzyme, concentration has U in the numerator
     solute = lipase
     for denominator, quantity_unit in product(units, repeat=2):
         for solvent in solvents:
             con = Container.create_solution(solute, solvent, concentration=f"1.1 U/{denominator}",
                                             total_quantity=f"10 {quantity_unit}")
             assert all(value > 0 for value in con.contents.values())
-            total = sum(Unit.convert(substance, f"{value} {config.moles_prefix}", quantity_unit) for
+            total = sum(Unit.convert(substance, f"{value} {config.moles_storage_unit}", quantity_unit) for
                         substance, value in con.contents.items())
             assert abs(total - 10) < epsilon, f"Making 10 {quantity_unit} of a 1.1 U/{denominator}" \
                                               f" solution of {solute} and {solvent} failed."
             conc = con.contents[solute] / \
-                sum(Unit.convert(substance, f"{value} {config.moles_prefix}", denominator)
+                sum(Unit.convert(substance, f"{value} {config.moles_storage_unit}", denominator)
                     for substance, value in con.contents.items())
             assert abs(conc - 1.1) < epsilon
```

### Comparing `pyplate-hte-0.4/tests/test_dilute.py` & `pyplate-hte-0.4.1/tests/test_dilute.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,11 +16,11 @@
     units = ['g', 'mol', 'mL']
     for numerator, denominator, quantity_unit in product(units, repeat=3):
         for solute in solutes:
             for solvent in solvents:
                 con = Container.create_solution(solute, solvent, concentration=f"0.001 {numerator}/{denominator}",
                                                 total_quantity=f"10 {quantity_unit}")
                 con2 = con.dilute(solute, f'0.0005 {numerator}/{denominator}', solvent)
-                new_concentration = Unit.convert(solute, f"{con2.contents[solute]} {config.moles_prefix}", numerator) / \
-                                    sum(Unit.convert(substance, f"{value} {config.moles_prefix}", denominator)
+                new_concentration = Unit.convert(solute, f"{con2.contents[solute]} {config.moles_storage_unit}", numerator) / \
+                                    sum(Unit.convert(substance, f"{value} {config.moles_storage_unit}", denominator)
                                         for substance, value in con2.contents.items())
                 assert new_concentration == pytest.approx(0.0005)
```

### Comparing `pyplate-hte-0.4/tests/test_recipe_amount_used.py` & `pyplate-hte-0.4.1/tests/test_recipe_amount_used.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-import numpy as np
 
+import numpy as np
+import pdb
 from pyplate.pyplate import Recipe, Container, Plate
 import pytest
+import logging 
+
+# Set up logging
+
 
 
-def test_amount_used(water, salt):
+def test_substance_used(water, salt):
     container = Container('container')
     salt_water = Container.create_solution(salt, water, concentration='1 M', total_quantity='100 mL')
     recipe = Recipe()
     recipe.uses(salt_water, container)
     recipe.transfer(salt_water, container, '10 mL')
     recipe.bake()
-    assert recipe.amount_used(substance=salt, timeframe='all', unit='mmol', destinations=[container]) == 10.0
+    assert recipe.substance_used(substance=salt, timeframe='all', unit='mmol', destinations=[container]) == 10.0
 
 
 def test_recipe_tracking_before(water):
     """
     Verify initial and mid-recipe substance volumes in a Recipe context.
 
     This test ensures accurate tracking of a substance's volume both before and during recipe execution, 
@@ -51,56 +56,74 @@
 
     recipe.bake()
     # Assertions
     step = recipe.steps[-1]
 
     print(step.frm)
     print(step.to)
-    assert recipe.amount_used(substance=water, timeframe='all', unit='mL') == 10.0
-    assert recipe.amount_used(substance=water, timeframe='dispensing', unit='mL') == 5.0
+    assert recipe.substance_used(substance=water, unit='mL', destinations=[container]) == 5.0
+    
 
 
 def test_container_to_plate(triethylamine, empty_plate):
     # TODO: double check volumes here
     """
     Tests the transfer of a substance from a container to a plate within a Recipe context.
 
-    This test verifies the correct volume handling and substance tracking during the transfer process in a recipe. It involves creating a container with a specified initial volume of triethylamine, transferring a portion of this volume to an empty plate, and then baking the recipe to finalize all operations.
+    This test verifies the correct volume handling and substance tracking during the transfer
+      process in a recipe. It involves creating a container with a specified initial volume 
+      of triethy-lamine, transferring a portion of this volume to an empty plate, and then
+      baking the recipe to finalize all operations.
 
     The test checks three main aspects:
-    - The volume of the source container (`container`) decreases by the transferred volume, expecting a reduction to '9.9 mL' from an initial '10 mL' after transferring '100 uL'.
-    - The volume of the destination plate (`empty_plate`) increases to match the transferred volume, expected to be '100 uL'.
-    - The amount of triethylamine used during the recipe matches the transferred volume, ensuring substance tracking aligns with the transfer operation.
+    - The volume of the source container (`container`) decreases by the transferred volume, expecting a
+      reduction to '9.9 mL' from an initial '10 mL' after transferring '100 uL'.
+    - The volume of the destination plate (`empty_plate`) increases to match the transferred volume, 
+    expected to be '100 uL'.
+    - The amount of triethylamine used during the recipe matches the transferred volume, 
+    ensuring substance tracking aligns with the transfer operation.
 
     Parameters:
     - triethylamine (Substance): A fixture providing triethylamine, the substance being transferred.
     - empty_plate (Plate): A fixture providing an empty plate, the destination for the transfer.
 
-    The test outputs the initial volume of the container, the source and destination of the final transfer step, and an related print statements. It asserts that the final volumes and substance usage match expected values.
+    The test outputs the initial volume of the container, the source and 
+    destination of the final transfer step, and an related print statements. It asserts 
+    that the final volumes and substance usage match expected values.
     """
 
     # create_recipe
     recipe = Recipe()
 
     # define initial and transfer volumes
     initial_volume = '10 mL'
     transfer_volume = '100 uL'
 
+    #define destinations
+    
     # define initial contents and create container
     initial_contents = [(triethylamine, initial_volume)]
-    container = recipe.create_container('container', max_volume='20 mL', initial_contents=initial_contents)
+    container = recipe.create_container('container', max_volume='20 mL', 
+                                        initial_contents=initial_contents)
 
     # Test if container.volume is correct intially
     assert container.volume == 0
 
     # Make sure that the recipe uses empty_plate
     recipe.uses(empty_plate)
 
+    #start first stage
+    recipe.start_stage('transfer_stage')
     recipe.transfer(container, empty_plate, transfer_volume)
+    recipe.end_stage('transfer_stage')
+
+    # Bake the recipe
     results = recipe.bake()
+
+    # Get the containers from the results
     container = results[container.name]
     plate = results[empty_plate.name]
 
     # Calculate expected volume
     expected_volume_plate = 400
     expected_volume_container = 400
 
@@ -108,25 +131,30 @@
     step = recipe.steps[-1]
 
     print(step.frm)
     print(step.to)
 
     print("Assertions start here")
 
-    assert pytest.approx(container.volume) == expected_volume_plate
-    assert (np.full((8, 12), expected_volume_container) == plate.volumes(unit='uL')).all()
-    assert pytest.approx(
-        recipe.amount_used(substance=triethylamine, timeframe='dispensing', unit='uL')) == expected_volume_plate
+    #Since 9600 muL is in the plate, the volume of the container should be 400 muL
+    assert pytest.approx(container.volume) == 400
+    
+    
+    #assert (np.full((8, 12), expected_volume_container) == plate.volumes(unit='uL')).all()
+    #100 muL is transferred to 96 wells in the plate, hence total expected value is 9600
+    assert pytest.approx(recipe.substance_used(substance=triethylamine, timeframe='transfer_stage', unit='uL', destinations=[empty_plate])) == 9600.0
+    # assert pytest.approx(
+    #     recipe.substance_used(substance=triethylamine, timeframe='dispensing', unit='uL')) == expected_volume_plate
 
 
-def test_amount_used_dilute(salt, water):
+def test_substance_used_dilute(salt, water):
     """
     Tests that the substance amount tracking is correctly tracked during dilution in a recipe.
 
-    This test checks the `amount_used` method  to correctly report the amount of salt used after diluting a saltwater solution. The procedure involves:
+    This test checks the `substance_used` method  to correctly report the amount of salt used after diluting a saltwater solution. The procedure involves:
     - Declaring a container with saltwater as part of a recipe.
     - Adding a specific amount of salt to increase the solution's concentration.
     - Diluting the solution to a target molarity of '0.5 M' using water.
     - Baking the recipe to complete the process.
 
     It asserts that:
     - The total amount of salt reported as used matches the expected '50 mmol', despite the dilution.
@@ -144,69 +172,82 @@
     # Create recipe
     recipe = Recipe()
 
     # container = recipe.create_container('container', '20 mL', [(salt_water, '10 mL')])
 
     # Define what the recipe uses
     recipe.uses(container)
-    salt_solution = recipe.create_solution(salt, water, concentration='0.5 M', total_quantity='20 mL')
+    salt_solution = recipe.create_solution(salt, water, concentration='0.5 M', 
+                                           total_quantity='20 mL')
     # container._add(salt_water, '10 mL')
 
+    # Transfer 10 mL of salt solution to container
+    recipe.start_stage('dilution_stage')
     recipe.transfer(salt_solution, container, '10 mL')
 
     # Add solute to recipe
     # container = container._add(salt, '50 mmol') #Does not do anything as the container that is used in the recipe is the one that was stored initially
     recipe.dilute(container, solute=salt, concentration='0.25 M', solvent=water)
+
+    
+    recipe.end_stage('dilution_stage')
+
+
     recipe.bake()
 
     assert container.volume == 0
     # Results would contain the pointers to the new containers, so assert from there
 
     expected_salt_amount = 5.0
-    assert recipe.amount_used(substance=salt, timeframe='dispensing', unit='mmol') == expected_salt_amount
+    assert recipe.substance_used(substance=salt, destinations=[container],timeframe='dilution_stage', unit='mmol') == expected_salt_amount
 
 
 # Testing create_solution
-def test_amount_used_create_solution(salt, water):
+def test_substance_used_create_solution(salt, water, empty_plate):
     """
     Tests that the substance amount tracking is accurately implemented during the creation of a solution within a recipe.
 
-    This test verifies the `amount_used` method to correctly report the amount of salt utilized in preparing a specific solution. The testing procedure includes:
+    This test verifies the `substance_used` method to correctly report the amount of salt utilized in preparing a specific solution. The testing procedure includes:
     - Initiating a recipe and declaring the usage of salt and water as solute and solvent, respectively.
     - Creating a solution with a predefined concentration of '0.5 M' and a total quantity of '20 mL', effectively dissolving the salt within the water.
     - Executing the `bake` method to finalize the creation of the solution.
 
     The assertions made are:
     - The initial volume of the container is checked before the solution creation, ensuring it starts from a baseline of zero.
-    - The amount of salt reported as used during the recipe matches the expected calculation, which is '10 mmol' for achieving the desired solution concentration and volume. This confirms the `amount_used` method's accuracy in reflecting substance usage throughout the recipe's actions.
+    - The amount of salt reported as used during the recipe matches the expected calculation, which is '10 mmol' for achieving the desired solution concentration and volume. This confirms the `substance_used` method's accuracy in reflecting substance usage throughout the recipe's actions.
 
     Parameters:
     - salt (Substance): The salt intended to be dissolved to create the solution.
     - water (Substance): The water used as a solvent for the solution.
 
     """
 
     # Create recipe
     recipe = Recipe()
     recipe.uses(salt, water)
 
+
+
     # Create solution and add to container
-    container = recipe.create_solution(salt, water, concentration='0.5 M', total_quantity='20 mL')
+    recipe.start_stage('stage1')
+    container = recipe.create_solution(salt, water, concentration='0.1 M', total_quantity='20 mL')
     ##What is the initial volume of container here?
     assert container.volume == 0
+    recipe.transfer(container, empty_plate, '10 mL')
+    recipe.end_stage('stage1')
 
     # Bake recipe
     recipe.bake()
 
     # Assertions
     expected_salt_amount = 10.0
-    assert recipe.amount_used(substance=salt, timeframe='all', unit='mmol') == expected_salt_amount
+    assert recipe.substance_used(substance=salt, unit='mmol', destinations=[container], timeframe='stage1') == expected_salt_amount
 
 # Try substance with solid and liquid
-def test_amount_used_create_solution_from(salt, water, triethylamine):
+def test_substance_used_create_solution_from(salt, water, triethylamine):
     """
     Tests accurate tracking of salt usage when creating a new solution from an existing diluted solution.
 
     This test simulates the scenario of diluting an existing salt solution with a different solvent (triethylamine) to create a new solution with the same concentration. The test procedure involves:
     - Creating an initial salt solution with a specified concentration and total quantity.
     - Creating a new solution from this initial solution, aiming to maintain the same concentration but with a different solvent, and specifying a unique name for the new container.
     - Baking the recipe to apply all declared operations.
@@ -221,49 +262,63 @@
     - water (Substance): The solvent for the initial solution.
     - triethylamine (Substance): The solvent for the new solution created from the existing one.
     """
    # Creating solution from a diluted solution
     recipe = Recipe()
     
     # Create initial solution and add to container
+    recipe.start_stage('stage1')
     initial_container_name = "initial_salt_solution"
     container = recipe.create_solution(salt, water, concentration='1 M', total_quantity='20 mL', name=initial_container_name)
     
+    recipe.end_stage('stage1')
+
+    recipe.start_stage('stage2')
     # Create solution from the initial one with a new solvent
     new_container_name = "new_solution_from_initial"
-    new_container = recipe.create_solution_from(container, solute=salt, concentration='0.5 M', 
-                                                          solvent=triethylamine, quantity='20 mL', name=new_container_name)
+    #pdb.set_trace()
+    new_container = recipe.create_solution_from(source=container, solute=salt, concentration='0.5 M', 
+                                                          solvent=water, quantity='10 mL', name=new_container_name)
     
     # Bake recipe to finalize
+
+    recipe.end_stage('stage2')
     results = recipe.bake()
 
     new_container = results[new_container.name]
     # Assertions for substance amount used and container volumes
-    expected_salt_amount = 10
-    assert recipe.amount_used(substance=salt, timeframe='during', unit='mmol') == expected_salt_amount, "The reported amount of salt used does not match the expected value."
+    expected_salt_amount_stage1 = 20.0
+    expected_salt_amount_stage2 = 0.0
+    #If destination for stage2 was new_container, then expected_salt_amount_stage2 would be 10.0
+
+    assert recipe.substance_used(substance=salt, timeframe='stage1', unit='mmol', destinations=[container,new_container]) == expected_salt_amount_stage1, "The reported amount of salt used does not match the expected value."
+    assert recipe.substance_used(substance=salt, timeframe='stage2', unit='mmol',destinations=[container,new_container]) == expected_salt_amount_stage2, "The reported amount of salt used does not match the expected value."
     #assert residual == 0, "Expected residual volume to be 0 after creating new solution."
     
-    assert new_container.volume == 20 , "Expected new container volume to match the specified total quantity for the new solution."
+
+    #Default unit is not Ml, so it shall be failing. Use Unit to change the units
+    #Changed it to check for millimoles
+    assert new_container.volume == 10000 , "Expected new container volume to match the specified total quantity for the new solution."
 
 
-def test_amount_used_remove(salt_water, salt):
+def test_substance_used_remove(salt_water, salt):
     """
     Tests the accuracy of substance amount tracking during the removal of a solution in a recipe.
 
-    This test verifies the `amount_used` method for correctly reporting the amount of salt removed from a container. The procedure includes:
+    This test verifies the `substance_used` method for correctly reporting the amount of salt removed from a container. The procedure includes:
     - Creating a recipe and a container with an initial volume of '20 mL' of saltwater, implying a certain concentration of salt.
     - Removing '10 mL' of the saltwater from the container, which would also remove a proportional amount of salt based on the solution's concentration.
     - Baking the recipe to finalize the removal process.
 
     The test asserts:
     - The amount of salt removed during the recipe matches the expected value based on the initial concentration and the volume removed. The expected salt amount should logically reflect the proportion of salt in the removed volume, which, in a homogenous solution, would be half of the initial amount if '20 mL' contained '50 mmol' of salt.
 
     Parameters:
     - salt_water (Container): A fixture representing the saltwater solution to be partially removed.
-    - salt (Substance): The salt substance, expected to be tracked through the `amount_used` method.
+    - salt (Substance): The salt substance, expected to be tracked through the `substance_used` method.
     """
 
     # Create recipe
     recipe = Recipe()
 
     # Deine initial contents
     initial_contents = [(salt, '50 mmol')]
@@ -276,71 +331,18 @@
     recipe.remove(container, salt)
 
     # Bake recipe
     recipe.bake()
 
     # Assertions
     expected_salt_amount = 0.0
-    assert recipe.amount_used(substance=salt, timeframe='dispensing', unit='mmol') == expected_salt_amount
+    assert recipe.substance_used(substance=salt,destinations=[container],unit='mmol') == expected_salt_amount
 
 
-def test_amount_used_with_no_usage(salt):
-
-    """
-    Verifies that the amount of a substance reported as used is zero when the substance is not utilized in the recipe.
-
-    This test case is designed to confirm the functionality of the `amount_used` method in scenarios where a specific substance is declared for a recipe but not actually used in any of the recipe steps. The key actions in this test include:
-    - Initiating a recipe without adding any steps that involve the use of the specified substance (salt, in this case).
-    - Finalizing the recipe preparation process by baking the recipe.
-    
-    The assertion checks:
-    - That the `amount_used` method correctly reports '0 mmol' for the salt, reflecting that it was not used during the recipe's preparation, thus ensuring accurate tracking of substance usage within the recipe.
-
-    Parameters:
-    - salt (Substance): The substance fixture representing salt, intended to verify the tracking of substance usage.
-    """
-
-    recipe = Recipe()
-    # No usage of salt
-    recipe.bake()
-    # Expecting 0 usage since salt wasn't used
-    assert recipe.amount_used(substance=salt, timeframe='all', unit='mmol') == 0.0
-
-
-def test_amount_used_incorrect_timeframe(salt_water, salt, empty_plate):
-    """
-    Ensures an error is raised when querying the amount of substance used with an unsupported timeframe.
-
-    This test aims to verify the error handling capabilities of the `amount_used` method within the `Recipe` class, particularly when an invalid or unsupported timeframe is specified. The test follows these steps:
-    - Initializes a recipe and declares the use of a saltwater solution.
-    - Transfers a specified volume of the saltwater solution to a plate, simulating a typical recipe action.
-    - Completes the recipe by invoking the `bake` method.
-    
-    The critical part of this test is the assertion that checks:
-    - A `ValueError` is raised when attempting to call `amount_used` with a timeframe argument that the method does not support (`'later'` in this case). The error message is expected to match "Unsupported timeframe," indicating that the method correctly identifies and rejects invalid timeframe inputs.
-
-    Parameters:
-    - salt_water (Container): A fixture representing the saltwater solution used in the recipe.
-    - salt (Substance): The substance fixture representing salt, intended to be tracked within the recipe.
-    - plate (Plate): A fixture representing a plate, to which the saltwater solution is transferred as part of the recipe.
-    """
-    recipe = Recipe()
-    container = Container('container')
-    recipe.uses(salt_water, container)
-    recipe.uses(empty_plate)
-    recipe.transfer(salt_water, empty_plate, '10 uL')
-    recipe.transfer(salt_water, container, '10 uL')
-    recipe.bake()
-
-    # Raising errors for unexpected timeframes
-    with pytest.raises(ValueError, match="Invalid timeframe"):
-        recipe.amount_used(substance=salt, timeframe='later', unit='mmol')
-
-
-def test_stages(water):
+def test_stages_subst(water):
     
     """
     Tests tracking of water usage across recipe stages, focusing on water
     transfers within a specific stage and overall recipe operations.
 
     This test evaluates the functionality of defining, executing, and tracking
     operations within named stages of a recipe using the `Recipe` class. It
@@ -368,16 +370,14 @@
       preparation.
     """
 
 
     recipe = Recipe()
 
     recipe.start_stage('stage1')
-    other_container = Container('other container')
-    recipe.uses(other_container)
     other_container = recipe.create_container('other container')
 
     # Add solute and solvent to the create_solution method
     initial_contents = [(water, '20 mL')]
 
     # Implicit definition of container being used
     container = recipe.create_container('container', '20 mL', initial_contents)
@@ -388,16 +388,17 @@
     
     recipe.end_stage('stage1')
     recipe.transfer(container, other_container, '2 mL')
     recipe.bake()
 
 
     destination_container = [other_container]
-    assert recipe.amount_used(water, timeframe='stage1', unit='mL') == 15.0
-    assert recipe.amount_used(water, timeframe='all', unit='mL') == 17.0
+    assert recipe.substance_used(water, timeframe='stage1', destinations=[container], unit='mL') == 5.0
+    assert recipe.substance_used(water, timeframe='stage1', destinations=[container, other_container], unit='mL') == 20.0
+    assert recipe.substance_used(water, timeframe='all', unit='mL') == 0.0
 
 
 def test_stages_2(water):
     """
     Tests water usage across containers and stages within a recipe, ensuring
     accurate tracking of water volume.
 
@@ -428,37 +429,37 @@
     - Asserts the water usage within 'stage1' and across specified containers
       aligns with expected actions taken during this stage.
 
     Parameters:
     - water (Substance): Represents the water used in the recipe's operations.
     """
     recipe = Recipe()
-    container1 = container1 = recipe.create_container(initial_contents=(water, "10mL"))
+    container1 = recipe.create_container(name='container1',initial_contents=[(water, "10 mL")])
     plate1 = Plate('plate1', '100 uL')
     plate2 = Plate('plate2', '100 uL')
-    recipe.uses(container1, plate1, plate2)
+    recipe.uses(plate1, plate2)
 
-    recipe.transfer(source=container1, dest=plate1, volume='2 mL')
+    recipe.transfer(source=container1, destination=plate1, quantity='10 uL')
 
     #fill the first cell in plate
-    recipe.fill_to(plate1[1,1],solvent=water, quantity='20 mL')
+    recipe.fill_to(plate1[1,1],solvent=water, quantity='20 uL')
 
     #start a new stage
     recipe.start_stage('stage1')
-    recipe.transfer(source=plate1, dest=plate2, volume='1 mL')
-    recipe.remove(water, plate2)
+    recipe.transfer(source=plate1, destination=plate2, quantity='1 uL')
+    recipe.remove(plate2, water)
     recipe.end_stage('stage1')
 
     #bake the recipe
     recipe.bake()
-    assert recipe.amount_used(water, timeframe='all', unit='mL', dest = [container1,plate1, plate2]) == 30.0
-    assert recipe.amount_used(water, timeframe='all', unit='mL', dest = [plate1, plate2]) == 22.0
-    #assert recipe.amount_used(water, timeframe='stage1', unit='mL', dest = [plate1, plate2]) == -1.0
-    assert recipe.amount_used(water, timeframe='all', unit='mL', dest = [plate1, plate2]) == 0.0
-    assert recipe.amount_used(water, timeframe='all', unit='mL', dest = [plate2]) == 1
+    assert recipe.substance_used(water, timeframe='all', unit='mL', dest = [container1,plate1, plate2]) == 30.0
+    assert recipe.substance_used(water, timeframe='all', unit='mL', dest = [plate1, plate2]) == 22.0
+    #assert recipe.substance_used(water, timeframe='stage1', unit='mL', dest = [plate1, plate2]) == -1.0
+    assert recipe.substance_used(water, timeframe='all', unit='mL', dest = [plate1, plate2]) == 0.0
+    assert recipe.substance_used(water, timeframe='all', unit='mL', dest = [plate2]) == 1
 
 
 def test_stages_dilute(water, salt):
     """
     Tests the dilution process across different stages within a recipe, focusing on a specific stage's volume and substance usage tracking.
 
     This test assesses the `Recipe` class's ability to handle complex procedures involving the creation of solutions, 
@@ -484,15 +485,15 @@
 
     Parameters:
     - water (Substance): The solvent used for creating solutions and performing dilution, representing water.
     - salt (Substance): The solute used for creating the initial solution, representing salt.
     """
     recipe = Recipe()
     container1 = recipe.create_solution(salt, water, concentration='1 M', total_quantity='10 mL')
-    water_stock = recipe.create_container(intial_contents=(water, "10 mL"))
+    water_stock = recipe.create_container(initial_contents=(water, "10 mL"))
 
     plate1 = Plate('plate1', '100 uL')
     plate2 = Plate('plate2', '100 uL')
     recipe.uses(plate1, plate2)
 
     recipe.transfer(source=container1, dest=plate1, volume='2 mL')
     recipe.start_stage('stage1')
@@ -502,12 +503,66 @@
     recipe.remove(water, plate2)
 
     recipe.end_stage('stage1')
 
     recipe.bake()
 
     #Assertions
-    assert recipe.amount_used(water, timeframe='stage1', unit='mL', ) == 2.0
+    assert recipe.substance_used(water, timeframe='stage1', unit='mL', ) == 2.0
+
+
+
+
+def test_substance_used_with_no_usage(salt):
+
+    """
+    Verifies that the amount of a substance reported as used is zero when the substance is not utilized in the recipe.
+
+    This test case is designed to confirm the functionality of the `substance_used` method in scenarios where a specific substance is declared for a recipe but not actually used in any of the recipe steps. The key actions in this test include:
+    - Initiating a recipe without adding any steps that involve the use of the specified substance (salt, in this case).
+    - Finalizing the recipe preparation process by baking the recipe.
+    
+    The assertion checks:
+    - That the `substance_used` method correctly reports '0 mmol' for the salt, reflecting that it was not used during the recipe's preparation, thus ensuring accurate tracking of substance usage within the recipe.
+
+    Parameters:
+    - salt (Substance): The substance fixture representing salt, intended to verify the tracking of substance usage.
+    """
 
+    recipe = Recipe()
+    # No usage of salt
+    recipe.bake()
+    # Expecting 0 usage since salt wasn't used
+    assert recipe.substance_used(substance=salt, timeframe='all', unit='mmol') == 0.0
+
+
+def test_substance_used_incorrect_timeframe(salt_water, salt, empty_plate):
+    """
+    Ensures an error is raised when querying the amount of substance used with an unsupported timeframe.
+
+    This test aims to verify the error handling capabilities of the `substance_used` method within the `Recipe` class, particularly when an invalid or unsupported timeframe is specified. The test follows these steps:
+    - Initializes a recipe and declares the use of a saltwater solution.
+    - Transfers a specified volume of the saltwater solution to a plate, simulating a typical recipe action.
+    - Completes the recipe by invoking the `bake` method.
+    
+    The critical part of this test is the assertion that checks:
+    - A `ValueError` is raised when attempting to call `substance_used` with a timeframe argument that the method does not support (`'later'` in this case). The error message is expected to match "Unsupported timeframe," indicating that the method correctly identifies and rejects invalid timeframe inputs.
+
+    Parameters:
+    - salt_water (Container): A fixture representing the saltwater solution used in the recipe.
+    - salt (Substance): The substance fixture representing salt, intended to be tracked within the recipe.
+    - plate (Plate): A fixture representing a plate, to which the saltwater solution is transferred as part of the recipe.
+    """
+    recipe = Recipe()
+    container = Container('container')
+    recipe.uses(salt_water, container)
+    recipe.uses(empty_plate)
+    recipe.transfer(salt_water, empty_plate, '10 uL')
+    recipe.transfer(salt_water, container, '10 uL')
+    recipe.bake()
 
+    # Raising errors for unexpected timeframes
+    with pytest.raises(ValueError, match="Invalid timeframe"):
+        recipe.substance_used(substance=salt, timeframe='later', unit='mmol')
 
     
+
```

### Comparing `pyplate-hte-0.4/tests/test_transfers.py` & `pyplate-hte-0.4.1/tests/test_transfers.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,86 +33,86 @@
     solution1_volume = 100 + Unit.convert(salt, '50 mmol', 'mL')
     solution2_volume = 100 + Unit.convert(sodium_sulfate, '50 mmol', 'mL')
     solution3, solution4 = Container.transfer(solution1, solution2, f"{solution1_volume*0.1} mL")
     # original solutions should be unchanged
     assert solution1.volume == Unit.convert_to_storage(solution1_volume, 'mL')
     assert solution2.volume == Unit.convert_to_storage(solution2_volume, 'mL')
     # 10 mL of water and 5 moles of salt should have been transferred
-    assert solution3.volume == Unit.convert_to_storage(solution1_volume*0.9, 'mL')
+    assert solution3.get_volume(unit='mL') == solution1_volume * 0.9
     assert solution4.volume == Unit.convert_to_storage(solution2_volume + solution1_volume*0.1, 'mL')
-    assert solution3.contents[water] == Unit.convert(water, '90 mL', config.moles_prefix)
-    assert solution3.contents[salt] == Unit.convert(salt, '45 mmol', config.moles_prefix)
-    assert solution4.contents[water] == pytest.approx(Unit.convert(water, '10 mL', config.moles_prefix))
-    assert solution4.contents[salt] == Unit.convert(salt, '5 mmol', config.moles_prefix)
+    assert solution3.contents[water] == Unit.convert(water, '90 mL', config.moles_storage_unit)
+    assert solution3.contents[salt] == Unit.convert(salt, '45 mmol', config.moles_storage_unit)
+    assert solution4.contents[water] == pytest.approx(Unit.convert(water, '10 mL', config.moles_storage_unit))
+    assert solution4.contents[salt] == Unit.convert(salt, '5 mmol', config.moles_storage_unit)
 
 
 def test_transfer_to_slice(plate1, solution1, salt):
     """
     Tests transferring from a container to each well in a slice.
     """
     solution1_volume = 100 + Unit.convert(salt, '50 mmol', 'mL')
-    to_transfer = solution1_volume / 100
+    to_transfer = round(solution1_volume / 100, 3)
     solution3, plate3 = Plate.transfer(solution1, plate1[:], f"{to_transfer} mL")
     # 1 mL of water should have been transferred to each well in the plate
-    assert plate3.volume() == pytest.approx(plate3[:].size * 1000 * to_transfer)  # volume() is in uL
-    assert numpy.allclose(plate3.volumes(unit='mL'), numpy.ones(plate3.wells.shape) * to_transfer)
+    assert plate3.get_volume(unit='uL') == pytest.approx(plate3[:].size * 1000 * to_transfer, abs=3)  # volume() is in uL
+    assert numpy.allclose(plate3.get_volumes(unit='mL'), numpy.ones(plate3.wells.shape) * to_transfer)
     # assert numpy.all(numpy.vectorize(lambda elem: abs(elem.volume - to_transfer) < epsilon)(plate3.wells))
     # Original solution and plate should be unchanged
     assert solution1.volume == Unit.convert_to_storage(solution1_volume, 'mL')
-    assert plate1.volume() == 0
+    assert plate1.get_volume() == 0
 
     solution4, plate4 = Plate.transfer(solution1, plate1[1, 1], f"{to_transfer} mL")
-    assert plate4.volume() == pytest.approx(1000 * to_transfer)
-    assert solution1.volume - solution4.volume == pytest.approx(Unit.convert_to_storage(to_transfer, 'mL'))
+    assert plate4.get_volume() == pytest.approx(1000 * to_transfer)
+    assert solution1.get_volume(unit='mL') - solution4.get_volume(unit='mL') == pytest.approx(to_transfer)
 
 
 def test_transfer_between_slices(plate1, plate2, solution1, solution2):
     """
     Tests transfer from the wells in one slice to the wells in another.
     """
     left_over_solution, plate3 = Plate.transfer(solution1, plate1[1, 1], '10 mL')
-    initial_volumes = plate3.volumes().copy()
+    initial_volumes = plate3.get_volumes().copy()
     # 10 mL of solution should in the first well
     assert initial_volumes[0, 0] == 10 * 1000
     plate4, _ = Plate.transfer(plate3[1, 1], plate3[8:], '0.1 mL')
-    volumes = plate4.volumes()
+    volumes = plate4.get_volumes()
     intended_result_volumes = numpy.zeros(volumes.shape)
     # Solution should have been transferred between
     #   the first well and the last row
     intended_result_volumes[0, 0] = (10 - 0.1 * 12) * 1000
     intended_result_volumes[7:] = 0.1 * 1000
     assert numpy.array_equal(volumes, intended_result_volumes)
     # Plate3 should not have been modified
-    assert numpy.array_equal(initial_volumes, plate3.volumes())
+    assert numpy.array_equal(initial_volumes, plate3.get_volumes())
 
     # Plate with first row containing 1mL of solution1
     left_over_solution1, plate5 = Plate.transfer(solution1, plate1[:1], '1 mL')
     # Plate with last row containing 2mL of solution2
     left_over_solution2, plate6 = Plate.transfer(solution2, plate2[8:], '2 mL')
     # Expected starting volumes
-    assert plate5.volume() == 12 * 1000 and plate6.volume() == 24 * 1000
+    assert plate5.get_volume() == 12 * 1000 and plate6.get_volume() == 24 * 1000
     plate7, plate8 = Plate.transfer(plate5[:1], plate6[8:], '1 mL')
     # From plate should be empty
-    assert plate7.volume() == 0
+    assert plate7.get_volume() == 0
     intended_result_volumes = numpy.zeros(plate8[:].shape)
     intended_result_volumes[7:] = 3 * 1000
     # Last row should have 3 mL in each well
-    assert numpy.array_equal(intended_result_volumes, plate8.volumes())
+    assert numpy.array_equal(intended_result_volumes, plate8.get_volumes())
 
 
 def test_transfer_from_slice(plate1, solution1):
     """
     Tests transferring from each well in a slice to a container.
     """
     # solution3, plate3 = plate1[:].transfer(solution1, '1 mL')
     solution3, plate3 = Plate.transfer(solution1, plate1[:], '1 mL')
     destination_solution = Container('destination', '100 mL')
     plate4, destination_solution = Container.transfer(plate3, destination_solution, '0.5 mL')
     # Original plate should have 1 mL in each well
-    assert numpy.array_equal(plate3.volumes(), numpy.ones(plate3[:].shape) * 1000)
+    assert numpy.array_equal(plate3.get_volumes(), numpy.ones(plate3[:].shape) * 1000)
     # Destination container should have 0.5 mL for each well
     assert destination_solution.volume == Unit.convert_to_storage(0.5 * plate3[:].size, 'mL')
     # Source wells should all have 0.5 mL
-    assert numpy.array_equal(plate4.volumes(), numpy.ones(plate4[:].shape) * 0.5 * 1000)
+    assert numpy.array_equal(plate4.get_volumes(), numpy.ones(plate4[:].shape) * 0.5 * 1000)
 
     plate4, destination_solution = Container.transfer(plate3[1, :], destination_solution, '0.5 mL')
-    assert plate3.volume() - plate4.volume() == 500 * plate3.n_columns
+    assert plate3.get_volume() - plate4.get_volume() == 500 * plate3.n_columns
```

