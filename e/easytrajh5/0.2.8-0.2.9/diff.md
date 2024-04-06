# Comparing `tmp/easytrajh5-0.2.8.tar.gz` & `tmp/easytrajh5-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytrajh5-0.2.8.tar", max compression
+gzip compressed data, was "easytrajh5-0.2.9.tar", max compression
```

## Comparing `easytrajh5-0.2.8.tar` & `easytrajh5-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1075 2023-11-06 04:17:56.072006 easytrajh5-0.2.8/LICENSE
--rw-r--r--   0        0        0    11881 2023-12-14 23:19:20.283954 easytrajh5-0.2.8/README.md
--rw-r--r--   0        0        0      151 2023-11-11 08:20:04.653180 easytrajh5-0.2.8/easytrajh5/__init__.py
--rw-r--r--   0        0        0      958 2023-11-23 04:05:58.643959 easytrajh5-0.2.8/easytrajh5/binary.py
--rw-r--r--   0        0        0     7785 2023-12-03 22:18:45.990323 easytrajh5-0.2.8/easytrajh5/cli.py
--rw-r--r--   0        0        0      720 2023-11-06 04:17:56.084931 easytrajh5-0.2.8/easytrajh5/data/select.yaml
--rw-r--r--   0        0        0     7803 2023-11-13 01:13:16.842471 easytrajh5-0.2.8/easytrajh5/fs.py
--rw-r--r--   0        0        0    11359 2023-12-14 23:19:20.285183 easytrajh5-0.2.8/easytrajh5/h5.py
--rw-r--r--   0        0        0     2122 2023-11-08 04:33:44.565318 easytrajh5-0.2.8/easytrajh5/manager.py
--rw-r--r--   0        0        0     7244 2023-11-06 04:17:56.083335 easytrajh5-0.2.8/easytrajh5/pdb.py
--rw-r--r--   0        0        0     1070 2023-12-11 22:58:59.065643 easytrajh5-0.2.8/easytrajh5/quantity.py
--rw-r--r--   0        0        0    13067 2023-11-28 02:00:48.931879 easytrajh5-0.2.8/easytrajh5/select.py
--rw-r--r--   0        0        0     7779 2023-11-28 01:53:47.376240 easytrajh5-0.2.8/easytrajh5/show.py
--rw-r--r--   0        0        0     5883 2023-12-19 05:42:19.411545 easytrajh5-0.2.8/easytrajh5/struct.py
--rw-r--r--   0        0        0    25004 2023-12-19 06:17:40.252636 easytrajh5-0.2.8/easytrajh5/traj.py
--rw-r--r--   0        0        0      543 2023-12-19 05:47:23.883014 easytrajh5-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    12629 1970-01-01 00:00:00.000000 easytrajh5-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-11-06 04:17:56.072006 easytrajh5-0.2.9/LICENSE
+-rw-r--r--   0        0        0    11881 2023-12-14 23:19:20.283954 easytrajh5-0.2.9/README.md
+-rw-r--r--   0        0        0      151 2023-11-11 08:20:04.653180 easytrajh5-0.2.9/easytrajh5/__init__.py
+-rw-r--r--   0        0        0      958 2023-11-23 04:05:58.643959 easytrajh5-0.2.9/easytrajh5/binary.py
+-rw-r--r--   0        0        0     7785 2023-12-03 22:18:45.990323 easytrajh5-0.2.9/easytrajh5/cli.py
+-rw-r--r--   0        0        0      720 2023-11-06 04:17:56.084931 easytrajh5-0.2.9/easytrajh5/data/select.yaml
+-rw-r--r--   0        0        0     7803 2023-11-13 01:13:16.842471 easytrajh5-0.2.9/easytrajh5/fs.py
+-rw-r--r--   0        0        0    11359 2023-12-14 23:19:20.285183 easytrajh5-0.2.9/easytrajh5/h5.py
+-rw-r--r--   0        0        0     2122 2023-11-08 04:33:44.565318 easytrajh5-0.2.9/easytrajh5/manager.py
+-rw-r--r--   0        0        0     7244 2023-11-06 04:17:56.083335 easytrajh5-0.2.9/easytrajh5/pdb.py
+-rw-r--r--   0        0        0     1070 2023-12-11 22:58:59.065643 easytrajh5-0.2.9/easytrajh5/quantity.py
+-rw-r--r--   0        0        0    13067 2023-11-28 02:00:48.931879 easytrajh5-0.2.9/easytrajh5/select.py
+-rw-r--r--   0        0        0     7779 2023-11-28 01:53:47.376240 easytrajh5-0.2.9/easytrajh5/show.py
+-rw-r--r--   0        0        0     5980 2023-12-20 23:38:18.647016 easytrajh5-0.2.9/easytrajh5/struct.py
+-rw-r--r--   0        0        0    25004 2023-12-19 06:17:40.252636 easytrajh5-0.2.9/easytrajh5/traj.py
+-rw-r--r--   0        0        0      543 2023-12-20 23:50:49.273352 easytrajh5-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    12629 1970-01-01 00:00:00.000000 easytrajh5-0.2.9/PKG-INFO
```

### Comparing `easytrajh5-0.2.8/LICENSE` & `easytrajh5-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/README.md` & `easytrajh5-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/easytrajh5/binary.py` & `easytrajh5-0.2.9/easytrajh5/binary.py`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/easytrajh5/cli.py` & `easytrajh5-0.2.9/easytrajh5/cli.py`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/easytrajh5/data/select.yaml` & `easytrajh5-0.2.9/easytrajh5/data/select.yaml`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/easytrajh5/fs.py` & `easytrajh5-0.2.9/easytrajh5/fs.py`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/easytrajh5/h5.py` & `easytrajh5-0.2.9/easytrajh5/h5.py`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/easytrajh5/manager.py` & `easytrajh5-0.2.9/easytrajh5/manager.py`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/easytrajh5/pdb.py` & `easytrajh5-0.2.9/easytrajh5/pdb.py`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/easytrajh5/quantity.py` & `easytrajh5-0.2.9/easytrajh5/quantity.py`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/easytrajh5/select.py` & `easytrajh5-0.2.9/easytrajh5/select.py`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/easytrajh5/show.py` & `easytrajh5-0.2.9/easytrajh5/show.py`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/easytrajh5/struct.py` & `easytrajh5-0.2.9/easytrajh5/struct.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,8 +167,13 @@
 
     return [e[1] for e in top_entries]
 
 
 def slice_parmed(pmd: parmed.Structure, i_atoms: [int]) -> parmed.Structure:
     # This function avoids the issue where parmed expects a bit
     # mask for selections for full selections but atom indices otherwise
-    return pmd if len(i_atoms) == len(pmd.atoms) else pmd[i_atoms]
+    if len(i_atoms) == len(pmd.atoms):
+        return pmd
+    result = pmd[i_atoms]
+    if hasattr(pmd, 'extra'):
+        result.extra = pmd.extra
+    return result
```

### Comparing `easytrajh5-0.2.8/easytrajh5/traj.py` & `easytrajh5-0.2.9/easytrajh5/traj.py`

 * *Files identical despite different names*

### Comparing `easytrajh5-0.2.8/pyproject.toml` & `easytrajh5-0.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easytrajh5"
-version = "0.2.8"
+version = "0.2.9"
 description = "MD trajectory library"
 authors = ["Bosco Ho <apposite@gmail.com>"]
 readme = "README.md"
 packages = [{include = "easytrajh5"}]
 
 [tool.poetry.scripts]
 easyh5 = 'easytrajh5.cli:h5'
```

### Comparing `easytrajh5-0.2.8/PKG-INFO` & `easytrajh5-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytrajh5
-Version: 0.2.8
+Version: 0.2.9
 Summary: MD trajectory library
 Author: Bosco Ho
 Author-email: apposite@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

