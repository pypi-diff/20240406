# Comparing `tmp/homa-0.24.tar.gz` & `tmp/homa-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homa-0.24.tar", last modified: Thu Apr  4 21:06:54 2024, max compression
+gzip compressed data, was "homa-0.25.tar", last modified: Sat Apr  6 12:55:24 2024, max compression
```

## Comparing `homa-0.24.tar` & `homa-0.25.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 21:06:54.450495 homa-0.24/
--rw-r--r--   0 taha       (501) staff       (20)     1072 2024-03-27 20:05:25.000000 homa-0.24/LICENSE
--rw-r--r--   0 taha       (501) staff       (20)     2422 2024-04-04 21:06:54.450313 homa-0.24/PKG-INFO
--rw-r--r--   0 taha       (501) staff       (20)     2241 2024-04-04 21:05:45.000000 homa-0.24/README.md
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 21:06:54.445998 homa-0.24/homa/
--rw-r--r--   0 taha       (501) staff       (20)      182 2024-04-04 15:42:04.000000 homa-0.24/homa/__init__.py
--rw-r--r--   0 taha       (501) staff       (20)      464 2024-04-04 13:08:57.000000 homa-0.24/homa/camera.py
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 21:06:54.448518 homa-0.24/homa/classes/
--rw-r--r--   0 taha       (501) staff       (20)      222 2024-04-03 16:22:17.000000 homa-0.24/homa/classes/Collection.py
--rw-r--r--   0 taha       (501) staff       (20)       93 2024-04-03 16:33:06.000000 homa-0.24/homa/classes/Logger.py
--rw-r--r--   0 taha       (501) staff       (20)      589 2024-04-04 15:46:34.000000 homa-0.24/homa/classes/Repository.py
--rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-03 21:21:15.000000 homa-0.24/homa/classes/__init__.py
--rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-03 15:09:00.000000 homa-0.24/homa/constants.py
--rw-r--r--   0 taha       (501) staff       (20)     1946 2024-04-04 15:39:07.000000 homa-0.24/homa/events.py
--rw-r--r--   0 taha       (501) staff       (20)     1058 2024-04-04 14:28:59.000000 homa-0.24/homa/filters.py
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 21:06:54.449313 homa-0.24/homa/helpers/
--rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-04 13:55:31.000000 homa-0.24/homa/helpers/__init__.py
--rw-r--r--   0 taha       (501) staff       (20)      301 2024-04-04 16:29:56.000000 homa-0.24/homa/helpers/alias.py
--rw-r--r--   0 taha       (501) staff       (20)       78 2024-04-04 13:53:19.000000 homa-0.24/homa/helpers/environment.py
--rw-r--r--   0 taha       (501) staff       (20)      330 2024-04-04 13:56:06.000000 homa-0.24/homa/helpers/kernel.py
--rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-04 13:56:03.000000 homa-0.24/homa/helpers.py
--rw-r--r--   0 taha       (501) staff       (20)     1733 2024-04-04 16:31:10.000000 homa-0.24/homa/main.py
--rw-r--r--   0 taha       (501) staff       (20)      804 2024-04-04 13:57:15.000000 homa-0.24/homa/orientation.py
--rw-r--r--   0 taha       (501) staff       (20)      283 2024-04-04 15:52:49.000000 homa-0.24/homa/shapes.py
--rw-r--r--   0 taha       (501) staff       (20)      460 2024-04-04 13:55:28.000000 homa-0.24/homa/spaces.py
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 21:06:54.447170 homa-0.24/homa.egg-info/
--rw-r--r--   0 taha       (501) staff       (20)     2422 2024-04-04 21:06:54.000000 homa-0.24/homa.egg-info/PKG-INFO
--rw-r--r--   0 taha       (501) staff       (20)      564 2024-04-04 21:06:54.000000 homa-0.24/homa.egg-info/SOURCES.txt
--rw-r--r--   0 taha       (501) staff       (20)        1 2024-04-04 21:06:54.000000 homa-0.24/homa.egg-info/dependency_links.txt
--rw-r--r--   0 taha       (501) staff       (20)       20 2024-04-04 21:06:54.000000 homa-0.24/homa.egg-info/requires.txt
--rw-r--r--   0 taha       (501) staff       (20)       11 2024-04-04 21:06:54.000000 homa-0.24/homa.egg-info/top_level.txt
--rw-r--r--   0 taha       (501) staff       (20)       38 2024-04-04 21:06:54.450565 homa-0.24/setup.cfg
--rw-r--r--   0 taha       (501) staff       (20)      671 2024-04-03 21:59:07.000000 homa-0.24/setup.py
-drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-04 21:06:54.449899 homa-0.24/tests/
--rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-04 14:06:35.000000 homa-0.24/tests/__init__.py
--rw-r--r--   0 taha       (501) staff       (20)      772 2024-04-04 14:23:48.000000 homa-0.24/tests/test_images.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-06 12:55:24.053753 homa-0.25/
+-rw-r--r--   0 taha       (501) staff       (20)     1072 2024-03-27 20:05:25.000000 homa-0.25/LICENSE
+-rw-r--r--   0 taha       (501) staff       (20)     2422 2024-04-06 12:55:24.053584 homa-0.25/PKG-INFO
+-rw-r--r--   0 taha       (501) staff       (20)     2241 2024-04-04 21:05:45.000000 homa-0.25/README.md
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-06 12:55:24.048668 homa-0.25/homa/
+-rw-r--r--   0 taha       (501) staff       (20)      228 2024-04-06 12:08:27.000000 homa-0.25/homa/__init__.py
+-rw-r--r--   0 taha       (501) staff       (20)      527 2024-04-06 11:32:01.000000 homa-0.25/homa/camera.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-06 12:55:24.051553 homa-0.25/homa/classes/
+-rw-r--r--   0 taha       (501) staff       (20)      222 2024-04-03 16:22:17.000000 homa-0.25/homa/classes/Collection.py
+-rw-r--r--   0 taha       (501) staff       (20)      490 2024-04-06 12:18:24.000000 homa-0.25/homa/classes/Image.py
+-rw-r--r--   0 taha       (501) staff       (20)       93 2024-04-03 16:33:06.000000 homa-0.25/homa/classes/Logger.py
+-rw-r--r--   0 taha       (501) staff       (20)      840 2024-04-06 11:37:57.000000 homa-0.25/homa/classes/Repository.py
+-rw-r--r--   0 taha       (501) staff       (20)     2941 2024-04-06 12:52:56.000000 homa-0.25/homa/classes/Window.py
+-rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-03 21:21:15.000000 homa-0.25/homa/classes/__init__.py
+-rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-03 15:09:00.000000 homa-0.25/homa/constants.py
+-rw-r--r--   0 taha       (501) staff       (20)     1223 2024-04-06 12:48:44.000000 homa-0.25/homa/events.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-06 12:55:24.052734 homa-0.25/homa/helpers/
+-rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-04 13:55:31.000000 homa-0.25/homa/helpers/__init__.py
+-rw-r--r--   0 taha       (501) staff       (20)      453 2024-04-06 10:48:09.000000 homa-0.25/homa/helpers/alias.py
+-rw-r--r--   0 taha       (501) staff       (20)       78 2024-04-05 11:50:14.000000 homa-0.25/homa/helpers/environment.py
+-rw-r--r--   0 taha       (501) staff       (20)      329 2024-04-06 12:06:52.000000 homa-0.25/homa/helpers/kernel.py
+-rw-r--r--   0 taha       (501) staff       (20)      385 2024-04-06 10:58:23.000000 homa-0.25/homa/helpers/string.py
+-rw-r--r--   0 taha       (501) staff       (20)      660 2024-04-06 12:18:06.000000 homa-0.25/homa/main.py
+-rw-r--r--   0 taha       (501) staff       (20)      804 2024-04-04 13:57:15.000000 homa-0.25/homa/orientation.py
+-rw-r--r--   0 taha       (501) staff       (20)     1044 2024-04-06 11:56:15.000000 homa-0.25/homa/shapes.py
+-rw-r--r--   0 taha       (501) staff       (20)      804 2024-04-05 12:16:17.000000 homa-0.25/homa/spaces.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-06 12:55:24.049672 homa-0.25/homa.egg-info/
+-rw-r--r--   0 taha       (501) staff       (20)     2422 2024-04-06 12:55:23.000000 homa-0.25/homa.egg-info/PKG-INFO
+-rw-r--r--   0 taha       (501) staff       (20)      600 2024-04-06 12:55:24.000000 homa-0.25/homa.egg-info/SOURCES.txt
+-rw-r--r--   0 taha       (501) staff       (20)        1 2024-04-06 12:55:23.000000 homa-0.25/homa.egg-info/dependency_links.txt
+-rw-r--r--   0 taha       (501) staff       (20)       20 2024-04-06 12:55:23.000000 homa-0.25/homa.egg-info/requires.txt
+-rw-r--r--   0 taha       (501) staff       (20)       11 2024-04-06 12:55:23.000000 homa-0.25/homa.egg-info/top_level.txt
+-rw-r--r--   0 taha       (501) staff       (20)       38 2024-04-06 12:55:24.053804 homa-0.25/setup.cfg
+-rw-r--r--   0 taha       (501) staff       (20)      671 2024-04-03 21:59:07.000000 homa-0.25/setup.py
+drwxr-xr-x   0 taha       (501) staff       (20)        0 2024-04-06 12:55:24.053213 homa-0.25/tests/
+-rw-r--r--   0 taha       (501) staff       (20)        0 2024-04-04 14:06:35.000000 homa-0.25/tests/__init__.py
+-rw-r--r--   0 taha       (501) staff       (20)      772 2024-04-04 14:23:48.000000 homa-0.25/tests/test_images.py
```

### Comparing `homa-0.24/LICENSE` & `homa-0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `homa-0.24/PKG-INFO` & `homa-0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homa
-Version: 0.24
+Version: 0.25
 Maintainer: Taha Shieenavaz
 Maintainer-email: tahashieenavaz@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 	<img
```

