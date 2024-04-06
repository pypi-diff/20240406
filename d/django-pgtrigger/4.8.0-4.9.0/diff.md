# Comparing `tmp/django_pgtrigger-4.8.0.tar.gz` & `tmp/django_pgtrigger-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgtrigger-4.8.0.tar", max compression
+gzip compressed data, was "django_pgtrigger-4.9.0.tar", max compression
```

## Comparing `django_pgtrigger-4.8.0.tar` & `django_pgtrigger-4.9.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1456 2023-10-09 20:26:59.434130 django_pgtrigger-4.8.0/LICENSE
--rw-r--r--   0        0        0     4461 2023-10-09 20:26:59.434130 django_pgtrigger-4.8.0/README.md
--rw-r--r--   0        0        0     1578 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/__init__.py
--rw-r--r--   0        0        0     3827 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/apps.py
--rw-r--r--   0        0        0     7462 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/compiler.py
--rw-r--r--   0        0        0     8236 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/contrib.py
--rw-r--r--   0        0        0    24682 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/core.py
--rw-r--r--   0        0        0     1116 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/features.py
--rw-r--r--   0        0        0     5192 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/installation.py
--rw-r--r--   0        0        0        0 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/management/__init__.py
--rw-r--r--   0        0        0        0 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/management/commands/__init__.py
--rw-r--r--   0        0        0     7368 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/management/commands/pgtrigger.py
--rw-r--r--   0        0        0    16633 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/migrations.py
--rw-r--r--   0        0        0      105 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/models.py
--rw-r--r--   0        0        0     4977 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/registry.py
--rw-r--r--   0        0        0    10643 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/runtime.py
--rw-r--r--   0        0        0     2529 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/utils.py
--rw-r--r--   0        0        0       83 2023-10-09 20:26:59.438130 django_pgtrigger-4.8.0/pgtrigger/version.py
--rw-r--r--   0        0        0     2400 2023-10-09 20:27:38.910215 django_pgtrigger-4.8.0/pyproject.toml
--rw-r--r--   0        0        0     5646 1970-01-01 00:00:00.000000 django_pgtrigger-4.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-10-16 01:24:34.490059 django_pgtrigger-4.9.0/LICENSE
+-rw-r--r--   0        0        0     4493 2023-10-16 01:24:34.490059 django_pgtrigger-4.9.0/README.md
+-rw-r--r--   0        0        0     1722 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/__init__.py
+-rw-r--r--   0        0        0     3827 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/apps.py
+-rw-r--r--   0        0        0     7462 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/compiler.py
+-rw-r--r--   0        0        0     8236 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/contrib.py
+-rw-r--r--   0        0        0    30197 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/core.py
+-rw-r--r--   0        0        0     1116 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/features.py
+-rw-r--r--   0        0        0     5192 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/installation.py
+-rw-r--r--   0        0        0        0 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/management/commands/__init__.py
+-rw-r--r--   0        0        0     7368 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/management/commands/pgtrigger.py
+-rw-r--r--   0        0        0    16633 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/migrations.py
+-rw-r--r--   0        0        0      105 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/models.py
+-rw-r--r--   0        0        0     4977 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/registry.py
+-rw-r--r--   0        0        0    10643 2023-10-16 01:24:34.494059 django_pgtrigger-4.9.0/pgtrigger/runtime.py
+-rw-r--r--   0        0        0     2529 2023-10-16 01:24:34.498059 django_pgtrigger-4.9.0/pgtrigger/utils.py
+-rw-r--r--   0        0        0       83 2023-10-16 01:24:34.498059 django_pgtrigger-4.9.0/pgtrigger/version.py
+-rw-r--r--   0        0        0     2400 2023-10-16 01:25:17.850000 django_pgtrigger-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5678 1970-01-01 00:00:00.000000 django_pgtrigger-4.9.0/PKG-INFO
```

### Comparing `django_pgtrigger-4.8.0/LICENSE` & `django_pgtrigger-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgtrigger-4.8.0/README.md` & `django_pgtrigger-4.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
 ## Documentation
 
 [View the django-pgtrigger docs here](https://django-pgtrigger.readthedocs.io/) to learn more about:
 
 * Trigger basics and motivation for using triggers.
 * How to use the built-in triggers and how to build custom ones.
 * Installing triggers on third-party models, many-to-many fields, and other advanced scenarios.
+* Writing conditional triggers.
 * Ignoring triggers dynamically and deferring trigger execution.
 * Multiple database, schema, and partitioning support.
 * Frequently asked questions, common issues, and upgrading.
 * The commands, settings, and module.
 
 ## Installation
```

### Comparing `django_pgtrigger-4.8.0/pgtrigger/__init__.py` & `django_pgtrigger-4.9.0/pgtrigger/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,18 @@
     Protect,
     ReadOnly,
     SoftDelete,
     UpdateSearchVector,
 )
 from pgtrigger.core import (
     After,
+    AllChange,
+    AllDontChange,
+    AnyChange,
+    AnyDontChange,
     Before,
     Condition,
     Deferred,
     Delete,
     F,
     Func,
     Immediate,
@@ -57,14 +61,18 @@
     default_app_config = "pgtrigger.apps.PGTriggerConfig"
 
 del django
 
 
 __all__ = [
     "After",
+    "AllChange",
+    "AllDontChange",
+    "AnyChange",
+    "AnyDontChange",
     "Before",
     "Condition",
     "constraints",
     "Deferred",
     "Delete",
     "disable",
     "enable",
```

### Comparing `django_pgtrigger-4.8.0/pgtrigger/apps.py` & `django_pgtrigger-4.9.0/pgtrigger/apps.py`

 * *Files identical despite different names*

### Comparing `django_pgtrigger-4.8.0/pgtrigger/compiler.py` & `django_pgtrigger-4.9.0/pgtrigger/compiler.py`

 * *Files identical despite different names*

### Comparing `django_pgtrigger-4.8.0/pgtrigger/contrib.py` & `django_pgtrigger-4.9.0/pgtrigger/contrib.py`

 * *Files identical despite different names*

### Comparing `django_pgtrigger-4.8.0/pgtrigger/features.py` & `django_pgtrigger-4.9.0/pgtrigger/features.py`

 * *Files identical despite different names*

### Comparing `django_pgtrigger-4.8.0/pgtrigger/installation.py` & `django_pgtrigger-4.9.0/pgtrigger/installation.py`

 * *Files identical despite different names*

### Comparing `django_pgtrigger-4.8.0/pgtrigger/management/commands/pgtrigger.py` & `django_pgtrigger-4.9.0/pgtrigger/management/commands/pgtrigger.py`

 * *Files identical despite different names*

### Comparing `django_pgtrigger-4.8.0/pgtrigger/migrations.py` & `django_pgtrigger-4.9.0/pgtrigger/migrations.py`

 * *Files identical despite different names*

### Comparing `django_pgtrigger-4.8.0/pgtrigger/registry.py` & `django_pgtrigger-4.9.0/pgtrigger/registry.py`

 * *Files identical despite different names*

### Comparing `django_pgtrigger-4.8.0/pgtrigger/runtime.py` & `django_pgtrigger-4.9.0/pgtrigger/runtime.py`

 * *Files identical despite different names*

### Comparing `django_pgtrigger-4.8.0/pgtrigger/utils.py` & `django_pgtrigger-4.9.0/pgtrigger/utils.py`

 * *Files identical despite different names*

### Comparing `django_pgtrigger-4.8.0/pyproject.toml` & `django_pgtrigger-4.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 name = "django-pgtrigger"
 packages = [
   { include = "pgtrigger" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "4.8.0"
+version = "4.9.0"
 description = "Postgres trigger support integrated with Django models."
 authors = ["Wes Kendall"]
 classifiers = [
   "Framework :: Django",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
```

### Comparing `django_pgtrigger-4.8.0/PKG-INFO` & `django_pgtrigger-4.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pgtrigger
-Version: 4.8.0
+Version: 4.9.0
 Summary: Postgres trigger support integrated with Django models.
 Home-page: https://github.com/Opus10/django-pgtrigger
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.8.0,<4
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
@@ -99,14 +99,15 @@
 ## Documentation
 
 [View the django-pgtrigger docs here](https://django-pgtrigger.readthedocs.io/) to learn more about:
 
 * Trigger basics and motivation for using triggers.
 * How to use the built-in triggers and how to build custom ones.
 * Installing triggers on third-party models, many-to-many fields, and other advanced scenarios.
+* Writing conditional triggers.
 * Ignoring triggers dynamically and deferring trigger execution.
 * Multiple database, schema, and partitioning support.
 * Frequently asked questions, common issues, and upgrading.
 * The commands, settings, and module.
 
 ## Installation
```

