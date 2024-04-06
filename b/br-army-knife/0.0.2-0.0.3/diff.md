# Comparing `tmp/br_army_knife-0.0.2.tar.gz` & `tmp/br_army_knife-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "br_army_knife-0.0.2.tar", last modified: Sat Apr  6 02:23:14 2024, max compression
+gzip compressed data, was "br_army_knife-0.0.3.tar", last modified: Sat Apr  6 03:00:01 2024, max compression
```

## Comparing `br_army_knife-0.0.2.tar` & `br_army_knife-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,9 @@
--rw-r--r--   0        0        0     1071 2024-04-06 00:56:12.949424 br_army_knife-0.0.2/LICENSE
--rw-r--r--   0        0        0       70 2024-04-06 01:49:21.616745 br_army_knife-0.0.2/README.md
--rw-r--r--   0        0        0      629 2024-04-06 02:23:14.124294 br_army_knife-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-06 00:56:12.949424 br_army_knife-0.0.2/src/__init__.py
--rw-r--r--   0        0        0        1 2024-04-06 00:56:12.949424 br_army_knife-0.0.2/src/files.py
--rw-r--r--   0        0        0      972 2024-04-06 01:49:21.616745 br_army_knife-0.0.2/src/lists.py
--rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 br_army_knife-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-06 00:56:12.949424 br_army_knife-0.0.3/LICENSE
+-rw-r--r--   0        0        0       70 2024-04-06 01:49:21.616745 br_army_knife-0.0.3/README.md
+-rw-r--r--   0        0        0      629 2024-04-06 03:00:01.648968 br_army_knife-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-06 00:56:12.949424 br_army_knife-0.0.3/src/br_army_knife/__init__.py
+-rw-r--r--   0        0        0      118 2024-04-06 02:30:49.413073 br_army_knife-0.0.3/src/br_army_knife/code.py
+-rw-r--r--   0        0        0      228 2024-04-06 02:38:26.423909 br_army_knife-0.0.3/src/br_army_knife/files.py
+-rw-r--r--   0        0        0      969 2024-04-06 02:32:37.295283 br_army_knife-0.0.3/src/br_army_knife/lists.py
+-rw-r--r--   0        0        0      542 2024-04-06 02:45:44.602568 br_army_knife-0.0.3/src/br_army_knife/logs.py
+-rw-r--r--   0        0        0      601 1970-01-01 00:00:00.000000 br_army_knife-0.0.3/PKG-INFO
```

### Comparing `br_army_knife-0.0.2/LICENSE` & `br_army_knife-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `br_army_knife-0.0.2/pyproject.toml` & `br_army_knife-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "br_army_knife"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Lucas Quaresma", email = "lucas.quaresma1@gmail.com" },
 ]
 description = "Under construction. Common utilities tools in python."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `br_army_knife-0.0.2/src/lists.py` & `br_army_knife-0.0.3/src/br_army_knife/lists.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 def unpack_nested_lists(nlst, mode="comprehension"):
-    """
-    This takes in unordered and unstrucured nested lists and flattens everything.
-    Example: 
-        Input:  [0, 1, [2, 3], [4, [5, [6, 7], 8], 9]]
-        Output: [0 ,1, 2, 3, 4, 5, 6, 7, 8, 9]
-    """
+    # This takes in unordered and unstrucured nested lists and flattens
+    # everything. Example: 
+    #     Input:  [0, 1, [2, 3], [4, [5, [6, 7], 8], 9]]
+    #     Output: [0 ,1, 2, 3, 4, 5, 6, 7, 8, 9]
+    
     match mode:
         case "comprehension":
             return [
                 item 
                 for sublist in nlst 
                 for item in (
                     unpack_nested_lists(sublist, mode="comprehension")
```

### Comparing `br_army_knife-0.0.2/PKG-INFO` & `br_army_knife-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: br_army_knife
-Version: 0.0.2
+Version: 0.0.3
 Summary: Under construction. Common utilities tools in python.
 Author-Email: Lucas Quaresma <lucas.quaresma1@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Project-URL: Homepage, https://github.com/luksquaresma/br_army_knife
 Project-URL: Issues, https://github.com/luksquaresma/br_army_knife/issues
```

