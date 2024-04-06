# Comparing `tmp/RelaDB-1.0.2.tar.gz` & `tmp/RelaDB-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RelaDB-1.0.2.tar", last modified: Sat Apr  6 02:55:40 2024, max compression
+gzip compressed data, was "RelaDB-1.0.3.tar", last modified: Sat Apr  6 03:08:06 2024, max compression
```

## Comparing `RelaDB-1.0.2.tar` & `RelaDB-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:55:40.174484 RelaDB-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-06 02:55:40.174484 RelaDB-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-04-06 02:55:34.000000 RelaDB-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 02:55:40.174484 RelaDB-1.0.2/RelaDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-06 02:55:40.000000 RelaDB-1.0.2/RelaDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-06 02:55:40.000000 RelaDB-1.0.2/RelaDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:55:40.000000 RelaDB-1.0.2/RelaDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 02:55:40.000000 RelaDB-1.0.2/RelaDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 02:55:40.174484 RelaDB-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2024-04-06 02:55:34.000000 RelaDB-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:08:06.501302 RelaDB-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-06 03:08:06.501302 RelaDB-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-04-06 03:08:02.000000 RelaDB-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 03:08:06.501302 RelaDB-1.0.3/RelaDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-04-06 03:08:06.000000 RelaDB-1.0.3/RelaDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-06 03:08:06.000000 RelaDB-1.0.3/RelaDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 03:08:06.000000 RelaDB-1.0.3/RelaDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 03:08:06.000000 RelaDB-1.0.3/RelaDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 03:08:06.501302 RelaDB-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3962 2024-04-06 03:08:02.000000 RelaDB-1.0.3/setup.py
```

### Comparing `RelaDB-1.0.2/PKG-INFO` & `RelaDB-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RelaDB
-Version: 1.0.2
+Version: 1.0.3
 Summary: A fast and lightweight relational db
 Home-page: https://github.com/D4r3d3vil/RelaDB
 Author: Mulham Alamry
 Author-email: mulhamreacts@gmail.com
 License: UNKNOWN
 Description: # RelaDB
         
@@ -100,15 +100,15 @@
         ##### `load(self) -> None`
         
         Loads the database schema and data from the SQLite file specified in the `db_file` attribute.
         
         ## Usage Example
         
         ```python
-        from ultrafastdb import Database
+        from relaDB import Database
         
         # Initialize database
         db = Database()
         
         # Create a table
         db.create("users", {"name": str, "age": int})
```

### Comparing `RelaDB-1.0.2/README.md` & `RelaDB-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 ##### `load(self) -> None`
 
 Loads the database schema and data from the SQLite file specified in the `db_file` attribute.
 
 ## Usage Example
 
 ```python
-from ultrafastdb import Database
+from relaDB import Database
 
 # Initialize database
 db = Database()
 
 # Create a table
 db.create("users", {"name": str, "age": int})
```

### Comparing `RelaDB-1.0.2/RelaDB.egg-info/PKG-INFO` & `RelaDB-1.0.3/RelaDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RelaDB
-Version: 1.0.2
+Version: 1.0.3
 Summary: A fast and lightweight relational db
 Home-page: https://github.com/D4r3d3vil/RelaDB
 Author: Mulham Alamry
 Author-email: mulhamreacts@gmail.com
 License: UNKNOWN
 Description: # RelaDB
         
@@ -100,15 +100,15 @@
         ##### `load(self) -> None`
         
         Loads the database schema and data from the SQLite file specified in the `db_file` attribute.
         
         ## Usage Example
         
         ```python
-        from ultrafastdb import Database
+        from relaDB import Database
         
         # Initialize database
         db = Database()
         
         # Create a table
         db.create("users", {"name": str, "age": int})
```

### Comparing `RelaDB-1.0.2/setup.py` & `RelaDB-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RelaDB',
-    version='1.0.2',
+    version='1.0.3',
     author='Mulham Alamry',
     author_email='mulhamreacts@gmail.com',
     description='A fast and lightweight relational db',
     long_description="""# RelaDB
 
 🔥 RelaDB is a lightweight set of classes for a relational database system designed for simplicity and speed. It integrates with SQLite and provides an easy-to-use API for managing database schemas, tables, and records in Python.
 
@@ -100,15 +100,15 @@
 ##### `load(self) -> None`
 
 Loads the database schema and data from the SQLite file specified in the `db_file` attribute.
 
 ## Usage Example
 
 ```python
-from ultrafastdb import Database
+from relaDB import Database
 
 # Initialize database
 db = Database()
 
 # Create a table
 db.create("users", {"name": str, "age": int})
```

