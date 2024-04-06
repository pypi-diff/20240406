# Comparing `tmp/redsauce-0.0.1.1.tar.gz` & `tmp/redsauce-0.0.1.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redsauce-0.0.1.1.tar", last modified: Sat Apr  6 00:32:26 2024, max compression
+gzip compressed data, was "redsauce-0.0.1.11.tar", last modified: Sat Apr  6 18:30:23 2024, max compression
```

## Comparing `redsauce-0.0.1.1.tar` & `redsauce-0.0.1.11.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:32:26.116566 redsauce-0.0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-06 00:32:22.000000 redsauce-0.0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-06 00:32:26.116566 redsauce-0.0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-06 00:32:22.000000 redsauce-0.0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:32:26.116566 redsauce-0.0.1.1/redsauce/
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-06 00:32:22.000000 redsauce-0.0.1.1/redsauce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-06 00:32:22.000000 redsauce-0.0.1.1/redsauce/pickles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-06 00:32:22.000000 redsauce-0.0.1.1/redsauce/utensils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:32:26.116566 redsauce-0.0.1.1/redsauce.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-06 00:32:26.000000 redsauce-0.0.1.1/redsauce.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-06 00:32:26.000000 redsauce-0.0.1.1/redsauce.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:32:26.000000 redsauce-0.0.1.1/redsauce.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 00:32:26.000000 redsauce-0.0.1.1/redsauce.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 00:32:26.000000 redsauce-0.0.1.1/redsauce.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:32:26.116566 redsauce-0.0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-06 00:32:22.000000 redsauce-0.0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:30:23.102989 redsauce-0.0.1.11/
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-06 18:30:19.000000 redsauce-0.0.1.11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-06 18:30:23.102989 redsauce-0.0.1.11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4421 2024-04-06 18:30:19.000000 redsauce-0.0.1.11/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:30:23.102989 redsauce-0.0.1.11/redsauce/
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-04-06 18:30:19.000000 redsauce-0.0.1.11/redsauce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-06 18:30:19.000000 redsauce-0.0.1.11/redsauce/pickles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-06 18:30:19.000000 redsauce-0.0.1.11/redsauce/utensils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:30:23.102989 redsauce-0.0.1.11/redsauce/utility/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-06 18:30:19.000000 redsauce-0.0.1.11/redsauce/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-04-06 18:30:19.000000 redsauce-0.0.1.11/redsauce/utility/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:30:23.102989 redsauce-0.0.1.11/redsauce.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-06 18:30:23.000000 redsauce-0.0.1.11/redsauce.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-06 18:30:23.000000 redsauce-0.0.1.11/redsauce.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:30:23.000000 redsauce-0.0.1.11/redsauce.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-06 18:30:23.000000 redsauce-0.0.1.11/redsauce.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-06 18:30:23.000000 redsauce-0.0.1.11/redsauce.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:30:23.102989 redsauce-0.0.1.11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 18:30:19.000000 redsauce-0.0.1.11/setup.py
```

### Comparing `redsauce-0.0.1.1/LICENSE` & `redsauce-0.0.1.11/LICENSE`

 * *Files identical despite different names*

### Comparing `redsauce-0.0.1.1/README.md` & `redsauce-0.0.1.11/README.md`

 * *Files identical despite different names*

### Comparing `redsauce-0.0.1.1/redsauce/__init__.py` & `redsauce-0.0.1.11/redsauce/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,37 +11,38 @@
 from redis.commands.json.path import Path
 from redis.commands.search.field import TagField, TextField, NumericField
 from redis.commands.search.indexDefinition import IndexDefinition, IndexType
 from redis.exceptions import DataError
 
 from .pickles import Redis
 from .utensils import queryRecord, getRecord, makeSerializable
-
+from .utility.logging import Sawyer
 
 
 class Generator:
     field_map = {
         'tag': TagField,
         'text': TextField,
         'number': NumericField
         # more to come
     }
 
     def __init__(self, yaml_path: str = None, connection = None):
         self.__on_cache_hit = self.__null_handler
         self.__on_cache_miss = self.__null_handler
+        self.yaml = None
         if yaml_path is None and connection is None:
             raise ValueError("Must provide either a path to a yaml file or a connection object.")
         if yaml_path is not None:
             self.yaml = ym.safe_load(open(yaml_path))
         if connection is not None:
-            if self.yaml is None:
-                self.yaml = {'redis': {'connection': connection}}
-            else:
+            if self.yaml:
                 self.yaml['redis']['connection'] = connection
+            else:
+                self.yaml = {'redis': {'connection': connection}}
         self.dbs = {}
         self.connection = self.yaml['redis'].pop('connection')
         self.load()
     
     def __null_handler(self, *args, **kwargs):
         pass
 
@@ -143,8 +144,12 @@
                     red.set(key, Path.root_path(), result)
                 if ttl:
                     self.redis.expire(key, ttl)
                 return result
             return wrapper
         return decorator
 
-__all__ = ['Generator', 'GlobalServices']
+__all__ = [
+    'Generator', 
+    'GlobalServices',
+    'Sawyer'
+    ]
```

### Comparing `redsauce-0.0.1.1/redsauce/pickles.py` & `redsauce-0.0.1.11/redsauce/pickles.py`

 * *Files identical despite different names*

### Comparing `redsauce-0.0.1.1/redsauce/utensils.py` & `redsauce-0.0.1.11/redsauce/utensils.py`

 * *Files identical despite different names*

