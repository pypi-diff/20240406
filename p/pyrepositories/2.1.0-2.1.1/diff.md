# Comparing `tmp/pyrepositories-2.1.0.tar.gz` & `tmp/pyrepositories-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrepositories-2.1.0.tar", last modified: Mon Apr  1 18:40:53 2024, max compression
+gzip compressed data, was "pyrepositories-2.1.1.tar", last modified: Sat Apr  6 15:57:08 2024, max compression
```

## Comparing `pyrepositories-2.1.0.tar` & `pyrepositories-2.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:40:53.105064 pyrepositories-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-01 18:40:53.105064 pyrepositories-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:40:53.105064 pyrepositories-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:40:53.101064 pyrepositories-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:40:53.105064 pyrepositories-2.1.0/src/pyrepositories/
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/src/pyrepositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/src/pyrepositories/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/src/pyrepositories/datatable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/src/pyrepositories/json_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     8878 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/src/pyrepositories/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-01 18:40:48.000000 pyrepositories-2.1.0/src/pyrepositories/pg_repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:40:53.105064 pyrepositories-2.1.0/src/pyrepositories.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-01 18:40:53.000000 pyrepositories-2.1.0/src/pyrepositories.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-01 18:40:53.000000 pyrepositories-2.1.0/src/pyrepositories.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:40:53.000000 pyrepositories-2.1.0/src/pyrepositories.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-01 18:40:53.000000 pyrepositories-2.1.0/src/pyrepositories.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-01 18:40:53.000000 pyrepositories-2.1.0/src/pyrepositories.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:57:08.726242 pyrepositories-2.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-06 15:57:08.722242 pyrepositories-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-06 15:57:04.000000 pyrepositories-2.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-06 15:57:04.000000 pyrepositories-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 15:57:08.726242 pyrepositories-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:57:08.722242 pyrepositories-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:57:08.722242 pyrepositories-2.1.1/src/pyrepositories/
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-04-06 15:57:04.000000 pyrepositories-2.1.1/src/pyrepositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3709 2024-04-06 15:57:04.000000 pyrepositories-2.1.1/src/pyrepositories/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-06 15:57:04.000000 pyrepositories-2.1.1/src/pyrepositories/datatable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-04-06 15:57:04.000000 pyrepositories-2.1.1/src/pyrepositories/json_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9346 2024-04-06 15:57:04.000000 pyrepositories-2.1.1/src/pyrepositories/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-06 15:57:04.000000 pyrepositories-2.1.1/src/pyrepositories/pg_repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 15:57:08.722242 pyrepositories-2.1.1/src/pyrepositories.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-06 15:57:08.000000 pyrepositories-2.1.1/src/pyrepositories.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-06 15:57:08.000000 pyrepositories-2.1.1/src/pyrepositories.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 15:57:08.000000 pyrepositories-2.1.1/src/pyrepositories.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-06 15:57:08.000000 pyrepositories-2.1.1/src/pyrepositories.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 15:57:08.000000 pyrepositories-2.1.1/src/pyrepositories.egg-info/top_level.txt
```

### Comparing `pyrepositories-2.1.0/pyproject.toml` & `pyrepositories-2.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pyrepositories"
-version = "2.1.0"
+version = "2.1.1"
 authors = [
   { name="kougen", email="info@kou-gen.net" },
 ]
 
 maintainers = [
   { name="Joshua Hegedus", email="josh.hegedus@outlook.com" },
 ]
```

### Comparing `pyrepositories-2.1.0/src/pyrepositories/__init__.py` & `pyrepositories-2.1.1/src/pyrepositories/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrepositories-2.1.0/src/pyrepositories/datasource.py` & `pyrepositories-2.1.1/src/pyrepositories/datasource.py`

 * *Files identical despite different names*

### Comparing `pyrepositories-2.1.0/src/pyrepositories/datatable.py` & `pyrepositories-2.1.1/src/pyrepositories/datatable.py`

 * *Files identical despite different names*

### Comparing `pyrepositories-2.1.0/src/pyrepositories/json_repository.py` & `pyrepositories-2.1.1/src/pyrepositories/json_repository.py`

 * *Files identical despite different names*

### Comparing `pyrepositories-2.1.0/src/pyrepositories/lib.py` & `pyrepositories-2.1.1/src/pyrepositories/lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -71,23 +71,40 @@
     def __str__(self):
         return f"{self.combination} {self.conditions}"
 
     def __repr__(self):
         return self.__str__()
 
 class FieldTypes(Enum):
+    @property
+    def content_type(self):
+        if self == FieldTypes.UUID:
+            return str
+        if self == FieldTypes.INT:
+            return int
+        if self == FieldTypes.STR:
+            return str
+        if self == FieldTypes.BOOL:
+            return bool
+        if self == FieldTypes.FLOAT:
+            return float
+        if self == FieldTypes.LIST:
+            return list
+        if self == FieldTypes.DICT:
+            return dict
+        
+
     INT = int
     STR = str
     UUID = 'uuid'
     BOOL = bool
     FLOAT = float
     LIST = list
     DICT = dict
 
-
 class FieldValue:
     def __init__(self, value: Any, entity_id: int | str):
         self.entity_id = entity_id
         self.value = value
 
 
 class FieldBase:
```

