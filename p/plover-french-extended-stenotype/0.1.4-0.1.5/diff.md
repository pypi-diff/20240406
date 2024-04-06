# Comparing `tmp/plover-french-extended-stenotype-0.1.4.tar.gz` & `tmp/plover-french-extended-stenotype-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plover-french-extended-stenotype-0.1.4.tar", last modified: Wed Feb 28 19:24:36 2024, max compression
+gzip compressed data, was "plover-french-extended-stenotype-0.1.5.tar", last modified: Fri Mar  1 10:27:27 2024, max compression
```

## Comparing `plover-french-extended-stenotype-0.1.4.tar` & `plover-french-extended-stenotype-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 stl       (1000) stl       (1000)        0 2024-02-28 19:24:36.076635 plover-french-extended-stenotype-0.1.4/
--rw-r--r--   0 stl       (1000) stl       (1000)     1481 2024-02-28 19:24:36.076635 plover-french-extended-stenotype-0.1.4/PKG-INFO
--rw-r--r--   0 stl       (1000) stl       (1000)      681 2024-02-28 12:53:31.000000 plover-french-extended-stenotype-0.1.4/README.md
-drwxr-xr-x   0 stl       (1000) stl       (1000)        0 2024-02-28 19:24:36.076635 plover-french-extended-stenotype-0.1.4/french_extended_stenotype/
--rw-r--r--   0 stl       (1000) stl       (1000)        0 2024-02-28 18:03:15.000000 plover-french-extended-stenotype-0.1.4/french_extended_stenotype/__init__.py
--rw-r--r--   0 stl       (1000) stl       (1000)     2294 2024-02-28 18:55:45.000000 plover-french-extended-stenotype-0.1.4/french_extended_stenotype/system.py
-drwxr-xr-x   0 stl       (1000) stl       (1000)        0 2024-02-28 19:24:36.076635 plover-french-extended-stenotype-0.1.4/plover_french_extended_stenotype.egg-info/
--rw-r--r--   0 stl       (1000) stl       (1000)     1481 2024-02-28 19:24:36.000000 plover-french-extended-stenotype-0.1.4/plover_french_extended_stenotype.egg-info/PKG-INFO
--rw-r--r--   0 stl       (1000) stl       (1000)      491 2024-02-28 19:24:36.000000 plover-french-extended-stenotype-0.1.4/plover_french_extended_stenotype.egg-info/SOURCES.txt
--rw-r--r--   0 stl       (1000) stl       (1000)        1 2024-02-28 19:24:36.000000 plover-french-extended-stenotype-0.1.4/plover_french_extended_stenotype.egg-info/dependency_links.txt
--rw-r--r--   0 stl       (1000) stl       (1000)       77 2024-02-28 19:24:36.000000 plover-french-extended-stenotype-0.1.4/plover_french_extended_stenotype.egg-info/entry_points.txt
--rw-r--r--   0 stl       (1000) stl       (1000)       19 2024-02-28 19:24:36.000000 plover-french-extended-stenotype-0.1.4/plover_french_extended_stenotype.egg-info/requires.txt
--rw-r--r--   0 stl       (1000) stl       (1000)       26 2024-02-28 19:24:36.000000 plover-french-extended-stenotype-0.1.4/plover_french_extended_stenotype.egg-info/top_level.txt
--rw-r--r--   0 stl       (1000) stl       (1000)        1 2024-02-28 13:11:33.000000 plover-french-extended-stenotype-0.1.4/plover_french_extended_stenotype.egg-info/zip-safe
--rw-r--r--   0 stl       (1000) stl       (1000)     1108 2024-02-28 19:24:36.076635 plover-french-extended-stenotype-0.1.4/setup.cfg
--rwxr-xr-x   0 stl       (1000) stl       (1000)       63 2024-02-28 12:53:31.000000 plover-french-extended-stenotype-0.1.4/setup.py
+drwxr-xr-x   0 stl       (1000) stl       (1000)        0 2024-03-01 10:27:27.164507 plover-french-extended-stenotype-0.1.5/
+-rw-r--r--   0 stl       (1000) stl       (1000)     1528 2024-03-01 10:27:27.164507 plover-french-extended-stenotype-0.1.5/PKG-INFO
+-rw-r--r--   0 stl       (1000) stl       (1000)      681 2024-02-28 12:53:31.000000 plover-french-extended-stenotype-0.1.5/README.md
+drwxr-xr-x   0 stl       (1000) stl       (1000)        0 2024-03-01 10:27:27.160507 plover-french-extended-stenotype-0.1.5/french_extended_stenotype/
+-rw-r--r--   0 stl       (1000) stl       (1000)        0 2024-02-28 18:03:15.000000 plover-french-extended-stenotype-0.1.5/french_extended_stenotype/__init__.py
+-rw-r--r--   0 stl       (1000) stl       (1000)     2310 2024-03-01 10:20:11.000000 plover-french-extended-stenotype-0.1.5/french_extended_stenotype/system.py
+drwxr-xr-x   0 stl       (1000) stl       (1000)        0 2024-03-01 10:27:27.164507 plover-french-extended-stenotype-0.1.5/plover_french_extended_stenotype.egg-info/
+-rw-r--r--   0 stl       (1000) stl       (1000)     1528 2024-03-01 10:27:27.000000 plover-french-extended-stenotype-0.1.5/plover_french_extended_stenotype.egg-info/PKG-INFO
+-rw-r--r--   0 stl       (1000) stl       (1000)      491 2024-03-01 10:27:27.000000 plover-french-extended-stenotype-0.1.5/plover_french_extended_stenotype.egg-info/SOURCES.txt
+-rw-r--r--   0 stl       (1000) stl       (1000)        1 2024-03-01 10:27:27.000000 plover-french-extended-stenotype-0.1.5/plover_french_extended_stenotype.egg-info/dependency_links.txt
+-rw-r--r--   0 stl       (1000) stl       (1000)       77 2024-03-01 10:27:27.000000 plover-french-extended-stenotype-0.1.5/plover_french_extended_stenotype.egg-info/entry_points.txt
+-rw-r--r--   0 stl       (1000) stl       (1000)       51 2024-03-01 10:27:27.000000 plover-french-extended-stenotype-0.1.5/plover_french_extended_stenotype.egg-info/requires.txt
+-rw-r--r--   0 stl       (1000) stl       (1000)       26 2024-03-01 10:27:27.000000 plover-french-extended-stenotype-0.1.5/plover_french_extended_stenotype.egg-info/top_level.txt
+-rw-r--r--   0 stl       (1000) stl       (1000)        1 2024-02-28 13:11:33.000000 plover-french-extended-stenotype-0.1.5/plover_french_extended_stenotype.egg-info/zip-safe
+-rw-r--r--   0 stl       (1000) stl       (1000)     1141 2024-03-01 10:27:27.164507 plover-french-extended-stenotype-0.1.5/setup.cfg
+-rwxr-xr-x   0 stl       (1000) stl       (1000)       63 2024-02-28 12:53:31.000000 plover-french-extended-stenotype-0.1.5/setup.py
```

### Comparing `plover-french-extended-stenotype-0.1.4/PKG-INFO` & `plover-french-extended-stenotype-0.1.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover-french-extended-stenotype
-Version: 0.1.4
+Version: 0.1.5
 Summary: Plover French Stenotype layout with extra keys
 Home-page: https://forge.gresille.org/stl/plover-french-extended-stenotype.git
 Author: stl
 Keywords: plover plover_plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: plover>=4.0.0.dev8
