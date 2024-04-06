# Comparing `tmp/seeder-0.0.1.tar.gz` & `tmp/seeder-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seeder-0.0.1.tar", last modified: Sat Apr  6 13:37:38 2024, max compression
+gzip compressed data, was "seeder-0.0.2.tar", last modified: Sat Apr  6 13:43:22 2024, max compression
```

## Comparing `seeder-0.0.1.tar` & `seeder-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 13:37:38.968754 seeder-0.0.1/
--rw-r--r--   0 solst      (501) staff       (20)    11337 2024-04-06 12:52:34.000000 seeder-0.0.1/LICENSE
--rw-r--r--   0 solst      (501) staff       (20)      111 2024-04-06 12:52:34.000000 seeder-0.0.1/MANIFEST.in
--rw-r--r--   0 solst      (501) staff       (20)     3284 2024-04-06 13:37:38.968624 seeder-0.0.1/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)     2704 2024-04-06 13:33:05.000000 seeder-0.0.1/README.md
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 13:37:38.968068 seeder-0.0.1/seeder.egg-info/
--rw-r--r--   0 solst      (501) staff       (20)     3284 2024-04-06 13:37:38.000000 seeder-0.0.1/seeder.egg-info/PKG-INFO
--rw-r--r--   0 solst      (501) staff       (20)      305 2024-04-06 13:37:38.000000 seeder-0.0.1/seeder.egg-info/SOURCES.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 13:37:38.000000 seeder-0.0.1/seeder.egg-info/dependency_links.txt
--rw-r--r--   0 solst      (501) staff       (20)       28 2024-04-06 13:37:38.000000 seeder-0.0.1/seeder.egg-info/entry_points.txt
--rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 13:36:40.000000 seeder-0.0.1/seeder.egg-info/not-zip-safe
--rw-r--r--   0 solst      (501) staff       (20)       67 2024-04-06 13:37:38.000000 seeder-0.0.1/seeder.egg-info/requires.txt
--rw-r--r--   0 solst      (501) staff       (20)        4 2024-04-06 13:37:38.000000 seeder-0.0.1/seeder.egg-info/top_level.txt
--rw-r--r--   0 solst      (501) staff       (20)      835 2024-04-06 13:36:11.000000 seeder-0.0.1/settings.ini
--rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-06 13:37:38.968787 seeder-0.0.1/setup.cfg
--rw-r--r--   0 solst      (501) staff       (20)     2585 2024-04-06 12:52:34.000000 seeder-0.0.1/setup.py
-drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 13:37:38.968439 seeder-0.0.1/sow/
--rw-r--r--   0 solst      (501) staff       (20)      319 2024-04-06 13:37:30.000000 seeder-0.0.1/sow/__init__.py
--rw-r--r--   0 solst      (501) staff       (20)     1533 2024-04-06 13:37:30.000000 seeder-0.0.1/sow/_modidx.py
--rw-r--r--   0 solst      (501) staff       (20)     5710 2024-04-06 13:37:30.000000 seeder-0.0.1/sow/core.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 13:43:22.654079 seeder-0.0.2/
+-rw-r--r--   0 solst      (501) staff       (20)    11337 2024-04-06 12:52:34.000000 seeder-0.0.2/LICENSE
+-rw-r--r--   0 solst      (501) staff       (20)      111 2024-04-06 12:52:34.000000 seeder-0.0.2/MANIFEST.in
+-rw-r--r--   0 solst      (501) staff       (20)     3287 2024-04-06 13:43:22.653951 seeder-0.0.2/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)     2704 2024-04-06 13:33:05.000000 seeder-0.0.2/README.md
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 13:43:22.653056 seeder-0.0.2/seeder/
+-rw-r--r--   0 solst      (501) staff       (20)      324 2024-04-06 13:43:12.000000 seeder-0.0.2/seeder/__init__.py
+-rw-r--r--   0 solst      (501) staff       (20)     1668 2024-04-06 13:43:12.000000 seeder-0.0.2/seeder/_modidx.py
+-rw-r--r--   0 solst      (501) staff       (20)     5710 2024-04-06 13:43:12.000000 seeder-0.0.2/seeder/core.py
+drwxr-xr-x   0 solst      (501) staff       (20)        0 2024-04-06 13:43:22.653807 seeder-0.0.2/seeder.egg-info/
+-rw-r--r--   0 solst      (501) staff       (20)     3287 2024-04-06 13:43:22.000000 seeder-0.0.2/seeder.egg-info/PKG-INFO
+-rw-r--r--   0 solst      (501) staff       (20)      314 2024-04-06 13:43:22.000000 seeder-0.0.2/seeder.egg-info/SOURCES.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 13:43:22.000000 seeder-0.0.2/seeder.egg-info/dependency_links.txt
+-rw-r--r--   0 solst      (501) staff       (20)       34 2024-04-06 13:43:22.000000 seeder-0.0.2/seeder.egg-info/entry_points.txt
+-rw-r--r--   0 solst      (501) staff       (20)        1 2024-04-06 13:36:40.000000 seeder-0.0.2/seeder.egg-info/not-zip-safe
+-rw-r--r--   0 solst      (501) staff       (20)       67 2024-04-06 13:43:22.000000 seeder-0.0.2/seeder.egg-info/requires.txt
+-rw-r--r--   0 solst      (501) staff       (20)        7 2024-04-06 13:43:22.000000 seeder-0.0.2/seeder.egg-info/top_level.txt
+-rw-r--r--   0 solst      (501) staff       (20)      847 2024-04-06 13:43:08.000000 seeder-0.0.2/settings.ini
+-rw-r--r--   0 solst      (501) staff       (20)       38 2024-04-06 13:43:22.654114 seeder-0.0.2/setup.cfg
+-rw-r--r--   0 solst      (501) staff       (20)     2585 2024-04-06 12:52:34.000000 seeder-0.0.2/setup.py
```

### Comparing `seeder-0.0.1/LICENSE` & `seeder-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `seeder-0.0.1/PKG-INFO` & `seeder-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: seeder
-Version: 0.0.1
+Version: 0.0.2
 Summary: util torch
-Home-page: https://github.com/dsm-72/sow
+Home-page: https://github.com/dsm-72/seeder
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for seeding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `seeder-0.0.1/README.md` & `seeder-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `seeder-0.0.1/seeder.egg-info/PKG-INFO` & `seeder-0.0.2/seeder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: seeder
-Version: 0.0.1
+Version: 0.0.2
 Summary: util torch
-Home-page: https://github.com/dsm-72/sow
+Home-page: https://github.com/dsm-72/seeder
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: utility for seeding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `seeder-0.0.1/settings.ini` & `seeder-0.0.2/settings.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [DEFAULT]
 repo = seeder
 lib_name = seeder
-version = 0.0.1
+version = 0.0.2
 min_python = 3.11
 license = apache2
 black_formatting = False
 doc_path = _docs
-lib_path = sow
+lib_path = seeder
 nbs_path = nbs
 recursive = True
 tst_flags = notest
 put_version_in_init = True
 branch = main
 custom_sidebar = False
 doc_host = https://dsm-72.github.io
-doc_baseurl = /sow
-git_url = https://github.com/dsm-72/sow
-title = sow
+doc_baseurl = /seeder
+git_url = https://github.com/dsm-72/seeder
+title = seeder
 audience = Developers
 author = dsm-72
 author_email = sumner.magruder@yale.edu
 copyright = 2023 onwards, dsm-72
 description = util torch
 keywords = utility for seeding
 language = English
```

### Comparing `seeder-0.0.1/setup.py` & `seeder-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `seeder-0.0.1/sow/core.py` & `seeder-0.0.2/seeder/core.py`

 * *Files identical despite different names*