### Comparing `homa-0.24/README.md` & `homa-0.25/README.md`

 * *Files identical despite different names*

### Comparing `homa-0.24/homa/orientation.py` & `homa-0.25/homa/orientation.py`

 * *Files identical despite different names*

### Comparing `homa-0.24/homa.egg-info/PKG-INFO` & `homa-0.25/homa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: homa
-Version: 0.24
+Version: 0.25
 Maintainer: Taha Shieenavaz
 Maintainer-email: tahashieenavaz@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 	<img
```

### Comparing `homa-0.24/homa.egg-info/SOURCES.txt` & `homa-0.25/homa.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 LICENSE
 README.md
 setup.py
 homa/__init__.py
 homa/camera.py
 homa/constants.py
 homa/events.py
-homa/filters.py
-homa/helpers.py
 homa/main.py
 homa/orientation.py
 homa/shapes.py
 homa/spaces.py
 homa.egg-info/PKG-INFO
 homa.egg-info/SOURCES.txt
 homa.egg-info/dependency_links.txt
 homa.egg-info/requires.txt
 homa.egg-info/top_level.txt
 homa/classes/Collection.py
+homa/classes/Image.py
 homa/classes/Logger.py
 homa/classes/Repository.py
+homa/classes/Window.py
 homa/classes/__init__.py
 homa/helpers/__init__.py
 homa/helpers/alias.py
 homa/helpers/environment.py
 homa/helpers/kernel.py
+homa/helpers/string.py
 tests/__init__.py
 tests/test_images.py
```

### Comparing `homa-0.24/setup.py` & `homa-0.25/setup.py`

 * *Files identical despite different names*

### Comparing `homa-0.24/tests/test_images.py` & `homa-0.25/tests/test_images.py`

 * *Files identical despite different names*

