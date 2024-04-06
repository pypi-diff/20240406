# Comparing `tmp/br_army_knife-0.0.3.tar.gz` & `tmp/br_army_knife-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "br_army_knife-0.0.3.tar", last modified: Sat Apr  6 03:00:01 2024, max compression
+gzip compressed data, was "br_army_knife-0.0.4.tar", last modified: Sat Apr  6 03:05:15 2024, max compression
```

## Comparing `br_army_knife-0.0.3.tar` & `br_army_knife-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1071 2024-04-06 00:56:12.949424 br_army_knife-0.0.3/LICENSE
--rw-r--r--   0        0        0       70 2024-04-06 01:49:21.616745 br_army_knife-0.0.3/README.md
--rw-r--r--   0        0        0      629 2024-04-06 03:00:01.648968 br_army_knife-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-06 00:56:12.949424 br_army_knife-0.0.3/src/br_army_knife/__init__.py
--rw-r--r--   0        0        0      118 2024-04-06 02:30:49.413073 br_army_knife-0.0.3/src/br_army_knife/code.py
--rw-r--r--   0        0        0      228 2024-04-06 02:38:26.423909 br_army_knife-0.0.3/src/br_army_knife/files.py
--rw-r--r--   0        0        0      969 2024-04-06 02:32:37.295283 br_army_knife-0.0.3/src/br_army_knife/lists.py
--rw-r--r--   0        0        0      542 2024-04-06 02:45:44.602568 br_army_knife-0.0.3/src/br_army_knife/logs.py
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 br_army_knife-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-06 00:56:12.949424 br_army_knife-0.0.4/LICENSE
+-rw-r--r--   0        0        0       70 2024-04-06 01:49:21.616745 br_army_knife-0.0.4/README.md
+-rw-r--r--   0        0        0      629 2024-04-06 03:05:15.934107 br_army_knife-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       31 2024-04-06 03:04:41.942008 br_army_knife-0.0.4/src/br_army_knife/__init__.py
+-rw-r--r--   0        0        0      118 2024-04-06 02:30:49.413073 br_army_knife-0.0.4/src/br_army_knife/code.py
+-rw-r--r--   0        0        0      228 2024-04-06 02:38:26.423909 br_army_knife-0.0.4/src/br_army_knife/files.py
+-rw-r--r--   0        0        0      969 2024-04-06 02:32:37.295283 br_army_knife-0.0.4/src/br_army_knife/lists.py
+-rw-r--r--   0        0        0      542 2024-04-06 02:45:44.602568 br_army_knife-0.0.4/src/br_army_knife/logs.py
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 br_army_knife-0.0.4/PKG-INFO
```

### Comparing `br_army_knife-0.0.3/LICENSE` & `br_army_knife-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `br_army_knife-0.0.3/pyproject.toml` & `br_army_knife-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "br_army_knife"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     { name = "Lucas Quaresma", email = "lucas.quaresma1@gmail.com" },
 ]
 description = "Under construction. Common utilities tools in python."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `br_army_knife-0.0.3/src/br_army_knife/lists.py` & `br_army_knife-0.0.4/src/br_army_knife/lists.py`

 * *Files identical despite different names*

### Comparing `br_army_knife-0.0.3/src/br_army_knife/logs.py` & `br_army_knife-0.0.4/src/br_army_knife/logs.py`

 * *Files identical despite different names*

### Comparing `br_army_knife-0.0.3/PKG-INFO` & `br_army_knife-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: br_army_knife
-Version: 0.0.3
+Version: 0.0.4
 Summary: Under construction. Common utilities tools in python.
 Author-Email: Lucas Quaresma <lucas.quaresma1@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/luksquaresma/br_army_knife
 Project-URL: Issues, https://github.com/luksquaresma/br_army_knife/issues
```

