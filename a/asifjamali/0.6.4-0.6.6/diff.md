# Comparing `tmp/asifjamali-0.6.4.tar.gz` & `tmp/asifjamali-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asifjamali-0.6.4.tar", last modified: Sat Apr  6 14:36:41 2024, max compression
+gzip compressed data, was "asifjamali-0.6.6.tar", last modified: Sat Apr  6 21:11:18 2024, max compression
```

## Comparing `asifjamali-0.6.4.tar` & `asifjamali-0.6.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:36:41.601178 asifjamali-0.6.4/
--rw-r--r--   0 root         (0) root         (0)     1056 2024-04-05 11:59:12.000000 asifjamali-0.6.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1475 2024-04-06 14:36:41.601178 asifjamali-0.6.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1105 2024-04-05 11:59:12.000000 asifjamali-0.6.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:36:41.597178 asifjamali-0.6.4/asifjamali/
--rw-r--r--   0 root         (0) root         (0)       22 2024-04-05 11:59:12.000000 asifjamali-0.6.4/asifjamali/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20304 2024-04-06 10:24:44.000000 asifjamali-0.6.4/asifjamali/musibat.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 14:36:41.601178 asifjamali-0.6.4/asifjamali.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1475 2024-04-06 14:36:41.000000 asifjamali-0.6.4/asifjamali.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      240 2024-04-06 14:36:41.000000 asifjamali-0.6.4/asifjamali.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 14:36:41.000000 asifjamali-0.6.4/asifjamali.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-06 14:36:41.000000 asifjamali-0.6.4/asifjamali.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-04-06 14:36:41.000000 asifjamali-0.6.4/asifjamali.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 14:36:41.601178 asifjamali-0.6.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      640 2024-04-06 10:24:22.000000 asifjamali-0.6.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 21:11:18.597797 asifjamali-0.6.6/
+-rw-r--r--   0 root         (0) root         (0)     1056 2024-03-14 23:59:10.000000 asifjamali-0.6.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1475 2024-04-06 21:11:18.593797 asifjamali-0.6.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1105 2024-03-14 23:59:10.000000 asifjamali-0.6.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 21:11:18.593797 asifjamali-0.6.6/asifjamali/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-15 00:00:14.000000 asifjamali-0.6.6/asifjamali/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20305 2024-04-07 01:46:46.000000 asifjamali-0.6.6/asifjamali/musibat.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-06 21:11:18.593797 asifjamali-0.6.6/asifjamali.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1475 2024-04-06 21:11:18.000000 asifjamali-0.6.6/asifjamali.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      240 2024-04-06 21:11:18.000000 asifjamali-0.6.6/asifjamali.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-06 21:11:18.000000 asifjamali-0.6.6/asifjamali.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-06 21:11:18.000000 asifjamali-0.6.6/asifjamali.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-06 21:11:18.000000 asifjamali-0.6.6/asifjamali.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-06 21:11:18.597797 asifjamali-0.6.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      640 2024-04-06 21:10:18.000000 asifjamali-0.6.6/setup.py
```

### Comparing `asifjamali-0.6.4/LICENSE` & `asifjamali-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `asifjamali-0.6.4/PKG-INFO` & `asifjamali-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asifjamali
-Version: 0.6.4
+Version: 0.6.6
 Summary: Team Musibat Bots
 Home-page: https://bitbucket.org/shahzain83/musibat
 Author: Shahzain Khan
 Author-email: technomusibat@hotmail.com
 License: MIT
 Project-URL: Bug Tracker, https://bitbucket.org/shahzain83/musibat/issues
 Description-Content-Type: text/markdown
```

### Comparing `asifjamali-0.6.4/README.md` & `asifjamali-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `asifjamali-0.6.4/asifjamali/musibat.py` & `asifjamali-0.6.6/asifjamali/musibat.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1 +1 @@
-import os, re, sys, time, json, socket, random, codecs, requests, subprocess
+import os, re, sys, time, json, socket, random, codecs, requests, subprocess
```

### Comparing `asifjamali-0.6.4/asifjamali.egg-info/PKG-INFO` & `asifjamali-0.6.6/asifjamali.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asifjamali
-Version: 0.6.4
+Version: 0.6.6
 Summary: Team Musibat Bots
 Home-page: https://bitbucket.org/shahzain83/musibat
 Author: Shahzain Khan
 Author-email: technomusibat@hotmail.com
 License: MIT
 Project-URL: Bug Tracker, https://bitbucket.org/shahzain83/musibat/issues
 Description-Content-Type: text/markdown
```

### Comparing `asifjamali-0.6.4/setup.py` & `asifjamali-0.6.6/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='asifjamali',
-    version='0.6.4',
+    version='0.6.6',
     author='Shahzain Khan',
     author_email='technomusibat@hotmail.com',
     description='Team Musibat Bots',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://bitbucket.org/shahzain83/musibat',
     project_urls = {
```
