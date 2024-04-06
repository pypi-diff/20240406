# Comparing `tmp/epidemik-0.0.5.tar.gz` & `tmp/epidemik-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epidemik-0.0.5.tar", last modified: Sat Apr  6 18:48:54 2024, max compression
+gzip compressed data, was "epidemik-0.0.6.tar", last modified: Sat Apr  6 18:50:26 2024, max compression
```

## Comparing `epidemik-0.0.5.tar` & `epidemik-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:48:54.268358 epidemik-0.0.5/
--rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.5/LICENSE
--rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 18:48:54.268176 epidemik-0.0.5/PKG-INFO
--rw-------   0 bgoncalves   (501) staff       (20)       54 2024-04-06 18:31:02.000000 epidemik-0.0.5/README.md
--rw-r--r--   0 bgoncalves   (501) staff       (20)      682 2024-04-06 18:46:32.000000 epidemik-0.0.5/pyproject.toml
--rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-06 18:48:54.268419 epidemik-0.0.5/setup.cfg
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:48:54.266435 epidemik-0.0.5/src/
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:48:54.267296 epidemik-0.0.5/src/epidemik/
--rw-------   0 bgoncalves   (501) staff       (20)    19363 2024-04-06 18:03:54.000000 epidemik-0.0.5/src/epidemik/EpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)     5961 2024-04-06 18:47:57.000000 epidemik-0.0.5/src/epidemik/NetworkEpiModel.py
--rw-r--r--   0 bgoncalves   (501) staff       (20)       94 2024-04-06 18:46:28.000000 epidemik-0.0.5/src/epidemik/__init__.py
-drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:48:54.267998 epidemik-0.0.5/src/epidemik.egg-info/
--rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 18:48:54.000000 epidemik-0.0.5/src/epidemik.egg-info/PKG-INFO
--rw-r--r--   0 bgoncalves   (501) staff       (20)      258 2024-04-06 18:48:54.000000 epidemik-0.0.5/src/epidemik.egg-info/SOURCES.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-06 18:48:54.000000 epidemik-0.0.5/src/epidemik.egg-info/dependency_links.txt
--rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-06 18:48:54.000000 epidemik-0.0.5/src/epidemik.egg-info/top_level.txt
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:50:26.595429 epidemik-0.0.6/
+-rw-------   0 bgoncalves   (501) staff       (20)     1073 2023-11-16 01:11:51.000000 epidemik-0.0.6/LICENSE
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 18:50:26.595218 epidemik-0.0.6/PKG-INFO
+-rw-------   0 bgoncalves   (501) staff       (20)       54 2024-04-06 18:31:02.000000 epidemik-0.0.6/README.md
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      682 2024-04-06 18:50:09.000000 epidemik-0.0.6/pyproject.toml
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       38 2024-04-06 18:50:26.595473 epidemik-0.0.6/setup.cfg
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:50:26.593719 epidemik-0.0.6/src/
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:50:26.594447 epidemik-0.0.6/src/epidemik/
+-rw-------   0 bgoncalves   (501) staff       (20)    19363 2024-04-06 18:03:54.000000 epidemik-0.0.6/src/epidemik/EpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)     5961 2024-04-06 18:47:57.000000 epidemik-0.0.6/src/epidemik/NetworkEpiModel.py
+-rw-r--r--   0 bgoncalves   (501) staff       (20)       96 2024-04-06 18:50:11.000000 epidemik-0.0.6/src/epidemik/__init__.py
+drwxr-xr-x   0 bgoncalves   (501) staff       (20)        0 2024-04-06 18:50:26.595029 epidemik-0.0.6/src/epidemik.egg-info/
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      592 2024-04-06 18:50:26.000000 epidemik-0.0.6/src/epidemik.egg-info/PKG-INFO
+-rw-r--r--   0 bgoncalves   (501) staff       (20)      258 2024-04-06 18:50:26.000000 epidemik-0.0.6/src/epidemik.egg-info/SOURCES.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        1 2024-04-06 18:50:26.000000 epidemik-0.0.6/src/epidemik.egg-info/dependency_links.txt
+-rw-r--r--   0 bgoncalves   (501) staff       (20)        9 2024-04-06 18:50:26.000000 epidemik-0.0.6/src/epidemik.egg-info/top_level.txt
```

### Comparing `epidemik-0.0.5/LICENSE` & `epidemik-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.5/PKG-INFO` & `epidemik-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.5
+Version: 0.0.6
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `epidemik-0.0.5/pyproject.toml` & `epidemik-0.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "epidemik"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Bruno Gonçalves", email="bgoncalves@data4sci.com" },
 ]
 description = "A pakage to simulate compartmental epidemic models"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `epidemik-0.0.5/src/epidemik/EpiModel.py` & `epidemik-0.0.6/src/epidemik/EpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.5/src/epidemik/NetworkEpiModel.py` & `epidemik-0.0.6/src/epidemik/NetworkEpiModel.py`

 * *Files identical despite different names*

### Comparing `epidemik-0.0.5/src/epidemik.egg-info/PKG-INFO` & `epidemik-0.0.6/src/epidemik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epidemik
-Version: 0.0.5
+Version: 0.0.6
 Summary: A pakage to simulate compartmental epidemic models
 Author-email: Bruno Gonçalves <bgoncalves@data4sci.com>
 Project-URL: Homepage, https://github.com/DataForScience/epidemik
 Project-URL: Issues, https://github.com/DataForScience/epidemik/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

