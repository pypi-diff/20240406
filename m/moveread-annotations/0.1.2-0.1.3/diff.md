# Comparing `tmp/moveread-annotations-0.1.2.tar.gz` & `tmp/moveread-annotations-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread-annotations-0.1.2.tar", last modified: Sat Apr  6 17:10:25 2024, max compression
+gzip compressed data, was "moveread-annotations-0.1.3.tar", last modified: Sat Apr  6 17:11:26 2024, max compression
```

## Comparing `moveread-annotations-0.1.2.tar` & `moveread-annotations-0.1.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:10:25.480515 moveread-annotations-0.1.2/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      866 2024-04-06 17:10:25.480515 moveread-annotations-0.1.2/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-05 16:24:36.000000 moveread-annotations-0.1.2/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      686 2024-04-06 17:10:23.000000 moveread-annotations-0.1.2/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-06 17:10:25.480515 moveread-annotations-0.1.2/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:10:25.470515 moveread-annotations-0.1.2/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:10:25.470515 moveread-annotations-0.1.2/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:10:25.470515 moveread-annotations-0.1.2/src/moveread/annotations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       86 2024-04-05 15:49:41.000000 moveread-annotations-0.1.2/src/moveread/annotations/__init__.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:10:25.470515 moveread-annotations-0.1.2/src/moveread/annotations/games/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       82 2024-04-05 18:52:46.000000 moveread-annotations-0.1.2/src/moveread/annotations/games/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1676 2024-04-06 14:11:45.000000 moveread-annotations-0.1.2/src/moveread/annotations/games/games.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:10:25.480515 moveread-annotations-0.1.2/src/moveread/annotations/images/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       77 2024-04-05 16:22:04.000000 moveread-annotations-0.1.2/src/moveread/annotations/images/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      938 2024-04-06 14:26:54.000000 moveread-annotations-0.1.2/src/moveread/annotations/images/images.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:10:25.480515 moveread-annotations-0.1.2/src/moveread/annotations/players/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      142 2024-04-05 19:04:45.000000 moveread-annotations-0.1.2/src/moveread/annotations/players/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      769 2024-04-06 14:26:36.000000 moveread-annotations-0.1.2/src/moveread/annotations/players/players.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:10:25.480515 moveread-annotations-0.1.2/src/moveread/annotations/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:03:55.000000 moveread-annotations-0.1.2/src/moveread/annotations/scripts/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1212 2024-04-06 17:09:13.000000 moveread-annotations-0.1.2/src/moveread/annotations/scripts/tsgen.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:10:25.480515 moveread-annotations-0.1.2/src/moveread/annotations/sheets/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       62 2024-04-05 16:22:22.000000 moveread-annotations-0.1.2/src/moveread/annotations/sheets/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      839 2024-04-06 14:26:45.000000 moveread-annotations-0.1.2/src/moveread/annotations/sheets/sheets.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:10:25.480515 moveread-annotations-0.1.2/src/moveread_annotations.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      866 2024-04-06 17:10:25.000000 moveread-annotations-0.1.2/src/moveread_annotations.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      782 2024-04-06 17:10:25.000000 moveread-annotations-0.1.2/src/moveread_annotations.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-06 17:10:25.000000 moveread-annotations-0.1.2/src/moveread_annotations.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       87 2024-04-06 17:10:25.000000 moveread-annotations-0.1.2/src/moveread_annotations.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       97 2024-04-06 17:10:25.000000 moveread-annotations-0.1.2/src/moveread_annotations.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-06 17:10:25.000000 moveread-annotations-0.1.2/src/moveread_annotations.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.840513 moveread-annotations-0.1.3/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      866 2024-04-06 17:11:26.840513 moveread-annotations-0.1.3/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      355 2024-04-05 16:24:36.000000 moveread-annotations-0.1.3/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      686 2024-04-06 17:11:24.000000 moveread-annotations-0.1.3/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-04-06 17:11:26.840513 moveread-annotations-0.1.3/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/moveread/annotations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       86 2024-04-05 15:49:41.000000 moveread-annotations-0.1.3/src/moveread/annotations/__init__.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/moveread/annotations/games/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       82 2024-04-05 18:52:46.000000 moveread-annotations-0.1.3/src/moveread/annotations/games/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1676 2024-04-06 14:11:45.000000 moveread-annotations-0.1.3/src/moveread/annotations/games/games.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/moveread/annotations/images/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       77 2024-04-05 16:22:04.000000 moveread-annotations-0.1.3/src/moveread/annotations/images/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      938 2024-04-06 14:26:54.000000 moveread-annotations-0.1.3/src/moveread/annotations/images/images.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/moveread/annotations/players/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      142 2024-04-05 19:04:45.000000 moveread-annotations-0.1.3/src/moveread/annotations/players/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      769 2024-04-06 14:26:36.000000 moveread-annotations-0.1.3/src/moveread/annotations/players/players.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.830513 moveread-annotations-0.1.3/src/moveread/annotations/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:03:55.000000 moveread-annotations-0.1.3/src/moveread/annotations/scripts/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1212 2024-04-06 17:09:13.000000 moveread-annotations-0.1.3/src/moveread/annotations/scripts/tsgen.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.840513 moveread-annotations-0.1.3/src/moveread/annotations/sheets/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       62 2024-04-05 16:22:22.000000 moveread-annotations-0.1.3/src/moveread/annotations/sheets/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      839 2024-04-06 14:26:45.000000 moveread-annotations-0.1.3/src/moveread/annotations/sheets/sheets.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-04-06 17:11:26.840513 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      866 2024-04-06 17:11:26.000000 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      782 2024-04-06 17:11:26.000000 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-04-06 17:11:26.000000 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       87 2024-04-06 17:11:26.000000 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       97 2024-04-06 17:11:26.000000 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-04-06 17:11:26.000000 moveread-annotations-0.1.3/src/moveread_annotations.egg-info/top_level.txt
```

### Comparing `moveread-annotations-0.1.2/PKG-INFO` & `moveread-annotations-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-annotations
-Version: 0.1.2
+Version: 0.1.3
 Summary: Annotation schemas for the Moveread Core
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-core
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: haskellian-either
```

### Comparing `moveread-annotations-0.1.2/pyproject.toml` & `moveread-annotations-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-annotations"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Annotation schemas for the Moveread Core"
 dependencies = [
   "pydantic", "haskellian-either",
   "moveread-labels", "moveread-boxes", "moveread-errors"
```

### Comparing `moveread-annotations-0.1.2/src/moveread/annotations/games/games.py` & `moveread-annotations-0.1.3/src/moveread/annotations/games/games.py`

 * *Files identical despite different names*

### Comparing `moveread-annotations-0.1.2/src/moveread/annotations/images/images.py` & `moveread-annotations-0.1.3/src/moveread/annotations/images/images.py`

 * *Files identical despite different names*

### Comparing `moveread-annotations-0.1.2/src/moveread/annotations/players/players.py` & `moveread-annotations-0.1.3/src/moveread/annotations/players/players.py`

 * *Files identical despite different names*

### Comparing `moveread-annotations-0.1.2/src/moveread/annotations/scripts/tsgen.py` & `moveread-annotations-0.1.3/src/moveread/annotations/scripts/tsgen.py`

 * *Files identical despite different names*

### Comparing `moveread-annotations-0.1.2/src/moveread/annotations/sheets/sheets.py` & `moveread-annotations-0.1.3/src/moveread/annotations/sheets/sheets.py`

 * *Files identical despite different names*

### Comparing `moveread-annotations-0.1.2/src/moveread_annotations.egg-info/PKG-INFO` & `moveread-annotations-0.1.3/src/moveread_annotations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-annotations
-Version: 0.1.2
+Version: 0.1.3
 Summary: Annotation schemas for the Moveread Core
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/python-core
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: haskellian-either
```

### Comparing `moveread-annotations-0.1.2/src/moveread_annotations.egg-info/SOURCES.txt` & `moveread-annotations-0.1.3/src/moveread_annotations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

