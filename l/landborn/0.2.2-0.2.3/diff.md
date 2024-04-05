# Comparing `tmp/landborn-0.2.2.tar.gz` & `tmp/landborn-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landborn-0.2.2.tar", last modified: Tue Mar 12 17:51:37 2024, max compression
+gzip compressed data, was "landborn-0.2.3.tar", last modified: Fri Apr  5 23:54:33 2024, max compression
```

## Comparing `landborn-0.2.2.tar` & `landborn-0.2.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-03-12 17:51:37.735041 landborn-0.2.2/
--rw-r--r--   0 mollynelson   (501) staff       (20)     1063 2024-02-16 00:51:51.000000 landborn-0.2.2/LICENSE
--rw-r--r--   0 mollynelson   (501) staff       (20)     1098 2024-03-12 17:51:37.734775 landborn-0.2.2/PKG-INFO
--rw-r--r--   0 mollynelson   (501) staff       (20)      871 2024-03-03 19:22:54.000000 landborn-0.2.2/README.md
-drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-03-12 17:51:37.732693 landborn-0.2.2/landborn/
--rw-r--r--   0 mollynelson   (501) staff       (20)      362 2024-03-12 17:15:22.000000 landborn-0.2.2/landborn/__init__.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     2938 2024-02-28 22:51:09.000000 landborn-0.2.2/landborn/barplot.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     7484 2024-03-12 17:48:39.000000 landborn-0.2.2/landborn/colormap.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     7102 2024-03-03 19:27:01.000000 landborn-0.2.2/landborn/functions.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     1068 2024-02-28 16:46:45.000000 landborn-0.2.2/landborn/jointplot.py
--rw-r--r--   0 mollynelson   (501) staff       (20)      781 2024-02-21 00:37:06.000000 landborn-0.2.2/landborn/lineplot.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     1830 2024-03-01 15:21:20.000000 landborn-0.2.2/landborn/scatterplot.py
--rw-r--r--   0 mollynelson   (501) staff       (20)     2292 2024-03-03 18:53:57.000000 landborn-0.2.2/landborn/swarmplot3.py
-drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-03-12 17:51:37.734387 landborn-0.2.2/landborn.egg-info/
--rw-r--r--   0 mollynelson   (501) staff       (20)     1098 2024-03-12 17:51:37.000000 landborn-0.2.2/landborn.egg-info/PKG-INFO
--rw-r--r--   0 mollynelson   (501) staff       (20)      359 2024-03-12 17:51:37.000000 landborn-0.2.2/landborn.egg-info/SOURCES.txt
--rw-r--r--   0 mollynelson   (501) staff       (20)        1 2024-03-12 17:51:37.000000 landborn-0.2.2/landborn.egg-info/dependency_links.txt
--rw-r--r--   0 mollynelson   (501) staff       (20)       24 2024-03-12 17:51:37.000000 landborn-0.2.2/landborn.egg-info/requires.txt
--rw-r--r--   0 mollynelson   (501) staff       (20)        9 2024-03-12 17:51:37.000000 landborn-0.2.2/landborn.egg-info/top_level.txt
--rw-r--r--   0 mollynelson   (501) staff       (20)       38 2024-03-12 17:51:37.735140 landborn-0.2.2/setup.cfg
--rw-r--r--   0 mollynelson   (501) staff       (20)      536 2024-03-12 17:15:27.000000 landborn-0.2.2/setup.py
+drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-05 23:54:33.556590 landborn-0.2.3/
+-rw-r--r--   0 mollynelson   (501) staff       (20)     1063 2024-02-16 00:51:51.000000 landborn-0.2.3/LICENSE
+-rw-r--r--   0 mollynelson   (501) staff       (20)     1098 2024-04-05 23:54:33.556177 landborn-0.2.3/PKG-INFO
+-rw-r--r--   0 mollynelson   (501) staff       (20)      871 2024-04-05 23:46:10.000000 landborn-0.2.3/README.md
+drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-05 23:54:33.552716 landborn-0.2.3/landborn/
+-rw-r--r--   0 mollynelson   (501) staff       (20)      407 2024-04-05 23:54:19.000000 landborn-0.2.3/landborn/__init__.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     5633 2024-04-05 16:26:56.000000 landborn-0.2.3/landborn/barplot.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     7484 2024-04-05 22:56:49.000000 landborn-0.2.3/landborn/colormap.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)      312 2024-04-05 23:14:31.000000 landborn-0.2.3/landborn/config.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)    15200 2024-04-05 23:18:51.000000 landborn-0.2.3/landborn/functions.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     5224 2024-04-05 22:40:43.000000 landborn-0.2.3/landborn/gradient.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     1068 2024-02-28 16:46:45.000000 landborn-0.2.3/landborn/jointplot.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     4793 2024-04-05 22:47:21.000000 landborn-0.2.3/landborn/lineplot.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     5908 2024-04-05 22:46:40.000000 landborn-0.2.3/landborn/scatterplot.py
+-rw-r--r--   0 mollynelson   (501) staff       (20)     2292 2024-03-03 18:53:57.000000 landborn-0.2.3/landborn/swarmplot3.py
+drwxr-xr-x   0 mollynelson   (501) staff       (20)        0 2024-04-05 23:54:33.555542 landborn-0.2.3/landborn.egg-info/
+-rw-r--r--   0 mollynelson   (501) staff       (20)     1098 2024-04-05 23:54:33.000000 landborn-0.2.3/landborn.egg-info/PKG-INFO
+-rw-r--r--   0 mollynelson   (501) staff       (20)      399 2024-04-05 23:54:33.000000 landborn-0.2.3/landborn.egg-info/SOURCES.txt
+-rw-r--r--   0 mollynelson   (501) staff       (20)        1 2024-04-05 23:54:33.000000 landborn-0.2.3/landborn.egg-info/dependency_links.txt
+-rw-r--r--   0 mollynelson   (501) staff       (20)       24 2024-04-05 23:54:33.000000 landborn-0.2.3/landborn.egg-info/requires.txt
+-rw-r--r--   0 mollynelson   (501) staff       (20)        9 2024-04-05 23:54:33.000000 landborn-0.2.3/landborn.egg-info/top_level.txt
+-rw-r--r--   0 mollynelson   (501) staff       (20)       38 2024-04-05 23:54:33.556764 landborn-0.2.3/setup.cfg
+-rw-r--r--   0 mollynelson   (501) staff       (20)      536 2024-04-05 23:54:17.000000 landborn-0.2.3/setup.py
```

### Comparing `landborn-0.2.2/LICENSE` & `landborn-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `landborn-0.2.2/PKG-INFO` & `landborn-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landborn
-Version: 0.2.2
+Version: 0.2.3
 Summary: Landborn Visualization Library
 Author: Molly Nelson
 Author-email: mollyynelson@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `landborn-0.2.2/README.md` & `landborn-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `landborn-0.2.2/landborn/colormap.py` & `landborn-0.2.3/landborn/colormap.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.2/landborn/jointplot.py` & `landborn-0.2.3/landborn/jointplot.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.2/landborn/swarmplot3.py` & `landborn-0.2.3/landborn/swarmplot3.py`

 * *Files identical despite different names*

### Comparing `landborn-0.2.2/landborn.egg-info/PKG-INFO` & `landborn-0.2.3/landborn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landborn
-Version: 0.2.2
+Version: 0.2.3
 Summary: Landborn Visualization Library
 Author: Molly Nelson
 Author-email: mollyynelson@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `landborn-0.2.2/setup.py` & `landborn-0.2.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_packages, setup
 
 setup(
     name='landborn',
     packages=find_packages(include=['landborn']),
-    version='0.2.2',
+    version='0.2.3',
     description='Landborn Visualization Library',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Molly Nelson',
     author_email="mollyynelson@gmail.com",
     license='MIT',
     install_requires=['pandas', 'numpy', 'matplotlib'],
```

