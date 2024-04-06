# Comparing `tmp/PathMePy-Gustoon-0.1.3.tar.gz` & `tmp/PathMePy-Gustoon-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PathMePy-Gustoon-0.1.3.tar", last modified: Mon Apr  1 08:05:59 2024, max compression
+gzip compressed data, was "PathMePy-Gustoon-0.2.tar", last modified: Sat Apr  6 08:43:07 2024, max compression
```

## Comparing `PathMePy-Gustoon-0.1.3.tar` & `PathMePy-Gustoon-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 08:05:59.457969 PathMePy-Gustoon-0.1.3/
--rw-rw-rw-   0        0        0     1069 2024-03-30 08:45:32.000000 PathMePy-Gustoon-0.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0      839 2024-04-01 08:05:59.454969 PathMePy-Gustoon-0.1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-01 08:05:59.404998 PathMePy-Gustoon-0.1.3/PathMePy_Gustoon/
--rw-rw-rw-   0        0        0      881 2024-04-01 08:05:03.000000 PathMePy-Gustoon-0.1.3/PathMePy_Gustoon/PathMePy.py
--rw-rw-rw-   0        0        0       75 2024-03-31 08:26:07.000000 PathMePy-Gustoon-0.1.3/PathMePy_Gustoon/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-01 08:05:59.451972 PathMePy-Gustoon-0.1.3/PathMePy_Gustoon.egg-info/
--rw-rw-rw-   0        0        0      839 2024-04-01 08:05:59.000000 PathMePy-Gustoon-0.1.3/PathMePy_Gustoon.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2024-04-01 08:05:59.000000 PathMePy-Gustoon-0.1.3/PathMePy_Gustoon.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 08:05:59.000000 PathMePy-Gustoon-0.1.3/PathMePy_Gustoon.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-04-01 08:05:59.000000 PathMePy-Gustoon-0.1.3/PathMePy_Gustoon.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      456 2024-03-31 08:33:03.000000 PathMePy-Gustoon-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-04-01 08:05:59.457969 PathMePy-Gustoon-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      909 2024-04-01 08:05:24.000000 PathMePy-Gustoon-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-06 08:43:07.377271 PathMePy-Gustoon-0.2/
+-rw-rw-rw-   0        0        0     1069 2024-03-30 08:45:32.000000 PathMePy-Gustoon-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      837 2024-04-06 08:43:07.366726 PathMePy-Gustoon-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-06 08:43:07.304329 PathMePy-Gustoon-0.2/PathMePy_Gustoon/
+-rw-rw-rw-   0        0        0     1162 2024-04-06 08:41:04.000000 PathMePy-Gustoon-0.2/PathMePy_Gustoon/PathMePy.py
+-rw-rw-rw-   0        0        0       75 2024-03-31 08:26:07.000000 PathMePy-Gustoon-0.2/PathMePy_Gustoon/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-06 08:43:07.363729 PathMePy-Gustoon-0.2/PathMePy_Gustoon.egg-info/
+-rw-rw-rw-   0        0        0      837 2024-04-06 08:43:06.000000 PathMePy-Gustoon-0.2/PathMePy_Gustoon.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2024-04-06 08:43:06.000000 PathMePy-Gustoon-0.2/PathMePy_Gustoon.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-06 08:43:06.000000 PathMePy-Gustoon-0.2/PathMePy_Gustoon.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-04-06 08:43:06.000000 PathMePy-Gustoon-0.2/PathMePy_Gustoon.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      456 2024-03-31 08:33:03.000000 PathMePy-Gustoon-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-06 08:43:07.378780 PathMePy-Gustoon-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      907 2024-04-06 08:42:02.000000 PathMePy-Gustoon-0.2/setup.py
```

### Comparing `PathMePy-Gustoon-0.1.3/LICENSE.txt` & `PathMePy-Gustoon-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PathMePy-Gustoon-0.1.3/PKG-INFO` & `PathMePy-Gustoon-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PathMePy-Gustoon
-Version: 0.1.3
+Version: 0.2
 Summary: A tool to add scripts to Path
 Author: Gustoon
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `PathMePy-Gustoon-0.1.3/PathMePy_Gustoon.egg-info/PKG-INFO` & `PathMePy-Gustoon-0.2/PathMePy_Gustoon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PathMePy-Gustoon
-Version: 0.1.3
+Version: 0.2
 Summary: A tool to add scripts to Path
 Author: Gustoon
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `PathMePy-Gustoon-0.1.3/setup.py` & `PathMePy-Gustoon-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 name='PathMePy-Gustoon',
-version='0.1.3',
+version='0.2',
 author='Gustoon',
 author_email='',
 description='A tool to add scripts to Path',
 long_description='''
 # PathMePy
 
 A tool to add scripts to Path
```

