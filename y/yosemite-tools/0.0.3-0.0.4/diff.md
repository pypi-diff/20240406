# Comparing `tmp/yosemite-tools-0.0.3.tar.gz` & `tmp/yosemite-tools-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yosemite-tools-0.0.3.tar", last modified: Sat Apr  6 03:45:52 2024, max compression
+gzip compressed data, was "yosemite-tools-0.0.4.tar", last modified: Sat Apr  6 04:39:57 2024, max compression
```

## Comparing `yosemite-tools-0.0.3.tar` & `yosemite-tools-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 03:45:52.173829 yosemite-tools-0.0.3/
--rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-06 03:45:52.173249 yosemite-tools-0.0.3/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-06 03:45:52.174010 yosemite-tools-0.0.3/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)      554 2024-04-06 03:45:47.000000 yosemite-tools-0.0.3/setup.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 03:45:52.163761 yosemite-tools-0.0.3/yosemite_tools/
--rw-r--r--   0 hammad     (501) staff       (20)       22 2024-04-05 14:18:10.000000 yosemite-tools-0.0.3/yosemite_tools/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 03:45:52.171645 yosemite-tools-0.0.3/yosemite_tools/modules/
--rw-r--r--   0 hammad     (501) staff       (20)      160 2024-04-05 14:26:33.000000 yosemite-tools-0.0.3/yosemite_tools/modules/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     8880 2024-04-05 14:13:25.000000 yosemite-tools-0.0.3/yosemite_tools/modules/inputs.py
--rw-r--r--   0 hammad     (501) staff       (20)     6337 2024-04-06 03:45:33.000000 yosemite-tools-0.0.3/yosemite_tools/modules/logger.py
--rw-r--r--   0 hammad     (501) staff       (20)     3213 2024-04-05 14:26:59.000000 yosemite-tools-0.0.3/yosemite_tools/modules/preconditions.py
--rw-r--r--   0 hammad     (501) staff       (20)    10620 2024-04-05 14:30:57.000000 yosemite-tools-0.0.3/yosemite_tools/modules/utils.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 03:45:52.172647 yosemite-tools-0.0.3/yosemite_tools.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-06 03:45:52.000000 yosemite-tools-0.0.3/yosemite_tools.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      397 2024-04-06 03:45:52.000000 yosemite-tools-0.0.3/yosemite_tools.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-06 03:45:52.000000 yosemite-tools-0.0.3/yosemite_tools.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-06 03:45:52.000000 yosemite-tools-0.0.3/yosemite_tools.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)       15 2024-04-06 03:45:52.000000 yosemite-tools-0.0.3/yosemite_tools.egg-info/top_level.txt
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:39:57.835408 yosemite-tools-0.0.4/
+-rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-06 04:39:57.834289 yosemite-tools-0.0.4/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-06 04:39:57.835643 yosemite-tools-0.0.4/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)      554 2024-04-06 04:39:52.000000 yosemite-tools-0.0.4/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:39:57.817838 yosemite-tools-0.0.4/yosemite_tools/
+-rw-r--r--   0 hammad     (501) staff       (20)       22 2024-04-05 14:18:10.000000 yosemite-tools-0.0.4/yosemite_tools/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:39:57.832042 yosemite-tools-0.0.4/yosemite_tools/modules/
+-rw-r--r--   0 hammad     (501) staff       (20)      160 2024-04-05 14:26:33.000000 yosemite-tools-0.0.4/yosemite_tools/modules/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8880 2024-04-05 14:13:25.000000 yosemite-tools-0.0.4/yosemite_tools/modules/inputs.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6337 2024-04-06 03:45:33.000000 yosemite-tools-0.0.4/yosemite_tools/modules/logger.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3163 2024-04-06 04:39:38.000000 yosemite-tools-0.0.4/yosemite_tools/modules/preconditions.py
+-rw-r--r--   0 hammad     (501) staff       (20)    10620 2024-04-05 14:30:57.000000 yosemite-tools-0.0.4/yosemite_tools/modules/utils.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:39:57.833334 yosemite-tools-0.0.4/yosemite_tools.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-06 04:39:57.000000 yosemite-tools-0.0.4/yosemite_tools.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      397 2024-04-06 04:39:57.000000 yosemite-tools-0.0.4/yosemite_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-06 04:39:57.000000 yosemite-tools-0.0.4/yosemite_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-06 04:39:57.000000 yosemite-tools-0.0.4/yosemite_tools.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       15 2024-04-06 04:39:57.000000 yosemite-tools-0.0.4/yosemite_tools.egg-info/top_level.txt
```

### Comparing `yosemite-tools-0.0.3/setup.py` & `yosemite-tools-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="yosemite-tools",
-    version="0.0.03",
+    version="0.0.04",
     author="Hammad Saeed",
     author_email="hammad@supportvectors.com",
     description="yosemite",
     long_description="""
 Yosemite
     """,
     packages=setuptools.find_packages(),
```

### Comparing `yosemite-tools-0.0.3/yosemite_tools/modules/inputs.py` & `yosemite-tools-0.0.4/yosemite_tools/modules/inputs.py`

 * *Files identical despite different names*

### Comparing `yosemite-tools-0.0.3/yosemite_tools/modules/logger.py` & `yosemite-tools-0.0.4/yosemite_tools/modules/logger.py`

 * *Files identical despite different names*

### Comparing `yosemite-tools-0.0.3/yosemite_tools/modules/preconditions.py` & `yosemite-tools-0.0.4/yosemite_tools/modules/preconditions.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
         self.logger = None
         if logger:
             self.logger = logger
         else:
             pass
         pass
 
-    @staticmethod
     def check_dir_exists(self, path: str):
         if self.logger:
             self.logger.info(f"[Precondition Verifier] Checking Directory: {path}")
         if not path:
             if self.logger:
                 self.logger.critical("[Precondition Verifier] Path is Required!")
             raise ValueError("Path is Required!")
@@ -34,16 +33,15 @@
                     raise ValueError(f"Path is not a directory: {path}")
             except Exception as e:
                 if self.logger:
                     self.logger.error(f"[Precondition Verifier] Error Reading Path: {e}")
                 raise ValueError(f"Error Reading Path: {e}")
         self.logger.info(f"[Precondition Verifier] Directory Exists: {path}")
         return path
-
-    @staticmethod
+    
     def check_file_exists(self, path: str):
         if self.logger:
             self.logger.info(f"[Precondition Verifier] Checking File: {path}")
         if not path:
             if self.logger:
                 self.logger.critical("[Precondition Verifier] Path is Required!")
             raise ValueError("Path is Required!")
@@ -60,15 +58,14 @@
         except Exception as e:
             if self.logger:
                 self.logger.error(f"[Precondition Verifier] Error Reading: {e}")
             raise ValueError(f"Error Reading: {e}")
         self.logger.info(f"[Precondition Verifier] File Exists: {path}")
         return path
 
-    @staticmethod
     def create_path(self, path: str):
         if self.logger:
             self.logger.info(f"[Precondition Verifier] Creating Path: {path}")
         try:
             path = pathlib.Path(path)
             path.mkdir(parents=True, exist_ok=True)
         except Exception as e:
```

### Comparing `yosemite-tools-0.0.3/yosemite_tools/modules/utils.py` & `yosemite-tools-0.0.4/yosemite_tools/modules/utils.py`

 * *Files identical despite different names*

