# Comparing `tmp/asifjamali-0.6.2.tar.gz` & `tmp/asifjamali-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asifjamali-0.6.2.tar", last modified: Fri Apr  5 22:52:00 2024, max compression
+gzip compressed data, was "asifjamali-0.6.4.tar", last modified: Sat Apr  6 14:36:41 2024, max compression
```

## Comparing `asifjamali-0.6.2.tar` & `asifjamali-0.6.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 master_dcyjsmtvvn  (1005) www-data    (33)        0 2024-04-05 22:52:00.328627 asifjamali-0.6.2/
--rw-rw-r--   0 master_dcyjsmtvvn  (1005) www-data    (33)     1056 2024-04-05 20:59:12.000000 asifjamali-0.6.2/LICENSE
--rw-r--r--   0 master_dcyjsmtvvn  (1005) www-data    (33)     1475 2024-04-05 22:52:00.328627 asifjamali-0.6.2/PKG-INFO
--rw-rw-r--   0 master_dcyjsmtvvn  (1005) www-data    (33)     1105 2024-04-05 20:59:12.000000 asifjamali-0.6.2/README.md
-drwxrwxr-x   0 master_dcyjsmtvvn  (1005) www-data    (33)        0 2024-04-05 22:52:00.324627 asifjamali-0.6.2/asifjamali/
--rw-rw-r--   0 master_dcyjsmtvvn  (1005) www-data    (33)       22 2024-04-05 20:59:12.000000 asifjamali-0.6.2/asifjamali/__init__.py
--rw-rw-r--   0 master_dcyjsmtvvn  (1005) www-data    (33)    20301 2024-04-06 03:49:30.000000 asifjamali-0.6.2/asifjamali/musibat.py
-drwxrwxr-x   0 master_dcyjsmtvvn  (1005) www-data    (33)        0 2024-04-05 22:52:00.328627 asifjamali-0.6.2/asifjamali.egg-info/
--rw-r--r--   0 master_dcyjsmtvvn  (1005) www-data    (33)     1475 2024-04-05 22:52:00.000000 asifjamali-0.6.2/asifjamali.egg-info/PKG-INFO
--rw-rw-r--   0 master_dcyjsmtvvn  (1005) www-data    (33)      240 2024-04-05 22:52:00.000000 asifjamali-0.6.2/asifjamali.egg-info/SOURCES.txt
--rw-rw-r--   0 master_dcyjsmtvvn  (1005) www-data    (33)        1 2024-04-05 22:52:00.000000 asifjamali-0.6.2/asifjamali.egg-info/dependency_links.txt
--rw-rw-r--   0 master_dcyjsmtvvn  (1005) www-data    (33)        9 2024-04-05 22:52:00.000000 asifjamali-0.6.2/asifjamali.egg-info/requires.txt
--rw-rw-r--   0 master_dcyjsmtvvn  (1005) www-data    (33)       11 2024-04-05 22:52:00.000000 asifjamali-0.6.2/asifjamali.egg-info/top_level.txt
--rw-rw-r--   0 master_dcyjsmtvvn  (1005) www-data    (33)       38 2024-04-05 22:52:00.328627 asifjamali-0.6.2/setup.cfg
--rw-rw-r--   0 master_dcyjsmtvvn  (1005) www-data    (33)      640 2024-04-06 03:49:24.000000 asifjamali-0.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:36:41.601178 asifjamali-0.6.4/
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-04-05 11:59:12.000000 asifjamali-0.6.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1475 2024-04-06 14:36:41.601178 asifjamali-0.6.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-04-05 11:59:12.000000 asifjamali-0.6.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:36:41.597178 asifjamali-0.6.4/asifjamali/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-04-05 11:59:12.000000 asifjamali-0.6.4/asifjamali/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20304 2024-04-06 10:24:44.000000 asifjamali-0.6.4/asifjamali/musibat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:36:41.601178 asifjamali-0.6.4/asifjamali.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1475 2024-04-06 14:36:41.000000 asifjamali-0.6.4/asifjamali.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-06 14:36:41.000000 asifjamali-0.6.4/asifjamali.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 14:36:41.000000 asifjamali-0.6.4/asifjamali.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-06 14:36:41.000000 asifjamali-0.6.4/asifjamali.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-06 14:36:41.000000 asifjamali-0.6.4/asifjamali.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 14:36:41.601178 asifjamali-0.6.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      640 2024-04-06 10:24:22.000000 asifjamali-0.6.4/setup.py
```

### Comparing `asifjamali-0.6.2/LICENSE` & `asifjamali-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `asifjamali-0.6.2/PKG-INFO` & `asifjamali-0.6.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asifjamali
-Version: 0.6.2
+Version: 0.6.4
 Summary: Team Musibat Bots
 Home-page: https://bitbucket.org/shahzain83/musibat
 Author: Shahzain Khan
 Author-email: technomusibat@hotmail.com
 License: MIT
 Project-URL: Bug Tracker, https://bitbucket.org/shahzain83/musibat/issues
 Description-Content-Type: text/markdown
```

### Comparing `asifjamali-0.6.2/README.md` & `asifjamali-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `asifjamali-0.6.2/asifjamali/musibat.py` & `asifjamali-0.6.4/asifjamali/musibat.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-import os, re, sys, time, json, socket, random, codecs, requests, subprocess
+import os, re, sys, time, json, socket, random, codecs, requests, subprocess
```

### Comparing `asifjamali-0.6.2/asifjamali.egg-info/PKG-INFO` & `asifjamali-0.6.4/asifjamali.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asifjamali
-Version: 0.6.2
+Version: 0.6.4
 Summary: Team Musibat Bots
 Home-page: https://bitbucket.org/shahzain83/musibat
 Author: Shahzain Khan
 Author-email: technomusibat@hotmail.com
 License: MIT
 Project-URL: Bug Tracker, https://bitbucket.org/shahzain83/musibat/issues
 Description-Content-Type: text/markdown
```

### Comparing `asifjamali-0.6.2/setup.py` & `asifjamali-0.6.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='asifjamali',
-    version='0.6.2',
+    version='0.6.4',
     author='Shahzain Khan',
     author_email='technomusibat@hotmail.com',
     description='Team Musibat Bots',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://bitbucket.org/shahzain83/musibat',
     project_urls = {
```
