# Comparing `tmp/nnsom-1.4.5.tar.gz` & `tmp/nnsom-1.4.6.tar.gz`

## Comparing `nnsom-1.4.5.tar` & `nnsom-1.4.6.tar`

### file list

```diff
@@ -1,8 +1,5 @@
--rw-r--r--   0        0        0    58907 2020-02-02 00:00:00.000000 nnsom-1.4.5/src/NNSOM/plots.py
--rw-r--r--   0        0        0    10365 2020-02-02 00:00:00.000000 nnsom-1.4.5/src/NNSOM/som.py
--rw-r--r--   0        0        0    22430 2020-02-02 00:00:00.000000 nnsom-1.4.5/src/NNSOM/utils.py
--rw-r--r--   0        0        0    16144 2020-02-02 00:00:00.000000 nnsom-1.4.5/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.5/LICENSE
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.5/README.md
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0    16163 2020-02-02 00:00:00.000000 nnsom-1.4.6/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nnsom-1.4.6/LICENSE
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nnsom-1.4.6/README.md
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 nnsom-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 nnsom-1.4.6/PKG-INFO
```

### Comparing `nnsom-1.4.5/.gitignore` & `nnsom-1.4.6/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1080,7 +1080,9 @@
 # Auto-generated tag files
 tags
 # Persistent undo
 [._]*.un~
 
 !/token.ini
 /token.ini
+/src
+src/.DS_Store
```

### Comparing `nnsom-1.4.5/pyproject.toml` & `nnsom-1.4.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 include = ["src/NNSOM/*.py"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/NNSOM"]
 
 [project]
 name = "NNSOM"
-version = "1.4.5"
+version = "1.4.6"
 description = "A SOM package"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 authors = [
   { name = "Dr. Hagan" },
   { name = "Dr. Amir Jafari", email = "amir.h.jafari@okstate.edu" },
```

### Comparing `nnsom-1.4.5/PKG-INFO` & `nnsom-1.4.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: NNSOM
-Version: 1.4.5
+Version: 1.4.6
 Summary: A SOM package
 Project-URL: Repository, https://github.com/amir-jafari/SOM
 Project-URL: Issues, https://github.com/amir-jafari/SOM/issues
 Author: Dr. Hagan, Lakshmi Sravya Chalapati, Ei Tanaka
 Author-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 Maintainer-email: "Dr. Amir Jafari" <amir.h.jafari@okstate.edu>
 License-File: LICENSE
```

