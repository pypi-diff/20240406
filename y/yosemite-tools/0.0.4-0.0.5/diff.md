# Comparing `tmp/yosemite-tools-0.0.4.tar.gz` & `tmp/yosemite-tools-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yosemite-tools-0.0.4.tar", last modified: Sat Apr  6 04:39:57 2024, max compression
+gzip compressed data, was "yosemite-tools-0.0.5.tar", last modified: Sat Apr  6 04:45:07 2024, max compression
```

## Comparing `yosemite-tools-0.0.4.tar` & `yosemite-tools-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:39:57.835408 yosemite-tools-0.0.4/
--rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-06 04:39:57.834289 yosemite-tools-0.0.4/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-06 04:39:57.835643 yosemite-tools-0.0.4/setup.cfg
--rw-r--r--   0 hammad     (501) staff       (20)      554 2024-04-06 04:39:52.000000 yosemite-tools-0.0.4/setup.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:39:57.817838 yosemite-tools-0.0.4/yosemite_tools/
--rw-r--r--   0 hammad     (501) staff       (20)       22 2024-04-05 14:18:10.000000 yosemite-tools-0.0.4/yosemite_tools/__init__.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:39:57.832042 yosemite-tools-0.0.4/yosemite_tools/modules/
--rw-r--r--   0 hammad     (501) staff       (20)      160 2024-04-05 14:26:33.000000 yosemite-tools-0.0.4/yosemite_tools/modules/__init__.py
--rw-r--r--   0 hammad     (501) staff       (20)     8880 2024-04-05 14:13:25.000000 yosemite-tools-0.0.4/yosemite_tools/modules/inputs.py
--rw-r--r--   0 hammad     (501) staff       (20)     6337 2024-04-06 03:45:33.000000 yosemite-tools-0.0.4/yosemite_tools/modules/logger.py
--rw-r--r--   0 hammad     (501) staff       (20)     3163 2024-04-06 04:39:38.000000 yosemite-tools-0.0.4/yosemite_tools/modules/preconditions.py
--rw-r--r--   0 hammad     (501) staff       (20)    10620 2024-04-05 14:30:57.000000 yosemite-tools-0.0.4/yosemite_tools/modules/utils.py
-drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:39:57.833334 yosemite-tools-0.0.4/yosemite_tools.egg-info/
--rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-06 04:39:57.000000 yosemite-tools-0.0.4/yosemite_tools.egg-info/PKG-INFO
--rw-r--r--   0 hammad     (501) staff       (20)      397 2024-04-06 04:39:57.000000 yosemite-tools-0.0.4/yosemite_tools.egg-info/SOURCES.txt
--rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-06 04:39:57.000000 yosemite-tools-0.0.4/yosemite_tools.egg-info/dependency_links.txt
--rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-06 04:39:57.000000 yosemite-tools-0.0.4/yosemite_tools.egg-info/requires.txt
--rw-r--r--   0 hammad     (501) staff       (20)       15 2024-04-06 04:39:57.000000 yosemite-tools-0.0.4/yosemite_tools.egg-info/top_level.txt
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:45:07.160101 yosemite-tools-0.0.5/
+-rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-06 04:45:07.159489 yosemite-tools-0.0.5/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)       38 2024-04-06 04:45:07.160215 yosemite-tools-0.0.5/setup.cfg
+-rw-r--r--   0 hammad     (501) staff       (20)      554 2024-04-06 04:44:59.000000 yosemite-tools-0.0.5/setup.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:45:07.152018 yosemite-tools-0.0.5/yosemite_tools/
+-rw-r--r--   0 hammad     (501) staff       (20)       22 2024-04-05 14:18:10.000000 yosemite-tools-0.0.5/yosemite_tools/__init__.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:45:07.157744 yosemite-tools-0.0.5/yosemite_tools/modules/
+-rw-r--r--   0 hammad     (501) staff       (20)      160 2024-04-05 14:26:33.000000 yosemite-tools-0.0.5/yosemite_tools/modules/__init__.py
+-rw-r--r--   0 hammad     (501) staff       (20)     8880 2024-04-05 14:13:25.000000 yosemite-tools-0.0.5/yosemite_tools/modules/inputs.py
+-rw-r--r--   0 hammad     (501) staff       (20)     6337 2024-04-06 03:45:33.000000 yosemite-tools-0.0.5/yosemite_tools/modules/logger.py
+-rw-r--r--   0 hammad     (501) staff       (20)     3943 2024-04-06 04:44:50.000000 yosemite-tools-0.0.5/yosemite_tools/modules/preconditions.py
+-rw-r--r--   0 hammad     (501) staff       (20)    10620 2024-04-05 14:30:57.000000 yosemite-tools-0.0.5/yosemite_tools/modules/utils.py
+drwxr-xr-x   0 hammad     (501) staff       (20)        0 2024-04-06 04:45:07.158677 yosemite-tools-0.0.5/yosemite_tools.egg-info/
+-rw-r--r--   0 hammad     (501) staff       (20)      437 2024-04-06 04:45:07.000000 yosemite-tools-0.0.5/yosemite_tools.egg-info/PKG-INFO
+-rw-r--r--   0 hammad     (501) staff       (20)      397 2024-04-06 04:45:07.000000 yosemite-tools-0.0.5/yosemite_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 hammad     (501) staff       (20)        1 2024-04-06 04:45:07.000000 yosemite-tools-0.0.5/yosemite_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       41 2024-04-06 04:45:07.000000 yosemite-tools-0.0.5/yosemite_tools.egg-info/requires.txt
+-rw-r--r--   0 hammad     (501) staff       (20)       15 2024-04-06 04:45:07.000000 yosemite-tools-0.0.5/yosemite_tools.egg-info/top_level.txt
```

### Comparing `yosemite-tools-0.0.4/setup.py` & `yosemite-tools-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="yosemite-tools",
-    version="0.0.04",
+    version="0.0.05",
     author="Hammad Saeed",
     author_email="hammad@supportvectors.com",
     description="yosemite",
     long_description="""
 Yosemite
     """,
     packages=setuptools.find_packages(),
```

### Comparing `yosemite-tools-0.0.4/yosemite_tools/modules/inputs.py` & `yosemite-tools-0.0.5/yosemite_tools/modules/inputs.py`

 * *Files identical despite different names*

### Comparing `yosemite-tools-0.0.4/yosemite_tools/modules/logger.py` & `yosemite-tools-0.0.5/yosemite_tools/modules/logger.py`

 * *Files identical despite different names*

### Comparing `yosemite-tools-0.0.4/yosemite_tools/modules/utils.py` & `yosemite-tools-0.0.5/yosemite_tools/modules/utils.py`

 * *Files identical despite different names*

