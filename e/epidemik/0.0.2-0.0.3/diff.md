# Comparing `tmp/epidemik-0.0.2.tar.gz` & `tmp/epidemik-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.2.tar", last modified: Sat Apr  6 18:26:30 2024, max compression
+gzip compressed data, was "epidemik-0.0.3.tar", last modified: Sat Apr  6 18:37:27 2024, max compression
```

## Comparing `epidemik-0.0.2.tar` & `epidemik-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:26:30.251761 epidemik-0.0.2/
--rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.2/LICENSE
--rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 18:26:30.251615 epidemik-0.0.2/PKG-INFO
--rw-------   0 bgoncalves   (501) staff       (20)       54 2024-04-06 18:19:33.000000 epidemik-0.0.2/README.md
--rw-r--r--   0 bgoncalves   (501) staff       (20)      682 2024-04-06 18:26:05.000000 epidemik-0.0.2/pyproject.toml
--rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-06 18:26:30.251798 epidemik-0.0.2/setup.cfg
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:26:30.250364 epidemik-0.0.2/src/
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:26:30.250936 epidemik-0.0.2/src/epidemik/
--rw-------   0 bgoncalves   (501) staff       (20)    19363 2024-04-06 18:03:54.000000 epidemik-0.0.2/src/epidemik/EpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)        0 2024-04-06 17:50:03.000000 epidemik-0.0.2/src/epidemik/__init__.py
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:26:30.251470 epidemik-0.0.2/src/epidemik.egg-info/
--rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 18:26:30.000000 epidemik-0.0.2/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 bgoncalves   (501) staff       (20)      226 2024-04-06 18:26:30.000000 epidemik-0.0.2/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-06 18:26:30.000000 epidemik-0.0.2/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-06 18:26:30.000000 epidemik-0.0.2/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:37:27.797661 epidemik-0.0.3/
+-rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.3/LICENSE
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 18:37:27.797465 epidemik-0.0.3/PKG-INFO
+-rw-------   0 bgoncalves   (501) staff       (20)       54 2024-04-06 18:31:02.000000 epidemik-0.0.3/README.md
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      682 2024-04-06 18:37:22.000000 epidemik-0.0.3/pyproject.toml
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-06 18:37:27.797701 epidemik-0.0.3/setup.cfg
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:37:27.796104 epidemik-0.0.3/src/
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:37:27.796707 epidemik-0.0.3/src/epidemik/
+-rw-------   0 bgoncalves   (501) staff       (20)    19363 2024-04-06 18:03:54.000000 epidemik-0.0.3/src/epidemik/EpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       29 2024-04-06 18:37:05.000000 epidemik-0.0.3/src/epidemik/__init__.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:37:27.797275 epidemik-0.0.3/src/epidemik.egg-info/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 18:37:27.000000 epidemik-0.0.3/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      226 2024-04-06 18:37:27.000000 epidemik-0.0.3/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-06 18:37:27.000000 epidemik-0.0.3/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       13 2024-04-06 18:37:27.000000 epidemik-0.0.3/src/epidemik.egg-info/top_level.txt
```

### Comparing `epidemik-0.0.2/LICENSE` & `epidemik-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.2/PKG-INFO` & `epidemik-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# epidemia - Compartmental Epidemic Models in Python
+# epidemik - Compartmental Epidemic Models in Python
```

### Comparing `epidemik-0.0.2/pyproject.toml` & `epidemik-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "epidemik"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Bruno Gonçalves", email="bgoncalves@data4sci.com" },
 ]
 description = "A pakage to simulate compartmental epidemic models"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `epidemik-0.0.2/src/epidemik/EpiModel.py` & `epidemik-0.0.3/src/epidemik/EpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.2/src/epidemik.egg-info/PKG-INFO` & `epidemik-0.0.3/src/epidemik.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.2
+Version: 0.0.3
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# epidemia - Compartmental Epidemic Models in Python
+# epidemik - Compartmental Epidemic Models in Python
```

