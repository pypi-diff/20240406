# Comparing `tmp/epidemik-0.0.8.tar.gz` & `tmp/epidemik-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.8.tar", last modified: Sat Apr  6 19:02:47 2024, max compression
+gzip compressed data, was "epidemik-0.0.9.tar", last modified: Sat Apr  6 19:07:07 2024, max compression
```

## Comparing `epidemik-0.0.8.tar` & `epidemik-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:02:47.034559 epidemik-0.0.8/
--rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.8/LICENSE
--rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 19:02:47.034380 epidemik-0.0.8/PKG-INFO
--rw-------   0 bgoncalves   (501) staff       (20)       54 2024-04-06 18:31:02.000000 epidemik-0.0.8/README.md
--rw-r--r--   0 bgoncalves   (501) staff       (20)      682 2024-04-06 19:02:36.000000 epidemik-0.0.8/pyproject.toml
--rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-06 19:02:47.034602 epidemik-0.0.8/setup.cfg
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:02:47.032836 epidemik-0.0.8/src/
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:02:47.033600 epidemik-0.0.8/src/epidemik/
--rw-------   0 bgoncalves   (501) staff       (20)    17749 2024-04-06 18:55:08.000000 epidemik-0.0.8/src/epidemik/EpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)     4701 2024-04-06 18:54:54.000000 epidemik-0.0.8/src/epidemik/NetworkEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)      289 2024-04-06 19:02:32.000000 epidemik-0.0.8/src/epidemik/__init__.py
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:02:47.034227 epidemik-0.0.8/src/epidemik.egg-info/
--rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 19:02:47.000000 epidemik-0.0.8/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 bgoncalves   (501) staff       (20)      258 2024-04-06 19:02:47.000000 epidemik-0.0.8/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-06 19:02:47.000000 epidemik-0.0.8/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-06 19:02:47.000000 epidemik-0.0.8/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:07:07.984857 epidemik-0.0.9/
+-rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.9/LICENSE
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 19:07:07.984698 epidemik-0.0.9/PKG-INFO
+-rw-------   0 bgoncalves   (501) staff       (20)       54 2024-04-06 18:31:02.000000 epidemik-0.0.9/README.md
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      682 2024-04-06 19:06:55.000000 epidemik-0.0.9/pyproject.toml
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-06 19:07:07.984894 epidemik-0.0.9/setup.cfg
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:07:07.974965 epidemik-0.0.9/src/
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:07:07.979695 epidemik-0.0.9/src/epidemik/
+-rw-------   0 bgoncalves   (501) staff       (20)    17839 2024-04-06 19:06:31.000000 epidemik-0.0.9/src/epidemik/EpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     4701 2024-04-06 18:54:54.000000 epidemik-0.0.9/src/epidemik/NetworkEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      289 2024-04-06 19:07:00.000000 epidemik-0.0.9/src/epidemik/__init__.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 19:07:07.984527 epidemik-0.0.9/src/epidemik.egg-info/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 19:07:07.000000 epidemik-0.0.9/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      258 2024-04-06 19:07:07.000000 epidemik-0.0.9/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-06 19:07:07.000000 epidemik-0.0.9/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-06 19:07:07.000000 epidemik-0.0.9/src/epidemik.egg-info/top_level.txt
```

### Comparing `epidemik-0.0.8/LICENSE` & `epidemik-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.8/PKG-INFO` & `epidemik-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.8
+Version: 0.0.9
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epidemik-0.0.8/pyproject.toml` & `epidemik-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "epidemik"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Bruno Gonçalves", email="bgoncalves@data4sci.com" },
 ]
 description = "A pakage to simulate compartmental epidemic models"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `epidemik-0.0.8/src/epidemik/EpiModel.py` & `epidemik-0.0.9/src/epidemik/EpiModel.py`

 * *Files 2% similar despite different names*

```diff
@@ -555,13 +555,16 @@
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 return np.real(eig.max())
         except:
             return None
 
     def __getitem__(self, key):
-        if key in self.values_.columns:
+        if type(key) != type([]):
+            key = set([key])
+
+        if len(key & set(self.values_.columns)) > 0:
             return self.values_[key]
-        elif key in self.values_ages_.columns:
+        elif len(key & set(self.values_ages_.columns)) > 0:
             return self.values_ages_[key]
         else:
             return None
```

### Comparing `epidemik-0.0.8/src/epidemik/NetworkEpiModel.py` & `epidemik-0.0.9/src/epidemik/NetworkEpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.8/src/epidemik.egg-info/PKG-INFO` & `epidemik-0.0.9/src/epidemik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.8
+Version: 0.0.9
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

