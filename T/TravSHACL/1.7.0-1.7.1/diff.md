# Comparing `tmp/TravSHACL-1.7.0.tar.gz` & `tmp/TravSHACL-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TravSHACL-1.7.0.tar", last modified: Thu Nov 23 10:47:21 2023, max compression
+gzip compressed data, was "TravSHACL-1.7.1.tar", last modified: Sat Apr  6 11:37:58 2024, max compression
```

## Comparing `TravSHACL-1.7.0.tar` & `TravSHACL-1.7.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:21.688610 TravSHACL-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35150 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2023-11-23 10:47:21.688610 TravSHACL-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:21.684610 TravSHACL-1.7.0/TravSHACL/
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/TravSHACL.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:21.684610 TravSHACL-1.7.0/TravSHACL/constraints/
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/constraints/Constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/constraints/MaxOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/constraints/MinMaxConstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1711 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/constraints/MinOnlyConstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/constraints/SPARQLConstraint.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/constraints/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:21.684610 TravSHACL-1.7.0/TravSHACL/core/
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/core/GraphTraversal.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/core/RulePattern.py
--rw-r--r--   0 runner    (1001) docker     (127)    10242 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/core/Shape.py
--rw-r--r--   0 runner    (1001) docker     (127)    23761 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/core/ShapeParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     9784 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/core/ShapeSchema.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:21.688610 TravSHACL-1.7.0/TravSHACL/rule_based_validation/
--rw-r--r--   0 runner    (1001) docker     (127)    13552 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/rule_based_validation/InstancesRetrieval.py
--rw-r--r--   0 runner    (1001) docker     (127)    34552 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/rule_based_validation/Validation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/rule_based_validation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:21.688610 TravSHACL-1.7.0/TravSHACL/sparql/
--rw-r--r--   0 runner    (1001) docker     (127)    27370 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/sparql/QueryGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/sparql/SPARQLEndpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/sparql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:21.688610 TravSHACL-1.7.0/TravSHACL/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     5330 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/utils/ValidationStats.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/utils/VariableGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/TravSHACL/utils/fileManagement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:21.688610 TravSHACL-1.7.0/TravSHACL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5586 2023-11-23 10:47:21.000000 TravSHACL-1.7.0/TravSHACL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-23 10:47:21.000000 TravSHACL-1.7.0/TravSHACL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-23 10:47:21.000000 TravSHACL-1.7.0/TravSHACL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-11-23 10:47:21.000000 TravSHACL-1.7.0/TravSHACL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-11-23 10:47:21.000000 TravSHACL-1.7.0/TravSHACL.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-11-23 10:47:21.688610 TravSHACL-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-23 10:47:21.688610 TravSHACL-1.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2023-11-23 10:47:12.000000 TravSHACL-1.7.0/tests/test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:58.206045 TravSHACL-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35150 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-06 11:37:58.206045 TravSHACL-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:58.202045 TravSHACL-1.7.1/TravSHACL/
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/TravSHACL.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:58.202045 TravSHACL-1.7.1/TravSHACL/constraints/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/constraints/Constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/constraints/MaxOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/constraints/MinMaxConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1711 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/constraints/MinOnlyConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/constraints/SPARQLConstraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/constraints/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:58.202045 TravSHACL-1.7.1/TravSHACL/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/core/GraphTraversal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/core/RulePattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10242 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/core/Shape.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24203 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/core/ShapeParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/core/ShapeSchema.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:58.202045 TravSHACL-1.7.1/TravSHACL/rule_based_validation/
+-rw-r--r--   0 runner    (1001) docker     (127)    13552 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/rule_based_validation/InstancesRetrieval.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34552 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/rule_based_validation/Validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/rule_based_validation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:58.202045 TravSHACL-1.7.1/TravSHACL/sparql/
+-rw-r--r--   0 runner    (1001) docker     (127)    27370 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/sparql/QueryGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/sparql/SPARQLEndpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/sparql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:58.206045 TravSHACL-1.7.1/TravSHACL/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     5330 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/utils/ValidationStats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/utils/VariableGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/TravSHACL/utils/fileManagement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:58.206045 TravSHACL-1.7.1/TravSHACL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-06 11:37:58.000000 TravSHACL-1.7.1/TravSHACL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-06 11:37:58.000000 TravSHACL-1.7.1/TravSHACL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 11:37:58.000000 TravSHACL-1.7.1/TravSHACL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-06 11:37:58.000000 TravSHACL-1.7.1/TravSHACL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 11:37:58.000000 TravSHACL-1.7.1/TravSHACL.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-06 11:37:58.206045 TravSHACL-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 11:37:58.206045 TravSHACL-1.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-04-06 11:37:53.000000 TravSHACL-1.7.1/tests/test_cases.py
```

### Comparing `TravSHACL-1.7.0/LICENSE` & `TravSHACL-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/PKG-INFO` & `TravSHACL-1.7.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TravSHACL
-Version: 1.7.0
+Version: 1.7.1
 Summary: A SHACL validator capable of planning the traversal and execution of the validation of a shape schema to detect violations early.
 Home-page: https://github.com/SDM-TIB/Trav-SHACL
-Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.7.0.tar.gz
+Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.7.1.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Project-URL: Documentation, https://sdm-tib.github.io/Trav-SHACL/
 Project-URL: Changes, https://sdm-tib.github.io/Trav-SHACL/changelog.html
 Project-URL: Source Code, https://github.com/SDM-TIB/Trav-SHACL
 Project-URL: Issue Tracker, https://github.com/SDM-TIB/Trav-SHACL/issues
@@ -35,14 +35,18 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/TravSHACL)](https://pypi.org/project/TravSHACL)
 [![Package Format](https://img.shields.io/pypi/format/TravSHACL)](https://pypi.org/project/TravSHACL)
 [![Package Status](https://img.shields.io/pypi/status/TravSHACL)](https://pypi.org/project/TravSHACL)
 [![Package Version](https://img.shields.io/pypi/v/TravSHACL)](https://pypi.org/project/TravSHACL)
 
+[![Publication](https://img.shields.io/badge/Publication-10.1145/3442381.3449877-green.svg)](https://doi.org/10.1145/3442381.3449877)
+[![Data](https://img.shields.io/badge/Data-10.25835/0035739-green.svg)](https://doi.org/10.25835/0035739)
+[![Experiment Scripts](https://img.shields.io/badge/Experiment%20Scripts-eval--www2021-green.svg)](https://github.com/SDM-TIB/Trav-SHACL/tree/eval-www2021)
+
 # ![Logo](https://raw.githubusercontent.com/SDM-TIB/Trav-SHACL/master/images/logo.png "Logo")
 
 We present Trav-SHACL, a SHACL engine capable of planning the traversal and execution of a shape schema in a way that invalid entities are detected early and needless validations are minimized.
 Trav-SHACL reorders the shapes in a shape schema for efficient validation and rewrites target and constraint queries for fast detection of invalid entities.
 The shape schema is validated against an RDF graph accessible via a SPARQL endpoint.
 
 ![Trav-SHACL Architecture](https://raw.githubusercontent.com/SDM-TIB/Trav-SHACL/master/docs/_images/architecture.png)
```

### Comparing `TravSHACL-1.7.0/README.md` & `TravSHACL-1.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/TravSHACL)](https://pypi.org/project/TravSHACL)
 [![Package Format](https://img.shields.io/pypi/format/TravSHACL)](https://pypi.org/project/TravSHACL)
 [![Package Status](https://img.shields.io/pypi/status/TravSHACL)](https://pypi.org/project/TravSHACL)
 [![Package Version](https://img.shields.io/pypi/v/TravSHACL)](https://pypi.org/project/TravSHACL)
 
+[![Publication](https://img.shields.io/badge/Publication-10.1145/3442381.3449877-green.svg)](https://doi.org/10.1145/3442381.3449877)
+[![Data](https://img.shields.io/badge/Data-10.25835/0035739-green.svg)](https://doi.org/10.25835/0035739)
+[![Experiment Scripts](https://img.shields.io/badge/Experiment%20Scripts-eval--www2021-green.svg)](https://github.com/SDM-TIB/Trav-SHACL/tree/eval-www2021)
+
 # ![Logo](https://raw.githubusercontent.com/SDM-TIB/Trav-SHACL/master/images/logo.png "Logo")
 
 We present Trav-SHACL, a SHACL engine capable of planning the traversal and execution of a shape schema in a way that invalid entities are detected early and needless validations are minimized.
 Trav-SHACL reorders the shapes in a shape schema for efficient validation and rewrites target and constraint queries for fast detection of invalid entities.
 The shape schema is validated against an RDF graph accessible via a SPARQL endpoint.
 
 ![Trav-SHACL Architecture](https://raw.githubusercontent.com/SDM-TIB/Trav-SHACL/master/docs/_images/architecture.png)
```

### Comparing `TravSHACL-1.7.0/TravSHACL/TravSHACL.py` & `TravSHACL-1.7.1/TravSHACL/TravSHACL.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/constraints/Constraint.py` & `TravSHACL-1.7.1/TravSHACL/constraints/Constraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/constraints/MaxOnlyConstraint.py` & `TravSHACL-1.7.1/TravSHACL/constraints/MaxOnlyConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/constraints/MinMaxConstraint.py` & `TravSHACL-1.7.1/TravSHACL/constraints/MinMaxConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/constraints/MinOnlyConstraint.py` & `TravSHACL-1.7.1/TravSHACL/constraints/MinOnlyConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/constraints/SPARQLConstraint.py` & `TravSHACL-1.7.1/TravSHACL/constraints/SPARQLConstraint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/core/GraphTraversal.py` & `TravSHACL-1.7.1/TravSHACL/core/GraphTraversal.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/core/RulePattern.py` & `TravSHACL-1.7.1/TravSHACL/core/RulePattern.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/core/Shape.py` & `TravSHACL-1.7.1/TravSHACL/core/Shape.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/core/ShapeParser.py` & `TravSHACL-1.7.1/TravSHACL/core/ShapeParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,22 +308,29 @@
 
                 for detail in filename.query(query[4].format(constraint=constraint_id)):
 
                     if isinstance(detail.asdict()['o'], rdflib.term.BNode):
                         qv_type = detail.asdict()['p']
                         qvs = detail.asdict()['o']
                         if len(filename.query(query[5].format(qvs=qvs))) != 0:
+                            dict_1 = None
                             for shape_ref in filename.query(query[5].format(qvs=qvs)):
-                                # dict_1 = [qv_type, ['shape', str(shape_ref.asdict()['shape_ref'])]]
                                 dict_1 = [qv_type, str(shape_ref.asdict()['shape_ref'])]
-                            exp_dict[str(constraint_id)].append(dict_1.copy())
+                            if dict_1 is not None:
+                                exp_dict[str(constraint_id)].append(dict_1.copy())
+                            else:
+                                raise NotImplementedError('It seems you are using an unsupported feature. Please, check your shape schema.')
                         else:
+                            dict_1 = None
                             for shape_ref in filename.query(query[6].format(qvs=qvs)):
                                 dict_1 = [qv_type, ['value', str(shape_ref.asdict()['shape_ref'])]]
-                            exp_dict[str(constraint_id)].append(dict_1.copy())
+                            if dict_1 is not None:
+                                exp_dict[str(constraint_id)].append(dict_1.copy())
+                            else:
+                                raise NotImplementedError('It seems you are using an unsupported feature. Please, check your shape schema.')
                     else:
                         # detail_dict = detail.asdict()
                         dict_2 = [str(detail['p']), str(detail['o'])]
                         exp_dict[str(constraint_id)].append(dict_2.copy())
 
         if filename.query(query[8].format(shape=name)):
             for constraint in filename.query(query[8].format(shape=name)):
```

### Comparing `TravSHACL-1.7.0/TravSHACL/core/ShapeSchema.py` & `TravSHACL-1.7.1/TravSHACL/core/ShapeSchema.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/rule_based_validation/InstancesRetrieval.py` & `TravSHACL-1.7.1/TravSHACL/rule_based_validation/InstancesRetrieval.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/rule_based_validation/Validation.py` & `TravSHACL-1.7.1/TravSHACL/rule_based_validation/Validation.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/sparql/QueryGenerator.py` & `TravSHACL-1.7.1/TravSHACL/sparql/QueryGenerator.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/sparql/SPARQLEndpoint.py` & `TravSHACL-1.7.1/TravSHACL/sparql/SPARQLEndpoint.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/utils/ValidationStats.py` & `TravSHACL-1.7.1/TravSHACL/utils/ValidationStats.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/utils/VariableGenerator.py` & `TravSHACL-1.7.1/TravSHACL/utils/VariableGenerator.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/utils/__init__.py` & `TravSHACL-1.7.1/TravSHACL/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL/utils/fileManagement.py` & `TravSHACL-1.7.1/TravSHACL/utils/fileManagement.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/TravSHACL.egg-info/PKG-INFO` & `TravSHACL-1.7.1/TravSHACL.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: TravSHACL
-Version: 1.7.0
+Version: 1.7.1
 Summary: A SHACL validator capable of planning the traversal and execution of the validation of a shape schema to detect violations early.
 Home-page: https://github.com/SDM-TIB/Trav-SHACL
-Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.7.0.tar.gz
+Download-URL: https://github.com/SDM-TIB/Trav-SHACL/archive/refs/tags/v1.7.1.tar.gz
 Author: Mónica Figuera, Philipp D. Rohde
 Author-email: philipp.rohde@tib.eu
 License: GNU/GPLv3
 Project-URL: Documentation, https://sdm-tib.github.io/Trav-SHACL/
 Project-URL: Changes, https://sdm-tib.github.io/Trav-SHACL/changelog.html
 Project-URL: Source Code, https://github.com/SDM-TIB/Trav-SHACL
 Project-URL: Issue Tracker, https://github.com/SDM-TIB/Trav-SHACL/issues
@@ -35,14 +35,18 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE)
 
 [![Python Versions](https://img.shields.io/pypi/pyversions/TravSHACL)](https://pypi.org/project/TravSHACL)
 [![Package Format](https://img.shields.io/pypi/format/TravSHACL)](https://pypi.org/project/TravSHACL)
 [![Package Status](https://img.shields.io/pypi/status/TravSHACL)](https://pypi.org/project/TravSHACL)
 [![Package Version](https://img.shields.io/pypi/v/TravSHACL)](https://pypi.org/project/TravSHACL)
 
+[![Publication](https://img.shields.io/badge/Publication-10.1145/3442381.3449877-green.svg)](https://doi.org/10.1145/3442381.3449877)
+[![Data](https://img.shields.io/badge/Data-10.25835/0035739-green.svg)](https://doi.org/10.25835/0035739)
+[![Experiment Scripts](https://img.shields.io/badge/Experiment%20Scripts-eval--www2021-green.svg)](https://github.com/SDM-TIB/Trav-SHACL/tree/eval-www2021)
+
 # ![Logo](https://raw.githubusercontent.com/SDM-TIB/Trav-SHACL/master/images/logo.png "Logo")
 
 We present Trav-SHACL, a SHACL engine capable of planning the traversal and execution of a shape schema in a way that invalid entities are detected early and needless validations are minimized.
 Trav-SHACL reorders the shapes in a shape schema for efficient validation and rewrites target and constraint queries for fast detection of invalid entities.
 The shape schema is validated against an RDF graph accessible via a SPARQL endpoint.
 
 ![Trav-SHACL Architecture](https://raw.githubusercontent.com/SDM-TIB/Trav-SHACL/master/docs/_images/architecture.png)
```

### Comparing `TravSHACL-1.7.0/TravSHACL.egg-info/SOURCES.txt` & `TravSHACL-1.7.1/TravSHACL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/setup.py` & `TravSHACL-1.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `TravSHACL-1.7.0/tests/test_cases.py` & `TravSHACL-1.7.1/tests/test_cases.py`

 * *Files identical despite different names*

