# Comparing `tmp/pyindrav2h-0.0.2.tar.gz` & `tmp/pyindrav2h-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyindrav2h-0.0.2.tar", last modified: Thu Apr  4 19:44:21 2024, max compression
+gzip compressed data, was "pyindrav2h-0.0.3.tar", last modified: Sat Apr  6 16:07:50 2024, max compression
```

## Comparing `pyindrav2h-0.0.2.tar` & `pyindrav2h-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-04 19:44:21.720760 pyindrav2h-0.0.2/
--rw-r--r--   0 paulmorris   (501) staff       (20)     1068 2024-04-04 19:31:06.000000 pyindrav2h-0.0.2/LICENSE
--rw-r--r--   0 paulmorris   (501) staff       (20)     4183 2024-04-04 19:44:21.719755 pyindrav2h-0.0.2/PKG-INFO
--rw-r--r--   0 paulmorris   (501) staff       (20)     2387 2024-04-04 19:43:34.000000 pyindrav2h-0.0.2/README.md
--rw-r--r--   0 paulmorris   (501) staff       (20)      756 2024-04-04 19:31:06.000000 pyindrav2h-0.0.2/pyproject.toml
--rw-r--r--   0 paulmorris   (501) staff       (20)       38 2024-04-04 19:44:21.720977 pyindrav2h-0.0.2/setup.cfg
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-04 19:44:21.708978 pyindrav2h-0.0.2/src/
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-04 19:44:21.714819 pyindrav2h-0.0.2/src/pyindrav2h/
--rw-r--r--   0 paulmorris   (501) staff       (20)      114 2024-04-04 19:31:06.000000 pyindrav2h-0.0.2/src/pyindrav2h/__init__.py
--rw-r--r--   0 paulmorris   (501) staff       (20)     2451 2024-04-04 19:31:06.000000 pyindrav2h-0.0.2/src/pyindrav2h/cli.py
--rw-r--r--   0 paulmorris   (501) staff       (20)     4634 2024-04-04 19:31:06.000000 pyindrav2h-0.0.2/src/pyindrav2h/connection.py
--rw-r--r--   0 paulmorris   (501) staff       (20)      746 2024-04-04 19:31:06.000000 pyindrav2h-0.0.2/src/pyindrav2h/exceptions.py
--rw-r--r--   0 paulmorris   (501) staff       (20)      551 2024-04-04 19:31:06.000000 pyindrav2h-0.0.2/src/pyindrav2h/v2hclient.py
--rw-r--r--   0 paulmorris   (501) staff       (20)     4066 2024-04-04 19:31:06.000000 pyindrav2h-0.0.2/src/pyindrav2h/v2hdevice.py
-drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-04 19:44:21.718621 pyindrav2h-0.0.2/src/pyindrav2h.egg-info/
--rw-r--r--   0 paulmorris   (501) staff       (20)     4183 2024-04-04 19:44:21.000000 pyindrav2h-0.0.2/src/pyindrav2h.egg-info/PKG-INFO
--rw-r--r--   0 paulmorris   (501) staff       (20)      425 2024-04-04 19:44:21.000000 pyindrav2h-0.0.2/src/pyindrav2h.egg-info/SOURCES.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)        1 2024-04-04 19:44:21.000000 pyindrav2h-0.0.2/src/pyindrav2h.egg-info/dependency_links.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)       48 2024-04-04 19:44:21.000000 pyindrav2h-0.0.2/src/pyindrav2h.egg-info/entry_points.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)       15 2024-04-04 19:44:21.000000 pyindrav2h-0.0.2/src/pyindrav2h.egg-info/requires.txt
--rw-r--r--   0 paulmorris   (501) staff       (20)       11 2024-04-04 19:44:21.000000 pyindrav2h-0.0.2/src/pyindrav2h.egg-info/top_level.txt
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-06 16:07:50.409372 pyindrav2h-0.0.3/
+-rw-r--r--   0 paulmorris   (501) staff       (20)     1068 2024-04-04 19:31:06.000000 pyindrav2h-0.0.3/LICENSE
+-rw-r--r--   0 paulmorris   (501) staff       (20)     4183 2024-04-06 16:07:50.408610 pyindrav2h-0.0.3/PKG-INFO
+-rw-r--r--   0 paulmorris   (501) staff       (20)     2387 2024-04-04 19:59:48.000000 pyindrav2h-0.0.3/README.md
+-rw-r--r--   0 paulmorris   (501) staff       (20)      756 2024-04-06 16:02:23.000000 pyindrav2h-0.0.3/pyproject.toml
+-rw-r--r--   0 paulmorris   (501) staff       (20)       38 2024-04-06 16:07:50.409509 pyindrav2h-0.0.3/setup.cfg
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-06 16:07:50.396456 pyindrav2h-0.0.3/src/
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-06 16:07:50.401147 pyindrav2h-0.0.3/src/pyindrav2h/
+-rw-r--r--   0 paulmorris   (501) staff       (20)      114 2024-04-06 16:02:37.000000 pyindrav2h-0.0.3/src/pyindrav2h/__init__.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)     2451 2024-04-04 19:31:06.000000 pyindrav2h-0.0.3/src/pyindrav2h/cli.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)     4634 2024-04-04 19:31:06.000000 pyindrav2h-0.0.3/src/pyindrav2h/connection.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)      746 2024-04-04 19:31:06.000000 pyindrav2h-0.0.3/src/pyindrav2h/exceptions.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)      551 2024-04-04 19:31:06.000000 pyindrav2h-0.0.3/src/pyindrav2h/v2hclient.py
+-rw-r--r--   0 paulmorris   (501) staff       (20)     4170 2024-04-06 15:54:41.000000 pyindrav2h-0.0.3/src/pyindrav2h/v2hdevice.py
+drwxr-xr-x   0 paulmorris   (501) staff       (20)        0 2024-04-06 16:07:50.407607 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/
+-rw-r--r--   0 paulmorris   (501) staff       (20)     4183 2024-04-06 16:07:50.000000 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/PKG-INFO
+-rw-r--r--   0 paulmorris   (501) staff       (20)      425 2024-04-06 16:07:50.000000 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/SOURCES.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)        1 2024-04-06 16:07:50.000000 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/dependency_links.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)       48 2024-04-06 16:07:50.000000 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/entry_points.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)       15 2024-04-06 16:07:50.000000 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/requires.txt
+-rw-r--r--   0 paulmorris   (501) staff       (20)       11 2024-04-06 16:07:50.000000 pyindrav2h-0.0.3/src/pyindrav2h.egg-info/top_level.txt
```

### Comparing `pyindrav2h-0.0.2/LICENSE` & `pyindrav2h-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.2/PKG-INFO` & `pyindrav2h-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyindrav2h
-Version: 0.0.2
+Version: 0.0.3
 Summary: API client and example CLI to interact with Indra V2H Chargers
 Author-email: Paul Morris <paul@creatingwake.com>
 License: MIT License
         
         Copyright (c) 2024 creatingwake
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyindrav2h-0.0.2/README.md` & `pyindrav2h-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.2/pyproject.toml` & `pyindrav2h-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyindrav2h"
-version = "0.0.2"
+version = "0.0.3"
 description = "API client and example CLI to interact with Indra V2H Chargers"
 readme = "README.md"
 authors = [{ name = "Paul Morris", email = "paul@creatingwake.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyindrav2h-0.0.2/src/pyindrav2h/cli.py` & `pyindrav2h-0.0.3/src/pyindrav2h/cli.py`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.2/src/pyindrav2h/connection.py` & `pyindrav2h-0.0.3/src/pyindrav2h/connection.py`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.2/src/pyindrav2h/exceptions.py` & `pyindrav2h-0.0.3/src/pyindrav2h/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.2/src/pyindrav2h/v2hclient.py` & `pyindrav2h-0.0.3/src/pyindrav2h/v2hclient.py`

 * *Files identical despite different names*

### Comparing `pyindrav2h-0.0.2/src/pyindrav2h/v2hdevice.py` & `pyindrav2h-0.0.3/src/pyindrav2h/v2hdevice.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,18 @@
     async def load_match(self):
         return await self.__set_mode(V2H_MODES['LOAD_MATCH'])
 
     async def idle(self):
         return await self.__set_mode(V2H_MODES['IDLE'])       
 
     async def schedule(self):
-        return await self.__set_mode(V2H_MODES['SCHEDULE'])  
+        return await self.__set_mode(V2H_MODES['SCHEDULE'])
+    
+    async def select_charger_mode(self, mode):
+        return await self.__set_mode(V2H_MODES[mode])
 
     async def refresh_stats(self):
         s = await self.connection.get("/telemetry/devices/" + self.serial + 
                                       "/latest")
         self.stats = s
         _LOGGER.debug(f"Stats: {s}")
         a = await self.connection.get("/transactions/" + self.serial +
```

### Comparing `pyindrav2h-0.0.2/src/pyindrav2h.egg-info/PKG-INFO` & `pyindrav2h-0.0.3/src/pyindrav2h.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyindrav2h
-Version: 0.0.2
+Version: 0.0.3
 Summary: API client and example CLI to interact with Indra V2H Chargers
 Author-email: Paul Morris <paul@creatingwake.com>
 License: MIT License
         
         Copyright (c) 2024 creatingwake
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