+Requires-Dist: plover_python_dictionary>=0.5.6
 
 # Plover French Extended Stenotype
 
 Plover plugin for an extended Stenotype layout and French dictionnary generated by Pluvier.
 
 ## Warning : Alpha version
```

### Comparing `plover-french-extended-stenotype-0.1.4/README.md` & `plover-french-extended-stenotype-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `plover-french-extended-stenotype-0.1.4/french_extended_stenotype/system.py` & `plover-french-extended-stenotype-0.1.5/french_extended_stenotype/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,11 +63,11 @@
 
 
 
 DICTIONARIES_ROOT = 'asset:french_extended_stenotype:dictionaries'
 
 DEFAULT_DICTIONARIES = (
     'fr_spelling.json',
-    'dicofr.json',
+    'pluvier_dicofr.json',
     'orthofr.json',
-    'verbs.json'
+    'pluvier_verbs.json'
 )
```

### Comparing `plover-french-extended-stenotype-0.1.4/plover_french_extended_stenotype.egg-info/PKG-INFO` & `plover-french-extended-stenotype-0.1.5/plover_french_extended_stenotype.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plover-french-extended-stenotype
-Version: 0.1.4
+Version: 0.1.5
 Summary: Plover French Stenotype layout with extra keys
 Home-page: https://forge.gresille.org/stl/plover-french-extended-stenotype.git
 Author: stl
 Keywords: plover plover_plugin
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: End Users/Desktop
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 Requires-Dist: plover>=4.0.0.dev8
+Requires-Dist: plover_python_dictionary>=0.5.6
 
 # Plover French Extended Stenotype
 
 Plover plugin for an extended Stenotype layout and French dictionnary generated by Pluvier.
 
 ## Warning : Alpha version
```

### Comparing `plover-french-extended-stenotype-0.1.4/setup.cfg` & `plover-french-extended-stenotype-0.1.5/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = plover-french-extended-stenotype
-version = 0.1.4
+version = 0.1.5
 description = Plover French Stenotype layout with extra keys
 long_description = file:README.md
 long_description_content_type = text/markdown
 keywords = plover plover_plugin
 author = stl
 author_mail = stl@gresille.org
 licence = Gnu General Public Licence v3 or later
@@ -22,14 +22,15 @@
 
 [options]
 zip_safe = True
 setup_requires = 
 	setuptools>=30.3.0
 install_requires = 
 	plover>=4.0.0.dev8
+	plover_python_dictionary>=0.5.6
 include_package_data = True
 packages = 
 	french_extended_stenotype
 
 [options.entry_points]
 plover.system = 
 	French Extended Stenotype = french_extended_stenotype.system
```

