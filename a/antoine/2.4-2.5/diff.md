# Comparing `tmp/antoine-2.4.tar.gz` & `tmp/antoine-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antoine-2.4.tar", last modified: Fri Apr  5 10:49:08 2024, max compression
+gzip compressed data, was "antoine-2.5.tar", last modified: Sat Apr  6 08:44:08 2024, max compression
```

## Comparing `antoine-2.4.tar` & `antoine-2.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-05 10:49:08.903540 antoine-2.4/
--rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-05 10:49:08.903340 antoine-2.4/PKG-INFO
--rw-r--r--   0 antoinebertin   (501) staff       (20)      261 2024-04-05 10:43:11.000000 antoine-2.4/README.md
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-05 10:49:08.902340 antoine-2.4/antoine/
--rw-r--r--   0 antoinebertin   (501) staff       (20)       42 2024-04-04 12:03:26.000000 antoine-2.4/antoine/__init__.py
--rw-r--r--   0 antoinebertin   (501) staff       (20)     2417 2024-04-05 10:48:28.000000 antoine-2.4/antoine/app.py
-drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-05 10:49:08.903114 antoine-2.4/antoine.egg-info/
--rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-05 10:49:08.000000 antoine-2.4/antoine.egg-info/PKG-INFO
--rw-r--r--   0 antoinebertin   (501) staff       (20)      211 2024-04-05 10:49:08.000000 antoine-2.4/antoine.egg-info/SOURCES.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)        1 2024-04-05 10:49:08.000000 antoine-2.4/antoine.egg-info/dependency_links.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)       50 2024-04-05 10:49:08.000000 antoine-2.4/antoine.egg-info/entry_points.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)        8 2024-04-05 10:49:08.000000 antoine-2.4/antoine.egg-info/top_level.txt
--rw-r--r--   0 antoinebertin   (501) staff       (20)       38 2024-04-05 10:49:08.903575 antoine-2.4/setup.cfg
--rw-r--r--   0 antoinebertin   (501) staff       (20)      574 2024-04-05 10:48:21.000000 antoine-2.4/setup.py
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-06 08:44:08.177748 antoine-2.5/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-06 08:44:08.177485 antoine-2.5/PKG-INFO
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      261 2024-04-05 10:43:11.000000 antoine-2.5/README.md
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-06 08:44:08.176492 antoine-2.5/antoine/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       42 2024-04-04 12:03:26.000000 antoine-2.5/antoine/__init__.py
+-rw-r--r--   0 antoinebertin   (501) staff       (20)     2925 2024-04-06 08:42:51.000000 antoine-2.5/antoine/app.py
+drwxr-xr-x   0 antoinebertin   (501) staff       (20)        0 2024-04-06 08:44:08.177243 antoine-2.5/antoine.egg-info/
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      206 2024-04-06 08:44:08.000000 antoine-2.5/antoine.egg-info/PKG-INFO
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      211 2024-04-06 08:44:08.000000 antoine-2.5/antoine.egg-info/SOURCES.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)        1 2024-04-06 08:44:08.000000 antoine-2.5/antoine.egg-info/dependency_links.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       50 2024-04-06 08:44:08.000000 antoine-2.5/antoine.egg-info/entry_points.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)        8 2024-04-06 08:44:08.000000 antoine-2.5/antoine.egg-info/top_level.txt
+-rw-r--r--   0 antoinebertin   (501) staff       (20)       38 2024-04-06 08:44:08.177932 antoine-2.5/setup.cfg
+-rw-r--r--   0 antoinebertin   (501) staff       (20)      574 2024-04-06 08:43:06.000000 antoine-2.5/setup.py
```

### Comparing `antoine-2.4/setup.py` & `antoine-2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='antoine',
-    version='2.4',
+    version='2.5',
     packages=['antoine'],  # 'antoine' is the name of the package
     author='Antoine Bertin',
     author_email='monolok35@gmail.com',
     description='Hiring Antoine is so much fun!',
     url='https://github.com/monolok/antoine/',
     license='MIT',
     entry_points={
```

