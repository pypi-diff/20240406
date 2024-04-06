# Comparing `tmp/nnsom-1.4.7.tar.gz` & `tmp/nnsom-1.4.8.tar.gz`

## Comparing `nnsom-1.4.7.tar` & `nnsom-1.4.8.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0    16133 2020-02-02 00:00:00.000000 nnsom-1.4.7/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.7/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.7/README.md
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 nnsom-1.4.7/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0    76901 2020-02-02 00:00:00.000000 nnsom-1.4.8/src/NNSOM/plots.py
+-rw-r--r--   0        0        0    10369 2020-02-02 00:00:00.000000 nnsom-1.4.8/src/NNSOM/som.py
+-rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 nnsom-1.4.8/src/NNSOM/utils.py
+-rw-r--r--   0        0        0    16114 2020-02-02 00:00:00.000000 nnsom-1.4.8/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.8/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.8/README.md
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 nnsom-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.8/PKG-INFO
```

### Comparing `nnsom-1.4.7/.gitignore` & `nnsom-1.4.8/.gitignore`

 * *Files 0% similar despite different names*

```diff
@@ -1075,9 +1075,7 @@
 # Auto-generated tag files
 tags
 # Persistent undo
 [._]*.un~
 
 !/token.ini
 /token.ini
-/src
-src/.DS_Store
```

### Comparing `nnsom-1.4.7/pyproject.toml` & `nnsom-1.4.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/**"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.4.7"
+version = "1.4.8"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.4.7/PKG-INFO` & `nnsom-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.4.7
+Version: 1.4.8
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

